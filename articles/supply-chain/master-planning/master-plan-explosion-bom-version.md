---
title: Expansión de una versión de lista de materiales
description: En este artículo se explica un escenario de planificación maestra que implica la expansión de una versión de la lista de materiales (L. MAT.).
author: roxanadiaconu
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ReqTransExplosion
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19211
ms.assetid: fe08c2e6-9cc5-4e34-bbb2-cd07843403b5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4f3c800d96805df38a2e31018f2d6c305e3ed7da
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "353917"
---
# <a name="explosion-of-a-bom-version"></a>Expansión de una versión de lista de materiales

[!include [banner](../includes/banner.md)]

En este artículo se explica un escenario de planificación maestra que implica la expansión de una versión de la lista de materiales (L. MAT.).

Una expansión de demanda de una versión de lista de materiales (L. MAT.) crea una demanda de cada elemento de línea de lista de materiales en un sitio específico y, posiblemente, en un almacén específico. Una lista de materiales específica de un sitio puede definir un almacén para cada línea de lista de materiales. Además, para cada línea de lista de materiales, la configuración de las dimensiones de artículos determina si es preciso especificar el almacén. La demanda resultante para cada elemento de línea de lista de materiales se convierte, a su vez, en el punto de partida para expansiones de demandas adicionales. El escenario de planificación maestra implica las condiciones siguientes:

-   La dimensión Sitio es obligatoria y debe especificarse en la transacción de demanda.
-   La dimensión Sitio es coherente. Por lo tanto, el sitio de menor nivel de demanda es equivalente al sitio de la transacción de demanda inicial.

La ilustración siguiente muestra el proceso de expansión de la demanda de planificación maestra. ![Expansión de la demanda con una versión de L. MAT](./media/multisitedemandexplosionscenariousingbomversion.gif)

<a name="additional-resources"></a>Recursos adicionales
--------

[Planificación maestra: cómo se establece la versión de la lista de materiales](master-plan-bom-version-determined.md)

[Planificación maestra y funcionalidad multisitio](master-plan-multisite-functionality.md)



