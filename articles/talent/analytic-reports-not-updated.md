---
title: Los informes de análisis no están actualizados
description: Este tema explica qué hacer si los cambios en los datos de un cliente no se muestran en los espacios de trabajo de un cliente.
author: andreabichsel
manager: AnnBe
ms.date: 11/02/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2018-11-02
ms.dyn365.ops.version: Talent
ms.openlocfilehash: d6a6487b50908093f876237ffef840a3144b3fe6
ms.sourcegitcommit: 608e68b603afef9eb98d8fb25e90109c2473ef87
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "857462"
---
# <a name="analytic-reports-are-not-updated"></a>Los informes de análisis no están actualizados

[!include [banner](includes/banner.md)]

**Emisión**

Los cambios de los datos de un cliente no aparecen en las pestañas **Análisis** de las áreas de trabajo de un cliente.

**Causa**

De forma predeterminada, los informes de Microsoft Power BI se actualizan cada cuatro horas, de acuerdo con la programación del trabajo por lotes de medida de implementación.

**Resolución**

Este problema podría ser simplemente una cuestión de control de tiempo. Siga estos pasos para iniciar el trabajo por lotes y actualizar las áreas de trabajo de análisis.

1. Abre la página **Trabajos por lotes** en **Administración del sistema \> Vínculos \> Trabajos por lotes \> Trabajos por lotes**. De manera alternativa, use Búsqueda y escriba **Trabajos por lotes**.
1. Encuentre el trabajo **Implementación de medida** en la lista.
1. Seleccione **Editar** en la parte superior de la página, y establezca la fecha /hora inicial programada a un valor que actualice el análisis más cercano a la hora actual.

![Trabajos por lotes](media/batch-jobs.png)
