---
title: Crear estructuras contables
description: Esta guía de tareas describe los pasos de la creación de una estructura contable.
author: aprilolson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DimensionConfigureAccountStructure, DimensionCreateAccountStructure, DimensionHierarchyAddLevel, DimensionHierarchyConstraintActivate
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a7dd71cc072d49f47b1d77d3a688984cd4aaa624
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "356401"
---
# <a name="create-account-structures"></a>Crear estructuras contables

[!include [task guide banner](../../includes/task-guide-banner.md)]

Esta guía de tareas describe los pasos de la creación de una estructura contable. Los pasos usan la empresa de datos de prueba USMF.

1. Vaya a Contabilidad general > Plan contable > Estructuras > Configurar estructuras contables.
2. Haga clic en Nueva para abrir el cuadro de diálogo desplegable.
3. En el campo Estructura contable, escriba un nombre para describir el propósito de la estructura contable.
4. En el campo Descripción, escriba una descripción para especificar el propósito de la estructura contable.
5. Haga clic en Crear.
6. Haga clic en Agregar segmento.
7. En la lista Dimensiones, seleccione la dimensión que se agregará a la estructura contable.
8. Haga clic en Agregar segmento.
9. Haga clic en Agregar segmento.
10. En la lista Dimensiones, seleccione la dimensión que se agregará a la estructura contable.
11. Haga clic en Agregar segmento.
12. Haga clic en Agregar segmento.
13. En la lista Dimensiones, seleccione la dimensión que se agregará a la estructura contable.
14. Haga clic en Agregar segmento.
15. En la cuadrícula, seleccione el segmento para editar los valores permitidos.
    * Por ejemplo, haga clic en Cuenta principal.  
16. En el campo Operador, seleccione una opción, como está entre e incluye.
17. En el campo Valor, escriba un valor.
    * Por ejemplo, 600000.  
18. En el campo hasta, escriba un valor.
    * Por ejemplo, 699999.  
19. Haga clic en Aplicar.
20. En la cuadrícula, seleccione el segmento para editar los valores permitidos.
    * Por ejemplo, Departamento.  
21. En el campo Operador, seleccione una opción, como está entre e incluye.
22. En el campo Valor, escriba un valor.
    * Por ejemplo, 022.  
23. En el campo hasta, escriba un valor.
    * Por ejemplo, 031.  
24. Haga clic en Agregar nuevos criterios.
25. En el campo Operador, seleccione una opción, como está entre e incluye.
26. En el campo Valor, escriba un valor.
    * Por ejemplo, 033.  
27. En el campo hasta, escriba un valor.
    * Por ejemplo, 034.  
28. Haga clic en Aplicar.
29. En la cuadrícula, seleccione el segmento para editar los valores permitidos.
    * Por ejemplo, Centro de coste.  
30. En el campo CostCenter, escriba un valor.
    * Por ejemplo, 007..021.  
31. Haga clic en Agregar.
32. En el campo MainAccount, escriba un valor.
    * Por ejemplo, 600000..699999  
33. En la cuadrícula, seleccione el segmento para editar los valores permitidos.
    * Por ejemplo, Departamento.  
34. En el campo Departamento, escriba un valor.
    * Por ejemplo, 032.  
35. En el campo CostCenter, escriba un valor.
    * Por ejemplo, 086.  
36. Haga clic en Validar.
37. Haga clic en Activar.
38. Haga clic en Activar.

