--- 
title: Crear una regla kanban de eventos de ventas
description: "Este procedimiento se centra en la configuración necesaria para crear una regla kanban que se activará durante la creación de pedidos de ventas."
author: ChristianRytt
manager: AnnBe
ms.date: 03/02/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: f1f66157b2e74ad1b490e10112cbc121ac9826fb
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---
# <a name="create-a-sales-event-kanban-rule"></a><span data-ttu-id="1d029-103">Crear una regla kanban de eventos de ventas</span><span class="sxs-lookup"><span data-stu-id="1d029-103">Create a sales event kanban rule</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="1d029-104">Este procedimiento se centra en la configuración necesaria para crear una regla kanban que se activará durante la creación de pedidos de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-104">This procedure focuses on the setup needed to create a kanban rule that is triggered during sales order creation.</span></span> <span data-ttu-id="1d029-105">La regla kanban de evento reaprovisiona los requisitos que se originan de las líneas de pedidos de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-105">The event kanban rule replenishes requirements that originate from sales order lines.</span></span> <span data-ttu-id="1d029-106">La empresa de datos de prueba utilizada para crear este procedimiento es USMF.</span><span class="sxs-lookup"><span data-stu-id="1d029-106">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="1d029-107">Está pensado para el ingeniero de procesos o el administrador de flujo de valor, ya que preparan la producción de un producto nuevo o modificado.</span><span class="sxs-lookup"><span data-stu-id="1d029-107">It is intended for the process engineer or the value stream manager as they prepare production of a new or modified product.</span></span>




## <a name="create-a-new-kanban-rule"></a><span data-ttu-id="1d029-108">Crear una nueva regla kanban</span><span class="sxs-lookup"><span data-stu-id="1d029-108">Create a new kanban rule</span></span>
1. <span data-ttu-id="1d029-109">Vaya a Reglas kanban.</span><span class="sxs-lookup"><span data-stu-id="1d029-109">Go to Kanban rules.</span></span>
2. <span data-ttu-id="1d029-110">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="1d029-110">Click New.</span></span>
3. <span data-ttu-id="1d029-111">En el campo Estrategia de reabastecimiento, seleccione "Evento".</span><span class="sxs-lookup"><span data-stu-id="1d029-111">In the Replenishment strategy field, select 'Event'.</span></span>
    * <span data-ttu-id="1d029-112">La selección de evento significa que la regla kanban se activa por un evento, por ejemplo, la creación de una línea de pedido de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-112">Selecting Event means that the kanban rule is triggered by an event, for example, creation of a sales order line.</span></span>   <span data-ttu-id="1d029-113">Esto se aplica a áreas donde cada kanban debe cubrir una demanda específica.</span><span class="sxs-lookup"><span data-stu-id="1d029-113">This is applied to areas where each kanban should cover a specific demand.</span></span>  
4. <span data-ttu-id="1d029-114">En el campo Actividad del primer plan, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="1d029-114">In the First plan activity field, enter or select a value.</span></span>
    * <span data-ttu-id="1d029-115">Seleccione Ensamblado final.</span><span class="sxs-lookup"><span data-stu-id="1d029-115">Select Final assembly.</span></span>  
5. <span data-ttu-id="1d029-116">Expanda la sección Detalles.</span><span class="sxs-lookup"><span data-stu-id="1d029-116">Expand the Details section.</span></span>
6. <span data-ttu-id="1d029-117">En el campo Producto, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="1d029-117">In the Product field, enter or select a value.</span></span>
    * <span data-ttu-id="1d029-118">Seleccione L0050.</span><span class="sxs-lookup"><span data-stu-id="1d029-118">Select L0050.</span></span>  

## <a name="define-an-event"></a><span data-ttu-id="1d029-119">Definir un evento</span><span class="sxs-lookup"><span data-stu-id="1d029-119">Define an event</span></span>
1. <span data-ttu-id="1d029-120">Expanda la sección Eventos.</span><span class="sxs-lookup"><span data-stu-id="1d029-120">Expand the Events section.</span></span>
2. <span data-ttu-id="1d029-121">En el campo Evento de ventas, seleccione "Automático".</span><span class="sxs-lookup"><span data-stu-id="1d029-121">In the Sales event field, select 'Automatic'.</span></span>
    * <span data-ttu-id="1d029-122">Al seleccionar el evento de ventas Automático, esta regla kanban se activará automáticamente cuando una línea de ventas coincida con el producto y la ubicación de recepción.</span><span class="sxs-lookup"><span data-stu-id="1d029-122">By selecting the sales event Automatic, this kanban rule will be triggered automatically when a sales line matches the product and receipt location.</span></span> <span data-ttu-id="1d029-123">En este procedimiento, es el producto L0050 del almacén 13.</span><span class="sxs-lookup"><span data-stu-id="1d029-123">In this procedure, it is product L0050 on warehouse 13.</span></span>  
3. <span data-ttu-id="1d029-124">Establezca la Cantidad mínima de eventos en "50".</span><span class="sxs-lookup"><span data-stu-id="1d029-124">Set Minimum event quantity to '50'.</span></span>
    * <span data-ttu-id="1d029-125">Con una cantidad de evento mínima de 50, la regla kanban solo se activará por eventos con una cantidad de 50 o más.</span><span class="sxs-lookup"><span data-stu-id="1d029-125">With a minimum event quantity of 50, the kanban rule will only be triggered by events with a quantity of 50 or more.</span></span>  
4. <span data-ttu-id="1d029-126">Expanda la sección Flujo de producción.</span><span class="sxs-lookup"><span data-stu-id="1d029-126">Expand the Production flow section.</span></span>
    * <span data-ttu-id="1d029-127">Observe que la Ubicación de recepción es el almacén 13.</span><span class="sxs-lookup"><span data-stu-id="1d029-127">Notice that the Receipt location is warehouse 13.</span></span> <span data-ttu-id="1d029-128">Esto significa que esta regla kanban se activará para esta ubicación.</span><span class="sxs-lookup"><span data-stu-id="1d029-128">This means that this kanban rule will be triggered for this location.</span></span>  
    * <span data-ttu-id="1d029-129">En este ejemplo, una línea de ventas para el producto L0050, con una cantidad de 50 o más, en el almacén 13, activará esta regla kanban.</span><span class="sxs-lookup"><span data-stu-id="1d029-129">In this example, a sales line for product L0050, with a quantity of 50 or more, on warehouse 13, will trigger this kanban rule.</span></span>  

## <a name="create-sales-line-to-trigger-event-kanban-rule"></a><span data-ttu-id="1d029-130">Crear línea de ventas para activar la regla kanban de evento</span><span class="sxs-lookup"><span data-stu-id="1d029-130">Create sales line to trigger event kanban rule</span></span>
1. <span data-ttu-id="1d029-131">Vaya a Todos los pedidos de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-131">Go to All sales orders.</span></span>
    * <span data-ttu-id="1d029-132">Se muestra una advertencia cuando se guarda la regla kanban, lo que significa que los kanbans se crearán en tiempo real durante la creación de pedidos de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-132">A warning is shown when the kanban rule is saved, which means that kanbans will be created in real-time during sales order creation.</span></span>  
2. <span data-ttu-id="1d029-133">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="1d029-133">Click New.</span></span>
3. <span data-ttu-id="1d029-134">En el campo Cuenta de cliente, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="1d029-134">In the Customer account field, enter or select a value.</span></span>
    * <span data-ttu-id="1d029-135">Por ejemplo, seleccione US-003.</span><span class="sxs-lookup"><span data-stu-id="1d029-135">For example, select US-003.</span></span>  
4. <span data-ttu-id="1d029-136">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="1d029-136">Click OK.</span></span>
5. <span data-ttu-id="1d029-137">En el campo Código de artículo, escriba 'L0050'.</span><span class="sxs-lookup"><span data-stu-id="1d029-137">In the Item number field, type 'L0050'.</span></span>
6. <span data-ttu-id="1d029-138">En el campo Sitio, escriba "1".</span><span class="sxs-lookup"><span data-stu-id="1d029-138">In the Site field, type '1'.</span></span>
    * <span data-ttu-id="1d029-139">Seleccione el sitio 1 porque el almacén 13 se encuentra en el sitio 1.</span><span class="sxs-lookup"><span data-stu-id="1d029-139">Select Site 1 because Warehouse 13 is on Site 1.</span></span>  
7. <span data-ttu-id="1d029-140">En el campo Almacén, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="1d029-140">In the Warehouse field, enter or select a value.</span></span>
    * <span data-ttu-id="1d029-141">Establezca el almacén en 13.</span><span class="sxs-lookup"><span data-stu-id="1d029-141">Set Warehouse to 13.</span></span>  
8. <span data-ttu-id="1d029-142">Establezca el valor de cantidad en '75'.</span><span class="sxs-lookup"><span data-stu-id="1d029-142">Set Quantity to '75'.</span></span>
    * <span data-ttu-id="1d029-143">Escriba una cantidad de 50 o superior, para activar la regla kanban creada.</span><span class="sxs-lookup"><span data-stu-id="1d029-143">Enter a quantity of 50 or greater, to trigger the created kanban rule.</span></span>  

## <a name="verify-that-kanban-is-created"></a><span data-ttu-id="1d029-144">Comprobar que se creó el kanban</span><span class="sxs-lookup"><span data-stu-id="1d029-144">Verify that kanban is created</span></span>
1. <span data-ttu-id="1d029-145">Haga clic en Producto y suministro.</span><span class="sxs-lookup"><span data-stu-id="1d029-145">Click Product and supply.</span></span>
2. <span data-ttu-id="1d029-146">Haga clic en Ver diagrama de árbol.</span><span class="sxs-lookup"><span data-stu-id="1d029-146">Click View pegging tree.</span></span>
    * <span data-ttu-id="1d029-147">Observe que se crea un kanban con la misma cantidad que la línea de ventas.</span><span class="sxs-lookup"><span data-stu-id="1d029-147">Notice that a kanban with the same quantity as the sales line is created.</span></span> <span data-ttu-id="1d029-148">También puede ver las emisiones de material necesarias para producir L0050.</span><span class="sxs-lookup"><span data-stu-id="1d029-148">You can also see the material issues needed to produce L0050.</span></span> <span data-ttu-id="1d029-149">Este es el último paso de este procedimiento.</span><span class="sxs-lookup"><span data-stu-id="1d029-149">This is the last step in this procedure.</span></span>  

