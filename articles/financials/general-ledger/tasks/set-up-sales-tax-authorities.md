---
title: Configuración de las autoridades fiscales
description: Las autoridades fiscales son las entidades a las que tienen que notificarse y pagarse los impuestos cobrados.
author: twheeloc
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxAuthority
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 909433a04c1185039938f6233b30c235e7b8ed8b
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "366360"
---
# <a name="set-up-sales-tax-authorities"></a>Configuración de las autoridades fiscales

[!include [task guide banner](../../includes/task-guide-banner.md)]

Las autoridades fiscales son las entidades a las que tienen que notificarse y pagarse los impuestos cobrados. Puede pagar los impuestos a la autoridad directamente o a través de una cuenta de proveedor que cree para la autoridad fiscal. Si lo hace, la empresa puede usar sus rutinas de pago habituales para pagar a la autoridad fiscal puntualmente. Si no configura la autoridad fiscal como proveedor, una persona deberá prepararle un pago manual en la fecha de vencimiento correspondiente. Esta tarea usa la empresa de demostración USMF.

1. Vaya a Impuestos >Impuestos indirectos >Impuestos >Autoridades fiscales.
2. Haga clic en Nuevo.
3. En el campo Autoridad, escriba un valor.
4. En el campo Nombre, escriba un valor.
5. En el campo Cuenta de proveedor, haga clic en el botón desplegable para abrir la búsqueda.
6. En la lista, busque y seleccione el registro deseado.
7. En la lista, haga clic en el vínculo de la fila seleccionada.
8. Seleccione el diseño del informe para su país o región si hay uno disponible. Si los diseños de informe no se corresponden con los requisitos de la autoridad fiscal, use el diseño predeterminado.
9. Especifique los valores en el formulario de redondeo y los campos Redondear para especificar cómo se debe redondear el importe total de impuestos que se debe pagar. Las diferencias de redondeo se registrarán en la configuración de Cuentas para transacciones automáticas en contabilidad general.
10. En el campo Redondear, escriba un número
11. Haga clic en Guardar.

