---
title: "Instalación y configuración de Microsoft Dynamics 365 for Finance and Operations #8211; Warehousing"
description: "Este tema describe cómo instalar y configurar Microsoft Dynamics 365 for Finance and Operations - Warehousing."
author: MarkusFogelberg
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: SysAADClientTable, WHSMobileAppField, WHSMobileAppFieldPriority, WHSRFMenu, WHSRFMenuItem, WHSWorker
audience: Application User, IT Pro
ms.reviewer: bis
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 267694
ms.assetid: d95d43b2-13ff-4189-a71a-3a1fb57d55ed
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: mafoge
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: HT
ms.sourcegitcommit: 69eeb90387ca5765c163c7d482295ea104cc078c
ms.openlocfilehash: 31e77b27d4bf95c997817b3a053b33119562adf8
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---

# <a name="install-and-configure-microsoft-dynamics-365-for-finance-and-operations-8211-warehousing"></a><span data-ttu-id="953e2-103">Instalación y configuración de Microsoft Dynamics 365 for Finance and Operations #8211; Warehousing</span><span class="sxs-lookup"><span data-stu-id="953e2-103">Install and configure Microsoft Dynamics 365 for Finance and Operations &#8211; Warehousing</span></span>

[!include[banner](../includes/banner.md)]


<span data-ttu-id="953e2-104">Este tema describe cómo instalar y configurar Microsoft Dynamics 365 for Finance and Operations - Warehousing.</span><span class="sxs-lookup"><span data-stu-id="953e2-104">This topic describes how to install and configure Microsoft Dynamics 365 for Finance and Operations - Warehousing.</span></span>

<span data-ttu-id="953e2-105">Finance and Operations - Warehousing es una aplicación disponible en Google Play Store y Windows Store.</span><span class="sxs-lookup"><span data-stu-id="953e2-105">Finance and Operations - Warehousing is an application available on Google Play Store and Windows Store.</span></span> <span data-ttu-id="953e2-106">En la versión actual de Finance and Operations, esta aplicación se proporciona como componente independiente, con implementación propia en los dispositivos utilizados para las tareas de almacén.</span><span class="sxs-lookup"><span data-stu-id="953e2-106">For the current version of Finance and Operations, this app is provided as a standalone component, which means self-deployment on devices used for warehouse tasks.</span></span> <span data-ttu-id="953e2-107">Para usar la aplicación en su entorno de Finance and Operations, deberá descargar la aplicación en cada dispositivo y configurarla para conectarse al entorno de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-107">In order to use the app in your Finance and Operations environment, you must download the app on each device and configure it to connect to your Finance and Operations environment.</span></span> <span data-ttu-id="953e2-108">Este tema describe cómo instalar la aplicación en los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="953e2-108">This topic describes how to install the app on your devices.</span></span> <span data-ttu-id="953e2-109">También se explica cómo configurar la aplicación para conectarla al entorno de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-109">It also explains how to configure the app to connect to your Finance and Operations environment.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="953e2-110">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="953e2-110">Prerequisites</span></span>
<span data-ttu-id="953e2-111">La aplicación está disponible para los sistemas operativos Android y Windows.</span><span class="sxs-lookup"><span data-stu-id="953e2-111">The app is available on Android and Windows operating systems.</span></span> <span data-ttu-id="953e2-112">Para utilizar esta aplicación, debe tener uno de los sistemas operativos admitidos siguientes instalado en los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="953e2-112">To use this app, you must have one of the following supported operating systems installed on your devices.</span></span> <span data-ttu-id="953e2-113">También debe tener una de las siguientes versiones admitidas de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-113">You must also have one of the following supported versions of Finance and Operations.</span></span> <span data-ttu-id="953e2-114">Use la información de la siguiente tabla para evaluar si su entorno de hardware y software está listo para admitir la instalación.</span><span class="sxs-lookup"><span data-stu-id="953e2-114">Use the information in the following table to evaluate if your hardware and software environment is ready to support the installation.</span></span>

| <span data-ttu-id="953e2-115">Plataforma</span><span class="sxs-lookup"><span data-stu-id="953e2-115">Platform</span></span>                    | <span data-ttu-id="953e2-116">Versión</span><span class="sxs-lookup"><span data-stu-id="953e2-116">Version</span></span>                                                                                                                                                                     |
|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="953e2-117">Android</span><span class="sxs-lookup"><span data-stu-id="953e2-117">Android</span></span>                     | <span data-ttu-id="953e2-118">4.4, 5.0, 6.0</span><span class="sxs-lookup"><span data-stu-id="953e2-118">4.4, 5.0, 6.0</span></span>                                                                                                                                                               |
| <span data-ttu-id="953e2-119">Windows (UWP)</span><span class="sxs-lookup"><span data-stu-id="953e2-119">Windows (UWP)</span></span>               | <span data-ttu-id="953e2-120">Windows 10 (todas las versiones)</span><span class="sxs-lookup"><span data-stu-id="953e2-120">Windows 10 (all versions)</span></span>                                                                                                                                                   |
| <span data-ttu-id="953e2-121">Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="953e2-121">Finance and Operations</span></span> | <span data-ttu-id="953e2-122">Versión 1611 de Microsoft Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="953e2-122">Microsoft Finance and Operations version 1611</span></span> <br><span data-ttu-id="953e2-123">– O bien –</span><span class="sxs-lookup"><span data-stu-id="953e2-123">-or-</span></span> <br><span data-ttu-id="953e2-124">La versión 7.0/7.0.1 de Microsoft Dynamics Dynamics AX y la plataforma de Microsoft Dynamics AX actualización 2 con la revisión KB 3210014</span><span class="sxs-lookup"><span data-stu-id="953e2-124">Microsoft Dynamics Dynamics AX version 7.0/7.0.1 and Microsoft Dynamics AX platform update 2 with hotfix KB 3210014</span></span> |

## <a name="get-the-app"></a><span data-ttu-id="953e2-125">Obtenga la aplicación</span><span class="sxs-lookup"><span data-stu-id="953e2-125">Get the app</span></span>
-   <span data-ttu-id="953e2-126">Windows (UWP): [Finance and Operations - Warehousing en Windows Store](https://www.microsoft.com/store/apps/9p1bffd5tstm)</span><span class="sxs-lookup"><span data-stu-id="953e2-126">Windows (UWP): [Finance and Operations - Warehousing on the Windows Store](https://www.microsoft.com/store/apps/9p1bffd5tstm)</span></span>
-   <span data-ttu-id="953e2-127">Android:</span><span class="sxs-lookup"><span data-stu-id="953e2-127">Android:</span></span>
    - [<span data-ttu-id="953e2-128">Finance and Operations - Warehousing en Google Play Store</span><span class="sxs-lookup"><span data-stu-id="953e2-128">Finance and Operations - Warehousing on the Google Play Store</span></span>](https://play.google.com/store/apps/details?id=com.Microsoft.Dynamics365forOperationsWarehousing)
    - [<span data-ttu-id="953e2-129">Finance and Operations - Warehousing en Zebra App Gallery</span><span class="sxs-lookup"><span data-stu-id="953e2-129">Finance and Operations - Warehousing on the Zebra App Gallery</span></span>](https://appgallery.zebra.com/showcase/apps/146?type=showcase)

## <a name="create-a-web-service-application-in-active-directory"></a><span data-ttu-id="953e2-130">Crear una aplicación de servicio Web en Active Directory</span><span class="sxs-lookup"><span data-stu-id="953e2-130">Create a web service application in Active Directory</span></span>
<span data-ttu-id="953e2-131">Para habilitar la aplicación para que interactúe con un servidor específico de Finance and Operations, debe registrar una aplicación de servicio Web en un Azure Active Directory para el inquilino de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-131">To enable the app to interact with a specific Finance and Operations server, you must register a web service application in a Azure Active Directory for the Finance and Operations tenant.</span></span> <span data-ttu-id="953e2-132">Por razones de seguridad, se recomienda que cree una aplicación de servicio Web para cada dispositivo que utilice.</span><span class="sxs-lookup"><span data-stu-id="953e2-132">For security reasons, we recommend that you create a web service application for each device that you use.</span></span> <span data-ttu-id="953e2-133">Para crear una solicitud de servicio Web en Azure Active Directory (Azure AD), realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="953e2-133">To create a web service application in Azure Active Directory (Azure AD), complete the following steps:</span></span>

1.  <span data-ttu-id="953e2-134">En un explorador web, vaya a <https://manage.windowsazure.com>.</span><span class="sxs-lookup"><span data-stu-id="953e2-134">In a web browser, go to <https://manage.windowsazure.com>.</span></span>
2.  <span data-ttu-id="953e2-135">Especifique el nombre y la contraseña del usuario que tiene acceso a la suscripción de Azure.</span><span class="sxs-lookup"><span data-stu-id="953e2-135">Enter the name and password for the user who has access to the Azure subscription.</span></span>
3.  <span data-ttu-id="953e2-136">En Azure Portal, en el panel de navegación izquierdo, haga clic en **Active Directory**.[](./media/wh-01-active-directory-example.png)[![wh-01-active-directory-example](./media/wh-01-active-directory-example.png)](./media/wh-01-active-directory-example.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-136">In Azure Portal, in the left navigation pane, click **Active Directory**.[](./media/wh-01-active-directory-example.png)[![wh-01-active-directory-example](./media/wh-01-active-directory-example.png)](./media/wh-01-active-directory-example.png)</span></span>
4.  <span data-ttu-id="953e2-137">En la cuadrícula, seleccione la instancia de Active Directory que usa Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-137">In the grid, select the Active Directory instance that is used by Finance and Operations.</span></span>
5.  <span data-ttu-id="953e2-138">En la barra de herramientas superior, haga clic en **Solicitudes**.</span><span class="sxs-lookup"><span data-stu-id="953e2-138">On the top toolbar, click **Applications**.</span></span> <span data-ttu-id="953e2-139">[![wh-02-active-directory-applications](./media/wh-02-active-directory-applications-1024x197.png)](./media/wh-02-active-directory-applications.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-139">[![wh-02-active-directory-applications](./media/wh-02-active-directory-applications-1024x197.png)](./media/wh-02-active-directory-applications.png)</span></span>
6.  <span data-ttu-id="953e2-140">En el panel inferior, haga clic en **Agregar**.</span><span class="sxs-lookup"><span data-stu-id="953e2-140">In the bottom pane, click **Add**.</span></span> <span data-ttu-id="953e2-141">Se inicia el asistente de **Agregar aplicación**.</span><span class="sxs-lookup"><span data-stu-id="953e2-141">The **Add application** wizard starts.</span></span>
7.  <span data-ttu-id="953e2-142">Escriba un nombre para la aplicación y seleccione **Aplicación web y/o API web**.</span><span class="sxs-lookup"><span data-stu-id="953e2-142">Enter a name for the application and select **Web application and/or web API**.</span></span> <span data-ttu-id="953e2-143">[![wh-03-active-directory-add-application](./media/wh-03-active-directory-add-application.png)](./media/wh-03-active-directory-add-application.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-143">[![wh-03-active-directory-add-application](./media/wh-03-active-directory-add-application.png)](./media/wh-03-active-directory-add-application.png)</span></span>
8.  <span data-ttu-id="953e2-144">Indique la dirección URL de inicio de sesión, que es la dirección URL de la aplicación web.</span><span class="sxs-lookup"><span data-stu-id="953e2-144">Enter the sign-on URL, which is your web app URL.</span></span> <span data-ttu-id="953e2-145">Esta dirección URL es la misma que la dirección URL de la implementación, pero se añade oauth al final.</span><span class="sxs-lookup"><span data-stu-id="953e2-145">This URL is the same as your deployment URL, but oauth is added to the end.</span></span> <span data-ttu-id="953e2-146">Indique el URI del identificador de la aplicación, este valor es obligatorio, pero no se requiere para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="953e2-146">Enter the App ID URI, this value is mandatory, but isn’t required for the authentication.</span></span> <span data-ttu-id="953e2-147">Asegúrese de que el URI de este identificador de la aplicación sea un URI simulado https://contosooperations/wmapp, ya que el uso de la dirección URL de la implementación puede provocar problemas de inicio de sesión en otras aplicaciones AAD como el complemento de Excel.</span><span class="sxs-lookup"><span data-stu-id="953e2-147">Make sure that this App ID URI is a mock URI like https://contosooperations/wmapp, since using the URL of your deployment can cause sign-in issues in other AAD applications such as the Excel Add-in.</span></span> <span data-ttu-id="953e2-148">[![WH-04-AD-add-properties3](./media/WH-04-AD-add-properties3.png)](./media/WH-04-AD-add-properties3.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-148">[![WH-04-AD-add-properties3](./media/WH-04-AD-add-properties3.png)](./media/WH-04-AD-add-properties3.png)</span></span>
9.  <span data-ttu-id="953e2-149">Vaya a la pestaña **Configurar**. [![wh-05-ad-configure-app](./media/wh-05-ad-configure-app.png)](./media/wh-05-ad-configure-app.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-149">Go to the **Configure** tab. [![wh-05-ad-configure-app](./media/wh-05-ad-configure-app.png)](./media/wh-05-ad-configure-app.png)</span></span>
10. <span data-ttu-id="953e2-150">Desplácese hasta que vea la sección **Permisos para otras aplicaciones**.</span><span class="sxs-lookup"><span data-stu-id="953e2-150">Scroll down until you see the **Permissions to other applications** section.</span></span> <span data-ttu-id="953e2-151">Haga clic en **Agregar aplicación**.</span><span class="sxs-lookup"><span data-stu-id="953e2-151">Click **Add application**.</span></span> <span data-ttu-id="953e2-152">[![wh-06-ad-app-add-permissions](./media/wh-06-ad-app-add-permissions.png)](./media/wh-06-ad-app-add-permissions.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-152">[![wh-06-ad-app-add-permissions](./media/wh-06-ad-app-add-permissions.png)](./media/wh-06-ad-app-add-permissions.png)</span></span>
11. <span data-ttu-id="953e2-153">Seleccione **Microsoft Dynamics ERP** en la lista.</span><span class="sxs-lookup"><span data-stu-id="953e2-153">Select **Microsoft Dynamics ERP** in the list.</span></span> <span data-ttu-id="953e2-154">Haga clic en el botón **Comprobación completa** en la esquina derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="953e2-154">Click the **Complete check** button in the right corner of the page.</span></span> <span data-ttu-id="953e2-155">[![wh-07-ad-select-permissions](./media/wh-07-ad-select-permissions.png)](./media/wh-07-ad-select-permissions.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-155">[![wh-07-ad-select-permissions](./media/wh-07-ad-select-permissions.png)](./media/wh-07-ad-select-permissions.png)</span></span>
12. <span data-ttu-id="953e2-156">En la lista **Delegar permisos**, seleccione todas las casillas.</span><span class="sxs-lookup"><span data-stu-id="953e2-156">In the **Delegate Permissions** list, select all the check boxes.</span></span> <span data-ttu-id="953e2-157">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="953e2-157">Click **Save**.</span></span> <span data-ttu-id="953e2-158">[![wh-08-ad-delegate-permissions](./media/wh-08-ad-delegate-permissions.png)](./media/wh-08-ad-delegate-permissions.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-158">[![wh-08-ad-delegate-permissions](./media/wh-08-ad-delegate-permissions.png)](./media/wh-08-ad-delegate-permissions.png)</span></span>
13. <span data-ttu-id="953e2-159">Tenga en cuenta la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="953e2-159">Make a note of the following information:</span></span>
    -   <span data-ttu-id="953e2-160">**Id. de cliente** - A medida que se desplaza hacia arriba en la página, verá **Id. de cliente**.</span><span class="sxs-lookup"><span data-stu-id="953e2-160">**Client ID** - As you scroll up the page, you will see **Client ID** displayed.</span></span>
    -   <span data-ttu-id="953e2-161">**Clave** - En la sección **Claves** cree una clave seleccionando la duración y copie la clave.</span><span class="sxs-lookup"><span data-stu-id="953e2-161">**Key** - In the **Keys** section, create a key by selecting duration, and copy the key.</span></span> <span data-ttu-id="953e2-162">Posteriormente se hará referencia a esta clave como **Secreto de cliente**.</span><span class="sxs-lookup"><span data-stu-id="953e2-162">This key will later be referred to as the **Client secret**.</span></span>

## <a name="create-and-configure-a-user-account-in-finance-and-operations"></a><span data-ttu-id="953e2-163">Crear y configurar una cuenta de usuario en Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="953e2-163">Create and configure a user account in Finance and Operations</span></span>
<span data-ttu-id="953e2-164">Para que Finance and Operations pueda utilizar su aplicación Azure AD, debe completar los siguientes pasos de configuración:</span><span class="sxs-lookup"><span data-stu-id="953e2-164">To enable Finance and Operations to use your Azure AD application, you need to complete the following configuration steps:</span></span>

1.  <span data-ttu-id="953e2-165">Cree una nueva cuenta de usuario en Azure Active Directory para el inquilino de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-165">Create a new user account in Azure Active Directory for the Finance and Operations tenant.</span></span> <span data-ttu-id="953e2-166">El propósito de esta cuenta de usuario es tener acceso al servicio personalizado específico de la aplicación Warehousing a la que se expone el servidor de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-166">The purpose of this user account is to access the specific custom service of the warehousing app, which the Finance and Operations server exposes.</span></span> <span data-ttu-id="953e2-167">Tras completar este paso, tendrá credenciales del usuario de WMDP, compuestas por una dirección de correo electrónico de WMDP y una contraseña de WMDP.</span><span class="sxs-lookup"><span data-stu-id="953e2-167">After completing this step, you will have WMDP user credentials, which consist of a WMDP email address and a WMDP password.</span></span> <span data-ttu-id="953e2-168">Para obtener información acerca de los pasos básicos para agregar usuarios a Azure AD y Finance and Operations, consulte a este tutorial: [Inscríbase para suscribirse a Finance and Operations](../../dev-itpro/dev-tools/sign-up-preview-subscription.md).</span><span class="sxs-lookup"><span data-stu-id="953e2-168">To learn about the basic steps for adding users to Azure AD and Finance and Operations, refer to this tutorial: [Sign up for a Finance and Operations subscription](../../dev-itpro/dev-tools/sign-up-preview-subscription.md).</span></span>
2.  <span data-ttu-id="953e2-169">Crear un usuario de Finance and Operations correspondiente a las credenciales de usuario de la aplicación Warehousing.</span><span class="sxs-lookup"><span data-stu-id="953e2-169">Create a Finance and Operations user that corresponds to the warehousing app user credentials.</span></span>
    1.  <span data-ttu-id="953e2-170">En Finance and Operations, vaya a **Administración del sistema** &gt; **Común** &gt; **Usuarios**.</span><span class="sxs-lookup"><span data-stu-id="953e2-170">In Finance and Operations, go to **System administration** &gt; **Common** &gt; **Users**.</span></span>
    2.  <span data-ttu-id="953e2-171">Cree un nuevo usuario.</span><span class="sxs-lookup"><span data-stu-id="953e2-171">Create a new user.</span></span>
    3.  <span data-ttu-id="953e2-172">Asigne el usuario del dispositivo móvil de almacén como se muestra en el captura de pantalla siguiente.</span><span class="sxs-lookup"><span data-stu-id="953e2-172">Assign the Warehouse mobile device user, as shown in the following screenshot.</span></span> <span data-ttu-id="953e2-173">[![wh-09-add-user-security-role](./media/wh-09-add-user-security-role.png)](./media/wh-09-add-user-security-role.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-173">[![wh-09-add-user-security-role](./media/wh-09-add-user-security-role.png)](./media/wh-09-add-user-security-role.png)</span></span>

3.  <span data-ttu-id="953e2-174">Asocie su aplicación Azure Active Directory con el usuario de la aplicación Warehousing.</span><span class="sxs-lookup"><span data-stu-id="953e2-174">Associate your Azure Active Directory application with the warehousing app user.</span></span>
    1.  <span data-ttu-id="953e2-175">En Finance and Operations, vaya a **Administración del sistema** &gt; **Configuración** &gt; **Aplicaciones de Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="953e2-175">In Finance and Operations, go to **System administration** &gt; **Setup** &gt; **Azure Active Directory applications**.</span></span>
    2.  <span data-ttu-id="953e2-176">Cree una línea nueva.</span><span class="sxs-lookup"><span data-stu-id="953e2-176">Create a new line.</span></span>
    3.  <span data-ttu-id="953e2-177">Introduzca el **Id. de cliente** (obtenido en la última sección), asígnele un nombre y seleccione el usuario creado previamente.</span><span class="sxs-lookup"><span data-stu-id="953e2-177">Enter the **Client ID** (obtained in the last section), give it a name, and select the previously created user.</span></span> <span data-ttu-id="953e2-178">Recomendamos que etiquete todos los dispositivos de modo que pueda quitar fácilmente su acceso a Finance and Operations de esta página en caso de que se pierdan.</span><span class="sxs-lookup"><span data-stu-id="953e2-178">We recommend that you tag all your devices so that you can easily remove their access to Finance and Operations from this page in case they are lost.</span></span> <span data-ttu-id="953e2-179">[![wh-10-ad-applications-form](./media/wh-10-ad-applications-form.png)](./media/wh-10-ad-applications-form.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-179">[![wh-10-ad-applications-form](./media/wh-10-ad-applications-form.png)](./media/wh-10-ad-applications-form.png)</span></span>

## <a name="configure-the-application"></a><span data-ttu-id="953e2-180">Configurar la aplicación</span><span class="sxs-lookup"><span data-stu-id="953e2-180">Configure the application</span></span>
<span data-ttu-id="953e2-181">Debe configurar la aplicación en el dispositivo para conectarse al servidor Finance and Operations a través de la aplicación Azure AD.</span><span class="sxs-lookup"><span data-stu-id="953e2-181">You must configure the app on the device to connect to the Finance and Operations server through the Azure AD application.</span></span> <span data-ttu-id="953e2-182">Para ello, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="953e2-182">To do this, complete the following steps.</span></span>

1.  <span data-ttu-id="953e2-183">En la aplicación, vaya a **Configuración de la conexión**.</span><span class="sxs-lookup"><span data-stu-id="953e2-183">In the app, go to **Connection settings**.</span></span>
2.  <span data-ttu-id="953e2-184">Borre el campo **Modo de demostración**.</span><span class="sxs-lookup"><span data-stu-id="953e2-184">Clear the **Demo mode** field.</span></span> <br><span data-ttu-id="953e2-185">[![wh-11-app-connection-settings-demo-mode](./media/wh-11-app-connection-settings-demo-mode-169x300.png)](./media/wh-11-app-connection-settings-demo-mode.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-185">[![wh-11-app-connection-settings-demo-mode](./media/wh-11-app-connection-settings-demo-mode-169x300.png)](./media/wh-11-app-connection-settings-demo-mode.png)</span></span>
3.  <span data-ttu-id="953e2-186">Especifique la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="953e2-186">Enter the following information:</span></span> 
    + <span data-ttu-id="953e2-187">**Id. de cliente de Azure Active Directory** - El identificador secreto de cliente se obtiene en el paso 13 en "Crear una aplicación de servicio Web en Active Directory".</span><span class="sxs-lookup"><span data-stu-id="953e2-187">**Azure Active directory client ID** - The client ID is obtained in step 13 in "Create a web service application in Active Directory".</span></span> 
    + <span data-ttu-id="953e2-188">**Secreto de cliente de Azure Active Directory** - El secreto de cliente se obtiene en el paso 13 en "Crear una aplicación de servicio Web en Active Directory".</span><span class="sxs-lookup"><span data-stu-id="953e2-188">**Azure Active directory client secret** - The client secret is obtained in step 13 in "Create a web service application in Active Directory".</span></span> 
    + <span data-ttu-id="953e2-189">**Recurso de Azure Active Directory** - El recurso del directorio Azure AD representa la URL raíz de Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="953e2-189">**Azure Active directory resource** - The Azure AD directory resource depicts the Finance and Operations root URL.</span></span> <span data-ttu-id="953e2-190">**Nota**: No termine este campo con un carácter de barra diagonal (/).</span><span class="sxs-lookup"><span data-stu-id="953e2-190">**Note**: Do not end this field with a forward slash character (/).</span></span> 
    + <span data-ttu-id="953e2-191">**Inquilino de Azure Active Directory**- El inquilino del directorio Azure AD empleado con el servidor de Finance and Operations: https://login.windows.net/your-AD-tenant-ID.</span><span class="sxs-lookup"><span data-stu-id="953e2-191">**Azure Active directory tenant** - The Azure AD directory tenant used with the Finance and Operations server: https://login.windows.net/your-AD-tenant-ID.</span></span> <span data-ttu-id="953e2-192">Por ejemplo: https://login.windows.net/contosooperations.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="953e2-192">For example: https://login.windows.net/contosooperations.onmicrosoft.com.</span></span>
    <br><span data-ttu-id="953e2-193">**Nota**: No termine este campo con un carácter de barra diagonal (/).</span><span class="sxs-lookup"><span data-stu-id="953e2-193">**Note**: Do not end this field with a forward slash character (/).</span></span> 
    + <span data-ttu-id="953e2-194">**Empresa** - Especifique la entidad jurídica en Finance and Operations a la que desea que se conecte la aplicación.</span><span class="sxs-lookup"><span data-stu-id="953e2-194">**Company** - Enter the legal entity in Finance and Operations to which you want the application to connect.</span></span> <br><span data-ttu-id="953e2-195">[![wh-12-app-connection-settings](./media/wh-12-app-connection-settings-169x300.png)](./media/wh-12-app-connection-settings.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-195">[![wh-12-app-connection-settings](./media/wh-12-app-connection-settings-169x300.png)](./media/wh-12-app-connection-settings.png)</span></span>
4.  <span data-ttu-id="953e2-196">Seleccione el botón **Atrás** en la esquina superior izquierda de la aplicación.</span><span class="sxs-lookup"><span data-stu-id="953e2-196">Select the **Back** button in the top-left corner of the application.</span></span> <span data-ttu-id="953e2-197">La aplicación se conectará ahora a su servidor Finance and Operations y aparecerá la pantalla de inicio de sesión del trabajador de almacén.</span><span class="sxs-lookup"><span data-stu-id="953e2-197">The application will now connect to your Finance and Operations server and the log-in screen for the warehouse worker will display.</span></span> <br><span data-ttu-id="953e2-198">[![wh-13-log-in-screen](./media/wh-13-log-in-screen-180x300.png)](./media/wh-13-log-in-screen.png)</span><span class="sxs-lookup"><span data-stu-id="953e2-198">[![wh-13-log-in-screen](./media/wh-13-log-in-screen-180x300.png)](./media/wh-13-log-in-screen.png)</span></span>

## <a name="remove-access-for-a-device"></a><span data-ttu-id="953e2-199">Quitar el acceso de un dispositivo</span><span class="sxs-lookup"><span data-stu-id="953e2-199">Remove access for a device</span></span>
<span data-ttu-id="953e2-200">En caso de un dispositivo perdido o defectuoso, debe quitar el acceso a Finance and Operations del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="953e2-200">In case of a lost or compromised device, you must remove access to Finance and Operations for the device.</span></span> <span data-ttu-id="953e2-201">Los siguientes pasos describen el proceso recomendado para quitar acceso.</span><span class="sxs-lookup"><span data-stu-id="953e2-201">The following steps describe the recommended process to remove access.</span></span>

1.  <span data-ttu-id="953e2-202">En Finance and Operations, vaya a **Administración del sistema** &gt; **Configuración** &gt; **Aplicaciones de Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="953e2-202">In Finance and Operations, go to **System administration** &gt; **Setup** &gt; **Azure Active Directory applications**.</span></span>
2.  <span data-ttu-id="953e2-203">Elimine la línea correspondiente al dispositivo del que desea eliminar el acceso.</span><span class="sxs-lookup"><span data-stu-id="953e2-203">Delete the line that corresponds to the device to which you want to remove access.</span></span> <span data-ttu-id="953e2-204">Anote el **Id. de cliente** utilizado para el dispositivo quitado.</span><span class="sxs-lookup"><span data-stu-id="953e2-204">Note down the **Client ID** used for the removed device.</span></span>
3.  <span data-ttu-id="953e2-205">Inicie sesión en el portal clásico de Azure en <https://manage.windowsazure.com>.</span><span class="sxs-lookup"><span data-stu-id="953e2-205">Sign in the Azure classic portal at <https://manage.windowsazure.com>.</span></span>
4.  <span data-ttu-id="953e2-206">Haga clic en el icono de **Active Directory** en el menú izquierdo y haga clic en el directorio deseado.</span><span class="sxs-lookup"><span data-stu-id="953e2-206">Click the **Active Directory** icon on the left menu, and then click the desired directory.</span></span>
5.  <span data-ttu-id="953e2-207">En el menú superior, haga clic en **Aplicaciones** y, a continuación, haga clic en la aplicación que desea configurar.</span><span class="sxs-lookup"><span data-stu-id="953e2-207">On the top menu, click **Applications**, and then click the application you want to configure.</span></span> <span data-ttu-id="953e2-208">Aparecerá la página de **Inicio rápido** con el inicio de sesión único y otra información de configuración.</span><span class="sxs-lookup"><span data-stu-id="953e2-208">The **Quick Start** page will appear with single sign-on and other configuration information.</span></span>
6.  <span data-ttu-id="953e2-209">Haga clic en la pestaña **Configurar**, desplácese hacia abajo y asegúrese de que el **Id. de cliente** de la aplicación sea el mismo que en el paso 2 de esta sección.</span><span class="sxs-lookup"><span data-stu-id="953e2-209">Click the **Configure** tab, scroll down and ensure that the **Client ID** of the application is the same as in step 2 in this section.</span></span>
7.  <span data-ttu-id="953e2-210">Haga clic en el botón **Eliminar** de la barra de comandos.</span><span class="sxs-lookup"><span data-stu-id="953e2-210">Click the **Delete** button in the command bar.</span></span>
8.  <span data-ttu-id="953e2-211">Haga clic en **Sí** en el mensaje de confirmación.</span><span class="sxs-lookup"><span data-stu-id="953e2-211">Click **Yes** in the confirmation message.</span></span>




