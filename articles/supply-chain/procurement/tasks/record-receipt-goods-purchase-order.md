---
title: Registrar la recepción de mercancías en el pedido de compra
description: Este procedimiento le muestra cómo registrar la recepción de mercancías directamente en un pedido de compra.
author: FrankDahl
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PurchTable, PurchCreateOrder, InventItemIdLookupPurchase, PurchEditLines
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: fdahl
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 14d1d43479f9864d8fd5ed94a98a654e75eeedf0
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "343222"
---
# <a name="record-the-receipt-of-goods-on-the-purchase-order"></a>Registrar la recepción de mercancías en el pedido de compra

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento le muestra cómo registrar la recepción de mercancías directamente en un pedido de compra. También es posible registrar la recepción de productos en el almacén y, a continuación, registrarla después en el pedido de compra. Esta tarea se realiza normalmente por un agente de compras o un coordinador de Proveedores. El ejemplo mostrado en esta guía se puede utilizar en la empresa de datos de demostración USMF. El ejemplo incluye pasos para crear un pedido de compra sencillo para que pueda reproducir el procedimiento como guía de tareas. Si estuviera utilizando el procedimiento en sus propios datos, empezaría en la subtarea Registrar recepción de mercancías.


## <a name="prepare-a-new-purchase-order-for-receipt-of-goods"></a>Preparar un nuevo pedido de compra para la recepción de mercancías
1. Vaya a Adquisición y abastecimiento > Pedidos de compra > Todos los pedidos de compra.
2. Haga clic en Nuevo.
3. En el campo Cuenta de proveedor, escriba "US-101".
4. Haga clic en Aceptar
5. En el campo Número de artículo, especifique M0001.
6. En el campo Cantidad, especifique 5.
7. En el panel de acciones, haga clic en Compra.
8. Haga clic en Confirmar.

## <a name="record-receipt-of-goods"></a>Registrar recepción de mercancías
1. En el panel de acciones, haga clic en Recibir.
2. Haga clic en Recepción de producto.
    * El campo Cantidad le permite seleccionar diferentes opciones para la cantidad que desea recibir. Por ejemplo, si se ha registrado una cantidad anteriormente en el almacén, puede seleccionar Cantidad registrada.  Para este ejemplo, utilice el valor Cantidad pedida.   
3. En el campo Recepción de producto, escriba cualquier valor.
    * Este campo se utiliza para especificar una referencia que se usará como asiento para el diario de recepción de productos.  
4. Expanda la sección Líneas.
5. Establezca el valor de cantidad en '4'.
    * Aquí puede especificar manualmente la cantidad que se está recibiendo para cada línea del pedido.  
6. Contraiga la sección Líneas.
7. Haga clic en Aceptar
    * Las mercancías se han registrado ahora como recibidas en el pedido de compra y se ha creado un diario de recepción de producto como documento para reflejar esto. Puede utilizar la acción Recepción de producto para revisar los diarios creados con el pedido de compra y ver qué se ha recibido y cuándo.  

