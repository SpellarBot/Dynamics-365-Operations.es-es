---
title: Crear y asociar una estación de hardware
description: Este procedimiento le muestra cómo crear una nueva estación de hardware.
author: jashanno
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailHardwareStation, RetailStoreTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 80df4fa663d208e28f5c9b031b6610d29286171c
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "330572"
---
# <a name="create-and-associate-a-hardware-station"></a>Crear y asociar una estación de hardware

[!include[task guide banner](../includes/task-guide-banner.md)]

Este procedimiento le muestra cómo crear una nueva estación de hardware. Se creará y se usará un nuevo perfil de hardware para agregar nuevas estaciones de hardware a un almacén predefinido (canal). Este procedimiento usa la empresa USRT en los datos de demostración.

1. Vaya a > Esenciales de comercio > Canales > .. > .. > .. > Perfiles de la estación de hardware.
2. Haga clic en Nuevo.
3. En el campo Id. de la estación de hardware, escriba “TestHWProfile”.
4. En el campo Nombre, escriba un valor.
5. En el campo Número de puerto, especifique un número.
6. En el campo Perfil de hardware, haga clic en el botón desplegable para abrir la búsqueda.
7. En la lista, busque y seleccione el registro deseado.
8. En la lista, haga clic en el vínculo de la fila seleccionada.
9. En el campo Nombre del paquete, haga clic en el botón desplegable para abrir la búsqueda.
10. En la lista, haga clic en el vínculo de la fila seleccionada.
    * Este es el paquete estándar que se incluye con un nuevo entorno. El número de versión puede variar.  
11. Haga clic en Guardar.
12. Cierre la página.
13. Vaya a Venta minorista y comercio > Canales > Todas las tiendas minoristas.
14. En la lista, seleccione la fila 17.
    * Si usa la empresa de datos de demostración de USRT, esta es la tienda de Houston.  
15. En la lista, haga clic en el vínculo de la fila seleccionada.
16. Alterne la expansión de la sección Estaciones de hardware.
17. Haga clic en Agregar.
18. En la lista, marque la fila seleccionada.
19. En el campo Id. del perfil, haga clic en el botón desplegable para abrir la búsqueda.
20. En la lista, busque y seleccione el registro deseado.
    * Este debe ser el nuevo perfil de estación de hardware que se creó en los pasos anteriores.  
21. En la lista, haga clic en el vínculo de la fila seleccionada.
22. En el campo Nombre de host, escriba un valor.
23. En el campo Id. de terminal EFT, escriba un valor.
24. Haga clic en Guardar.

