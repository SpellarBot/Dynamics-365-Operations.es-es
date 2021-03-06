---
title: Definir reglas y directivas de idoneidad para prestaciones
description: Este registro mostrará cómo puede crear reglas y directivas de opción a prestaciones y después asignar reglas a las prestaciones.
author: andreabichsel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicySourceDocumentRuleType, SysPolicyListPage, SysPolicy, HcmBenefitEligibilityPolicy, HcmBenefit
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: d0d35266c95cfbf3473a14fec47a1c748229dd25
ms.sourcegitcommit: 608e68b603afef9eb98d8fb25e90109c2473ef87
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "859238"
---
# <a name="define-benefit-eligibility-rules-and-policies"></a>Definir reglas y directivas de idoneidad para prestaciones

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este registro mostrará cómo puede crear reglas y directivas de opción a prestaciones y después asignar reglas a las prestaciones.  

La empresa de datos de prueba utilizada para crear este registro es USMF.


## <a name="create-benefit-eligibility-policy-rule-type"></a>Creación de tipos de reglas de directivas de opción de prestaciones
1. Vaya a Recursos humanos > Prestaciones > Idoneidad > Tipos de reglas de idoneidad de prestaciones.
2. Haga clic en Nuevo.
3. En el campo Nombre de regla, escriba un valor.
4. En el campo Descripción, escriba un valor.
5. En el campo Nombre de consulta, haga clic en el botón desplegable para abrir la búsqueda.
6. En la lista, haga clic en el vínculo de la fila seleccionada.
7. Haga clic en Guardar.
8. Cierre la página.

## <a name="benefit-eligibility-policy"></a>Directiva de idoneidad de beneficio
1. Vaya a Recursos humanos > Prestaciones > Idoneidad > Políticas de opción a prestaciones.
2. Seleccione una directiva de prestación existente.
3. En la lista, haga clic en el vínculo de la fila seleccionada.
4. Expanda las secciones Organizaciones de directivas.  Aquí puede agregar o quitar cualquier organización que desee incluir en la directiva.
5. Expanda o contraiga la sección Reglas de directivas.
6. En la lista, busque la regla de directiva que creó anteriormente.
7. Haga clic en Crear regla de directivas.
8. En el campo Fecha de vigencia, especifique la fecha en la que desea que la directiva entrara en vigor.
    * Al definir las fechas de vigencia y finales, podrá realizar cambios futuros en las reglas de las directivas, así como ya no tendrá que volver a la directiva cuando desee que los cambios surtan efecto.  
9. 
    * Por ejemplo, si quisiera que la regla solo se aplicase a los directores de ventas, podría crear la cláusula Where para decir: Where descripción del puesto equals director de ventas.  Puede incluir operadores "And" u "Or" en las instrucciones Where de las reglas.  
10. Haga clic en Aceptar
11. Cierre la página.
12. Cierre la página.

## <a name="assign-rule-to-benefit"></a>Asignación de reglas a prestaciones
1. Vaya a Recursos humanos > Prestaciones > Prestaciones.
2. En la lista, busque y seleccione el registro deseado.
3. En la lista, haga clic en el vínculo de la fila seleccionada.
4. Expanda o contraiga la sección Regla de idoneidad.
5. Haga clic en Editar.
6. En el campo Idoneidad, seleccione Basada en reglas en la lista.
7. En el campo Tipo de regla, haga clic en el botón desplegable para abrir la búsqueda.
8. En la lista, busque y seleccione la regla que creó anteriormente.
9. En la lista, haga clic en el vínculo de la fila seleccionada.
10. Haga clic en Guardar.
11. Cierre el formulario.

