---
title: Comprobar la disponibilidad de existencias
description: Este procedimiento le muestra cómo comprobar el inventario disponible y el inventario físico disponible para un número de artículo concreto.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventOnHandItemListPage, SysQueryForm, InventDimParmFixed, InventSupply, DefaultDashboard, WHSInventPhysicalOnhand, WHSOnHand
audience: Application User
ms.reviewer: ''
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 26a8f51eda1f4249862a23fa0103b7a144d974a1
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "338001"
---
# <a name="check-the-availability-of-stock"></a>Comprobar la disponibilidad de existencias

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento le muestra cómo comprobar el inventario disponible y el inventario físico disponible para un número de artículo concreto. También se muestra cómo obtener la información de suministro relacionada con un artículo. El inventario físico disponible es el inventario disponible que se tiene a mano, es decir, se ha comprado, recibido y registrado. El inventario disponible incluye el inventario disponible que se tiene a mano, pero también el inventario pedido y que se espera pero aún no se ha recibido o registrado. Puede revisar este procedimiento con los datos de prueba de la empresa USMF o utilizar sus propios datos. Si está usando USMF, puede utilizar los valores del ejemplo mostrados. Estas tareas las realizará normalmente un trabajador del almacén.


## <a name="check-on-hand-inventory-for-an-item"></a>Comprobar el inventario disponible de un artículo
1. Vaya a Gestión de inventario > Consultas e informes > Inventario disponible.
2. Seleccione la fila Número de artículo.
    * Para consultar el inventario disponible por número de artículo, seleccione la fila donde Tabla está establecido en Inventario disponible y Campo está establecido en Número de artículo.  
3. En el campo Criterios, seleccione el artículo que desea consultar.
    * Si utiliza a la empresa de datos de prueba USMF, puede seleccionar "M9201".  
4. Haga clic en Aceptar
5. Haga clic en Dimensiones.
    * La ficha Dimensiones permite seleccionar cuánto detalle desea ver sobre su inventario disponible. Si necesita los datos relacionados con la reserva, debe mostrar todas las dimensiones de inventario para los artículos que usan los procesos avanzados de almacén (WHS).  
6. Haga clic en Aceptar
7. En el panel de acciones, haga clic en Información relacionada.
    * Si no ve esto, es posible que tenga que hacer clic en los puntos suspensivos (…) para ver opciones adicionales del panel de acciones.  
8. Haga clic en Visión general de suministros.
    * La ficha Visión general de suministros proporciona la información para un artículo específico, como la cantidad disponible, el plazo y la información del proveedor.  
9. Expanda la sección Disponible.
10. Expanda la sección Proveedores.
11. Cierre la página.
12. Cierre la página.

## <a name="check-physical-on-hand-inventory"></a>Comprobar el inventario físico disponible
1. Vaya a Gestión de almacén > Consultas e informes > Inventario físico disponible.
2. En el campo Código de artículo, escriba un valor.
    * Puede utilizar los campos Sitio y Almacén para filtrar la lista de artículos.  
3. Actualice la página.
4. Haga clic en Mostrar dimensiones.
    * La ficha Mostrar dimensiones permite seleccionar cuánto detalle desea ver sobre su inventario disponible.  
5. Haga clic en Aceptar
6. Cierre la página.

## <a name="check-on-hand-inventory-by-location"></a>Comprobar el inventario disponible por ubicación
1. Vaya a Gestión de almacén > Consultas e informes > Inventario disponible por ubicación.
2. En el campo Almacén, escriba un valor.
    * Si utiliza a la empresa de datos de prueba USMF, puede usar “51".  
3. Actualice la página.
4. Haga clic en Mostrar dimensiones.
5. Haga clic en Aceptar
6. Cierre la página.

