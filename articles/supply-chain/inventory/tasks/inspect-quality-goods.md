---
title: Inspeccionar la calidad de las mercancías
description: Este procedimiento muestra cómo procesar un pedido de calidad.
author: perlynne
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventQualityOrderTable, InventQualityOrderLineResults, HcmWorkerLookUp
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: perlynne
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f9e9d750f116db62519ac7148f19bf62050430e9
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "315438"
---
# <a name="inspect-the-quality-of-goods"></a>Inspeccionar la calidad de las mercancías

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento muestra cómo procesar un pedido de calidad. Puede ejecutar esta guía en la empresa de datos de demostración USMF. Antes de comenzar este procedimiento de ejemplo, debe confirmar el pedido de compra "000016" y registrar una recepción de producto. Esto crea automáticamente un pedido de calidad. Las inspecciones de calidad las lleva a cabo normalmente un empleado de control de calidad.


## <a name="select-a-quality-order"></a>Selección de un pedido de calidad
1. Vaya a Gestión del inventario > Tareas periódicas > Administración de calidad > Pedidos de calidad.
2. En la lista, marque la fila seleccionada.
    * Seleccione el pedido de calidad que se creó antes de empezar este procedimiento.  

## <a name="record-test-results"></a>Registrar resultados de prueba
1. Haga clic en Resultados.
2. Haga clic en Editar.
3. En el campo Cantidad de resultado, especifique un número.
4. En la lista, marque la fila seleccionada.
5. En el campo Resultado, haga clic en el botón desplegable para abrir la búsqueda.
6. En la lista, busque y seleccione el registro deseado.
    * En este ejemplo, el resultado se basa en un resultado predefinido. Normalmente, registrará un resultado de prueba más específico, como el tamaño u otra dimensión.  
7. En la lista, haga clic en el vínculo de la fila seleccionada.
8. Haga clic en Guardar.
9. Cierre la página.

## <a name="validate-the-quality-order"></a>Validar el pedido de calidad
1. Haga clic en Validar.
2. En el campo Validado por, haga clic en el botón desplegable para abrir la búsqueda.
    * Seleccione el usuario que realiza la inspección.  
3. En la lista, haga clic en el vínculo de la fila seleccionada.
4. Haga clic en Seleccionar.
5. Haga clic en Aceptar
6. Cierre la página.

