---
title: Crear y asociar registros
description: Este procedimiento muestra cómo crear un registro de punto de venta (PDV).
author: rubencdelgado
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailTerminalTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: rubendel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 07e4b9f32a3a74b273272bd0b759d35c2a963e2e
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "360656"
---
# <a name="create-and-associate-registers"></a>Crear y asociar registros

[!include[task guide banner](../includes/task-guide-banner.md)]

Este procedimiento muestra cómo crear un registro de punto de venta (PDV). Este procedimiento usa la empresa de datos de demostración USRT.

1. Vaya a Venta minorista y comercio > Configuración de canal > Configuración de PDV > PDV > Cajas registradoras.
2. Haga clic en Nuevo.
3. En el campo Número de registro, escriba un id. para el nuevo registro.
    * El id. de registro incluye normalmente códigos que ayudan a asignar el registro a la tienda a la que pertenece y a la ubicación dentro del almacén.  
4. En el campo Nombre, escriba un nombre descriptivo para el registro.
5. En el campo Número de tienda, especifique o seleccione un valor.
6. En el campo Perfil de hardware, especifique o seleccione un valor.
    * Los perfiles de hardware se utilizan para especificar los periféricos comerciales que se conectarán con el registro, como la caja registradora y la impresora de recibos.  
7. En el campo Perfil visual, especifique o seleccione un valor.
    * Los perfiles visuales se utilizan para especificar las imágenes usadas en el fondo del PDV y la página de inicio de sesión así como los temas para el PDV.  
8. En el campo Número de caja registradora de PDV de EFT, escriba un valor.
    * El número de registro de PDV de EFT se utiliza para informar al procesador de pagos de qué terminal de pago está enviando solicitudes de autorización. Este valor a menudo se denomina "Id. de terminal" o "TID". El TID se puede encontrar generalmente en una etiqueta adhesiva del dispositivo de pago.  
9. Haga clic en Guardar.

