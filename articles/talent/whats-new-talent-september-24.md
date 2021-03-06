---
title: Novedades y cambios en Dynamics 365 for Talent Core HR (24 de septiembre de 2018)
description: Este tema describe las características que son nuevas o que se han cambiado en Microsoft Dynamics 365 for Talent Core HR.
author: Darinkramer
manager: AnnBe
ms.date: 09/21/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2018-09-30
ms.dyn365.ops.version: Talent
ms.openlocfilehash: 24526a5884c6c5d30d1f49077b88a24364aa4365
ms.sourcegitcommit: 608e68b603afef9eb98d8fb25e90109c2473ef87
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "856170"
---
# <a name="whats-new-or-changed-in-dynamics-365-for-talent-core-hr-september-24-2018"></a>Novedades y cambios en Dynamics 365 for Talent Core HR (24 de septiembre de 2018)

[!include [banner](includes/banner.md)]

**Compilación 8.1.1015.0**

Este tema describe las características que son nuevas o que se han cambiado en Core HR.

## <a name="currency-added-to-benefits"></a>Divisa agregada a prestaciones

Se han actualizado los planes de prestaciones para incluir la divisa de la prestación. Este nuevo campo también está disponible en las prestaciones de los trabajadores inscritos. Este nuevo campo es parte del privilegio de seguridad Mantener beneficios y Ver una lista de beneficios.

## <a name="update-proration-process--leave-and-absence"></a>Actualizar proceso de prorrateo - bajas y ausencias

Las organizaciones conceden tiempo libre de manera diferente basándose en cuándo los empleados se unen y dejan la empresa. Para los empleados que salen de la organización, algunos tienen que finalizar la prima en la fecha final, mientras que otros se basan en el último día trabajado para detener el proceso de acumulación. Estos cambios proporcionan a las organizaciones la capacidad para elegir cuándo finalizar la inscripción durante el proceso de finalización. Estas nuevas opciones son parte de los privilegios para dar de baja a un trabajador y dar de baja a un trabajador del autoservicio de directores. 

## <a name="other-changes"></a>Otros cambios

Este lanzamiento incluye varias correcciones de errores adicionales.

## <a name="known-issue"></a>Problema conocido

-   **Problema:** Al agregar nuevos archivos adjuntos a un trabajador, los botones **Nuevo** y **Editar** se atenúan. **Solución alternativa**: Antes de abrir la página de los datos adjuntos, asegúrese de que los cuadros informativos de la página **Trabajador** estén cerrados. Si se cierran los cuadros informativos cuando la página **Trabajador** se carga, los botones de datos adjuntos se habilitan. (Este problema se corregirá en la siguiente actualización de la plataforma).
