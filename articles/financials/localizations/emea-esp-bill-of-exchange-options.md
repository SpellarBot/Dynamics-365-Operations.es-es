---
title: Opciones de letras de cambio españolas
description: Este tema describe opciones y cambios específicos en el proceso de letra de cambio básico implementado en Microsoft Dynamics 365 for Finance and Operations para las entidades jurídicas en España.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustParameters, BankBillOfExchangeTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 264644
ms.search.region: Spain
ms.author: v-elgolu
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 18a1d87406a9de4a78116398a2c2018feb87ff8c
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "370460"
---
# <a name="spanish-bill-of-exchange-options"></a>Opciones de letras de cambio españolas

[!include [banner](../includes/banner.md)]

Este tema describe opciones y cambios específicos en el proceso de letra de cambio básico implementado en Microsoft Dynamics 365 for Finance and Operations para las entidades jurídicas en España.

Para las entidades jurídicas en España, la funcionalidad de letra de cambio tiene opciones adicionales:

-   Validación de los diarios de letra de cambio
-   Fechas de los diarios de letra de cambio

## <a name="accounts-receivable-parameters-for-spanish-bills-of-exchange"></a>Parámetros de clientes para letras de cambio españolas
Para configurar los parámetros para letras de cambio de entidades jurídicas en España, vaya a **Parámetros de clientes** &gt; **Letra de cambio ES**.

## <a name="validation-for-bill-of-exchange-journals"></a>Validación de los diarios de letra de cambio
Si el parámetro **Validación del diario de letra de cambio** está establecido en **Sí**, no se registra una letra de cambio cuando las transacciones tienen el mismo número de asiento y distintas fechas de transacción. Este parámetro se aplica a las transacciones del diario contable. Este parámetro solo se utiliza cuando el diario admite un número de asiento y cuando la opción **Validación del diario de letra de cambio** está seleccionada en la página **Parámetros de clientes**. El parámetro **Validación del diario de letra de cambio** afecta a los siguientes documentos:

-   Diario de creación de letra de cambio
-   Diario de envíos
-   Diario de impago de letras de cambio
-   Diario de renegociación de letras de cambio
-   Diario de liquidación de letra de cambio
-   Diario de pagos

## <a name="dates-in-bill-of-exchange-journals"></a>Fechas de los diarios de letra de cambio
Si el parámetro **Tratamiento de fecha en diario de letra de cambio** está establecido en **Sí**, la fecha de transacción de los diarios de letra de cambio se actualiza a la fecha de vencimiento cuando se usa una propuesta de pago. El parámetro **Tratamiento de fecha en diario de letra de cambio** afecta a los siguientes documentos:

-   Diario de envíos
-   Diario de impago de letras de cambio
-   Diario de renegociación de letras de cambio




