---
title: Modificar formatos de informe electrónico al aplicar de nuevo plantillas de Excel
description: Este tema proporciona información acerca de cómo puede modificar el formato de informes electrónicos (ER) que se usa para generar documentos empresariales reaplicando una plantilla de Excel modificada.
author: NickSelin
manager: AnnBe
ms.date: 06/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: ERSolutionTable, ERVendorTable, ERWorkspace
audience: Developer, IT Pro, Application user
ms.reviewer: kfend
ms.search.scope: Operations
ms.custom: 27621
ms.assetid: e3f7960d-2e01-46a7-9ac8-c355ac933cd6
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8707f7b184bb66648edd0e48672c5514a0a5caf1
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "313667"
---
# <a name="modify-electronic-reporting-formats-by-reapplying-excel-templates"></a>Modificar formatos de informe electrónico al aplicar de nuevo plantillas de Excel

[!include [banner](../includes/banner.md)]

La herramienta de informes electrónicos (ER) se usa para generar documentos empresariales en formato electrónico. Para generar un documento empresarial, debe crear un formato de ER, y luego usar el diseñador de ER para definir el diseño de documento empresarial y especificar los datos que se deben incluir en él. A continuación puede ejecutar el formato de ER para generar el documento empresarial.

La herramienta de ER se puede usar para generar documentos empresariales como archivos de Microsoft Excel. Puede usar un documento de Excel como plantilla para estos documentos. Para definir el diseño de documento en el diseñador de ER, puede importar el contenido del documento de Excel que desea utilizar como plantilla en el formato definido de ER. Para más detalles y practicar este escenario, reproduzca la guía de tareas **Diseñar una configuración ER para generar informes en formato OPENXML** (parte del proceso empresarial 7.5.4.3 Adquirir/Desarrollar componentes de solución/servicios de la TI (10677)).

Si edita el documento de Excel que se usa como plantilla para un documento empresarial, la nueva funcionalidad de ER permite reaplicar la plantilla actualiza al formato de ER. El formato de ER se actualiza a continuación para ajustarse a la plantilla actualizada. Para más detalles sobre esta funcionalidad, reproduzca la guía de tareas **Modificar un formato de ER reaplicando una plantilla de Excel** (parte del proceso empresarial 7.5.5.3 Adquirir o desarrollar componentes de soluciones y servicios de TI (10683)). En el paso de la guía de tareas donde importa una plantilla actualizada, utilice plantilla modificada del archivo de Excel de informe de pago, SampleVendPaymWsReport2, como plantilla.
