---
title: Confirmación de lote y matrícula
description: Este tema describe cómo configurar y aplicar confirmación de lote y matrícula desde un dispositivo móvil.
author: Mirzaab
manager: AnnBe
ms.date: 05/26/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSRFAutoConfirm
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 269384
ms.search.region: Global
ms.author: mirzaab
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: efab5b11782fd2344fb5f532272007d187c1465b
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "344234"
---
# <a name="batch-and-license-plate-confirmation"></a>Confirmación de lote y matrícula

[!include [banner](../includes/banner.md)]

La confirmación de lote le permite confirmar que se eligió el lote correcto en el dispositivo móvil. En la selección inicial del trabajo solo para los artículos superiores al lote, donde superior al lote indica que el lote supera a la ubicación en la jerarquía de la búsqueda, debe comprobar que el lote elegido se corresponde con el lote en la línea del trabajo. 

La confirmación de matrícula le permite confirmar que se eligió la matrícula correcta en el dispositivo móvil. Al seleccionar el trabajo en una ubicación de la etapa, debe comprobar que la matrícula elegida coincide con la matrícula que está asociada al trabajo. Si el trabajo se ha iniciado con la digitalización de una matrícula, este paso de confirmación se omitirá.

## <a name="where-it-applies"></a>Dónde se aplica
La confirmación se aplica en los casos siguientes:

- La confirmación de lote se aplica a las selecciones iniciales de trabajo para los artículos superiores al lote.
- La confirmación de la matrícula se aplica a las selecciones de ubicaciones de la etapa.

## <a name="set-up-batch-and-license-plate-confirmation"></a>Configurara la confirmación de lote y matrícula
Puede configurar la confirmación del lote y de matrícula desde los elementos de menú del dispositivo móvil.  
1.  En los elementos de menú del dispositivo móvil, especifique la configuración de la confirmación del trabajo.  
2.  Seleccione la opción para la confirmación de lote o matrícula. Ambas opciones están disponibles para las selecciones del tipo de trabajo que no tengan habilitada la confirmación automática.  
