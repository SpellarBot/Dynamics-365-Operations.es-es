---
title: Liquidar un cheque con pago diferido de un cliente
description: Puede liquidar un cheque posfechado después de que el banco lo haya desactivado.
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustPostDatedChecks, SystemDate, LedgerJournalTable, LedgerJournalTransDaily, LedgerTransVoucher
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 86cefaac99a1ce5aa777f4f62456c3248045cc27
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "338254"
---
# <a name="settle-a-postdated-check-from-a-customer"></a>Liquidar un cheque con pago diferido de un cliente

[!include [task guide banner](../../includes/task-guide-banner.md)]

Puede liquidar un cheque posfechado después de que el banco lo haya desactivado. Esta transacción financiera también se eliminará la transacción de cuenta puente para el cheque posfechado. 

Las siguientes tareas se deben realizar antes de comenzar esta.

1) Configuración de cheques con pago diferido

2) Registrar un cheque con pago diferido para un cliente 



El rol de esta guía de tareas es Tesorero.



Este procedimiento usa la empresa de demostración USMF.

1. Vaya a Crédito y cobros > Consultas e informes > Pagos > Cheques con fecha futura de cliente.
2. Haga clic en Liquidar.
3. Haga clic en Liquidar entidades de compensación.
    * Liquide la cuenta del cliente para la transacción de cheque.  
4. Cierre la página.
5. Vaya a Contabilidad general > Movimientos de diario > Diarios generales.
6. En el campo Mostrar, seleccione una opción.
7. Active o desactive la casilla Mostrar sólo creados por el usuario.
8. En la lista, busque y seleccione el registro deseado.
9. Haga clic en Líneas.
10. Haga clic en Asiento.
11. Cierre la página.

