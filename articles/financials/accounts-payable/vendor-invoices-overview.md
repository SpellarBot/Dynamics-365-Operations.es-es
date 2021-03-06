---
title: Visión general de facturas de proveedores
description: Este artículo ofrece información general relativa a facturas de proveedor. Las facturas de proveedor son solicitudes de pago para productos y servicios que se han recibido. Las facturas de proveedor pueden representar una cuenta para servicios en curso ose pueden basar en pedidos de compra para artículos y servicios específicos.
author: abruer
manager: AnnBe
ms.date: 03/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendorInvoiceWorkspace, VendInvoiceInfoListPage
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 13971
ms.assetid: 0ec4dbc0-2eeb-423b-8592-4b5d37e559d3
ms.search.region: Global
ms.author: abruer
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1d7cec48b1e01d308cfc67260ac82a50a8d76844
ms.sourcegitcommit: 9796d022a8abf5c07abcdee6852ee34f06d2eb57
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/12/2019
ms.locfileid: "975811"
---
# <a name="vendor-invoices-overview"></a>Visión general de facturas de proveedores

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]

Este artículo ofrece información general relativa a facturas de proveedor. Las facturas de proveedor son solicitudes de pago para productos y servicios que se han recibido. Las facturas de proveedor pueden representar una cuenta para servicios en curso ose pueden basar en pedidos de compra para artículos y servicios específicos. 

## <a name="vendor-invoices"></a>Facturas de proveedores

Una factura de proveedor de un pedido de compra es una factura que se produce cuando se reciben productos o servicios de acuerdo con un pedido de compra que se ha configurado con un proveedor. La factura de proveedor contiene un encabezado y una o varias líneas para artículos o servicios. Una factura de proveedor finaliza el ciclo de pedido de compra con la recepción de producto en la factura de proveedor. 

Aunque algunas facturas de proveedor están relacionadas con un pedido de compra, las facturas de proveedor también pueden contener las líneas que no se corresponden con las líneas de pedido de compra. También puede crear facturas de proveedor que no estén asociadas a ningún pedido de compra. Estas facturas de proveedor pueden representar servicios en curso, como una cuenta de servicios, y no es necesario hacer referencia a un pedido de compra cuando se agreguen. 

Hay varias formas de especificar una factura de proveedor:

-   El registro de facturas de proveedor le permite especificar rápidamente las facturas que no hacen referencia a un pedido de compra, de modo que puede acumular el gasto. Mediante el diario de aprobación de facturas de proveedor, puede seleccionar dichas facturas y registrarlas al saldo del proveedor para invertir la acumulación.
-   El diario de facturas de proveedor le permite especificar rápidamente las facturas que no hacen referencia a un pedido de compra, en un único paso.
-   Junto con el grupo de facturas de proveedor, el registro de facturas de proveedor le permite especificar rápidamente facturas para acumular el gasto. Puede abrir los pedidos de compra asociados más tarde para registrar la factura en la cuenta de gastos.
-   Las páginas **Facturas de proveedor abiertas** y **Facturas de proveedor pendientes** le permiten crear facturas de proveedor a partir de pedidos de compra confirmados.

La discusión siguiente proporciona más información sobre cómo las páginas **Facturas de proveedor abiertas** o **Facturas de proveedor pendientes** para crear una factura de proveedor a partir de un pedido de compra.

## <a name="understanding-invoice-line-quantities"></a>Comprensión de las cantidades de línea de factura
Cuando abre una factura de proveedor desde un pedido de compra relacionado, las líneas de factura se crean a partir del pedido de compra. De forma predeterminada, las cantidades se toman de la cantidad de recepción de producto. Sin embargo, puede usar cualquiera de los comportamientos predeterminados siguientes:

-   **Cantidad que se recibe ahora**: use esta opción para envíos parciales. El valor predeterminado del campo **Cantidad** proviene del campo de cantidad **Recibir ahora** en el pedido de compra.
-   **Cantidad pedida**: use esta opción para envíos completos. El valor predeterminado del campo **Cantidad** procede del campo de cantidad **Pedido** del pedido de compra.
-   **Cantidad registrada**: use esta opción si el artículo requiere el registro, según lo especificado en la página **Grupos de modelos de artículo**. El valor predeterminado del campo **Cantidad** es la cantidad física de actualización registrada.
-   **Cantidad de la recepción de producto**: use esta opción si una recepción de producto se ha recibido ya para el pedido. El valor predeterminado del campo **Cantidad** procede de la cantidad total de recepciones de producto disponibles.
-   **Cantidad y servicios registrados**: use esta opción si las cantidades se han registrado en los diarios de recepción para los artículos mantenidos en existencias o los artículos que no se encuentran en existencias. Esta opción también incluye servicios, independientemente de si se registran.

Si su entidad jurídica usa la conciliación de facturas, puede ver los resultados de la conciliación de cantidad en la columna **Cantidad de recepciones de producto para asignar**. También puede usar el comando de menú **Detalles coincidentes** en la ficha **Revisar** para ver los resultados de conciliación de cantidad.

## <a name="adding-a-line-that-wasnt-on-the-purchase-order"></a>Agregar una línea que no estaba en el pedido de compra
Puede agregar una nueva línea que no estaba en el pedido de compra a la factura de proveedor. Debe seleccionar un número de artículo o una categoría de compras. Puede agregar cantidades, precios y los importes a la línea. La línea solo se incluirá en las directivas de conciliación para los totales de factura.

## <a name="submitting-a-vendor-invoice-for-review"></a>Envío de facturas de proveedor para su revisión
La organización puede usar flujos de trabajo para gestionar el proceso de revisión de facturas de proveedor. La revisión de flujo de trabajo puede ser necesaria para el encabezado de factura, la línea de factura, o ambos. Los controles de flujo de trabajo se aplican al encabezado o la línea, en función de dónde está el enfoque al hacer clic en el control. En lugar del botón **Registrar**, verá un botón **Enviar** que puede usar para enviar la factura de proveedor mediante el proceso de revisión.

## <a name="matching-vendor-invoices-to-product-receipts"></a>Conciliación de facturas de proveedor a recepciones de producto
Puede especificar y guardar la información de facturas de proveedor y asignar líneas de factura a líneas de recepción de producto. También puede conciliar cantidades parciales para una línea. 

Puede crear una factura de proveedor basada en los artículos de línea de recepción de producto recibidos hasta la fecha, incluso si no se han recibido todos los artículos de un pedido de compra en particular. Por ejemplo, esta opción se podría usar si un proveedor envía una factura al mes que cubre todas las entregas que envía a lo largo del mes. Cada recepción de producto representa una entrega parcial o completa de los artículos del pedido de compra. 

Al registrar la factura, la cantidad de **Recordatorio de factura** de cada artículo se actualiza con el total de las cantidades recibidas de las recepciones de producto seleccionadas. Si las cantidades tanto de **Recordatorio de factura** como de **Pendiente de entrega** para todos los artículos del pedido de compra son 0 (cero), el estado del pedido de compra cambia a **Facturado**. Si la cantidad de **Recordatorio de factura** no es 0, el estado del pedido de compra no cambia y se podrán entrar facturas adicionales para este.

En esta opción se supone que se ha registrado al menos una recepción de producto para el pedido de compra. La factura de proveedor se basa en estas recepciones de producto y refleja sus cantidades. La información financiera de la factura se basa en la información especificada al registrar la factura.

Para obtener más información, consulte [Registrar la factura de proveedor y cuadrarla con la cantidad recibida](../accounts-receivable/tasks/record-vendor-invoice-match-against-received-quantity.md)

## <a name="working-with-multiple-invoices"></a>Trabajar con múltiples facturas

Puede trabajar con varias facturas a la vez y registrarlas al mismo tiempo. Si debe crear varias facturas, use la página **Facturas de proveedor pendientes**. Si debe registrar e imprimir varias facturas de proveedor, utilice la página del diario de aprobación de facturas Si usa el diario de aprobación de facturas, debe registrarse al menos una recepción de producto para el pedido de compra y debe registrarse una factura del pedido de compra en un registro de facturas. La información financiera de la factura proviene de la factura registrada en el registro.

## <a name="recovering-vendor-invoices-that-are-in-use"></a>Recuperar facturas de proveedor que se están usando

Mientras se está utilizando una factura de proveedor, esta no puede editarse por otro usuario. Sin embargo, el estado de una factura puede indicar a veces que la factura se está utilizando, aunque no se esté editando activamente. Por ejemplo, la aplicación puede haber detenido la respuesta mientras la factura estaba siendo editada o un usuario puede haber dejado de forma inadvertida la factura abierta en la aplicación.

Puede usar la página **Recuperar facturas de proveedor** para recuperar o para liberar las facturas de proveedores que se han llevan usándose más de cuatro horas, para que se puedan editar. Puede abrir esta página desde la navegación **Tarea periódica** o una sección en el espacio de trabajo **Entrada de la factura de proveedor**. Después de que se recupera una factura, ésta estará disponible para editarse en la página **Factura de proveedor**.

Puede obtener acceso a la página **Recuperar las facturas de proveedor** solo si tiene asignados derecho y privilegio de seguridad **Recuperar las facturas de proveedor en uso**. Además, el parámetro **Permitir recupear de la factura de proveedor** de la página **Parámetros de proveedores** se debe activar.

## <a name="additional-resources"></a>Recursos adicionales

 - [Configurar directivas de factura de proveedor](../accounts-receivable/tasks/set-up-vendor-invoice-policies.md) 

 - [Introducir datos de factura en el sistema de proveedores mediante una factura de proveedor](tasks/key-invoice-data-ap-system-vendor-invoice.md)

 - [Introducir datos de factura en el sistema de proveedores mediante un diario de aprobación](tasks/key-invoice-data-into-ap-system-approval-journal.md)

 - [Introducir datos de factura en el sistema de proveedores mediante un grupo de facturas](tasks/key-invoice-data-into-ap-system-invoice-pool.md)

 - [Registrar una factura de proveedor en el diario de facturas](tasks/record-vendor-invoice-invoice-journal.md)

