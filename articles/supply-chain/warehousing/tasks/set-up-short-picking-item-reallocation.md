---
title: Configuración de la reasignación de artículos para la selección corta
description: Este procedimiento muestra cómo permitir que los trabajadores del almacén busquen rápidamente ubicaciones alternativas si no hay suficiente inventario en la ubicación a la que les han dirigido.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSWorkException, WHSWorker
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: mirzaab
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: bf56a0811c4793ee2e3eaf78c8696c3c29e984c3
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "361231"
---
# <a name="set-up-short-picking-item-reallocation"></a>Configuración de la reasignación de artículos para la selección corta

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento muestra cómo permitir que los trabajadores del almacén busquen rápidamente ubicaciones alternativas si no hay suficiente inventario en la ubicación a la que les han dirigido. Se puede usar un proceso automático de reasignación, que usa las directivas de la ubicación para recuperar las mercancías si está disponibles en otra ubicación. Como alternativa, cuando se usa la reasignación manual, se muestra una lista de las ubicaciones con la cantidad disponible en el dispositivo móvil, para que el trabajador del almacén elija de qué ubicación usar el inventario. Puede utilizar este procedimiento en la empresa de datos de demostración USMF. Este procedimiento es para una función que se ha agregado en la versión 1611 de Dynamics 365 for Operations.


## <a name="set-up-work-exceptions"></a>Configurar excepciones de trabajo
1. Ir a Gestión de almacenes > Configurar > Trabajo > Excepciones de trabajo.
2. Haga clic en Nuevo.
    * Es posible definir varias excepciones de trabajo con directivas de la reasignación de artículo diferentes para permitir el trabajador del almacén para elegir uno basado en las necesidades de envío que están procesando.  
3. En el campo Código de excepción de trabajo, escriba un valor.
    * Dé a la excepción de trabajo un título para indicar para qué se utiliza. Por ejemplo, manual de picking corto.  
4. En el campo Descripción, escriba un valor.
5. En el campo Tipo de excepción, seleccione "Selección corta".
6. Active la casilla Ajustar inventario.
    * Esta opción significa que el inventario se ajusta automáticamente a 0 en la ubicación de picking corto.  
7. En el campo Código de tipo de ajuste predeterminado, especifique o seleccione un valor.
    * Por ejemplo, en USMF puede seleccionar "Quitar Res Adj Out".  
8. En el campo Reasignación de artículos, seleccione Manual.
    * Si selecciona Manual o Automático y manual, el trabajador del almacén debe estar habilitado para usar la reasignación manual.  

## <a name="set-up-a-worker-to-use-manual-item-reallocation"></a>Configurar un trabajador para usar la reasignación manual de artículos
1. Cierre la página.
2. Ir a Gestión de almacenes > Configuración > Empleado.
3. Haga clic en Editar.
4. En la lista, seleccione trabajador 24.
5. Expanda la sección Trabajo.
6. Seleccione Sí en el campo Permitir reasignación de artículos manual.

