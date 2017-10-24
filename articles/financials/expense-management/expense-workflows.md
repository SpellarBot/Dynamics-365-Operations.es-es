---
title: Configurar flujos de trabajo de los gastos
description: Puede configurar un proceso de flujo de trabajo que se usa para revisar y aprobar documentos de gastos y viajes.
author: saraschi2
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.search.region: Global
ms.author: saraschi2
ms.search.validFrom:
- month/year of release that feature was introduced in
- in format yyyy-mm-dd
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: eb8ff11a03ba18b78595cd04f63b2456aec53bf2
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---

# <a name="set-up-workflows-for-expense"></a><span data-ttu-id="9d56b-103">Configurar flujos de trabajo de los gastos</span><span class="sxs-lookup"><span data-stu-id="9d56b-103">Set up workflows for expense</span></span>

[!include[banner](../includes/banner.md)]<span data-ttu-id="9d56b-104"> Puede configurar un proceso de flujo de trabajo que se usa para revisar y aprobar documentos de gastos y viajes.</span><span class="sxs-lookup"><span data-stu-id="9d56b-104"> You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="9d56b-105">Los documentos para los que pueden definirse los flujos de trabajo incluyen informes de gastos, pedidos de viaje y solicitudes de anticipo.</span><span class="sxs-lookup"><span data-stu-id="9d56b-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="9d56b-106">Un flujo de trabajo representa un proceso empresarial.</span><span class="sxs-lookup"><span data-stu-id="9d56b-106">A workflow represents a business process.</span></span> <span data-ttu-id="9d56b-107">El flujo de trabajo define cómo se gestiona un documento en el sistema e indica quién debe completar una tarea o aprobar un documento.</span><span class="sxs-lookup"><span data-stu-id="9d56b-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="9d56b-108">El uso del sistema de flujo de trabajo en su organización le ofrece varias ventajas:</span><span class="sxs-lookup"><span data-stu-id="9d56b-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="9d56b-109">**Procesos coherentes**: puede definir el proceso de aprobación para documentos específicos como, por ejemplo, solicitudes de compra e informes de gastos.</span><span class="sxs-lookup"><span data-stu-id="9d56b-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="9d56b-110">El sistema de flujo de trabajo le ayuda a garantizar que los documentos se procesan y se aprueban de manera coherente y eficaz.</span><span class="sxs-lookup"><span data-stu-id="9d56b-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="9d56b-111">Visibilidad de procesos: puede realizar el seguimiento del estado, el historial y las medidas de rendimiento de una instancia de flujo de trabajo determinada.</span><span class="sxs-lookup"><span data-stu-id="9d56b-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="9d56b-112">De este modo puede determinar si los cambios deben realizarse en el flujo de trabajo para mejorar la eficacia.</span><span class="sxs-lookup"><span data-stu-id="9d56b-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="9d56b-113">Lista de trabajo centralizada: los usuarios pueden ver una lista de trabajo centralizada para ver las tareas y aprobaciones de flujo de trabajo que tienen asignadas.</span><span class="sxs-lookup"><span data-stu-id="9d56b-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="9d56b-114">**Tipos de flujo de trabajo que puede crear**</span><span class="sxs-lookup"><span data-stu-id="9d56b-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="9d56b-115">En la siguiente tabla se describen los tipos de flujo de trabajo que se pueden crear en **Gastos**.</span><span class="sxs-lookup"><span data-stu-id="9d56b-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>

| <span data-ttu-id="9d56b-116">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="9d56b-116">**Type**</span></span>                           | <span data-ttu-id="9d56b-117">**Use este tipo para**</span><span class="sxs-lookup"><span data-stu-id="9d56b-117">**Use this type to**</span></span>                                                 |     
|------------------------------------|----------------------------------------------------------------------|
| <span data-ttu-id="9d56b-118">**Informe de gastos**</span><span class="sxs-lookup"><span data-stu-id="9d56b-118">**Expense report**</span></span>                 | <span data-ttu-id="9d56b-119">Cree flujos de trabajo de aprobación para los informes de gastos.</span><span class="sxs-lookup"><span data-stu-id="9d56b-119">Create approval workflows for expense reports.</span></span>                       |      
| <span data-ttu-id="9d56b-120">**Registro automático de informe de gastos**</span><span class="sxs-lookup"><span data-stu-id="9d56b-120">**Expense report auto posting**</span></span>    | <span data-ttu-id="9d56b-121">Cree flujos de trabajo del registro automático para los informes de gastos.</span><span class="sxs-lookup"><span data-stu-id="9d56b-121">Create automatic posting workflows for expense reports.</span></span>              |     
| <span data-ttu-id="9d56b-122">**Elemento de línea de gastos**</span><span class="sxs-lookup"><span data-stu-id="9d56b-122">**Expense line item**</span></span>              | <span data-ttu-id="9d56b-123">Cree flujos de trabajo de aprobación para los artículos de línea en los informes de gastos.</span><span class="sxs-lookup"><span data-stu-id="9d56b-123">Create approval workflows for line items on expense reports.</span></span>         |     
| <span data-ttu-id="9d56b-124">**Registro automático de artículo de línea de gasto**</span><span class="sxs-lookup"><span data-stu-id="9d56b-124">**Expense line item auto posting**</span></span> | <span data-ttu-id="9d56b-125">Cree flujos de trabajo de registro automático para los artículos de línea en los informes de gastos.</span><span class="sxs-lookup"><span data-stu-id="9d56b-125">Create automatic posting workflows for line items on expense reports.</span></span>|
| <span data-ttu-id="9d56b-126">**Pedido de viaje**</span><span class="sxs-lookup"><span data-stu-id="9d56b-126">**Travel requisition**</span></span>             | <span data-ttu-id="9d56b-127">Cree flujos de trabajo de aprobación para solicitudes de viaje.</span><span class="sxs-lookup"><span data-stu-id="9d56b-127">Create approval workflows for travel requisitions.</span></span>                   |    
| <span data-ttu-id="9d56b-128">**Solicitud de anticipo**</span><span class="sxs-lookup"><span data-stu-id="9d56b-128">**Cash advance request**</span></span>           | <span data-ttu-id="9d56b-129">Cree flujos de aprobación para las solicitudes de anticipo.</span><span class="sxs-lookup"><span data-stu-id="9d56b-129">Create approval workflows for cash advance requests.</span></span>                 |     
| <span data-ttu-id="9d56b-130">**Devolución de impuestos de IVA**</span><span class="sxs-lookup"><span data-stu-id="9d56b-130">**VAT tax recovery**</span></span>               | <span data-ttu-id="9d56b-131">Cree flujos de trabajo de aprobación para la devolución del impuesto sobre el valor añadido (VAT).</span><span class="sxs-lookup"><span data-stu-id="9d56b-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span> |       
