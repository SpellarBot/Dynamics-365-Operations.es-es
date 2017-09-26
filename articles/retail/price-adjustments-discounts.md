---
title: Ajustes de precios y descuentos
description: "Este artículo proporciona información acerca de los ajustes de precios y descuentos en Microsoft Dynamics 365 for Retail."
author: scott-tucker
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-365-retail
ms.technology: 
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations, Retail
ms.custom: 15891
ms.assetid: bab5adf3-ddf0-4c22-a2eb-b4d25b88de99
ms.search.region: global
ms.search.industry: Retail
ms.author: scotttuc
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.translationtype: Human Translation
ms.sourcegitcommit: 59b51840c05fe649cf322bfa64737a321728a5aa
ms.openlocfilehash: caa701dfcbffe045d701442b1a39b88ea5f43125
ms.contentlocale: es-es
ms.lasthandoff: 06/20/2017

---

# <a name="price-adjustments-and-discounts"></a>Ajustes de precios y descuentos

[!include[banner](includes/banner.md)]


Este artículo proporciona información acerca de los ajustes de precios y descuentos en Microsoft Dynamics 365 for Retail.

En Dynamics 365 for Retail, puede realizar ajustes de precios a los productos y también puede configurar los descuentos que se aplican a un artículo de línea o una transacción en el punto de venta (PDV), en un pedido de ventas del centro de llamadas o en un pedido en línea. Tanto los ajustes de precios como los descuentos se pueden vincular a grupos de precios. Para los ajustes de precios y descuentos, puede especificar una sola fecha inicial y la fecha final o un período que se repite, un código de descuento y algunos atributos adicionales. Los ajustes de precios y los descuentos se pueden aplicar a productos, variantes o categorías. Si se aplica más de un descuento a un producto, un cliente puede recibir uno de los descuentos o un descuento combinado, en función de la configuración del descuento. Dynamics 365 for Retail aplica automáticamente el descuento o la combinación de descuentos que proporcionan el mejor precio al cliente. Cuando configure un ajuste de precio o un descuento, asegúrese de confirmar que los grupos de precios se asignan a los canales, catálogos, afiliaciones o programas de fidelidad correctos a los que desea que el descuento se aplique. Además, si desea generar automáticamente el id. de descuento, puede configurar secuencias numéricas en la página **Parámetros de ventas al por menor** antes de definir un nuevo descuento o ajuste de precios. **Nota**: puede eliminar un ajuste de precios o un descuento. Sin embargo, se perderá la información estadística.

### <a name="types-of-discounts"></a>Tipos de descuentos

Hay cuatro tipos de descuentos comerciales:

-   **Descuento simple**: un único porcentaje o importe.
-   **Descuento por cantidades**: un descuento que se aplica cuando se compran dos o más productos.
-   **Descuento combinado**: un descuento que se aplica cuando se compra una combinación concreta de productos.
-   **Descuento por umbral**: un descuento que se aplica cuando el total de la transacción es superior al importe especificado.

Tanto los ajustes de precios como los descuentos se pueden asociar con los grupos de precios. A continuación, los grupos de precios pueden asociarse con canales, catálogos, afiliaciones y programas de fidelidad.



