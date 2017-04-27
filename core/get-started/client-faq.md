---
title: Preguntas frecuentes sobre el cliente de Dynamics 365 for Operations
description: "Este artículo proporciona respuestas a preguntas frecuentes acerca del cliente de Microsoft Dynamics 365 for Operations."
author: jasongre
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 12334
ms.assetid: a9a57f0e-a67c-46b1-83c9-5d6350fb3b86
ms.search.region: Global
ms.author: jasongre
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 4bb647cfd3f012efbffa93a81462c538a24ac850
ms.openlocfilehash: 2c99b2e1f7ddecb61be62832ca1a8d3ac1fd21a8
ms.lasthandoff: 03/31/2017


---

# <a name="dynamics-365-for-operations-client-faq"></a>Preguntas frecuentes sobre el cliente de Dynamics 365 for Operations

[!include[banner](../includes/banner.md)]


Este artículo proporciona respuestas a preguntas frecuentes acerca del cliente de Microsoft Dynamics 365 for Operations.

<a name="why-arent-symbols-loaded-when-i-use-dynamics-365-for-operations"></a>¿Por qué no se cargan los símbolos cuando uso Dynamics 365 for Operations?
-----------------------------------------------------------------

Las opciones de seguridad del explorador pueden impedir que los símbolos se carguen correctamente. Para resolver este problema, pruebe los siguientes pasos:

-   Si tiene este problema en Internet Explorer, haga clic en **Herramientas** y después haga clic en **Opciones de Internet**.  En el cuadro de diálogo Opciones de Internet, en la pestaña **Privacidad**, haga clic en **Nivel personalizado** y asegúrese de que la opción **Descarga de fuentes** está activada.
-   De lo contrario, puede que tenga que agregar el sitio de Microsoft Dynamics 365 for Operations a la lista de sitios de confianza.

## <a name="i-miss-the-ribbon-from-dynamics-ax-2012-can-i-keep-action-pane-tabs-open-all-the-time"></a>No veo la cinta de opciones de Dynamics AX 2012. ¿Puedo mantener las pestañas del Panel de acciones abiertas todo el tiempo?
Estamos planeando implementar esta característica pronto. Los usuarios podrán elegir entonces mantener las pestañas de los paneles de acciones abiertas todo el tiempo. De lo contrario, las pestañas se contraerán cuando no se usen, para lograr más espacio en la pantalla para la página.

## <a name="why-do-i-sometimes-see-different-shortcut-menus-when-i-rightclick"></a>¿Por qué a veces veo diferentes menús contextuales cuando hago clic con el botón secundario?
Si hace clic con el botón secundario en un campo editable (o si se selecciona texto), se mostrará el menú contextual del explorador. Este menú le concede acceso a los comandos **Cortar**, **Copiar** y **Pegar**. No podemos integrar estos comandos en los menús contextuales de Dynamics 365 for Operations porque, por motivos de seguridad, los exploradores no nos permiten obtener acceso mediante programación al portapapeles del sistema.

Si hace clic con el botón secundario en una etiqueta de campo o el valor de un control de solo lectura, verá el menú contextual de Dynamics 365 for Operations.

Para facilitar el acceso al teclado, planeamos implementar un método abreviado de teclado en el futuro que abra el menú contextual de Dynamics 365 for Operations.

## <a name="where-is-the-view-details-functionality-in-dynamics-365-for-operations"></a>¿Dónde se encuentra la funcionalidad Ver detalles en Dynamics 365 for Operations?
La opción **Ver detalles** solo está disponible de dos formas diferentes:

-   Si un control tiene capacidades **Ver detalles **, y si el control tiene un valor, ese valor se muestra como hipervínculo. Puede hacer clic en el hipervínculo para abrir una página que contiene detalles adicionales.
-   **Ver detalles** también es una opción en los menús contextuales de Dynamics 365 for Operations. Para obtener más información acerca de cuándo se muestran los menús contextuales de Dynamics 365 for Operations al hacer clic con el botón secundario, consulte la sección anterior.




