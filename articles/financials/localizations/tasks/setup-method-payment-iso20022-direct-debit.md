---
title: Configuración de la forma de pago para domiciliaciones bancarias ISO20022
description: Este procedimiento muestra cómo configurar la forma de pago de domiciliación bancaria ISO20022 del cliente o cualquier otro tipo de pago mediante informes electrónicos.
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustPaymMode
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 953a3cffc356ab44163944318e7e7d542a113112
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "349685"
---
# <a name="setup-method-of-payment-for-iso20022-direct-debit"></a>Configuración de la forma de pago para domiciliaciones bancarias ISO20022

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento muestra cómo configurar la forma de pago de domiciliación bancaria ISO20022 del cliente o cualquier otro tipo de pago mediante informes electrónicos. 



Antes de completar esta tarea, debe definir las configuraciones de formato de exportación y las cuentas de pago.



Este procedimiento se creó con los datos de demostración de la empresa DEMF.



Este es el tercero de cinco procedimientos que muestra el proceso de pago del cliente mediante las configuraciones de informes electrónicos.

1. Vaya a Clientes > Configuración de pagos > Formas de pago.
2. Use el filtro rápido para buscar registros. Por ejemplo, filtre por el campo Forma de pago, por el valor "ELECTRONIC".
3. Haga clic en Editar.
4. En el campo Cuenta de pago, especifique los valores "DEMF OPER".
5. Expanda la sección Formatos de archivo.
6. Seleccione Sí en el campo Informes electrónicos genéricos.
7. En el campo Configuración de formato de exportación, especifique o seleccione un valor.
    * En la lista, seleccione ISO20022 Domiciliación bancaria (DE).  Si la lista está vacía, no hay ninguna configuración de formato de exportación de pago de cliente importada y activa.  
8. Seleccione Sí en el campo Requerir orden.
    * Seleccione el parámetro Requerir orden para los formatos de pago del cliente, que requieren la información de la orden incluida en el mensaje de pago, como la domiciliación bancaria SEPA.  
9. Haga clic en Guardar.

