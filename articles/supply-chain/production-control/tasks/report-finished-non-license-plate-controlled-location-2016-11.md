--- 
title: "Notificar como terminado a una ubicación controlada por matrícula"
description: "Esta guía de tareas muestra un ejemplo de notificación como finalizado en una ubicación que no está controlada mediante matrículas de entidad de almacén."
author: ChristianRytt
manager: AnnBe
ms.date: 06/23/2016
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
ms.openlocfilehash: 34fac03a0ff3d71a2349b66f8f85e4e124dcd708
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---
# <a name="report-as-finished-to-a-plate-controlled-location"></a><span data-ttu-id="7e343-103">Notificar como terminado a una ubicación controlada por matrícula</span><span class="sxs-lookup"><span data-stu-id="7e343-103">Report as finished to a plate-controlled location</span></span> 

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="7e343-104">Esta guía de tareas muestra un ejemplo de notificación como finalizado en una ubicación que no está controlada mediante matrículas de entidad de almacén.</span><span class="sxs-lookup"><span data-stu-id="7e343-104">This task guide shows an example of reporting as finished to a location that isn't license plate–controlled.</span></span> <span data-ttu-id="7e343-105">Una directiva aplicable de trabajo es el requisito previo para esta tarea.</span><span class="sxs-lookup"><span data-stu-id="7e343-105">An applicable work policy is the prerequisite for this task.</span></span> <span data-ttu-id="7e343-106">Una guía de tareas anterior mostraba la configuración de la directiva de trabajo.</span><span class="sxs-lookup"><span data-stu-id="7e343-106">A previous task guide showed the setup of the work policy.</span></span> <span data-ttu-id="7e343-107">Esta guía de tareas requiere la aplicación Dynamics AX 7.0.1 o versiones posteriores.</span><span class="sxs-lookup"><span data-stu-id="7e343-107">This task guide requires Dynamics AX application 7.0.1 or later.</span></span>




## <a name="set-up-an-output-location"></a><span data-ttu-id="7e343-108">Configurar una ubicación de salida</span><span class="sxs-lookup"><span data-stu-id="7e343-108">Set up an output location</span></span>
1. <span data-ttu-id="7e343-109">Vaya a Administración de la organización > Recursos > Grupos de recursos..</span><span class="sxs-lookup"><span data-stu-id="7e343-109">Go to Organization administration > Resources > Resource groups.</span></span>
2. <span data-ttu-id="7e343-110">En la lista, seleccione el grupo de recursos "5102".</span><span class="sxs-lookup"><span data-stu-id="7e343-110">In the list, select resource group '5102'.</span></span>
3. <span data-ttu-id="7e343-111">Haga clic en Editar.</span><span class="sxs-lookup"><span data-stu-id="7e343-111">Click Edit.</span></span>
4. <span data-ttu-id="7e343-112">En el campo Almacén de salida, especifique "51".</span><span class="sxs-lookup"><span data-stu-id="7e343-112">In the Output warehouse field, enter '51'.</span></span>
5. <span data-ttu-id="7e343-113">En el campo Ubicación de salida, especifique "001".</span><span class="sxs-lookup"><span data-stu-id="7e343-113">In the Output location field, enter '001'.</span></span>
    * <span data-ttu-id="7e343-114">La ubicación 001 no es una ubicación controlada mediante matrículas de entidad de almacén.</span><span class="sxs-lookup"><span data-stu-id="7e343-114">Location 001 isn't a license plate–controlled location.</span></span> <span data-ttu-id="7e343-115">Puede configurar una ubicación de salida que no sea de matrículas de entidad de almacén si existe una directiva aplicable de trabajo para la ubicación.</span><span class="sxs-lookup"><span data-stu-id="7e343-115">You can set up a non–license plate output location only if an applicable work policy exists for the location.</span></span>  

## <a name="create-a-production-order-and-report-it-as-finished"></a><span data-ttu-id="7e343-116">Crear un pedido de producción y notificarlo como terminado</span><span class="sxs-lookup"><span data-stu-id="7e343-116">Create a production order and report it as finished</span></span>
1. <span data-ttu-id="7e343-117">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="7e343-117">Close the page.</span></span>
2. <span data-ttu-id="7e343-118">Vaya a Control de producción > Pedidos de producción > Todos los pedidos de producción.</span><span class="sxs-lookup"><span data-stu-id="7e343-118">Go to Production control > Production orders > All production orders.</span></span>
3. <span data-ttu-id="7e343-119">Haga clic en Nuevo pedido de producción.</span><span class="sxs-lookup"><span data-stu-id="7e343-119">Click New production order.</span></span>
4. <span data-ttu-id="7e343-120">En el campo Número de artículo, especifique "L0101".</span><span class="sxs-lookup"><span data-stu-id="7e343-120">In the Item number field, enter 'L0101'.</span></span>
5. <span data-ttu-id="7e343-121">Haga clic en Crear.</span><span class="sxs-lookup"><span data-stu-id="7e343-121">Click Create.</span></span>
6. <span data-ttu-id="7e343-122">En el panel de acciones, haga clic en Pedido de producción.</span><span class="sxs-lookup"><span data-stu-id="7e343-122">On the Action Pane, click Production order.</span></span>
7. <span data-ttu-id="7e343-123">Haga clic en Estimación.</span><span class="sxs-lookup"><span data-stu-id="7e343-123">Click Estimate.</span></span>
8. <span data-ttu-id="7e343-124">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="7e343-124">Click OK.</span></span>
9. <span data-ttu-id="7e343-125">Haga clic en Inicio.</span><span class="sxs-lookup"><span data-stu-id="7e343-125">Click Start.</span></span>
10. <span data-ttu-id="7e343-126">Haga clic en la ficha General.</span><span class="sxs-lookup"><span data-stu-id="7e343-126">Click the General tab.</span></span>
11. <span data-ttu-id="7e343-127">En el campo Consumo automático de L. MAT, seleccione "Nunca".</span><span class="sxs-lookup"><span data-stu-id="7e343-127">In the Automatic BOM consumption field, select 'Never'.</span></span>
12. <span data-ttu-id="7e343-128">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="7e343-128">Click OK.</span></span>
13. <span data-ttu-id="7e343-129">Haga clic en Notificar como terminado.</span><span class="sxs-lookup"><span data-stu-id="7e343-129">Click Report as finished.</span></span>
14. <span data-ttu-id="7e343-130">Haga clic en la ficha General.</span><span class="sxs-lookup"><span data-stu-id="7e343-130">Click the General tab.</span></span>
15. <span data-ttu-id="7e343-131">Seleccione Sí en el campo Aceptar error.</span><span class="sxs-lookup"><span data-stu-id="7e343-131">Select Yes in the Accept error field.</span></span>
16. <span data-ttu-id="7e343-132">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="7e343-132">Click OK.</span></span>
17. <span data-ttu-id="7e343-133">En el panel de acciones, haga clic en Almacén.</span><span class="sxs-lookup"><span data-stu-id="7e343-133">On the Action Pane, click Warehouse.</span></span>
18. <span data-ttu-id="7e343-134">Haga clic en Detalles del trabajo.</span><span class="sxs-lookup"><span data-stu-id="7e343-134">Click Work details.</span></span>
    * <span data-ttu-id="7e343-135">Cuando el pedido de producción se ha notificado como finalizado, no se ha generado ningún trabajo para ubicación.</span><span class="sxs-lookup"><span data-stu-id="7e343-135">When the production order was reported as finished, no work was generated for put-away.</span></span> <span data-ttu-id="7e343-136">Esto ocurre porque se define una directiva de trabajo que impide que el trabajo se genere cuando el producto L0101 se notifique como finalizado para la ubicación 001.</span><span class="sxs-lookup"><span data-stu-id="7e343-136">This occurs because a work policy is defined that prevents work from being generated when product L0101 is reported as finished to location 001.</span></span>  

