---
title: Enviar artículos devueltos a inspección
description: Al registrar un artículo devuelto, establezca que un artículo se debe enviar para inspección antes de devolverlo al inventario o de usarlo de algún otro modo.
author: ShylaThompson
manager: AnnBe
ms.date: 05/01/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WMSJournalTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: ShylaThompson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 70aafb752b2c847d5d48236fd5d201a73e088c24
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "334091"
---
# <a name="pass-returned-items-on-to-inspection"></a>Enviar artículos devueltos a inspección 

[!include [banner](../includes/banner.md)]


Al registrar un artículo devuelto, se puede determinar que un artículo se debe enviar para inspección antes de devolverlo al inventario o de usarlo de algún otro modo.

1.  Haga clic en **Gestión del inventario** \> **Diarios** \> **Recepción de artículos** \> **Recepción de artículos**.
    
    \-o-
    
    Haga clic en **Gestión del inventario** \> **Diarios** \> **Recepción de artículos** \> **Entrada desde producción**.

2.  En el formulario **Diario de ubicaciones**, registre la recepción de un artículo de la manera habitual.
    

    > [!NOTE]
    > <P>Para obtener más información sobre el registro de la recepción de artículos devueltos, consulte <A href="register-the-receipt-of-returned-items.md">Registrar la recepción de artículos devueltos</A></P>



3.  En la pestaña **Valores predeterminados** , en la área **Modo de manipulación**, seleccione la casilla **Gestión de cuarentena**.

Se solicitará al sistema que cree una orden de cuarentena, y la persona o departamento responsable de las inspecciones responderá a esta orden mediante el formulario **Orden de Cuarentena**.

## <a name="see-also"></a>Consulte también

[Inspeccionar artículos devueltos](take-returned-items-through-inspection.md)

[Especificar la disposición de artículos devueltos](specify-how-to-dispose-of-returned-items.md)

