---
title: "Configuración de códigos de barra"
description: "En este artículo se describe cómo usar códigos de barras en Microsoft Dynamics 365 for Operations - Retail."
author: josaw1
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core, Retail
ms.custom: 15971
ms.assetid: 6b4b2ac2-0344-41aa-8818-62c30017d5ac
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 0c6a7bdc4ba82dd57ab3e395e6dfb0ae4de31fc4
ms.openlocfilehash: 7734a08756f5b737744f9c8ce1d358be020b859f
ms.lasthandoff: 03/31/2017


---

# <a name="set-up-bar-codes"></a>Configuración de códigos de barra

[!include[banner](includes/banner.md)]


En este artículo se describe cómo usar códigos de barras en Microsoft Dynamics 365 for Operations - Retail.

Puede usar códigos de barras para comprar y vender productos, realizar un seguimiento de las variantes del producto y configurar los clientes y empleados. También puede usar códigos de barras para emitir y endosar cupones, tarjetas de regalo y notas de crédito. Puede configurar productos comerciales para que tengan códigos de barras estándar o códigos de barras internos personalizados. Los productos pueden tener más de un código de barras. Por ejemplo, un producto puede tener varios códigos de barras si procede de distintos fabricantes o si tiene variaciones de tamaño, estilo o color. Los códigos de barras pueden incluir el peso o el precio del producto. Las máscaras de código de barras son plantillas que se usan para crear códigos de barras. **Nota**: si asigna un código de barras único a cada combinación de variantes, puede digitalizar el código de barras en la caja registradora para que el programa determine la variante del producto que se vende. También puede recopilar y consultar estadísticas sobre las venta por variante. Se puede asignar un número único a cada grupo de tamaños, colores y estilos que identifique a este grupo en el código de barras. Dynamics 365 for Operations usa la máscara de código de barras para generar códigos de barras automáticamente para cada combinación de variantes. Esta funcionalidad puede ser útil si existen muchos tamaños, colores y estilos, ya que el número de combinaciones aumenta significativamente con cada código de variante que se agrega. Si no se usa esta funcionalidad, es necesario asignar códigos de barras manualmente a cada combinación que represente una variante de producto. Los códigos de barras se crean manual o automáticamente. Para crear códigos de barras, realice las siguientes tareas en el orden en el que aparecen.

1.  [Configuración de los caracteres de máscara de código de barras](set-up-bar-code-masks.md).
2.  [Configuración de máscaras de código de barras](set-up-bar-code-masks.md).
3.  Configure códigos de barras.
4.  Cree códigos de barras para productos.


<a name="see-also"></a>Consulte también
--------

[Configuración de máscaras de código de barras](set-up-bar-code-masks.md)



