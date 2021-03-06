---
title: Crear facturas de pedidos de ventas
description: Esta guía de tarea describe la facturación de un pedido de ventas e incluye la combinación de facturas y el procesamiento por lotes.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SalesTableListPage, SalesEditLines,  SysQueryForm, SysRecurrence
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5a57d204c0dcb44cbce7a0cc4d2f00b75b57e219
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "353319"
---
# <a name="create-sales-order-invoices"></a>Crear facturas de pedidos de ventas

[!include [task guide banner](../../includes/task-guide-banner.md)]

Esta guía de tarea describe la facturación de un pedido de ventas e incluye la combinación de facturas y el procesamiento por lotes. Este procedimiento usa la empresa de demostración USMF.


## <a name="create-an-invoice-from-a-sales-order"></a>Crear una factura a partir de un pedido de ventas
1. Vaya a Clientes > Pedidos > Pedidos de venta enviados pero no facturados.
2. Seleccione un pedido de ventas en la lista. 
3. En el panel de acciones, haga clic en Factura.
4. Haga clic en Factura.
    * Tenga en cuenta que este pedido de ventas tiene varios albaranes asociados con él. Solo mostrará la palabra <multiple> en lugar del número de albarán.  
5. Expanda la sección Parámetros.
    * El registro se debe establecer en Sí para registrar la factura. También puede desactivar el registro y solo imprimir la factura. Sin embargo, puede lograr el mismo resultado creando una factura de proforma en lugar de una factura.  
    * Esta opción es la que se usa para trabajos por lotes. El trabajo por lotes se ejecuta al registrar pedidos de ventas.    
6. En el campo Imprimir, seleccione "Después de".
7. Seleccione Sí para Imprimir factura.
    * La gestión de impresión puede imprimir varias copias de la factura y también enviar la factura por correo electrónico como archivo PDF.  
8. En el campo Imprimir costes, seleccione "Resumir".
9. En el campo Comprobar límite de crédito, seleccione "Saldo".
10. Haga clic en Cancelar.

## <a name="combine-orders-into-a-single-invoice"></a>Combinar pedidos en una única factura
1. Vaya a Clientes > Pedidos > Todos los pedidos de venta.
2. Localice a un cliente que tenga varias facturas abiertas.
3. Seleccione un pedido de ventas abierto.
4. Seleccione otro pedido de ventas abierto del mismo cliente.
5. En el panel de acciones, haga clic en Factura.
6. Haga clic en Factura.
7. Expanda la sección Parámetros.
8. En el campo Cantidad, seleccione 'Todo'.
    * Tenga en cuenta que hay dos facturas que aparecen en la sección de descripción. Ahora vamos a combinarlas en una única factura.  
9. En el campo Actualización conjunta para, seleccione "Cuenta de facturación".
10. Haga clic en Organizar para combinar los pedidos de ventas en una única factura.
    * Los dos pedidos de ventas se combinan ahora en una única factura.   
11. Haga clic en Cancelar.
12. Haga clic en Sí.

## <a name="post-invoices-in-a-batch"></a>Registrar facturas en un lote
1. Vaya a Clientes > Facturas > Facturación por lotes > Factura.
2. Haga clic en Seleccionar.
3. Haga clic en Aceptar
4. Haga clic en Lote.
5. Haga clic en Sí para activar el procesamiento por lotes.
6. Haga clic en Periodicidad.
7. Seleccione Días
8. Haga clic en Aceptar
9. Haga clic en Aceptar
10. Haga clic en Cancelar.
11. Haga clic en Sí.

