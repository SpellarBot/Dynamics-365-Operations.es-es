---
title: Definir proceso de recuento cíclico de ubicaciones parcial
description: Al usar planes de recuento cíclico para crear trabajos de recuento, puede dirigir las operaciones de recuento en curso solicitando que solo los productos específicos y las variantes de producto se cuenten en lugar de todos los inventarios disponibles en la ubicación.
author: ShylaThompson
manager: AnnBe
ms.date: 06/23/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 3aafb42cea1664b0629f57fe4492736601902cc1
ms.sourcegitcommit: bacad87e2b9146e08e6fe16af01356954eb90574
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/01/2019
ms.locfileid: "373420"
---
# <a name="define-partial-location-cycle-counting-process"></a><span data-ttu-id="2a146-103">Definir proceso de recuento cíclico de ubicaciones parcial</span><span class="sxs-lookup"><span data-stu-id="2a146-103">Define partial location cycle counting process</span></span> 

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="2a146-104">Al usar planes de recuento cíclico para crear trabajos de recuento, puede dirigir las operaciones de recuento en curso solicitando que solo los productos específicos y las variantes de producto se cuenten en lugar de todos los inventarios disponibles en la ubicación.</span><span class="sxs-lookup"><span data-stu-id="2a146-104">When you use cycle count plans to create counting work, you can guide the actual counting operations by requesting that only specific products and product variants be counted instead of all on-hand inventory at the location.</span></span> <span data-ttu-id="2a146-105">Al filtrar según productos específicos, el responsable del almacén puede reducir los costes generales de revisión, ayudar a evitar errores de consolidación y ahorrar tiempo.</span><span class="sxs-lookup"><span data-stu-id="2a146-105">By filtering on specific products, the warehouse manager can reduce review overhead, help prevent consolidation mistakes, and save time.</span></span> <span data-ttu-id="2a146-106">Normalmente, un administrador de almacén realiza las tareas de configuración.</span><span class="sxs-lookup"><span data-stu-id="2a146-106">Typically, a warehouse manager performs the setup tasks.</span></span> <span data-ttu-id="2a146-107">Puede explorar este procedimiento en los datos de la empresa de demostración USMF o utilizar sus propios datos.</span><span class="sxs-lookup"><span data-stu-id="2a146-107">You can go through this procedure in the USMF demo data company or in your own data.</span></span>


## <a name="create-a-cycle-counting-work-template"></a><span data-ttu-id="2a146-108">Cree una plantilla de trabajo de recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="2a146-108">Create a cycle counting work template</span></span>
1. <span data-ttu-id="2a146-109">Vaya a Gestión de almacenes > Configurar > Trabajo > Plantillas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="2a146-109">Go to Warehouse management > Setup > Work > Work templates.</span></span>
2. <span data-ttu-id="2a146-110">En el campo Tipo de pedido de trabajo, seleccione "Recuento cíclico".</span><span class="sxs-lookup"><span data-stu-id="2a146-110">In the Work order type field, select 'Cycle counting'.</span></span>
3. <span data-ttu-id="2a146-111">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="2a146-111">Click New.</span></span>
4. <span data-ttu-id="2a146-112">En el campo Número de secuencia, especifique un número.</span><span class="sxs-lookup"><span data-stu-id="2a146-112">In the Sequence number field, enter a number.</span></span>
    * <span data-ttu-id="2a146-113">El criterio de ordenación es del número más pequeño al número más grande.</span><span class="sxs-lookup"><span data-stu-id="2a146-113">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="2a146-114">El valor debe ser mayor que 0 (cero).</span><span class="sxs-lookup"><span data-stu-id="2a146-114">The value must be more than 0 (zero).</span></span>  
5. <span data-ttu-id="2a146-115">En la lista, marque la fila seleccionada.</span><span class="sxs-lookup"><span data-stu-id="2a146-115">In the list, mark the selected row.</span></span>
6. <span data-ttu-id="2a146-116">En el campo Plantilla de trabajo, escriba un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-116">In the Work template field, type a value.</span></span>
7. <span data-ttu-id="2a146-117">En el campo Descripción de la plantilla de trabajo, escriba un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-117">In the Work template description field, type a value.</span></span>
8. <span data-ttu-id="2a146-118">En el campo Id. del grupo de trabajo, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-118">In the Work pool ID field, enter or select a value.</span></span>
9. <span data-ttu-id="2a146-119">En el campo Prioridad de trabajo, especifique un número.</span><span class="sxs-lookup"><span data-stu-id="2a146-119">In the Work priority field, enter a number.</span></span>
10. <span data-ttu-id="2a146-120">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="2a146-120">Click Save.</span></span>
11. <span data-ttu-id="2a146-121">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="2a146-121">Click New.</span></span>
12. <span data-ttu-id="2a146-122">En la lista, marque la fila seleccionada.</span><span class="sxs-lookup"><span data-stu-id="2a146-122">In the list, mark the selected row.</span></span>
13. <span data-ttu-id="2a146-123">En el campo Tipo de trabajo, seleccione "Recuento".</span><span class="sxs-lookup"><span data-stu-id="2a146-123">In the Work type field, select 'Counting'.</span></span>
14. <span data-ttu-id="2a146-124">En el campo Identificador de la clase de trabajo, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-124">In the Work class ID field, enter or select a value.</span></span>
15. <span data-ttu-id="2a146-125">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="2a146-125">Click Save.</span></span>
16. <span data-ttu-id="2a146-126">Haga clic en Saltos de línea de trabajo.</span><span class="sxs-lookup"><span data-stu-id="2a146-126">Click Work line breaks.</span></span>
17. <span data-ttu-id="2a146-127">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="2a146-127">Click New.</span></span>
18. <span data-ttu-id="2a146-128">En el campo Número de secuencia, especifique un número.</span><span class="sxs-lookup"><span data-stu-id="2a146-128">In the Sequence number field, enter a number.</span></span>
    * <span data-ttu-id="2a146-129">El criterio de ordenación es del número más pequeño al número más grande.</span><span class="sxs-lookup"><span data-stu-id="2a146-129">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="2a146-130">El valor debe ser mayor que 0 (cero).</span><span class="sxs-lookup"><span data-stu-id="2a146-130">The value must be more than 0 (zero).</span></span>  
19. <span data-ttu-id="2a146-131">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="2a146-131">Click Save.</span></span>
20. <span data-ttu-id="2a146-132">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="2a146-132">Close the page.</span></span>
21. <span data-ttu-id="2a146-133">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="2a146-133">Close the page.</span></span>

## <a name="create-a-cycle-counting-plan"></a><span data-ttu-id="2a146-134">Cree un plan de recuento cíclico</span><span class="sxs-lookup"><span data-stu-id="2a146-134">Create a cycle counting plan</span></span>
1. <span data-ttu-id="2a146-135">Vaya a Administración de almacenes > Configuración > Recuento de ciclos > Planes de recuento cíclico.</span><span class="sxs-lookup"><span data-stu-id="2a146-135">Go to Warehouse management > Setup > Cycle counting > Cycle count plans.</span></span>
2. <span data-ttu-id="2a146-136">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="2a146-136">Click New.</span></span>
3. <span data-ttu-id="2a146-137">En el campo Id. de plan de recuento cíclico, escriba un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-137">In the Cycle counting plan ID field, type a value.</span></span>
4. <span data-ttu-id="2a146-138">En el campo Descripción, escriba un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-138">In the Description field, type a value.</span></span>
5. <span data-ttu-id="2a146-139">En el campo Número máximo de recuentos cíclicos, especifique un número.</span><span class="sxs-lookup"><span data-stu-id="2a146-139">In the Maximum number of cycle counts field, enter a number.</span></span>
6. <span data-ttu-id="2a146-140">En el campo Plantilla de trabajo, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-140">In the Work template field, enter or select a value.</span></span>
7. <span data-ttu-id="2a146-141">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="2a146-141">Click New.</span></span>
8. <span data-ttu-id="2a146-142">En el campo Número de secuencia, especifique un número.</span><span class="sxs-lookup"><span data-stu-id="2a146-142">In the Sequence number field, enter a number.</span></span>
    * <span data-ttu-id="2a146-143">El criterio de ordenación es del número más pequeño al número más grande.</span><span class="sxs-lookup"><span data-stu-id="2a146-143">The sort order is from the smallest number to the largest number.</span></span> <span data-ttu-id="2a146-144">El valor debe ser mayor que 0 (cero).</span><span class="sxs-lookup"><span data-stu-id="2a146-144">The value must be more than 0 (zero).</span></span>  
9. <span data-ttu-id="2a146-145">En el campo Descripción, escriba un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-145">In the Description field, type a value.</span></span>
10. <span data-ttu-id="2a146-146">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="2a146-146">Click Save.</span></span>
11. <span data-ttu-id="2a146-147">Haga clic en Definir consulta de producto.</span><span class="sxs-lookup"><span data-stu-id="2a146-147">Click Define product query.</span></span>
12. <span data-ttu-id="2a146-148">En la lista, marque la fila seleccionada.</span><span class="sxs-lookup"><span data-stu-id="2a146-148">In the list, mark the selected row.</span></span>
13. <span data-ttu-id="2a146-149">En el campo Criterios, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="2a146-149">In the Criteria field, enter or select a value.</span></span>
14. <span data-ttu-id="2a146-150">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="2a146-150">Click OK.</span></span>
15. <span data-ttu-id="2a146-151">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="2a146-151">Close the page.</span></span>
