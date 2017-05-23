---
title: "Expansión de una versión de lista de materiales"
description: "En este artículo se explica un escenario de planificación maestra que implica la expansión de una versión de la lista de materiales (L. MAT.)."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqTransExplosion
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 19211
ms.assetid: fe08c2e6-9cc5-4e34-bbb2-cd07843403b5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: fd3392eba3a394bd4b92112093c1f1f9b894426d
ms.openlocfilehash: 057485f707c1f7442bfced3ec1a1492999733db4
ms.contentlocale: es-es
ms.lasthandoff: 04/25/2017


---

# <a name="explosion-of-a-bom-version"></a>Expansión de una versión de lista de materiales

[!include[banner](../includes/banner.md)]


En este artículo se explica un escenario de planificación maestra que implica la expansión de una versión de la lista de materiales (L. MAT.).

Una expansión de demanda de una versión de lista de materiales (L. MAT.) crea una demanda de cada elemento de línea de lista de materiales en un sitio específico y, posiblemente, en un almacén específico. Una lista de materiales específica de un sitio puede definir un almacén para cada línea de lista de materiales. Además, para cada línea de lista de materiales, la configuración de las dimensiones de artículos determina si es preciso especificar el almacén. La demanda resultante para cada elemento de línea de lista de materiales se convierte, a su vez, en el punto de partida para expansiones de demandas adicionales. El escenario de planificación maestra implica las condiciones siguientes:

-   La dimensión Sitio es obligatoria y debe especificarse en la transacción de demanda.
-   La dimensión Sitio es coherente. Por lo tanto, el sitio de menor nivel de demanda es equivalente al sitio de la transacción de demanda inicial.

La ilustración siguiente muestra el proceso de expansión de la demanda de planificación maestra. ![Expansión de la demanda con una versión de L. MAT](./media/multisitedemandexplosionscenariousingbomversion.gif)

<a name="see-also"></a>Consulte también
--------

[Planificación maestra: cómo se establece la versión de la lista de materiales](master-plan-bom-version-determined.md)

[Planificación maestra y funcionalidad multisitio](master-plan-multisite-functionality.md)



