---
title: Datos clave de facturas en el sistema de proveedores mediante el diario de aprobación
description: Esta guía de la tarea le mostrará cómo usar el registro de facturas para crear facturas y, después, utilizar el diario de aprobación para actualizar las cuentas de gastos.
author: abruer
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransInvoiceRegister, HcmWorkerLookUp, LedgerJournalTransApprove, LedgerJournalTransApproveFetchVouchers, LedgerTransVoucher
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: abruer
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 048eda77064b6aa3f666e998a8e551d2f7adc385
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "363531"
---
# <a name="key-invoice-data-into-ap-system-using-approval-journal"></a>Datos clave de facturas en el sistema de proveedores mediante el diario de aprobación

[!include [task guide banner](../../includes/task-guide-banner.md)]

Esta guía de la tarea le mostrará cómo usar el registro de facturas para crear facturas y, después, utilizar el diario de aprobación para actualizar las cuentas de gastos.


## <a name="create-and-post-and-invoice"></a>Crear y registrar una factura
1. Vaya a Proveedores > Facturas > Registro de facturas.
2. Haga clic en Nuevo.
3. Seleccione el nombre del registro de facturas que desee usar.
4. En la lista, haga clic en el vínculo de la fila seleccionada.
5. Haga clic en las líneas para abrir el registro y especificar las líneas de gastos.
6. Seleccione un proveedor. Por ejemplo, escriba o seleccione US-104
7. En el campo Factura, escriba un valor.
8. En el campo Descripción, escriba un valor.
9. En el campo Crédito, escriba un número.
10. En el campo Aprobado por, haga clic en el botón desplegable para abrir la búsqueda.
11. Resalte un aprobador y haga clic en Seleccionar para seleccionar el aprobador.
12. Haga clic en Registrar.
13. Cierre la página.
14. Cierre la página.

## <a name="approve-an-invoice"></a>Aprobar una factura
1. Vaya a Proveedores > Facturas > Aprobación de facturas.
2. Haga clic en Nuevo.
3. Seleccione el nombre del diario de aprobación de facturas que desee usar.
4. En la lista, haga clic en el vínculo de la fila seleccionada.
5. Haga clic en las líneas para mostrar una página donde podrá seleccionar las facturas que desea aprobar.
6. Seleccione Buscar asientos para mostrar todas las facturas que están listas para su aprobación.
7. Marque la factura que ha creado.
8. Haga clic en Seleccionar.
    * Los asientos que seleccionó arriba se mueven en esta lista después de que los seleccione.  
9. Haga clic en Aceptar
10. Haga clic en el campo del número de cuenta para agregar una cuenta de gastos en la factura.
11. Especifique un número de cuenta y salga del campo con el tabulador. Por ejemplo, escriba 600120.
12. Haga clic en Registrar.
13. Haga clic en el asiento para ver las entradas que se han registrado.
    * La cuenta de factura pendiente de aprobación se anula y se reemplaza con la cuenta de gastos real.  

