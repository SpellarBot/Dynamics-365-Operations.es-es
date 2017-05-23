---
title: Mantener pedidos planificados
description: "En este artículo se proporciona información sobre el modo de administrar pedidos planificados. Describe cómo puede actualizar el estado de los pedidos planificados, ponerlos en firme y filtrar por pedidos planificados que tengan el mismo estado que un pedido planificado seleccionado."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqTransPo
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 19151
ms.assetid: 54123f4c-b4ca-4ce4-9358-b067aa04c968
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: fd3392eba3a394bd4b92112093c1f1f9b894426d
ms.openlocfilehash: df3b7d285e2aa4c3e1fc102b821c30bdc7c9fb83
ms.contentlocale: es-es
ms.lasthandoff: 04/25/2017


---

# <a name="maintain-planned-orders"></a>Mantener pedidos planificados

[!include[banner](../includes/banner.md)]


En este artículo se proporciona información sobre el modo de administrar pedidos planificados. Describe cómo puede actualizar el estado de los pedidos planificados, ponerlos en firme y filtrar por pedidos planificados que tengan el mismo estado que un pedido planificado seleccionado.

Puede gestionar pedidos planificados desde el espacio de trabajo **Planificación maestra**, la lista **Pedido planificado** o las listas **Pedidos de producción planificados**, **Pedidos de compra planificados** y **Transferencia planificada**. Puede usar el campo **Estado** para ayudar a realizar un seguimiento del progreso. Se usan los siguientes valores:

-   Cuando la planificación maestra genera pedidos planificados, estos tienen un estado **No procesado**.
-   Si decide no poner en firme un pedido planificado, puede darle un estado **Finalizado**.
-   Si decide poner en firme un pedido planificado, puede darle el estado de **Aprobado**. Este estado indica que aprueba poner en firme el pedido planificado pero que aún no está puesto en firme.

**Nota:** un pedido planificado aprobado se transfiere en su estado actual al siguiente cálculo de planificación maestra. Puede poner en firme los pedidos planificados haciendo clic en **En firme**. Puede poner en firme los siguientes pedidos planificados:

-   El pedido planificado que está seleccionado.
-   Varios pedidos planificados.
-   Los pedidos planificados generados por una expansión desde la página **Expansión**. Haga clic en **Pedidos planificados**, seleccione el pedido planificado y, a continuación, haga clic en **En firme**.

Al poner en firme un pedido planificado, este se mueve a la sección de pedidos del módulo relevante. **Nota:** puede hacer clic con el botón secundario en un pedido planificado que tenga un estado concreto y filtrar para otros pedidos planificados que tengan el mismo estado. Esta función es útil si, por ejemplo, desea filtrar todos los pedidos planificados que tengan el estado **Aprobado** para después ponerlos en firme.

<a name="see-also"></a>Consulte también
--------

[Planes maestros](master-plans.md)



