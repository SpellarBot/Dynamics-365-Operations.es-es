---
title: Reabastecimiento con kanbans de transporte
description: "Este tema describe cómo el kanban de transporte se usa para el reabastecimiento para las actividades de fabricación."
author: johanhoffmann
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: KanbanBoardTransferJob, KanbanFlow, KanbanRules
audience: Application User
ms.reviewer: bis
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 
ms.assetid: 
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: johanho
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 152b7908364db82481c5af4a05a9775fbabca042
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---

# <a name="replenishment-with-withdrawal-kanbans"></a><span data-ttu-id="0ca9a-103">Reabastecimiento con kanbans de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-103">Replenishment with withdrawal kanbans</span></span>

[!include[banner](../includes/banner.md)]


<span data-ttu-id="0ca9a-104">Este tema describe cómo el kanban de transporte se usa para el reabastecimiento para las actividades de fabricación.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-104">This topic describes how the withdrawal kanban is used for material replenishment for manufacturing activities.</span></span>

## <a name="workflow-for-material-replenishment-that-uses-the-withdrawal-kanban"></a><span data-ttu-id="0ca9a-105">El flujo de trabajo para reabastecimiento de material que utiliza el kanban de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-105">Workflow for material replenishment that uses the withdrawal kanban</span></span>
-------------------------------------------------------------------

<span data-ttu-id="0ca9a-106">El kanban de transporte se puede utilizar para mover un kanban de un único artículo entre los almacenes y las ubicaciones de producción donde se consume el material.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-106">The withdrawal kanban can be used to move a kanban of a single item between warehouses and production locations where the material is consumed.</span></span> <span data-ttu-id="0ca9a-107">El kanban de transporte admite una solución basada en extracción para el reabastecimiento de material, donde se requiere una señal de extracción para activar un suministro para una demanda específica.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-107">The withdrawal kanban supports a pull-based solution for material replenishment, where a pull signal is required in order to trigger supply for a specific demand.</span></span> 

<span data-ttu-id="0ca9a-108">La situación siguiente muestra el sistema de reabastecimiento basado en extracción donde una señal de extracción activa la creación de un kanban para reabastecer material para un proceso de producción.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-108">The following scenario shows a pull-based replenishment system where a pull signal triggers the creation of a kanban to replenish material for a production process.</span></span> 

<span data-ttu-id="0ca9a-109">[![La señal de extracción activa la creación de un kanban para reabastecer material para un proceso de producción](./media/material-replenishment-with-withdrawal-kanban.png)](./media/material-replenishment-with-withdrawal-kanban.png)</span><span class="sxs-lookup"><span data-stu-id="0ca9a-109">[![Pull signal triggers the creation of a kanban to replenish material for a production process](./media/material-replenishment-with-withdrawal-kanban.png)](./media/material-replenishment-with-withdrawal-kanban.png)</span></span>

1.  <span data-ttu-id="0ca9a-110">Kanban de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-110">Withdrawal kanban</span></span>
2.  <span data-ttu-id="0ca9a-111">Ubicación "desde" kanban y ubicación de colocación para trabajo de almacén</span><span class="sxs-lookup"><span data-stu-id="0ca9a-111">Kanban “from” location and put location for warehouse work</span></span>
3.  <span data-ttu-id="0ca9a-112">Ubicación "a" kanban y ubicación de entrada de producción</span><span class="sxs-lookup"><span data-stu-id="0ca9a-112">Kanban “to” location and production input location</span></span>
4.  <span data-ttu-id="0ca9a-113">Proceso de fabricación</span><span class="sxs-lookup"><span data-stu-id="0ca9a-113">Manufacturing process</span></span>
5.  <span data-ttu-id="0ca9a-114">Trabajo del almacén para el picking de kanban</span><span class="sxs-lookup"><span data-stu-id="0ca9a-114">Warehouse work for kanban picking</span></span>
6.  <span data-ttu-id="0ca9a-115">Ubicaciones de almacén para la materia prima</span><span class="sxs-lookup"><span data-stu-id="0ca9a-115">Warehouse locations for raw material</span></span>
7.  <span data-ttu-id="0ca9a-116">Almacén de material</span><span class="sxs-lookup"><span data-stu-id="0ca9a-116">Material warehouse</span></span>
8.  <span data-ttu-id="0ca9a-117">Almacén de fabricación</span><span class="sxs-lookup"><span data-stu-id="0ca9a-117">Manufacturing warehouse</span></span>

<span data-ttu-id="0ca9a-118">En esta situación, un proceso de fabricación (4) consume material de una ubicación de entrada de producción (3) en el almacén de la fabricación (8).</span><span class="sxs-lookup"><span data-stu-id="0ca9a-118">In this scenario, a manufacturing process (4) consumes material from a production input location (3) in the manufacturing warehouse (8).</span></span> <span data-ttu-id="0ca9a-119">Cuando una unidad de gestión de material (kanban) se consume, se registra como vacía.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-119">When a handling unit of the material (kanban) is consumed, it’s registered as empty.</span></span> <span data-ttu-id="0ca9a-120">Una señal de reabastecimiento se crea para el origen del artículo y se crea un nuevo kanban (1).</span><span class="sxs-lookup"><span data-stu-id="0ca9a-120">A replenishment signal is created for the item origin, and a new kanban (1) is created.</span></span> <span data-ttu-id="0ca9a-121">En este caso, origen del artículo consta de ubicaciones en el almacén de material (7).</span><span class="sxs-lookup"><span data-stu-id="0ca9a-121">In this case, the item origin consists of locations in the material warehouse (7).</span></span> <span data-ttu-id="0ca9a-122">El material de kanban se selecciona y se coloca en una ubicación (2) en el mismo el almacén.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-122">The material for the kanban is picked and put to a location (2) in the same warehouse.</span></span> <span data-ttu-id="0ca9a-123">Cuando se selecciona el material, está listo para su transferencia de la ubicación 2 a la ubicación de entrada de producción (3) en el almacén de fabricación (8).</span><span class="sxs-lookup"><span data-stu-id="0ca9a-123">When the material is picked, it’s ready to be transferred from location 2 to the production input location (3) in the manufacturing warehouse (8).</span></span>

## <a name="configure-warehouse-work-for-kanban-picking-for-the-withdrawal-kanban"></a><span data-ttu-id="0ca9a-124">Configurar del trabajo del almacén para el picking de kanban para el kanban de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-124">Configure warehouse work for kanban picking for the withdrawal kanban</span></span>

<span data-ttu-id="0ca9a-125">Para habilitar la selección de la materia prima para el kanban de transporte, configure las plantillas de oleada, las plantillas de trabajo y las directivas de ubicación para el tipo de pedido de trabajo **Picking de kanban** .</span><span class="sxs-lookup"><span data-stu-id="0ca9a-125">To enable raw material picking for the withdrawal kanban, configure wave templates, work templates, and location directives for the **Kanban picking** work order type.</span></span> <span data-ttu-id="0ca9a-126">Este tipo de pedido de trabajo no admite solo el proceso de picking para el kanban de transporte.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-126">This work order type doesn’t just support the picking process for the withdrawal kanban.</span></span> <span data-ttu-id="0ca9a-127">También admite el proceso de picking para el kanban de fabricación.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-127">It also supports the picking process for the manufacturing kanban.</span></span> <span data-ttu-id="0ca9a-128">Sin embargo, puede configurar un proceso independiente de selección para cada tipo de kanban separando las plantillas de oleada, las plantillas de trabajo y las directivas de la ubicación.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-128">However, you can configure a separate picking process for each type of kanban by separating the wave templates, work templates, and location directives.</span></span> <span data-ttu-id="0ca9a-129">Para separar las plantillas de oleada, las plantillas de trabajo y las directivas de ubicación, establezca criterios en el tipo de actividad (**Proceso** o **Transferencia**) en las consultas de esas entidades.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-129">To separate the wave templates, work templates, and location directives, set criteria on the activity type (**Process** or **Transfer**) in the queries for those entities.</span></span>

## <a name="configure-the-withdrawal-kanban"></a><span data-ttu-id="0ca9a-130">Configurar el kanban de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-130">Configure the withdrawal kanban</span></span>

<span data-ttu-id="0ca9a-131">La actividad de transferencia que se usa para el kanban de transporte se configura como parte de un plan de actividades activado en un flujo de producción Lean (producción ajustada).</span><span class="sxs-lookup"><span data-stu-id="0ca9a-131">The transfer activity that is used for the withdrawal kanban is configured as part of an activated activity plan in a Lean production flow.</span></span> <span data-ttu-id="0ca9a-132">Como parte de la configuración de la actividad de transferencia, especifique las ubicaciones "desde" y "hasta" para la transferencia.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-132">As part of the configuration of the transfer activity, you specify the “from” and “to” locations for the transfer.</span></span> <span data-ttu-id="0ca9a-133">Después de configurar la actividad de transferencia, puede asignarla a una regla kanban del tipo **Transporte**.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-133">After you configure the transfer activity, you can assign it to a kanban rule of the **Withdrawal** type.</span></span> <span data-ttu-id="0ca9a-134">La regla kanban establece las directivas y las configuraciones para el kanban de transporte.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-134">The kanban rule sets the policies and configurations for the withdrawal kanban.</span></span> <span data-ttu-id="0ca9a-135">La cantidad de kanban define cuántas unidades de la unidad de manipulación tiene el kanban durante el proceso de transferencia.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-135">The quantity of the kanban defines how many units of the handling unit the kanban carries during the transfer process.</span></span> <span data-ttu-id="0ca9a-136">Se usa la cantidad de kanban fija cuando está selecciona la estrategia de reabastecimiento fija.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-136">The fixed kanban quantity is used when the Fixed replenishment strategy is selected.</span></span> <span data-ttu-id="0ca9a-137">Esta cantidad define cuántos kanbans son necesarios para impedir que las existencias o el inventario de la generación se ejecuten en el origen de la demanda.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-137">This quantity defines how many kanbans that are required in order to prevent stock or build inventory from running out at the source of demand.</span></span> <span data-ttu-id="0ca9a-138">La cantidad fija se puede calcular en función de la demanda real, la demanda histórica y los niveles de servicio.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-138">The fixed quantity can be calculated based on actual demand, historical demand, and service levels.</span></span> <span data-ttu-id="0ca9a-139">Las dos casos siguientes describen cómo puede gestionar el reabastecimiento de material que utiliza el kanban de transporte.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-139">The following two scenarios describe how you can manage material replenishment that uses the withdrawal kanban.</span></span>

## <a name="scenario-1-replenish-a-production-input-location-by-using-a-fixed-withdrawal-kanban"></a><span data-ttu-id="0ca9a-140">Situación 1: Completar una ubicación de entrada de producción mediante un kanban de transporte fijo</span><span class="sxs-lookup"><span data-stu-id="0ca9a-140">Scenario 1: Replenish a production input location by using a fixed withdrawal kanban</span></span>

<span data-ttu-id="0ca9a-141">Un proceso de fabricación consume materia prima comprada en una ubicación de entrada de producción que está en el almacén e producción.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-141">A manufacturing process consumes a purchased raw material from a production input location that is in the production warehouse.</span></span> <span data-ttu-id="0ca9a-142">Cuando la materia prima se recibe del proveedor se almacena en ubicaciones en el almacén material.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-142">When the raw material is received from the vendor, it’s stored in locations in the material warehouse.</span></span> <span data-ttu-id="0ca9a-143">Dado que la demanda de materiales se considera estable durante un período, se configuran para suministrar la producción en un flujo de kanban de cantidad fija.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-143">Because the demand for the material is considered stable over a period, it’s set up to supply the production in a fixed quantity kanban flow.</span></span> <span data-ttu-id="0ca9a-144">Cuando un kanban se consume en la ubicación de entrada de producción, se registra una señal vacía y se crea un nuevo kanban del mismo tipo que se agrega al flujo de trabajo.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-144">When a kanban is consumed at the production input location, an empty signal is registered, and a new kanban of the same type is added to the flow.</span></span> 

<span data-ttu-id="0ca9a-145">La señal vacía se puede configurar para que se muestre automáticamente cuando un kanban se completa.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-145">The empty signal can be configured to occur automatically when a kanban is completed.</span></span> <span data-ttu-id="0ca9a-146">O bien, la señal vacía se puede configurar como interacción manual que se proporciona desde el tablero de transferencia de kanban o desde un menú en el dispositivo de mano.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-146">Alternatively, the empty signal can be set up as a manual interaction that is given either from the Kanban transfer board or from a menu on the hand-held device.</span></span> <span data-ttu-id="0ca9a-147">El tablero de kanban de transferencia es el espacio de trabajo en la que todas las actividades en el ciclo de vida del kanban se gestionan.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-147">The Kanban transfer board is the workspace where all activities in the kanban life cycle are managed.</span></span> 

<span data-ttu-id="0ca9a-148">Cuando se crea el kanban, una línea de oleada para la materia prima se agrega a una oleada de kanban para el almacén de material.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-148">When the kanban is created, a wave line for the raw material is added to a kanban wave for the material warehouse.</span></span> <span data-ttu-id="0ca9a-149">En la sección de la lista de selección del tablero de transferencia de kanban, el estado del material y los procesos relacionados con el almacén se pueden controlar desde la creación de la oleada hasta la creación de trabajo, hasta que el material esté disponible en la ubicación de “transferencia desde” y esté listo para transferirse a la entrada de producción.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-149">In the picking list section of the Kanban transfer board, the status of the material and related warehouse processes can be monitored from wave creation to work creation, until the material is on-hand in the “transfer from” location and is ready to be transferred to the production input locations.</span></span> <span data-ttu-id="0ca9a-150">El kanban se puede completar desde el tablero de transferencia de kanban o desde un menú del dispositivo de mano.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-150">The kanban can be completed either from the Kanban transfer board or from a menu on the hand-held device.</span></span> 

<span data-ttu-id="0ca9a-151">En esta situación, el trabajo de selección en el almacén de material se procesa como una actividad.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-151">In this scenario, the picking work in the material warehouse is processed as one activity.</span></span> <span data-ttu-id="0ca9a-152">La actividad de transferencia entre el almacén de material y el almacén de producción se procesa como actividad independiente.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-152">The transfer activity between the material warehouse and the production warehouse is processed as a separate activity.</span></span> <span data-ttu-id="0ca9a-153">Este enfoque puede ser útil si, por ejemplo, hay una distancia física grande entre los dos almacenes.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-153">This approach can be useful if, for example, there is a large physical distance between the two warehouses.</span></span> <span data-ttu-id="0ca9a-154">En este caso, la actividad de transferencia de kanban puede representar una carga del camión.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-154">In this case, the kanban transfer activity can represent a truck load.</span></span> 

<span data-ttu-id="0ca9a-155">Si la distancia entre las ubicaciones del almacén y la ubicación de entrada de producción es pequeña, es posible que sea más eficaz incluir la actividad de transferencia en el proceso de picking.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-155">If the distance between the warehouse locations and the production input location is small, it might be more efficient to include the transfer activity in the picking process.</span></span> <span data-ttu-id="0ca9a-156">A continuación, después de seleccionar el material, se puede poner directamente en la ubicación de entrada de producción.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-156">Then, after the material is picked, it can be put directly to the production input location.</span></span> <span data-ttu-id="0ca9a-157">Para admitir este proceso, configure la actividad de transferencia para que se complete automáticamente cuando el trabajo de selección del kanban de transporte se procese.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-157">To support this process, you configure the transfer activity so that it’s automatically completed when the pick work of the withdrawal kanban is processed.</span></span>

## <a name="scenario-2-automatically-complete-the-transfer-activity-when-kanban-picking-work-is-processed"></a><span data-ttu-id="0ca9a-158">Situación 2: Automáticamente complete la actividad de transferencia cuando se procesa el trabajo del picking de kanban</span><span class="sxs-lookup"><span data-stu-id="0ca9a-158">Scenario 2: Automatically complete the transfer activity when kanban picking work is processed</span></span>

<span data-ttu-id="0ca9a-159">En el escenario siguiente, la actividad de transferencia de kanban de transporte se configura para transferir entre dos ubicaciones del mismo almacén.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-159">In the following scenario, the transfer activity of the withdrawal kanban is configured to transfer between two locations in the same warehouse.</span></span> <span data-ttu-id="0ca9a-160">La actividad de la transferencia de kanban de transporte se establece para que se complete automáticamente.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-160">The transfer activity of the withdrawal kanban is set up so that it’s completed automatically.</span></span> 

<span data-ttu-id="0ca9a-161">[![La actividad de la transferencia se completa automáticamente cuando se procesa el trabajo de picking](./media/transfer-activities-when-processing-kanban-picking.png)](./media/transfer-activities-when-processing-kanban-picking.png)</span><span class="sxs-lookup"><span data-stu-id="0ca9a-161">[![Transfer activity is automatically completed when kanban picking work is processed](./media/transfer-activities-when-processing-kanban-picking.png)](./media/transfer-activities-when-processing-kanban-picking.png)</span></span>

1.  <span data-ttu-id="0ca9a-162">Almacén compartido para materias primas y producción</span><span class="sxs-lookup"><span data-stu-id="0ca9a-162">Shared warehouse for raw materials and production</span></span>
2.  <span data-ttu-id="0ca9a-163">Ubicaciones de almacén para materias primas</span><span class="sxs-lookup"><span data-stu-id="0ca9a-163">Warehouse locations for raw materials</span></span>
3.  <span data-ttu-id="0ca9a-164">Ubicación "desde" kanban y ubicación de colocación para trabajo de almacén</span><span class="sxs-lookup"><span data-stu-id="0ca9a-164">Kanban “from” location and put location for warehouse work</span></span>
4.  <span data-ttu-id="0ca9a-165">Kanban de transporte</span><span class="sxs-lookup"><span data-stu-id="0ca9a-165">Withdrawal kanban</span></span>
5.  <span data-ttu-id="0ca9a-166">Ubicación de entrada de producción</span><span class="sxs-lookup"><span data-stu-id="0ca9a-166">Production input location</span></span>
6.  <span data-ttu-id="0ca9a-167">Proceso de fabricación</span><span class="sxs-lookup"><span data-stu-id="0ca9a-167">Manufacturing process</span></span>

<span data-ttu-id="0ca9a-168">Después de consumir un kanban en la ubicación de entrada de producción, el kanban se notifica como vacío y se agrega un nuevo kanban al flujo.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-168">After a kanban is consumed at the production input location, the kanban is reported as empty, and a new kanban is added to the flow.</span></span> <span data-ttu-id="0ca9a-169">Cuando se crea el kanban, una línea de oleada se agrega a una oleada de kanban.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-169">When the kanban is created, a wave line is added to a kanban wave.</span></span> <span data-ttu-id="0ca9a-170">Cuando se procesa la oleada de kanban, el trabajo del almacén para el picking de kanban se crea.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-170">When the kanban wave is processed, warehouse work for kanban picking is created.</span></span> <span data-ttu-id="0ca9a-171">El trabajador del almacén procesa el trabajo para el picking de kanban y el trabajo lo guía para que seleccione el material del kanban en una ubicación de almacén.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-171">The warehouse worker processes the work for kanban picking and is directed by the work to pick the material for the kanban in a warehouse location.</span></span> <span data-ttu-id="0ca9a-172">Cuando este trabajador del almacén confirma la selección, el kanban se completa automáticamente y el trabajador del almacén es guiado para que coloque el material en la ubicación de entrada de producción.</span><span class="sxs-lookup"><span data-stu-id="0ca9a-172">As this warehouse worker confirms the pick, the kanban is automatically completed, and the warehouse worker is guided to the put the material to the production input location.</span></span>

