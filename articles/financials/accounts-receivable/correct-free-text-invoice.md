---
title: Corrección de una factura de servicios
description: Este artículo explica cómo corregir una factura de servicios que se ha registrado y cómo reenviarla como factura corregida.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/22/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustFreeInvoice
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 13991
ms.assetid: 2a0a4789-8619-4974-bef9-0923cc848420
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: c8c1b90b7b2c02a53e53cc13d70445a237b126d4
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "364612"
---
# <a name="correct-a-free-text-invoice"></a>Corrección de una factura de servicios

[!include [banner](../includes/banner.md)]

Este artículo explica cómo corregir una factura de servicios que se ha registrado y cómo reenviarla como factura corregida.

Para corregir una factura de servicios que ya se ha registrado, ábrala. En la página **Factura**, seleccione **Cancelar** y, a continuación seleccione **Corregir factura**. Seleccione un código de razón, agregue comentarios y seleccione la fecha para la nueva factura corregida. Puede modificar la factura corregida y registrarla. 

Al registrar la factura corregida, se crea una factura de cancelación por un importe de crédito que sea igual al importe de la factura original. Por lo tanto, el saldo combinado de las facturas original y de cancelación es igual a 0 (cero). La factura de cancelación se liquida con la factura original. 

Después de registrar la factura corregida, tendrá tres facturas:

-   **Factura original**: factura que contiene la información que está corrigiendo.
-   **Factura de cancelación**: factura de crédito que genera el sistema para cancelar la factura corregida más recientemente.
-   **Factura corregida**: factura que contiene la información de factura corregida.

Puede identificar la cancelación y la corrección de facturas de dos maneras:

-   La página **Todas las facturas de servicios** incluye una columna **Corrección** donde puede ver qué facturas se han cancelado y qué facturas se han corregido.
-   El encabezado de la factura de servicios muestra un estado de **Factura de cancelación '\[número de factura\]'** o **Factura corregida '\[número de factura\]'**.

> [!NOTE]
> Esta característica solo está disponible si se selecciona la clave de configuración **Corrección de factura de servicios**.



