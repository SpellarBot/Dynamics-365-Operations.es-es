---
title: Configurar letras de cambio
description: Este tema describe los pasos para configurar letras de cambio.
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: Operations, Core
ms.custom: 269964
ms.assetid: f2077165-da90-4359-ab12-e05717728dc7
ms.search.region: global
ms.author: abruer
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: 0c6a7bdc4ba82dd57ab3e395e6dfb0ae4de31fc4
ms.openlocfilehash: ce2142d946085d8bfc577accf1bb31a89ea29156
ms.lasthandoff: 03/31/2017


---

# <a name="set-up-bills-of-exchange"></a>Configurar letras de cambio

[!include[banner](../includes/banner.md)]


Este tema describe los pasos para configurar letras de cambio.

Una letra de cambio es una orden escrita o electrónica de un cliente que se especifica que otra parte, normalmente un banco, debería pagar un importe establecido a la empresa. Al usar una letra de cambio como pago de una factura de pedido de ventas o de servicios, se abona en la cuenta del cliente el importe correspondiente. Ese abono se garantiza mediante la letra de cambio hasta que el cliente la pague al banco. Normalmente, la factura se liquida con la letra de cambio en la fecha de vencimiento. Cuando reciba una notificación del banco que indique que la letra de cambio se ha liquidado, podrá cerrarla. Puede librar una letra de cambio a través del banco en cualquiera de estos momentos:

-   En la fecha de vencimiento. Este enfoque se conoce como remesa al cobro.
-   Antes de la fecha de vencimiento, normalmente en la fecha de descuento que se especifica en las condiciones de pago establecidas para el cliente. Al registrar la transacción, el importe del descuento se registra en una cuenta de gastos. El resto del importe es pasivo hasta que el banco recibe el pago del cliente. Este enfoque se conoce como remesa al descuento.

## <a name="set-up-posting-profiles-for-bills-of-exchange"></a>Configuración de perfiles de contabilización para letras de cambio
Use la página **Perfiles de contabilización del cliente** para configurar los perfiles de contabilización que puede utilizar con las letras de cambio, impagos de letras de cambio, remesas al cobro y remesas al descuento. En el campo **Extracto de cuenta**, seleccione la cuenta resumida en la que se deben registrar los importes de las letras de cambio. Esta cuenta se adeuda o abona dependiendo del tipo transacción de la letra de cambio:
-   Para las letras de cambio, se cargará el importe correspondiente en esta cuenta cuando se registre la letra de cambio y se abonará cuando se registre una remesa al descuento o una remesa al cobro.
-   Para los impagos de letra de cambio, se cargará el importe correspondiente en esta cuenta cuando se registre el impago de letra de cambio.
-   Para las remesas al cobro, se cargará el importe correspondiente en esta cuenta cuando se registre una remesa al cobro.
-   Para las remesas al descuento, se cargará el importe correspondiente en esta cuenta cuando se registre una remesa al descuento.

En el campo **Liquidar cuenta**, seleccione la cuenta de efectivo en la que se deben registrar las letras de cambio. Se cargará el importe correspondiente en esta cuenta cuando se liquide la letra de cambio. En el campo **Pagos de impuestos por adelantado**, seleccione la cuenta resumida en la que se deben registrar los importes de impuestos cuando se usan letras de cambio para anticipos. En el campo **Deudas por efectos descontados**, seleccione la cuenta en la que desea registrar el importe de descuento de remesas al descuento. Se abonará el importe correspondiente en esta cuenta cuando se registre una remesa al descuento.

## <a name="set-up-accounts-receivable-parameters-for-bills-of-exchange"></a>Configurar los parámetros de clientes para letras de cambio
En la página de **parámetros de clientes**, los perfiles de contabilización predeterminados para letras de cambio se introducen en la ficha **Impuestos y contabilidad**. Las secuencias numéricas se definen en la ficha **Secuencias numéricas**.
Configurar nombres de diario para letras de cambio
------------------------------------------

En la página **Nombre de diario**, cree al menos cinco nombres de diario para las letras de cambio. Aquí se muestran los tipos de diarios:
-   **Librado de letra de cambio del cliente**: crea un nombre de diario para el diario de creación de letra de cambio.
-   **Impago de letra de cambio de cliente**: crea un nombre de diario para el diario de impago de letras de cambio.
-   **Renegociación de letra de cambio de cliente**: crea un nombre de diario para el diario de renegociación de letras de cambio.
-   **Remesa bancaria del cliente**: crea un nombre de diario para el diario de envíos.
-   **Liquidación de letras de cambio del cliente**: crea un nombre de diario para el diario de liquidación de letra de cambio.

En la página del formulario de asiento de diario de cada diario de letra de cambio, puede especificar información sobre la letra de cambio en la ficha **Letra de cambio**. Una vez que las líneas de diario de la letra de cambio se hayan registrado, podrá verlas en la página **Consulta de diario de letras de cambio** y en la página **Estadísticas de letras de cambio**.
Configurar métodos de pago para las letras de cambio
-----------------------------------------------

En la página **Formas de pago**, configure al menos un método de pago para las letras de cambio. Si trabaja con más de un banco, configure un método de pago que corresponda al formato de envío que cada banco requiere para las letras de cambio.
Configurar cuotas de pago para letras de cambio
-----------------------------------------

Una cuota de pago es un cargo asociado al proceso de cobro de pagos a los clientes. Se pueden asociar múltiples líneas de configuración de cuota de pago a cada cuota de pago. Puede usar las líneas de configuración para controlar cómo se calculan los importes predeterminados de las cuotas de pago. Por ejemplo, puede crear líneas de configuración para los métodos de pago, especificaciones de pago, divisas y períodos de tiempo. También puede crear líneas de configuración para un porcentaje o importe basado en intervalos diarios. Por ejemplo, puede configurar un porcentaje de interés que se basa en el período de tiempo en que vence un pago. Si el banco cobra distintas cuotas para distintos tipos de remesas, tales como **Cobro** o **Descuento**, configure una línea de cuota de pago independiente para cada tipo de remesa.
Configurar cuotas de envío para archivos de remesa bancarios
------------------------------------------------

En la página **Cuentas bancarias**, puede configurar cuotas de envío que cobra un banco por cada archivo de remesa generado. Estas cuotas se registran cuando se haya confirmado la remesa y se conozcan los importes de cuota realizados. Las cuotas de envío son diferentes a las cuotas de pago, que se cobran a los clientes y están asociadas a las líneas de diario.
Configurar diseños de documento para letras de cambio
---------------------------------------------

En la página **Cuentas bancarias**, haga clic en **Configurar** y especifique el diseño necesario para cada cuenta bancaria para la que generará documentos de letra de cambio.
Configurar clientes para letras de cambio
--------------------------------------

En la página **Clientes**, para cada cliente que ha acordado pagar mediante una letra de cambio, puede configurar un método predeterminado para el pago de las letras de cambio en la ficha **Valores predeterminados del pago**.





