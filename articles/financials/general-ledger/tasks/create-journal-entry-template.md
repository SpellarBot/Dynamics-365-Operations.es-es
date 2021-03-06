---
title: Creación de un movimiento de diario mediante una plantilla
description: Los asientos del diario registrados se pueden guardar como plantillas de asientos y aplicarse en un nuevo asiento del diario.
author: aprilolson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransDaily, LedgerJournalTransVoucherTemplate
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4a749740b62e39202d502a112f947679f85ca085
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "316818"
---
# <a name="create-a-journal-entry-using-template"></a>Creación de un movimiento de diario mediante una plantilla

[!include [task guide banner](../../includes/task-guide-banner.md)]

Los asientos del diario registrados se pueden guardar como plantillas de asientos y aplicarse en un nuevo asiento del diario. Este procedimiento usa la empresa de demostración USMF.

1. Contabilidad general > Movimientos de diario > Diarios generales. Haga clic en Nuevo.
    * Este procedimiento comienza por crear y registrar un asiento de diario, pero cualquier asiento del diario previamente registrado se puede guardar como plantilla.  
2. En el campo Nombre, haga clic en el botón desplegable para abrir la búsqueda.
3. En la lista, busque y seleccione el registro deseado.
4. En la lista, haga clic en el vínculo de la fila seleccionada.
5. Haga clic en Líneas.
6. Especifique una cuenta para el tipo Cuenta.
7. En el campo Descripción, escriba un valor.
8. Especifique un importe en el campo Débito.
9. Haga clic en Nuevo.
10. Especifique una cuenta diferente para el tipo Cuenta.
11. En el campo Descripción, escriba un valor.
12. Especifique un importe en el campo Débito.
13. Haga clic en Nuevo.
14. En el campo Cuenta, especifique los valores deseados.
15. En el campo Descripción, escriba un valor.
16. Especifique un importe en el campo Crédito para saldar el asiento.
17. Haga clic en Registrar.
18. Haga clic en Funciones.
19. Haga clic en la plantilla Guardar asiento.
20. Este procedimiento supone un tipo de plantilla de porcentaje. Haga clic en Aceptar
    * • Porcentaje: los importes del asiento se convierten en factores de porcentaje, lo que permite aplicar cualquier importe cuando se selecciona la plantilla de asientos.  • Importe: los importes reales se almacenarán y se aplicarán.  
21. Haga clic en Diarios generales.
22. Haga clic en Nuevo.
23. En el campo Nombre, haga clic en el botón desplegable para abrir la búsqueda.
24. En la lista, haga clic en el vínculo de la fila seleccionada.
25. Haga clic en Líneas.
26. Haga clic en Funciones.
27. Haga clic en Seleccionar plantilla de asientos.
28. Busque la plantilla que ha creado anteriormente. Haga clic en Aceptar
    * Es posible que tenga que hacer clic en el paso anterior y seleccionar la plantilla correcta si existen otras plantillas.  
29. En el campo Importe, especifique el importe que se aplicará el asiento.
    * El campo de importe solo se muestra si la plantilla de asientos es del tipo Porcentaje.  
30. Haga clic en Aceptar

