---
title: Desactivar una versión de flujo de producción
description: Cuando ya no se necesita una versión del flujo de producción activa, se puede desactivar.
author: cvocph
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LeanProductionFlow
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: conradv
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 091cafd02bd568323e586373fc8b0f983afee343
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "340761"
---
# <a name="deactivate-a-production-flow-version"></a>Desactivar una versión de flujo de producción

[!include [task guide banner](../../includes/task-guide-banner.md)]

Cuando ya no se necesita una versión del flujo de producción activa, se puede desactivar. Debe usar esta opción únicamente si todas las reglas kanban y las actividades han terminado y no están activadas de nuevo. Tenga en cuenta que la fecha de caducidad de todas las reglas kanban relacionadas con esta versión del flujo de producción se actualizarán con la fecha y hora actuales. 

Para modificar una versión de flujo de producción activa, considere configurar una fecha de vencimiento para la versión activa y cree una nueva versión. Esto le permitirá continuar con sus operaciones de producción mientras prepara la nueva versión y las reglas kanban relacionadas. 

Para que una versión del flujo de producción activa expire, deberá establecer una fecha de vencimiento. En ese sentido, la desactivación es más bien una excepción que una regla. 

Para este procedimiento necesita un flujo de producción con una versión que se pueda desactivar. No intente esto en un entorno de producción salvo que totalmente convencido de que la versión que está completamente obsoleta.


## <a name="deactivate-a-production-flow-version"></a>Desactivar una versión de flujo de producción
1. Vaya a Control de producción > Configuración > Flujo de producción lean > Flujos de producción.
2. En la lista, busque y seleccione el registro deseado.
3. En la lista, haga clic en el vínculo de la fila seleccionada.
4. En la lista, busque y seleccione el registro deseado.
5. Haga clic en Desactivar.
    * No continúe si no está convencido de que esta versión del flujo de producción está obsoleta. Haciendo clic en Acepar expirarán todas las reglas kanban activas y se pondrá fin de forma inmediata a todas las actividades de producción y de reabastecimiento de esta versión del flujo de producción.  
6. Haga clic en Aceptar

