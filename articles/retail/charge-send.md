---
title: Enviar pedidos desde otra tienda mediante la características de envío Caro
description: Este tema describe la característica de envío Cargo.
author: ashishmsft
manager: AnnBe
ms.date: 10/10/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Retail
ms.author: asharchw
ms.search.validFrom: 2017-10-10
ms.dyn365.ops.version: Retail July 2017 update
ms.openlocfilehash: e5351086c56d13ef98937aec066be00cdf88fd37
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "354078"
---
# <a name="ship-orders-from-another-store-by-using-the-charge-send-feature"></a>Enviar pedidos desde otra tienda mediante la características de envío Caro

[!include [banner](includes/banner.md)]

Con la característica de envío Cargo de Dynamics 365 for Retail, los pedidos del cliente se pueden realizar en una tienda y enviar desde otra tienda.

Los pedidos de clientes en el cliente de punto de venta (PDV) admiten varias opciones de cumplimiento. Algunos ejemplos de opciones de cumplimiento:

- Recogida en la misma tienda en otra fecha.
- Recogida en la misma tienda en la misma o en otra fecha.
- Envío del almacén de envío predeterminado que está asignado a la tienda, y entrega en una fecha específica.

La característica de envío Cargo utiliza las siguientes operaciones de PDV: Envío de todos los productos y Envío de productos seleccionados. Esto permite que el empleado de la tienda seleccione el “envío desde" la ubicación desde la que se puede cumplir el pedido o la línea de pedido. De forma predeterminada, la ubicación de “envío desde" es el almacén de envío asociado al almacén. Sin embargo, el empleado de la tienda puede cambiar esta ubicación y seleccionar cualquier tienda que esté definida en el grupo de localizadores de tiendas asignado a la tienda.

La capacidad para seleccionar direcciones de “envío a” se mantiene sin cambio.

Los métodos de envío que se pueden usar para cumplir la línea de pedido se basan en la configuración de modos válidos de entrega de productos y direcciones. Dado que las reglas sobre modos válidos de entrega sólo se mantienen en Central Retail, el cliente de PDV realiza una llamada en tiempo real para capturar los modos de entrega válidos para una línea de envío.
