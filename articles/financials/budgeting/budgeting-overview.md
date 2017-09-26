---
title: "Página principal de Gestión presupuestaria"
description: "En este tema, se proporciona una visión general de los componentes de la funcionalidad de gestión presupuestaria, las herramientas de gestión presupuestaria y las funciones de informes de Microsoft Dynamics 365 for Finance and Operations, Enterprise Edition."
author: twheeloc
manager: AnnBe
ms.date: 08/09/2017
ms.topic: index-page
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 106043
ms.assetid: 702f692e-ad1c-4798-8d3e-c3cf8591d3fa
ms.search.region: Global
ms.author: twheeloc
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 529751c09b8f99f986cad23a633bea661929d558
ms.openlocfilehash: e59c29370353a6e4a67d2b892e2024ca78d560fc
ms.contentlocale: es-es
ms.lasthandoff: 08/09/2017

---

# <a name="budgeting-home-page"></a>Página principal de Gestión presupuestaria

[!include[banner](../includes/banner.md)]


En este tema, se proporciona una visión general de los componentes de la funcionalidad de gestión presupuestaria, las herramientas de gestión presupuestaria y las funciones de informes de Finance and Operations. 

<a name="components-of-budgeting-functionality"></a>Componentes de la funcionalidad de gestión presupuestaria
-------------------------------------

El ciclo de planificación de recursos para una empresa consta, normalmente, de las actividades de planificación, gestión presupuestaria y previsión.

[![Componentes de la funcionalidad Gestión presupuestaria](./media/budgeting-functionality-components.jpg)](./media/budgeting-functionality-components.jpg)

Los procesos tanto para la planificación estratégica a largo plazo como para la planificación presupuestaria anual se admiten a través de un documento de plan presupuestario. Los documentos del plan presupuestario están estrechamente integrados con Microsoft Excel. Los usuarios pueden configurar escenarios monetarios y cuantitativos sin límites y, también, definir una jerarquía organizativa de gestión presupuestaria para admitir métodos de gestión presupuestaria ascendentes y descendentes. Una vez establecido y aprobado un presupuesto en Finance and Operations, el plan presupuestario se convierte en una entrada de registro presupuestario. Las entradas de registro presupuestario proporcionan herramientas para mantener el presupuesto y para mantener los importes localizables por los códigos de presupuesto. Las entradas de registro presupuestario le permiten revisar presupuestos originales, realizar transferencias y transferir importes de presupuesto del año anterior. En función del presupuesto establecido, una empresa puede habilitar el control presupuestario. El nivel de control depende de la cultura de la organización y del nivel de vencimiento de la organización. Las organizaciones que tienen un nivel de vencimiento bajo pueden dejar el presupuesto "tal cual" y ser más reactivas que proactivas si un presupuesto no cumple las expectativas. Otras organizaciones pueden habilitar las directivas de control presupuestario que impiden a los usuarios comprar si no hay fondos presupuestarios disponibles.

Por último, las organizaciones muy maduras pueden establecer una cultura de organización en la que se forme a los empleados acerca de los objetivos de la organización y cuyos objetivos se puedan perseguir a través de directivas como "Considerar una reunión en línea en lugar de un viaje". Finance and Operations incluye un marco de control presupuestario que permite a la dirección de la empresa seleccionar un control rígido (que impide los registros que superarían el presupuesto) o un control flexible (con el que se advierte a los usuarios que superarán los fondos presupuestarios disponibles, pero se les permite decidir cómo continuar). Por último, puede usar las previsiones continuas. Una previsión continua es una comparación periódica de los valores de presupuesto frente a los valores reales y se usa para definir si el funcionamiento de la empresa se adecua al presupuesto. La previsión continua también se usa para identificar tendencias. En Finance and Operations se admiten las previsiones continuas, a través de un documento de plan presupuestario, como las actividades iniciales de planificación. Las previsiones continuas se pueden realizar en paralelo con la planificación para el próximo ciclo presupuestario.

-   [Presupuesto básico: visión general y configuración](basic-budgeting-overview-configuration.md)
-   [Control presupuestario: visión general y configuración](budget-control-overview-configuration.md)
-   [Planificación presupuestaria: visión general y configuración](budget-planning-overview-configuration.md)
-   [Previsión de puestos](position-forecasting.md)
-   [Documentos de justificación de la planificación presupuestaria](budget-planning-justification-docs.md)
-   [Plantillas de Microsoft Excel para la planificación presupuestaria](budget-planning-excel-templates.md)

## <a name="budgeting-tools-in-finance-and-operations"></a>Herramientas de gestión presupuestaria de Finance and Operations
[![Herramientas de gestión presupuestaria](./media/budgeting-tools.jpg)](./media/budgeting-tools.jpg) 

Existen otras funciones de planificación y gestión presupuestaria en Finance and Operations que se integran con los presupuestos contables.

-   **Presupuestos de recursos**: los presupuestos de recursos incluyen la planificación de componentes de coste presupuestario detallados para puestos, grupos de compensación, etc.
-   **Presupuestos de activos fijos**: según la información de activos fijos, puede calcular la depreciación planificada y registrar otras transacciones planificadas relacionadas con activos fijos.
-   **Presupuestos de proyecto**: en el módulo de proyectos, puede crear previsiones de proyecto detalladas. Las previsiones de proyectos incluirán detalles acerca de las horas, los gastos, las cuotas y los artículos planificados.
-   **Previsión de demanda**: en función de los datos de transacción históricos, puede estimar la demanda de inventario futura y crear previsiones de demanda.

Para obtener información sobre cómo trasladar los datos de planificación de otros módulos a los planes presupuestarios, vea [Integración de la planificación presupuestaria con otros módulos](budget-planning-integration-other-modules.md).

## <a name="user-interface-and-reporting-capabilities"></a>Interfaz de usuario y funciones de informes
En Finance and Operations, los usuarios pueden crear planes presupuestarios directamente en el cliente de Finance and Operations (mediante una página de documento de plan presupuestario configurable) o en Excel. Excel ofrece varias capacidades adicionales. Por ejemplo, puede usar los datos externos como origen para un plan presupuestario, realizar cálculos personalizados, y usar gráficos y tablas dinámicas de Microsoft. Se pueden configurar la mayoría de las variables en el proceso de planificación presupuestaria. 

Por ejemplo, puede definir quién realiza los presupuestos, qué se presupuesta y cómo es el proceso. Aunque puede usar Excel para la planificación presupuestaria, Finance and Operations se usa como fuente de información única y ayuda a evitar problemas de control presupuestario. Se pueden usar procesos periódicos para incorporar los datos iniciales de gestión presupuestaria en el plan presupuestario. Para los informes, Finance and Operations ofrece un conjunto de páginas de consulta estándares que le permiten ver y analizar los datos de los presupuestos. A los datos del plan presupuestario se puede obtener acceso a través del Management Reporter y se pueden mostrar escenarios del plan presupuestario independientes como columnas en el informe del Management Reporter.






