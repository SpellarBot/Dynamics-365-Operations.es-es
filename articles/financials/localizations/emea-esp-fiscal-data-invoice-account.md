---
title: Usar datos fiscales de la cuenta de factura
description: Para las entidades jurídicas en España, la funcionalidad Usar datos fiscales de cuenta de factura permite la actualización automática de datos fiscales de los pedidos de ventas, las facturas de texto sin formato y los pedidos de compra, en función de la información de la cuenta de facturación. Este tema proporciona información sobre la funcionalidad Usar datos fiscales de cuenta de factura y explica cómo configurarla.
author: ShylaThompson
manager: AnnBe
ms.date: 10/31/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustParameters, VendParameters
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 265224
ms.search.region: Spain
ms.author: v-elgolu
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 805fc2e8fcadc9538e69a0e8d945cae3b52f4b8d
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "370474"
---
# <a name="use-fiscal-data-from-the-invoice-account"></a>Usar datos fiscales de la cuenta de factura

[!include [banner](../includes/banner.md)]

Para las entidades jurídicas en España, la funcionalidad Usar datos fiscales de cuenta de factura permite la actualización automática de datos fiscales de los pedidos de ventas, las facturas de texto sin formato y los pedidos de compra, en función de la información de la cuenta de facturación. Este tema proporciona información sobre la funcionalidad Usar datos fiscales de cuenta de factura y explica cómo configurarla.

Para las entidades jurídicas en España, la funcionalidad Usar datos fiscales de cuenta de factura permite la actualización automática de datos fiscales de los pedidos de ventas, las facturas de texto sin formato y los pedidos de compra, en función de la información de la cuenta de facturación. Los datos fiscales que actualizan incluye el nombre del cliente o proveedor, la dirección y la información fiscal. La funcionalidad Usar datos fiscales de cuenta de factura afecta a los siguientes módulos:

-   Proveedores Página de cambio **Cuenta de facturación**
-   Adquisición y abastecimiento
-   Clientes
-   Ventas y marketing

## <a name="accounts-payable-and-procurement-and-sourcing"></a>Proveedores y Adquisición y abastecimiento
Para gestionar la oportunidad de actualización automática de datos fiscales en cambio de cuenta de facturación del módulo Proveedores, debe configurar un parámetro Usar datos fiscales de cuenta de factura en la ficha Factura de la página **Parámetros de proveedores**. Las opciones siguientes están disponibles:

-   **Nunca**: la información se acualiza desde la cuenta del proveedor.
-   **Siempre**: la información se acualiza desde la cuenta de facturación.
-   **Preguntar**: Se le pide al usuario que especifique si la información debe actualizarse desde la cuenta de facturación o la del proveedor.

Cuando se define el parámetro **Usar datos fiscales de cuenta de factura**, pueden actualizarse tres campos de una orden de compra en función del valor del parámetro. Cuando se modifica el campo **Cuenta de facturación**, los campos siguientes se actualizan con la información de la cuenta de facturación:

-   Nombre
-   Grupo de impuestos sobre las ventas
-   Exención fiscal

## <a name="accounts-receivable-and-sales-and-marketing"></a>Clientes, ventas y marketing
Para gestionar la oportunidad de actualización automática de datos fiscales en cambio de **Cuenta de facturación** del módulo **Proveedores**, debe configurar un parámetro "**Usar datos fiscales de cuenta de factura**" en la ficha desplegable **Factura** de la ficha **Actualizaciones** en la página **Parámetros de cliente**. Las opciones siguientes están disponibles:

-   **Nunca**: la información se acualiza desde la cuenta del cliente.
-   **Siempre**: la información se acualiza desde la cuenta de facturación.
-   **Preguntar**: Se le pide al usuario que especifique si la información debe actualizarse desde la cuenta de facturación o la del cliente.

Cuando se establece el parámetro **Usar datos fiscales de cuenta de factura**, es posible actualizar los documentos siguientes desde Clientes:

-   Pedidos de ventas
-   Facturas de servicios

Cuando se modifica el campo **Cuenta de facturación**, los campos siguientes pueden actualizarse con la información de la cuenta de facturación:

-   Nombre
-   Grupo de impuestos sobre las ventas
-   Exención fiscal




