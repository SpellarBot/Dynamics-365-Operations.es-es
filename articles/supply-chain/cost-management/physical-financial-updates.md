---
title: Actualizaciones físicas y financieras
description: En este tema se proporciona un resumen de qué tipos de transacciones aumentan y reducen las cantidades de inventario.
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventTrans, InventTransVoucher
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 75023
ms.assetid: 128340e1-c573-48e6-b835-6c350d8dd0fb
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9ba628dbf63d3b124583e6b873530f1459b07562
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "322591"
---
# <a name="physical-and-financial-updates"></a>Actualizaciones físicas y financieras

[!include [banner](../includes/banner.md)]

En este tema se proporciona un resumen de qué tipos de transacciones aumentan y reducen las cantidades de inventario. 

Las transacciones de inventario se pueden actualizar físicamente y financieramente en Microsoft Dynamics 365 for Finance and Operations. Algunos tipos de transacciones financieras y físicas aumentan las cantidades de inventario, mientras que otros reducen la cantidad.

## <a name="physical-increases"></a>Incrementos físicos
Cuando se registra una transacción física, el estado del registro de la transacción es **Recibido**. Las siguientes transacciones se consideran incrementos físicos:

-   Recibo del pedido de compra
-   Devolución en albarán del pedido de ventas
-   Notificación de un pedido de producción como terminado
-   Por producto en una lista de selección de pedidos de producción

## <a name="financial-increases"></a>Incrementos financieros
Cuando se registra una transacción de recepción financiera, el estado del registro de la transacción que aumenta la cantidad es **Comprado**. Las siguientes transacciones se consideran incrementos financieros:

-   Factura de proveedor
-   Factura del pedido de ventas para una devolución
-   Gestión de costes del pedido de producción
-   Diarios de inventario de cantidad positiva, como movimiento, pérdidas y ganancias, recuento, lista de materiales y transferencia

## <a name="transactions-that-increase-quantity"></a>Transacciones que aumentan la cantidad.
Las transacciones que aumentan la cantidad se registran en el precio de coste promedio móvil. Finance and Operations calcula un precio de coste promedio móvil basado en el coste de cada una de las transacciones para cada dimensión de inventario de la que se efectúa un seguimiento financiero. Para obtener información acerca del precio de coste promedio móvil, consulte [Precio de coste promedio móvil](running-average-cost-price.md).

## <a name="transactions-that-decrease-quantity"></a>Transacciones que reducen la cantidad
Finance and Operations utiliza el precio de coste promedio móvil cuando se registra una transacción que reduce la cantidad, independientemente de qué modelo de inventario está asociado a ese inventario. La transacción que reduce la cantidad no debe haberse marcado para otra transacción antes de registrarse. Si el inventario físico disponible llega a ser negativo, Finance and Operations utiliza el coste de inventario definido para el artículo en la página **Artículo**. **Nota**: si la funcionalidad multisitio está activada, este coste será en su lugar el coste de inventario definido para un sitio en la página **Configuración predeterminada de pedido**.

## <a name="physical-issues-vs-financial-issues"></a>Emisiones físicas frente a emisiones financieras
Cuando se registra una transacción de emisión física, el estado del registro de la transacción es **Deducido**. Las siguientes transacciones se consideran emisiones físicas:

-   Diario de listas de selección de órdenes de producción
-   Albarán del pedido de ventas
-   Devolución del albarán de pedido de compra

Cuando se registra una transacción financiera, el estado del registro de la transacción es **Vendido**. Las siguientes transacciones se consideran emisiones financieras:

-   Finalización de un pedido de producción
-   Factura del pedido de ventas
-   Devolución de facturas de proveedor
-   Diarios de inventario de cantidad negativa, como movimiento, pérdidas y ganancias, recuento, lista de materiales y transferencia

Las transacciones que reducen la cantidad se registran en el precio de coste promedio móvil. De este modo, el procedimiento de cierre de inventario es necesario para liquidar las transacciones de emisión con las transacciones de recepción en función del modelo de inventario asignado a cada artículo.



