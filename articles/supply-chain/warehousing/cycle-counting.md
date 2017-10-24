---
title: "Recuento cíclico"
description: "Este artículo describe cómo puede usar el recuento cíclico con la solución de almacenamiento que está disponible en Gestión de almacenes. Este artículo no se aplica a la solución de almacenamiento que está disponible en Gestión de inventarios."
author: MarkusFogelberg
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: WHSCycleCountPlan, WHSCycleCountPlanListPage, WHSCycleCountThreshold, WHSWorkTableListPage
audience: Application User
ms.reviewer: bis
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 50671
ms.assetid: 49f5c431-b043-4170-aa24-b7d5d1ee063e
ms.search.region: Global
ms.author: mafoge
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 2437d3efe7841021ff4bd35f307fddddc76eb4c6
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---

# <a name="cycle-counting"></a><span data-ttu-id="9e4e5-104">Recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="9e4e5-104">Cycle counting</span></span>

[!include[banner](../includes/banner.md)]


<span data-ttu-id="9e4e5-105">Este artículo describe cómo puede usar el recuento cíclico con la solución de almacenamiento que está disponible en Gestión de almacenes.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-105">This article describes how you can use cycle counting with the warehousing solution that is available in Warehouse management.</span></span> <span data-ttu-id="9e4e5-106">Este artículo no se aplica a la solución de almacenamiento que está disponible en Gestión de inventarios.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-106">This article doesn't apply to the warehousing solution that's available in Inventory management.</span></span>

<span data-ttu-id="9e4e5-107">La cuenta de ciclo es un proceso de almacén que puede usar para revisar artículos de inventario disponibles.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-107">Cycle counting is a warehouse process that you can use to audit on-hand inventory items.</span></span> <span data-ttu-id="9e4e5-108">El proceso del recuento cíclico se puede describir en tres pasos:</span><span class="sxs-lookup"><span data-stu-id="9e4e5-108">The cycle counting process can be described in three steps:</span></span>

1.  <span data-ttu-id="9e4e5-109">**Crear un trabajo de recuento cíclico**: el trabajo recuento cíclico se pueden crear automáticamente en función de los parámetros de umbral para artículos o mediante un plan de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-109">**Create cycle counting work** – Cycle counting work can be created automatically, based on threshold parameters for items or by using a cycle counting plan.</span></span> <span data-ttu-id="9e4e5-110">También puede crear manualmente trabajos de recuento cíclico mediante los parámetros de almacén o de artículo en las páginas **Trabajo de recuento cíclico por artículo** o **Trabajo de recuento cíclico por ubicación**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-110">Alternatively, you can manually create cycle counting work by using the item or warehouse parameters on the **Cycle count work by item** page or the **Cycle count work by location** page.</span></span>
2.  <span data-ttu-id="9e4e5-111">**Procesar el recuento cíclico**: una vez creado el trabajo de recuento cíclico, realice el trabajo de recuento cíclico contando los artículos de una ubicación de almacén y usando a continuación un dispositivo móvil para especificar el resultado en Microsoft Dynamics 365 for Finance and Operations.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-111">**Process the cycle count** – After cycle counting work is created, you do the cycle counting work by counting items in a warehouse location and then using a mobile device to enter the result in Microsoft Dynamics 365 for Finance and Operations.</span></span> <span data-ttu-id="9e4e5-112">Como alternativa, puede contar los artículos de una ubicación de almacén sin crear el trabajo de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-112">Alternatively, you can count items in a warehouse location without creating cycle counting work.</span></span> <span data-ttu-id="9e4e5-113">Este proceso se denomina *recuento cíclico puntual*.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-113">This process is referred to as *spot cycle counting*.</span></span>
3.  <span data-ttu-id="9e4e5-114">**Resolver diferencias en el valor de recuento**: tras un recuento cíclico, todos los artículos que tengan diferencias en el valor del recuento tendrán un estado de trabajo de **Revisión pendiente** en la página **Todo el trabajo**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-114">**Resolve differences in the counted value** – After a cycle count, any items that have differences in the counted value will have a work status of **Pending review** on the **All work** page.</span></span> <span data-ttu-id="9e4e5-115">Puede resolver estas diferencias en la página **Revisión pendiente del trabajo de recuento cíclico**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-115">You can resolve these differences on the **Cycle count work pending review** page.</span></span>

<span data-ttu-id="9e4e5-116">En la ilustración siguiente se muestra el proceso de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-116">The following illustration shows the cycle counting process.</span></span> ![Flujo del proceso de recuento cíclico](./media/performcyclecountinginawarehouselocation.jpg)

## <a name="cycle-counting-prerequisites"></a><span data-ttu-id="9e4e5-118">Requisitos previos de recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="9e4e5-118">Cycle counting prerequisites</span></span>
<span data-ttu-id="9e4e5-119">La tabla siguiente muestra los requisitos previos que deben cumplirse para poder usar el recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-119">The following table shows the prerequisites that must be in place before you can use cycle counting.</span></span>
<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="9e4e5-120">Requisito previo</span><span class="sxs-lookup"><span data-stu-id="9e4e5-120">Prerequisite</span></span></th>
<th><span data-ttu-id="9e4e5-121">Descripción</span><span class="sxs-lookup"><span data-stu-id="9e4e5-121">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="9e4e5-122">Artículo</span><span class="sxs-lookup"><span data-stu-id="9e4e5-122">Item</span></span></td>
<td><span data-ttu-id="9e4e5-123">El artículo se debe habilitar para procesos de administración de almacenes.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-123">The item must be enabled for warehouse management processes.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9e4e5-124">Almacén</span><span class="sxs-lookup"><span data-stu-id="9e4e5-124">Warehouse</span></span></td>
<td><span data-ttu-id="9e4e5-125">El almacén se debe habilitar para procesos de administración de almacenes.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-125">The warehouse must be enabled for warehouse management processes.</span></span> <span data-ttu-id="9e4e5-126">Para habilitar el almacén para procesos de administración de almacenes, en la página <strong>Almacenes</strong>, seleccione el almacén y, a continuación, seleccione la opción <strong>Usar procesos de gestión de almacenes</strong>.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-126">To enable the warehouse for warehouse management processes, on the <strong>Warehouses</strong> page, select the warehouse, and then select the <strong>Use warehouse management processes</strong> option.</span></span> <span data-ttu-id="9e4e5-127">Para permitir que los trabajadores muevan pallets durante un recuento cíclico, en la ficha desplegable <strong>Administración de almacenes</strong>, seleccione la opción <strong>Permitir movimientos de pallet durante el recuento cíclico</strong>.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-127">To enable workers to move pallets during a cycle count, on the <strong>Warehouse management</strong> FastTab, select the <strong>Allow pallet moves during cycle counting</strong> option.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9e4e5-128">Grupos de trabajo</span><span class="sxs-lookup"><span data-stu-id="9e4e5-128">Work pools</span></span></td>
<td><span data-ttu-id="9e4e5-129">Opcional: Crear un grupo de trabajo para segregar el trabajo del almacén, en función del tipo de trabajo (en este caso, el trabajo de recuento cíclico).</span><span class="sxs-lookup"><span data-stu-id="9e4e5-129">Optional: Create a work pool to segregate the warehouse work, based on the type of work (in this case, cycle counting work).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9e4e5-130">Ubicaciones</span><span class="sxs-lookup"><span data-stu-id="9e4e5-130">Locations</span></span></td>
<td><span data-ttu-id="9e4e5-131">Habilitar el recuento cíclico de ubicaciones.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-131">Enable cycle counting for locations.</span></span> <span data-ttu-id="9e4e5-132">Para permitir el recuento cíclico para una ubicación de almacén, en la página <strong>Perfiles de ubicación</strong>, seleccione la opción <strong>Permitir recuento cíclico</strong>.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-132">To enable cycle counting for a warehouse location, on the <strong>Location profiles</strong> page, select the <strong>Allow cycle counting</strong> option.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9e4e5-133">Parámetros de gestión de almacenes</span><span class="sxs-lookup"><span data-stu-id="9e4e5-133">Warehouse management parameters</span></span></td>
<td><span data-ttu-id="9e4e5-134">Configurar parámetros para el recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-134">Set up parameters for cycle counting.</span></span> <span data-ttu-id="9e4e5-135">En la página <strong>Parámetros de gestión de almacenes</strong>, especifique el código del tipo de ajuste predeterminado, el id. de clase de trabajo y la prioridad de trabajo para el recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-135">On the <strong>Warehouse management parameters</strong> page, specify the default adjustment type code, work class ID, and work priority for cycle counting.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="9e4e5-136">Dispositivo móvil</span><span class="sxs-lookup"><span data-stu-id="9e4e5-136">Mobile device</span></span></td>
<td><ul>
<li><span data-ttu-id="9e4e5-137">Cree un elemento de menú para uno de los siguientes métodos en la página <strong>Elementos de menú del dispositivo móvil</strong>:</span><span class="sxs-lookup"><span data-stu-id="9e4e5-137">Create a menu item for one of the following methods on the <strong>Mobile device menu items</strong> page:</span></span>
<ul>
<li><span data-ttu-id="9e4e5-138">Recuento cíclico dirigido por el usuario</span><span class="sxs-lookup"><span data-stu-id="9e4e5-138">User directed cycle counting</span></span></li>
<li><span data-ttu-id="9e4e5-139">Recuento cíclico dirigido por el sistema</span><span class="sxs-lookup"><span data-stu-id="9e4e5-139">System directed cycle counting</span></span></li>
<li><span data-ttu-id="9e4e5-140">Agrupación de recuentos cíclicos</span><span class="sxs-lookup"><span data-stu-id="9e4e5-140">Cycle count grouping</span></span></li>
<li><span data-ttu-id="9e4e5-141">Recuento cíclicos puntual</span><span class="sxs-lookup"><span data-stu-id="9e4e5-141">Spot cycle counting</span></span></li>
</ul>
</li>
<li><span data-ttu-id="9e4e5-142">Configure un menú para el dispositivo móvil.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-142">Set up a menu for the mobile device.</span></span></li>
<li><span data-ttu-id="9e4e5-143">Cree una cuenta de usuario de trabajo y asigne un menú de dispositivo móvil al id. de usuario de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-143">Create a work user account, and assign a mobile device menu to the work user ID.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="9e4e5-144">Tarea de configuración relacionada</span><span class="sxs-lookup"><span data-stu-id="9e4e5-144">Related setup task</span></span></td>
<td><span data-ttu-id="9e4e5-145">Configurar un plan de recuento cíclico para una ubicación de almacén.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-145">Set up a cycle counting plan for a warehouse location.</span></span></td>
</tr>
</tbody>
</table>

## <a name="automatically-create-cycle-counting-work"></a><span data-ttu-id="9e4e5-146">Crear automáticamente el trabajo de recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="9e4e5-146">Automatically create cycle counting work</span></span>
<span data-ttu-id="9e4e5-147">Existen dos formas de programar la creación recurrente del trabajo de recuento cíclico: configurar umbrales de recuento cíclico o configurar planes de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-147">There are two ways to schedule recurring creation of cycle counting work: set up cycle counting thresholds or set up cycle counting plans.</span></span>

-   <span data-ttu-id="9e4e5-148">Un umbral de recuento cíclico indica el límite de cantidad o porcentaje de los artículos de inventario.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-148">A cycle counting threshold indicates the quantity or percentage limit of inventory items.</span></span> <span data-ttu-id="9e4e5-149">El trabajo de recuento cíclico se crea automáticamente cuando se alcance el límite de umbral.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-149">Cycle counting work is automatically created when the threshold limit is reached.</span></span>
-   <span data-ttu-id="9e4e5-150">El plan de recuento cíclico crea trabajo de recuento cíclico inmediatamente o periódicamente a través de una trabajo por lotes.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-150">A cycle counting plan creates cycle counting work either immediately or periodically through a batch job.</span></span> <span data-ttu-id="9e4e5-151">Cuando se crea el trabajo de recuento cíclico, la línea de trabajo de recuento incluye información acerca de la ubicación que se contará.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-151">When cycle counting work is created, the counting work line includes information about the location to count.</span></span> <span data-ttu-id="9e4e5-152">El inventario disponible asociado a esta ubicación no se bloquea y está por lo tanto disponible para el proceso de reserva y de salida aunque exista un trabajo de recuento abierto.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-152">The on-hand inventory that is associated with this location isn't blocked, and is therefore available for reservation and outbound processing, even though open counting work exists.</span></span>

### <a name="create-cycle-counting-work-based-on-threshold-parameters-for-items"></a><span data-ttu-id="9e4e5-153">Crear un trabajo de recuento cíclico basado en parámetros de umbral para artículos</span><span class="sxs-lookup"><span data-stu-id="9e4e5-153">Create cycle counting work, based on threshold parameters for items</span></span>

<span data-ttu-id="9e4e5-154">El trabajo de recuento cíclico se puede crear cuando el número de artículos está por debajo de un valor de umbral específico en una ubicación.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-154">Cycle counting work can be created when the number of items falls below a specific threshold value in a location.</span></span> <span data-ttu-id="9e4e5-155">Por ejemplo, hay 60 artículos en una ubicación que tiene un umbral del recuento cíclico de 40.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-155">For example, there are 60 items in a location that has a cycle counting threshold of 40.</span></span> <span data-ttu-id="9e4e5-156">Durante una transacción de pedido de ventas, 25 artículos se seleccionan de la ubicación y se colocan en una ubicación provisional.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-156">During a sales order transaction, 25 items are picked from the location and put in a staging location.</span></span> <span data-ttu-id="9e4e5-157">Dado que el nuevo recuento de artículos, 35, es inferior a la cantidad umbral, el trabajo de recuento cíclico se crea automáticamente para la ubicación.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-157">Because the new item count, 35, is less than the threshold quantity, cycle counting work is automatically created for the location.</span></span>

### <a name="schedule-cycle-counting-work"></a><span data-ttu-id="9e4e5-158">Trabajo de recuento cíclico de programación</span><span class="sxs-lookup"><span data-stu-id="9e4e5-158">Schedule cycle counting work</span></span>

<span data-ttu-id="9e4e5-159">Puede programar los planes de recuento cíclico para crear trabajo de recuento cíclico inmediatamente o periódicamente.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-159">You can schedule cycle counting plans to create cycle counting work immediately or periodically.</span></span> <span data-ttu-id="9e4e5-160">Al configurar planes de recuento cíclico, puede controlar el grupo de trabajo para el que se crea el trabajo de recuento cíclico, el número máximo de recuentos cíclicos que se crean para artículos en distintas ubicaciones y el número de días antes de que una ubicación de almacén se cuente de nuevo.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-160">By setting up cycle counting plans, you can control the work pool that cycle counting work is created for, the maximum number of cycle counts that are created for items in different locations, and the number of days before a warehouse location is counted again.</span></span> <span data-ttu-id="9e4e5-161">Por ejemplo, un artículo está disponible en tres ubicaciones del almacén y el número máximo de recuentos cíclicos se establece en **2**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-161">For example, an item is available in three locations in the warehouse, and the maximum number of cycle counts is set to **2**.</span></span> <span data-ttu-id="9e4e5-162">En este caso, al ejecutar el plan de recuento cíclico, se crean dos recuentos cíclico para las dos ubicaciones en las que está presente el artículo.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-162">In this case, when you run the cycle counting plan, two cycle counts are created for the two locations where the item is present.</span></span> <span data-ttu-id="9e4e5-163">Como otro ejemplo, establece el número de días entre recuentos cíclicos en **5**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-163">As another example, you set the number of days between cycle counts to **5**.</span></span> <span data-ttu-id="9e4e5-164">En este caso, el trabajo de recuento cíclico se crea cada cinco días.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-164">In this case, cycle counting work is created every five days.</span></span> <span data-ttu-id="9e4e5-165">Sin embargo, si el trabajo de recuento cíclico se procesa el día 3, el siguiente trabajo de recuento cíclico se creará cinco días después del último recuento cíclico procesado, el día 8.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-165">However, if cycle counting work is processed on day 3, the next cycle counting work will be created five days after the last cycle counting was processed, on day 8.</span></span>

## <a name="create-cycle-counting-work-manually"></a><span data-ttu-id="9e4e5-166">Crear un trabajo de recuento cíclico manualmente</span><span class="sxs-lookup"><span data-stu-id="9e4e5-166">Create cycle counting work manually</span></span>
<span data-ttu-id="9e4e5-167">Para crear el trabajo de recuento cíclico manualmente, puede usar las páginas **Trabajo de recuento cíclico por artículo** o **Trabajo de recuento cíclico por ubicación**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-167">To create cycle counting work manually, you can use the **Cycle count work by item** or **Cycle count work by location** page.</span></span> <span data-ttu-id="9e4e5-168">Puede especificar el número máximo de recuentos cíclicos que se deben crear.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-168">You can specify the maximum number of cycle counts to create.</span></span> <span data-ttu-id="9e4e5-169">Por ejemplo, si el encargado de almacén especifica un valor de **5**, se crea un trabajo de recuento cíclico para cinco ubicaciones aunque el artículo esté presente en 10 ubicaciones.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-169">For example, if the warehouse manager specifies a value of **5**, cycle counting work is created for five locations, even if the item is present in 10 locations.</span></span> <span data-ttu-id="9e4e5-170">También puede seleccionar un id. de grupo de trabajo para el que se crean los id. de trabajo de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-170">You can also select a work pool ID to assign the cycle counting work IDs that are created to.</span></span> <span data-ttu-id="9e4e5-171">Cuando se procesa un id. de grupo de trabajo para el recuento cíclico, los id. de trabajo de recuento cíclico que se asignan al grupo de trabajo se procesan como un grupo.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-171">When a work pool ID is processed for cycle counting, the cycle counting work IDs that are assigned to the work pool are processed as a group.</span></span>

## <a name="perform-a-cycle-count-by-using-a-mobile-device"></a><span data-ttu-id="9e4e5-172">Realizar un recuento cíclico mediante un dispositivo móvil</span><span class="sxs-lookup"><span data-stu-id="9e4e5-172">Perform a cycle count by using a mobile device</span></span>
<span data-ttu-id="9e4e5-173">Hay varios métodos para procesar un trabajo de recuento cíclico mediante Finance and Operations en un dispositivo móvil:</span><span class="sxs-lookup"><span data-stu-id="9e4e5-173">There are several methods for processing cycle counting work by using Finance and Operations on a mobile device:</span></span>

-   <span data-ttu-id="9e4e5-174">**Dirigido por el usuario**: el trabajador puede especificar un id. de trabajo de recuento cíclico que tiene el estado de **Abierto**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-174">**User directed** – The worker can specify a cycle counting work ID that has a status of **Open**.</span></span>
-   <span data-ttu-id="9e4e5-175">**Dirigido por el sistema**: Finance and Operations asigna al trabajador un identificador de trabajo de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-175">**System directed** – Finance and Operations assigns a cycle counting work ID to the worker.</span></span>
-   <span data-ttu-id="9e4e5-176">**Agrupación de recuentos cíclicos**: el trabajador puede agrupar los id. de trabajo de recuento cíclico que son específicos de una ubicación, un área o a un grupo de trabajo en particular.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-176">**Cycle count grouping** – The worker can group cycle counting work IDs that are specific to a particular location, zone, or work pool.</span></span>
-   <span data-ttu-id="9e4e5-177">**Recuento cíclico puntual**: el trabajador puede contar los artículos de una ubicación de almacén en cualquier momento, sin crear el trabajo de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-177">**Spot cycle counting** – The worker can count items in a warehouse location at any time, without creating cycle counting work.</span></span> <span data-ttu-id="9e4e5-178">Para realizar el recuento cíclico puntual en una ubicación, el trabajador especifica el id. de ubicación.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-178">To perform spot cycle counting in a location, the worker enters the location ID.</span></span>

<span data-ttu-id="9e4e5-179">En el siguiente ejemplo se muestra cómo puede realizar un recuento cíclico puntual mediante un dispositivo móvil.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-179">The following example shows how you can perform spot cycle counting by using a mobile device.</span></span> <span data-ttu-id="9e4e5-180">Las instrucciones que ve el trabajador en el dispositivo varían, en función de la configuración del elemento de menú para el recuento cíclico puntual.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-180">The instructions that the worker sees on the device vary, depending on the setup of the menu item for spot cycle counting.</span></span>

1.  <span data-ttu-id="9e4e5-181">En el dispositivo móvil, seleccione el elemento de menú para procesar el trabajo de recuento cíclico puntual.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-181">On the mobile device, select the menu item to process spot cycle counting work.</span></span>
2.  <span data-ttu-id="9e4e5-182">Registre la ubicación para la que desea realizar el recuento cíclico puntual.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-182">Register the location to perform spot cycle counting for.</span></span>
3.  <span data-ttu-id="9e4e5-183">Registre y confirme el número de artículo y la cantidad contada del artículo.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-183">Register and confirm the item number and the counted item quantity.</span></span> <span data-ttu-id="9e4e5-184">**Nota:** El estado del trabajo de recuento cíclico se actualiza como **Revisión pendiente** o como **Cerrado** en la página **Todo el trabajo**, en función de los parámetros establecidos en la página **Trabajador**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-184">**Note:** The status of the cycle counting work is updated to either **Pending review** or **Closed** on the **All work** page, depending on the parameters that are set on the **Worker** page.</span></span>
4.  <span data-ttu-id="9e4e5-185">Opcional: repita el paso 3 para los artículos restantes de la ubicación y confirme que no haya artículos adicionales disponibles para contar.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-185">Optional: Repeat step 3 for the remaining items in the location, and confirm that no additional items are available for counting.</span></span>

## <a name="resolve-cycle-counting-differences"></a><span data-ttu-id="9e4e5-186">Resolver diferencia de recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="9e4e5-186">Resolve cycle counting differences</span></span>
<span data-ttu-id="9e4e5-187">Se produce una diferencia de recuento cíclico en los siguientes escenarios si la opción **Es un supervisor de recuentos cíclicos** se establece en **No** para un identificador de usuario de trabajo:</span><span class="sxs-lookup"><span data-stu-id="9e4e5-187">A cycle counting difference occurs in the following scenarios if the **Is a cycle count supervisor** option is set to **No** for a work user ID:</span></span>

-   <span data-ttu-id="9e4e5-188">El valor de recuento no se encuentra dentro de los límites de desviación que se especifican en los campos **Límite de porcentaje máximo** o **Límite de la cantidad máxima** en la página **Usuarios de trabajo**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-188">The counted value isn't within the deviation limits that are specified in the **Maximum percentage limit** or **Maximum quantity limit** fields on the **Work users** page.</span></span> <span data-ttu-id="9e4e5-189">Por ejemplo, la cantidad de inventario disponible en una ubicación es de 50 y el límite de desviación del usuario de trabajo es de 10.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-189">For example, the on-hand inventory quantity in a location is 50, and the deviation limit for the work user is 10.</span></span> <span data-ttu-id="9e4e5-190">Si el usuario de trabajo especifica un valor que no está entre 40 y 60, se produce una diferencia.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-190">If the work user enters a value that isn't between 40 and 60, a difference occurs.</span></span>
-   <span data-ttu-id="9e4e5-191">El valor de recuento cíclico difiere de la cantidad de inventario disponible y no se establecen límites de desviación.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-191">The counted value differs from the on-hand inventory quantity, and no deviation limits are set.</span></span>

<span data-ttu-id="9e4e5-192">Puede ajustar diferencias en el valor de recuento y aceptar a continuación el valor de recuento en la página **Revisión pendiente del trabajo de recuento cíclico**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-192">You can adjust differences in the counted value and then accept the counted value on the **Cycle count pending review** page.</span></span> <span data-ttu-id="9e4e5-193">Puede comprobar el recuento modificado de la cantidad del artículo en la página **Inventario disponible por ubicación**.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-193">You can verify the modified count of the item quantity on the **On hand by location** page.</span></span> <span data-ttu-id="9e4e5-194">El valor de recuento se rechaza si no se puede aprobar la diferencia.</span><span class="sxs-lookup"><span data-stu-id="9e4e5-194">The counted value is rejected if the difference can't be approved.</span></span>

# <a name="see-also"></a><span data-ttu-id="9e4e5-195">Consulte también</span><span class="sxs-lookup"><span data-stu-id="9e4e5-195">See also</span></span>
[<span data-ttu-id="9e4e5-196">Configurar dispositivos móviles para el trabajo de almacén</span><span class="sxs-lookup"><span data-stu-id="9e4e5-196">Configure mobile devices for warehouse work</span></span>](configure-mobile-devices-warehouse.md)



