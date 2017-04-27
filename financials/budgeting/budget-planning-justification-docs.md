---
title: "Planificación presupuestaria para documentos de justificación"
description: "Los documentos de justificación proporcionan una descripción para aquellos que solicitan un presupuesto para explicar por qué es necesario un presupuesto específico."
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: Operations, Core
ms.custom: 259594
ms.assetid: 52576fad-32b9-48f2-8197-c11ec313fc29
ms.search.region: Global
ms.author: ryansand
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: 0c6a7bdc4ba82dd57ab3e395e6dfb0ae4de31fc4
ms.openlocfilehash: c86d01fec3d8d7c210c7e73a034f4e9e384a0dcf
ms.lasthandoff: 03/31/2017


---

# <a name="budget-planning-justification-documents"></a>Planificación presupuestaria para documentos de justificación

[!include[banner](../includes/banner.md)]


Los documentos de justificación proporcionan una descripción para aquellos que solicitan un presupuesto para explicar por qué es necesario un presupuesto específico. 

El administrador presupuestario crea una plantilla del plan presupuestario en Microsoft Word y la asigna al proceso de planificación presupuestaria actual. A continuación, los propietarios de presupuesto pueden abrir la plantilla y tener los datos rellenados automáticamente en Word en función de su solicitud de presupuesto. Posteriormente, pueden agregar texto o datos adicionales antes de guardar y adjuntar el documento de justificación personalizado a su plan presupuestario.

##### <a name="set-up-microsoft-dynamics-office-add-in-for-microsoft-word"></a>Configure el complemento de Microsoft Dynamics Office para Microsoft Word

1.  Abra un nuevo documento de Microsoft Word.
2.  Haga clic en **Insertar** en la cinta de opciones y haga clic en **Tienda**.
3.  Busque el complemento de Microsoft Dynamics Office y haga clic en **Agregar**.
4.  En Word, en el panel derecho, haga clic en **Agregar información de servidor**.
5.  Escriba o pegue la dirección URL del servidor y haga clic en **Aceptar**.

##### <a name="define-the-justification-template-in-microsoft-word"></a>Defina la plantilla de justificación en Microsoft Word

1.  Haga clic en **Diseño** en el complemento de Microsoft Dynamics Office una vez que haya iniciado sesión.
2.  Para obtener información del encabezado, utilice el botón **Agregar campos**.
3.  Seleccione el origen de datos de entidad de BudgetPlanJustification y haga clic en **Siguiente**. **Nota:** Esta entidad es necesaria para cualquier documento de justificación. Se pueden utilizar otras entidades, pero la nueva carga en Microsoft Dynamics 365 for Operations fallará si no se incluye esta entidad.
4.  Agregue las etiquetas y los valores BudgetPlanName, BudgetPlanPreparer, ResponsibilityCenter y DocumentNumber en el documento de Word. **Nota:** Si es necesario, puede usar sus propias etiquetas personalizadas en lugar de las etiquetas estándar.
5.  Haga clic en **Hecho** para completar la sección de encabezado.
6.  Para el detalle de nivel de línea de los importes del plan presupuestario, haga clic en **Agregar tabla**.
7.  Una vez más, seleccione el origen de datos de entidad de BudgetPlanJustification y haga clic en **Siguiente**.
8.  Agregue campos para EffectiveDate, ScenarioName, AccountDisplayValue y AccountingCurrencyExpenseAmount. **Nota:** Si hay comentarios disponibles para agregar dentro de las líneas individuales del plan presupuestario, estos se pueden agregar a la tabla aquí.
9.  Agregue cualquier instrucción adicional para proporcionar al usuario final y realice cualquier formato o estilo necesario al documento.
10. Guarde el documento en su equipo local y cierre el archivo antes de continuar.

##### <a name="set-up-the-budget-planning-process-to-use-the-justification-template"></a>Configure el proceso de planificación presupuestaria para usar la plantilla de justificación

1.  En Microsoft Dynamics 365 for Operations, vaya a **Gestión presupuestaria** &gt; **Configuración** &gt; **Planificación presupuestaria** &gt; **Plantillas de documento de justificación**.
2.  Haga clic **Nuevo** y busque su documento de Microsoft Word recién creado.
3.  Escribe un nombre y una descripción para la plantilla. Haga clic en **Aceptar**.
4.  Vaya a **Gestión presupuestaria** &gt; **Configurar** &gt; **Planificación** **presupuestaria** &gt; **Proceso de planificación presupuestaria**.
5.  Seleccione el proceso en el que debe utilizarse la plantilla de justificación y haga clic en **Editar**.
6.  En el campo **Plantilla de documento de justificación**, seleccione la plantilla adecuada y guarde.

##### <a name="edit-and-save-personalized-justification-documents"></a>Edite y guarde los documentos de justificación personalizados

1.  En Dynamics 365 for Operations, cree un nuevo plan presupuestario o abra un plan presupuestario existente.
2.  En el menú desplegable **Justificación**, seleccione **Crear nueva justificación**.
3.  Tras completar los detalles, seleccione el documento personalizado que desea cargar desde el menú desplegable **Justificación**.




