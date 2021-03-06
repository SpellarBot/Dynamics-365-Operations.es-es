---
title: Crear proveedores de configuración y marcarlos como activos
description: En los pasos siguientes se explica cómo un usuario administrador del sistema o con rol de desarrollador de informes electrónicos puede crear un proveedor de configuraciones para realizar informes electrónicos (ER).
author: NickSelin
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERWorkspace, ERVendorPart, ERVendorTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 13a27c2fec2a2b226e9ae8d5b8f9a61e8b79ceb0
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "362243"
---
# <a name="create-configuration-providers-and-mark-them-as-active"></a>Crear proveedores de configuración y marcarlos como activos

[!include [task guide banner](../../includes/task-guide-banner.md)]

En los pasos siguientes se explica cómo un usuario administrador del sistema o con rol de desarrollador de informes electrónicos puede crear un proveedor de configuraciones para realizar informes electrónicos (ER). Cada configuración de informes electrónicos hará referencia al proveedor como autor de la configuración. En este ejemplo, creará un proveedor de configuración para la empresa de demostración, Litware, Inc. Estos pasos se pueden realizar en cualquier empresa a medida que los proveedores de configuración de ER se comparten entre todas las empresas.


## <a name="create-a-provider"></a>Creación de un proveedor
1. Vaya a Administración de la organización > Espacios de trabajo > Informes electrónicos.
2. Haga clic en Proveedores de configuración.
3. Haga clic en Nuevo.
    * Cada registro de proveedor tiene un nombre y dirección URL únicos. Revise el contenido de esta página y omita este procedimiento si ya existe un registro para Litware, Inc. (http://www.litware.com).  
4. En el campo Nombre, especifique "Litware, Inc.".
    * Litware, Inc.  
5. En el campo Dirección de Internet, escriba "http://www.litware.com".
    * http://www.litware.com  
6. Haga clic en Guardar.
7. Cierre la página.

## <a name="select-as-an-active-provider"></a>Selección como proveedor activo
1. Seleccione el proveedor Litware, Inc.
2. Haga clic en Definir como activo.

