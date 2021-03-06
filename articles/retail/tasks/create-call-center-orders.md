---
title: Crear pedidos de centro de llamadas
description: Este procedimiento le guía por la búsqueda de un cliente, la creación de un nuevo pedido, la búsqueda de un producto y el cobro de pagos del cliente.
author: josaw1
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: MCRCustomerService, SalesTable, MCRSourceIdTargetLookup, MCRSalesQuickQuote, MCRSalesOrderRecap, MCRCustPaymDialog, MCRCustPaymLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4867ad67dc570ab42420ba12fc7dc2da6b5ba503
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "334321"
---
# <a name="create-call-center-orders"></a>Crear pedidos de centro de llamadas

[!include[task guide banner](../includes/task-guide-banner.md)]

Este procedimiento le guía por la búsqueda de un cliente, la creación de un nuevo pedido, la búsqueda de un producto y el cobro de pagos del cliente. Este procedimiento usa la empresa de datos de demostración USRT y está pensado para el funcionario de ventas. Requisitos previos: el usuario que complete el procedimiento se configura como usuario del centro de llamadas y el catálogo semestral de Fabrikam se publica con al menos un código fuente en él.

1. Vaya a Venta minorista y comercio > Clientes > Servicio atención al cliente.
2. En el campo SearchText, especifique los criterios de búsqueda para buscar el cliente.
    * Para este procedimiento de ejemplo, escriba “karen” y presione el tabulador.  
3. Haga clic en Buscar
    * Dado que solo hay un cliente llamado Karen en los datos de demostración, se seleccionarán automáticamente.  
4. Haga clic en Nuevo pedido de ventas.
5. Expanda o contraiga la sección Encabezado de pedido de ventas.
6. Seleccione el código fuente para el catálogo.
    * Si no hay códigos de origen activos, puede cerrar el campo Origen y omitir este paso.  
7. Haga clic en Agregar línea.
8. En el campo Código de artículo, especifique el término de búsqueda del artículo.
    * Para este procedimiento de ejemplo, escriba un número de artículo parcial de "8111 " y presione el tabulador. Esto hará que se muestre la ventana de búsqueda del artículo.  
9. Seleccionar el producto que se agregará al pedido de ventas
10. Especifique la cantidad de ventas.
11. Haga clic en Crear.
12. Haga clic en Completar para capturar el pago del cliente.
13. Haga clic en Agregar.
    * El vínculo "Agregar" se encuentra en la pestaña de pagos. Si está contraída, abra la pestaña de pagos.  
14. Seleccione el método de pago.
    * Para este procedimiento, seleccione el método de pago en efectivo.  
15. Cierre la página.
16. Especifique el importe.
    * Para este procedimiento, especifique un importe igual al saldo del pedido que se puede ver en la página Resumen de pedido de ventas a la izquierda del campo de importe. Esto le permitirá que completar el pedido como totalmente pagado.  
17. Haga clic en Aceptar
18. Haga clic en Enviar.

