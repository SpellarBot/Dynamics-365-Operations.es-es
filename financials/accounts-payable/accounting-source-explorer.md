---
title: Explorador de origen de contabilidad
description: "Este artículo proporciona información acerca del explorador del origen de contabilidad, que puede usar para análisis detallado de la información de origen detrás de asientos contables de la contabilidad general."
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 15391
ms.assetid: 57b95899-7298-43c0-8034-45b5d993cbf2
ms.search.region: Global
ms.author: peakerbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 9f4d7fdd8cfa7a540fce219f6ae4792e57dfbe44
ms.openlocfilehash: 8913e61285d5d180883471991b659ddcb260afe3
ms.lasthandoff: 03/31/2017


---

# <a name="accounting-source-explorer"></a>Explorador de origen de contabilidad

[!include[banner](../includes/banner.md)]


Este artículo proporciona información acerca del explorador del origen de contabilidad, que puede usar para análisis detallado de la información de origen detrás de asientos contables de la contabilidad general.

El Explorador de origen de la contabilidad es una nueva página que muestra la información de origen. Puede usar el Explorador del origen de contabilidad como herramienta independiente o analizar los detalles detrás de asientos contables de la contabilidad general. Por ejemplo, puede usar el Explorador de origen de contabilidad para obtener la información de origen detallada para un saldo en Saldo de comprobación o para una transacción de asiento. Puede usar la característica Exportar a Microsoft Excel para segmentar y desglosar la información en Microsoft Excel (por ejemplo, en una tabla dinámica o un informe de tablas dinámicas).

El Explorador de origen de contabilidad siempre muestra el mismo importe total por cuenta contable que muestra la Contabilidad general (por ejemplo, en un Saldo de comprobación). Como en un Saldo de comprobación, puede mostrar segmentos en columnas independientes. Solo tiene que seleccionar el conjunto adecuado de dimensiones financieras. 

Puede usar parámetros para definir un intervalo de fechas para el análisis. Esta funcionalidad también es similar a la funcionalidad de Saldo de comprobación.

Para todos los documentos que usan el marco del documento de origen, El explorador de origen de contabilidad muestra información adicional basada en las distribuciones contables y, si procede, en distribuciones contables del proyecto. Esta información incluye el tipo de importe monetario, el proyecto, la actividad, la categoría y la propiedad de línea. A continuación se muestran algunos ejemplos del análisis que puede realizar:

-   Desviaciones entre los pedidos de compra y las facturas de proveedor, porque cada desviación está representada por un tipo de importe monetario, como la desviación de cargos
-   Gastos y horas facturables frente a no facturables por proyecto, unidad de negocio y cuenta principal

Para documentos de origen que usen el concepto de identidades de referencia de documento de origen, el Explorador de origen de contabilidad muestra incluso más detalles, como el cliente, el proveedor, el trabajador, el producto, la cantidad, el texto de unidad y las descripciones. A continuación se muestran algunos ejemplos del análisis que puede realizar:

-   Los gastos de hotel por unidad de negocio y el marca de hotel para un período fiscal, en función de los informes de gastos
-   Descuentos por proveedor, producto, departamento

Para estos documentos, también puede navegar hasta el documento de origen real desde el Explorador de origen de contabilidad.



