---
title: Recuento de etiquetas de inventario
description: Este artículo proporciona información sobre el recuento de etiquetas, que se usa para comparar el contenido real de un almacén con el inventario disponible.
author: MarkusFogelberg
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventJournalCount, InventJournalCountTag
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 11594
ms.assetid: 03772d0e-5c37-454c-ab85-82bc8b60a76d
ms.search.region: Global
ms.author: mafoge
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: dff899d0e6d94287c0f1924fe1787189d79c09f4
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "328962"
---
# <a name="inventory-tag-counting"></a>Recuento de etiquetas de inventario

[!include [banner](../includes/banner.md)]

[!include [retail name](../includes/retail-name.md)]

Este artículo proporciona información sobre el recuento de etiquetas, que se usa para comparar el contenido real de un almacén con el inventario disponible.

Al crear líneas en la página **Recuento de etiquetas**, coloca un número de etiqueta en cada artículo de inventario, como un número del 1 al 500. Durante el recuento, escribe el código de artículo y la cantidad en una etiqueta correspondiente. Esta etiqueta se puede usar como la base para la entrada del diario de recuento de etiquetas. Tras registra el diario de recuento de etiquetas, se crea un diario de recuento nuevo en la página **Recuento**. El nuevo diario se basa en las líneas de diario de recuento de etiquetas que ha creado. Para contar las etiquetas de artículos por una dimensión de inventario específica, seleccione la dimensión en la página **Mostrar dimensiones** que aparece al crear el diario de recuento de etiquetas. Por ejemplo, para contar artículos de un almacén especifico, active la casilla **Almacén**. Si el control deslizante **Bloquear artículos durante el recuento** de la página **Parámetros de gestión de inventario y almacenes** está seleccionado, los artículos no se pueden actualizar físicamente durante el recuento. Sin embargo, los artículos de los diarios de recuento de etiquetas no se bloquean durante el recuento. Las transacciones de inventario no se crean hasta que las líneas de recuento de etiquetas se registran y se transfieren a un diario de recuento. Si las etiquetas se colocan aleatoriamente y desea identificar las etiquetas que faltan, haga clic en el encabezado de columna **Etiqueta** para ordenar las líneas por etiqueta.

<a name="additional-resources"></a>Recursos adicionales
--------

[Recuento cíclico](../warehousing/cycle-counting.md)
