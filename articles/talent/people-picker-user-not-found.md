---
title: El usuario no puede encontrar en el selector de personas en Attract u Onboard
description: Este tema explica qué hacer cuando los usuarios en la compañía arrendataria no aparecen en el selector de personas en las aplicaciones Dynamics 365 for Talent Attract u Onboard.
author: ChrisChua
manager: AnnBe
ms.date: 01/22/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: chrichua
ms.search.validFrom: 2019-01-22
ms.dyn365.ops.version: Talent
ms.openlocfilehash: 2d4a74ee2cc65153c1f9fdc1b42c2fc440d188d6
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "306166"
---
# <a name="azure-active-directory-users-not-found-in-people-picker"></a><span data-ttu-id="42ecd-103">No se encuentran usuarios de Azure Active Directory en el selector de personas</span><span class="sxs-lookup"><span data-stu-id="42ecd-103">Azure Active Directory users not found in People Picker</span></span>

[!include [banner](includes/banner.md)]

## <a name="issue"></a><span data-ttu-id="42ecd-104">Emisión</span><span class="sxs-lookup"><span data-stu-id="42ecd-104">Issue</span></span>

<span data-ttu-id="42ecd-105">Algunos usuarios válidos en Microsoft Azure Active Directory (Azure AD) para el arrendatario no aparecen al buscar el nombre en el selector de personas en las aplicaciones Dynamics 365 for Talent Attract u Onboard.</span><span class="sxs-lookup"><span data-stu-id="42ecd-105">Certain valid users in Microsoft Azure Active Directory (Azure AD) for the tenant do not appear when searching for the name in the People Picker in the Dynamics 365 for Talent Attract or Onboard applications.</span></span>

## <a name="cause"></a><span data-ttu-id="42ecd-106">Causa</span><span class="sxs-lookup"><span data-stu-id="42ecd-106">Cause</span></span>

<span data-ttu-id="42ecd-107">No determinados tipos de usuario no se admiten actualmente en las aplicaciones Attract u Onboard.</span><span class="sxs-lookup"><span data-stu-id="42ecd-107">Certain user types are not currently supported in the Attract and Onboard applications.</span></span> <span data-ttu-id="42ecd-108">Compruebe que el usuario no sea un usuario invitado de Azure AD Business to Business (B2B).</span><span class="sxs-lookup"><span data-stu-id="42ecd-108">Verify that the user is not an Azure AD Business to Business (B2B) guest user.</span></span> <span data-ttu-id="42ecd-109">La información del "tipo de usuario” se puede encontrar en la sección Azure Active Directory en el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="42ecd-109">"User Type" information can be found in the Azure Active Directory blade on the Azure portal.</span></span>

<span data-ttu-id="42ecd-110">Para obtener más información sobre Azure B2B, consulte [Qué es acceso de usuario invitado en Azure Active Directory B2B](https://docs.microsoft.com/en-us/azure/active-directory/b2b/what-is-b2b).</span><span class="sxs-lookup"><span data-stu-id="42ecd-110">For more information about Azure B2B, see [What is guest user access in Azure Active Directory B2B](https://docs.microsoft.com/en-us/azure/active-directory/b2b/what-is-b2b).</span></span>

<span data-ttu-id="42ecd-111">Para los usuarios de no-B2B, hay algunos usuarios que pueden tener una propiedad "Tipo de usuario" incompleta en el objeto **Usuario**.</span><span class="sxs-lookup"><span data-stu-id="42ecd-111">For non-B2B users, there are certain users who may have an incomplete "User Type" property on the **User** object.</span></span> <span data-ttu-id="42ecd-112">Esto se puede comprobar y corregir a través del módulo Azure AD Powershell.</span><span class="sxs-lookup"><span data-stu-id="42ecd-112">This can be verified and fixed using the Azure AD Powershell module.</span></span> <span data-ttu-id="42ecd-113">Para obtener más información, vea [Azure AD](https://docs.microsoft.com/en-us/powershell/module/azuread/?view=azureadps-2.0).</span><span class="sxs-lookup"><span data-stu-id="42ecd-113">For more information, see [Azure AD](https://docs.microsoft.com/en-us/powershell/module/azuread/?view=azureadps-2.0).</span></span>

## <a name="resolution"></a><span data-ttu-id="42ecd-114">Resolución</span><span class="sxs-lookup"><span data-stu-id="42ecd-114">Resolution</span></span>

<span data-ttu-id="42ecd-115">Para completar los pasos siguientes y resolver el problema, deberá disponer de permisos "Administrador global” en el arrendatario de Azure Active Directory o permisos para **User.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="42ecd-115">To complete the following steps to resolve the issue, you will need to have "Global Administrator" permissions on the Azure Active Directory tenant or permissions for **User.ReadWrite.All**.</span></span>

<span data-ttu-id="42ecd-116">Para comprobar el "Tipo de usuario" para el usuario afectado.</span><span class="sxs-lookup"><span data-stu-id="42ecd-116">To verify the "User Type" for the affected user.</span></span>

```
PS C:\>Get-AzureADUser -ObjectId "testUpn@tenant.com"
```
<span data-ttu-id="42ecd-117">El comando devuelve la siguiente información.</span><span class="sxs-lookup"><span data-stu-id="42ecd-117">The command returns the following information.</span></span>
```
ObjectId                             DisplayName UserPrincipalName      UserType
--------                             ----------- -----------------      --------
5e8b0f4d-2cd4-4e17-9467-b0f6a5c0c4d0 New user    testUpn@tenant.com     
```
<span data-ttu-id="42ecd-118">Tenga en cuenta la propiedad **UserType** en el usuario.</span><span class="sxs-lookup"><span data-stu-id="42ecd-118">Note the **UserType** property on the user.</span></span> <span data-ttu-id="42ecd-119">Si **UserType** está en blanco, por ejemplo no "Miembro “o “Invitado,” actualice **UserType** mediante el comando siguiente.</span><span class="sxs-lookup"><span data-stu-id="42ecd-119">If the **UserType** is blank, for example not "Member" or "Guest", update the **UserType** using the following command.</span></span>

```
PS C:\>Set-AzureADUser -ObjectId "testUpn@tenant.com" -UserType Member
```