---
title: Reclasificar activos fijos
description: Para reclasificar un activo fijo, debe transferirlo a un grupo de activos fijos nuevo o asignarle un número de activo fijo nuevo en el mismo grupo.
author: saraschi2
manager: AnnBe
ms.date: 10/30/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d8e289e2c18fd28829fb4b749933ae1d84e0b631
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "323304"
---
# <a name="reclassify-fixed-assets"></a>Reclasificar activos fijos

[!include [task guide banner](../../includes/task-guide-banner.md)]

Para reclasificar un activo fijo, debe transferirlo a un grupo de activos fijos nuevo o asignarle un número de activo fijo nuevo en el mismo grupo. 

Cuando se reclasifica un activo fijo:

• Todos los modelos de valor del activo fijo existente se crean para el activo fijo nuevo. Cualquier información que se haya configurado para el activo fijo se copia en el activo fijo nuevo. El estado de los modelos de valor para el activo fijo original es Cerrado. 

• Los modelos de valor nuevo de un nuevo activo fijo contienen la fecha de reclasificación en el campo Fecha de adquisición. La fecha del campo Fecha de ejecución de la depreciación se copia de la información del activo original. Si ya se inició la depreciación, el campo Fecha en la que se ejecutó la última depreciación mostrará la fecha de reclasificación. 

• Las transacciones de activos fijos existentes para el activo fijo original se cancelan y se vuelven a generar para el activo fijo nuevo.

1. Vaya a Activos fijos > Tareas periódicas > Reclasificación.
2. En el campo Grupo de activos fijos, seleccione el grupo a reclasificar.
3. En el campo número de activo fijo, seleccione el activo fijo a reclasificar.
4. En el campo Nuevo grupo de activos fijos, seleccione un grupo al que transferirle el activo fijo.
    * Si el nuevo grupo de activos fijos está vinculado a una secuencia numérica, el campo Nuevo número de activo fijo se actualiza con el número de la nueva secuencia numérica del grupo de activos fijos. De no ser así, el campo Nuevo número de activo fijo se actualizará con el número de la secuencia numérica que esté configurada en la página de los parámetros de activo fijo. Si no hay configurada una secuencia numérica en la página de parámetros del Activo fijo, introduzca un número en el campo Nuevo número de activo fijo.  
5. En el campo Fecha de reclasificación, escriba una fecha.
6. En el campo Series de asientos, especifique o seleccione un valor.
7. Haga clic en Aceptar

