---
title: Generar documentos electrónicos y actualizar datos de aplicación utilizando ER
description: Puede diseñar los formatos de informes electrónicos (ER) que se pueden usar en la aplicación Finance and Operations para generar documentos electrónicos salientes. También puede diseñar formatos de ER que analizan los documentos electrónicos entrantes y usan el contenido en esos documentos para actualizar los datos de la aplicación.
author: NickSelin
manager: AnnBe
ms.date: 11/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: ERSolutionTable, ERVendorTable, ERWorkspace
audience: Developer, IT Pro, Application user
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 27621
ms.assetid: 018a11ae-854c-4f36-9358-8c39baca882d
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 2a989b0000766478c71b243d7793b2fc8c4ece28
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "349225"
---
# <a name="generate-electronic-documents-and-update-application-data-by-using-er"></a>Generar documentos electrónicos y actualizar datos de aplicación utilizando ER

[!include [banner](../includes/banner.md)]

Puede diseñar los formatos de informes electrónicos (ER) que se pueden usar en la aplicación Finance and Operations para generar documentos electrónicos salientes. También puede diseñar formatos de ER que analizan los documentos electrónicos entrantes y usan el contenido en esos documentos para actualizar los datos de la aplicación.

Con esta funcionalidad, un único formato de ER se puede usar para generar documentos electrónicos salientes y actualizar los datos de la aplicación. Esta función también se puede en las situaciones siguientes:

- Para evitar el uso repetido de datos de la aplicación en procesos posteriores puede marcar un dato de aplicación inmediatamente después que se usa para generar documentos electrónicos. Por ejemplo, puede marcar transacciones de pago como ya procesadas inmediatamente después de que se hayan incluido en un mensaje de pago generado.
- Para archivar los detalles del procesamiento de los documentos electrónicos que se han generado mediante la lógica de ER. Por ejemplo, una identificación única del mensaje de pago que se genera mediante la expresión de ER. La expresión se basa en la información especificada al cuadro de diálogo de ER cuando el formato de ER se ejecuta para generar documentos.

Para obtener más información acerca de esta función, reproduzca el conjunto de documentos Generar ER con las guías de tareas de actualización de los datos de la aplicación (parte del proceso empresarial 7.5.4.3 Adquirir/Desarrollar componentes de solución/servicios de la TI (10677)), que describen los detalles de la generación de informes y el archivado de intrastat. Los archivos siguientes son necesarios para completar determinados pasos en estas guías de tareas. Descargue y guardar estos archivos en su equipo local.

- [Configuración del modelo de datos de ER: intrastat (modelo)](https://go.microsoft.com/fwlink/?linkid=849038)
- [Configuración de la asignación del modelo de ER: intrastat (asignación)](https://go.microsoft.com/fwlink/?linkid=849038)
- [Configuración del formato de ER: intrastat (formato)](https://go.microsoft.com/fwlink/?linkid=849038)
