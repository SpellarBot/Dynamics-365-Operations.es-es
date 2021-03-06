---
title: MX-00010 Cancelar facturas electrónicas
description: Puede cancelar una factura electrónica CFDI validada y certificada anteriormente por el PAC.
author: sndray
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: EInvoiceCFDIJournal_AR
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Mexico
ms.author: sndray
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c0e5980c024c1e28df2d6da68385c370236417f5
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "370438"
---
# <a name="mx-00010-cancel-an-electronic-invoice"></a>MX-00010 Cancelar facturas electrónicas

[!include [task guide banner](../../includes/task-guide-banner.md)]

Puede cancelar una factura electrónica CFDI validada y certificada anteriormente por el PAC. También puede cancelar una factura electrónica CFDI mediante el proceso manual.


## <a name="cancel-a-cfdi-electronic-invoice"></a>Cancelación de una factura electrónica CFDI
1. Vaya a Clientes > Consultas e informes > CFDI (facturas electrónicas).
2. Seleccione una factura electrónica con estado Aprobada.
3. Haga clic en el vínculo del número de factura para ver los detalles.
4. En el panel de acciones, haga clic en Funciones.
5. Haga clic en Cancelar CFDI.
6. Cierre la página.
7. Vaya a Clientes > Facturas > Facturas electrónicas > Proceso de exportar/importar factura electrónica.
8. Haga clic en Aceptar
    * Cuando se confirma la cancelación, el estado de la factura electrónica cambia a Cancelada.  
9. Vaya a Clientes > Consultas e informes > CFDI (facturas electrónicas).
10. Seleccione la factura cancelada para comprobar el estado.

## <a name="manually-cancel-a-cfdi-electronic-invoice"></a>Cancelación manual de una factura electrónica CFDI
1. Seleccione una factura con estado Aprobada.
2. En el panel de acciones, haga clic en Funciones.
3. Haga clic en Cancelación manual.
4. Especifique la fecha de cancelación.
5. En el campo Nombre de clave de cancelación, escriba el motivo de la cancelación.
6. Haga clic en Aceptar para confirmar la cancelación de la factura electrónica.
    * El estado de la factura electrónica es Cancelación manual.  

