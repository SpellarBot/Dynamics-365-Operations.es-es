---
title: "Inicializar datos semilla en un nuevo entorno de distribución"
description: "En este artículo se describen los datos que se crean como parte del proceso de inicialización para Microsoft Dynamics 365 for Operations - Retail."
author: josaw1
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations, Core, Retail
ms.custom: 49621
ms.assetid: 4dc762eb-190e-4485-8f55-b0cafc81bc37
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b1f91f863c8da35362ebb3036e76aa10d95ba65
ms.openlocfilehash: b5290bb62ab8ad71b06b0478ccaf6dbb61454170
ms.contentlocale: es-es
ms.lasthandoff: 04/26/2017


---

# <a name="initialize-seed-data-in-a-new-retail-environment"></a>Inicializar datos semilla en un nuevo entorno de distribución

[!include[banner](includes/banner.md)]


En este artículo se describen los datos que se crean como parte del proceso de inicialización para Microsoft Dynamics 365 for Operations - Retail.

Después de que la solución de venta minorista se haya desplegado con los servicios de ciclo de vida de Microsoft Dynamics, debe inicializar la configuración de venta minorista para crear los datos de configuración básicos. **Importante:** antes de inicializar la configuración de venta minorista, asegúrese de que haya especificado un idioma y una dirección postal para cada entidad jurídica en la que va a configurar tiendas de venta minorista. Este paso se debe completar para cada entidad jurídica que se use para la venta minorista. Para inicializar la configuración de venta minorista, siga estos pasos.

1.  Inicie el cliente de Dynamics 365 for Operations.
2.  Haga clic en **Venta minorista y comercio** &gt; **Configuración de sede central** &gt; **Parámetros** &gt; **Parámetros comerciales**.
3.  Haga clic en **Inicializar**.

Inicialización crea los datos de configuración siguientes predeterminados:

-   Trabajos y subtrabajos del programador de ventas minoristas
-   Esquema del canal comercial
-   Programaciones de distribución de ventas minoristas
-   Diseños de pantalla predeterminados, que incluyen bloqueos, imágenes y temas
-   Información de zona horaria
-   Operaciones de punto de venta (PDV)
-   Permisos de PDV
-   Informes de canales
-   Metadatos de atributos
-   Plantillas de validación de entidad
-   Trabajo por lotes para purgar historial de la sesión de intercambio de datos comerciales

Además, el registro relacionado con la industria de la tarjeta de pago se habilita para la base de datos de Dynamics 365 for Operations. **Nota:** hay una opción para configurar por separado el programador de venta minorista. Esta opción permite restablecer la configuración del programador de venta minorista a sus valores predeterminados. Después de que la inicialización esté completada, debe configurar los datos adicionales de la venta minorista. A continuación se incluyen algunos ejemplos:

-   Parámetros comerciales
-   Parámetros del Programador de tareas Retail
-   Canales comerciales
-   Cajas registradoras y dispositivos
-   Varios




