---
title: Actualizaciones de facturas para devoluciones
description: Esta funcionalidad también admite los procesos empresariales de muchas organizaciones que deciden que la misma persona facture pedidos de devolución y de ventas a la vez.
author: ShylaThompson
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SMAServiceOrderTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 2f962641f7fdae18a360567d6f37348fabbfc302
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "364382"
---
# <a name="perform-invoice-updates-for-returns"></a>Actualizaciones de facturas para devoluciones 

[!include [banner](../includes/banner.md)]


Un pedido de devolución es un tipo de pedido de ventas marcado como artículo devuelto. Por lo tanto, la página de lista **Todos los pedidos de venta** se usa para generar facturas para los pedidos de devolución en lugar del formulario **Pedidos de devolución**. Esta funcionalidad también admite los procesos empresariales de muchas organizaciones que deciden que la misma persona facture pedidos de devolución y de ventas a la vez.

Dado que la factura para un artículo devuelto es para un importe negativo, se denomina nota de abono.

Al configurar la actualización de factura para el procesamiento por lotes, el pedido de ventas del tipo **Pedido devuelto** debe tener un estado de línea de devolución de **Recibido**, lo que indica que el albarán del pedido se ha actualizado.

## <a name="post-an-invoice-for-a-return-order"></a>Registrar una factura para un pedido de devolución

1.  Haga clic en **Clientes** \> **Común** \> **Pedidos de ventas** \> **Todos los pedidos de ventas**.

2.  Seleccione un pedido de ventas para el que se muestra **Pedido devuelto** en el campo **Tipo de pedido**.

3.  En el panel de acciones, en la ficha **Factura**, en el grupo **Generar**, haga clic en **Factura**.

4.  En la pestaña **Parámetros**, seleccione la casilla de verificación **Registrar**.

5.  Revise la información del formulario y realice los cambios pertinentes.

6.  Haga clic en **Aceptar**. La nota de abono se ha registrado.

## <a name="see-also"></a>Consulte también

[Actualizaciones de albaranes para devoluciones](packing-slip-updates-returns.md)

  


