---
title: Contenido de Power BI sobre configurar la seguridad para el análisis de la contabilidad de costes
description: Este tema explica cómo puede extender la seguridad de nivel de acceso en contabilidad de costes a la seguridad de nivel de fila en Microsoft Power BI. Esta funcionalidad ayuda a garantizar que los usuarios ven solo los datos de Power BI a los que se les conceden acceso.
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Operations
ms.custom: 270294
ms.assetid: 3a7ba8b0-ac57-4159-9cd8-4308f6021f36
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: d1cd378a58d4a4fe4388238f97e84a8e2b07937b
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "352882"
---
# <a name="set-up-security-for-the-cost-accounting-analysis-power-bi-content"></a>Contenido de Power BI sobre configurar la seguridad para el análisis de la contabilidad de costes

[!include [banner](../includes/banner.md)]

Este tema explica cómo puede extender la seguridad de nivel de acceso en contabilidad de costes a la seguridad de nivel de fila en Microsoft Power BI. Esta funcionalidad ayuda a garantizar que los usuarios ven solo los datos de Power BI a los que se les conceden acceso.

## <a name="overview"></a>Información general

El contenido de Microsoft Power BI sobre **Análisis de la contabilidad de costes** utiliza la seguridad de nivel de fila de Power BI para limitar el acceso a un usuario. La seguridad se basa en la jerarquía organizativa del nivel de acceso que se configura en los parámetros de contabilidad de costes. Para obtener más información acerca del contenido de Power BI sobre **Análisis de la contabilidad de costes**, consulte el [Contenido de Power BI sobre el análisis de la contabilidad de costes](cost-accounting-analysis-content-pack.md).

## <a name="setup"></a>Configurar
Para extender la seguridad de nivel de acceso a Power BI, el propietario de contenido de Power BI debe seguir estos pasos.

> [!NOTE]
> El usuario que publica el contenido de Power BI sobre el **Análisis de la contabilidad de costes** se convierte automáticamente en el propietario. Solo un propietario puede configurar la seguridad en Power BI. Asimismo, hasta que un propietario agregue a otros usuarios en PowerBI.com, nadie excepto el propietario podrá ver los datos en el contenido de Power BI sobre el **análisis de la contabilidad de costes**.

1. Publicar el archivo de definición para Power BI.
2. Iniciar sesión en PowerBI.com.
3. Encuentre el conjunto de datos para el contenido de Power BI sobre el **Análisis de la contabilidad de costes**.
4. Abrir la página de seguridad.

    ![Abrir la página de seguridad](./media/CA-picture-1.png)

5. El rol **Controlador de objeto de coste** ya está creado. Agregar otros miembros que forman parte de la jerarquía organizativa del nivel de acceso de la contabilidad de costes.

    ![Agregar miembros](./media/CA-picture-2.png)

Los usuarios que se agregan al rol de **Controlador de objeto de coste** solo verán los datos que se les permite ver, según la definición de la jerarquía organizativa del nivel de acceso de la contabilidad de costes.

> [!NOTE]
> La seguridad de nivel de fila se aplica a los mosaicos e informes de Microsoft Dynamics 365 for Finance and Operations que se insertan desde Power BI.

## <a name="updating-security"></a>Actualizar la seguridad
Si se crean actualizaciones para la seguridad de nivel de acceso en contabilidad de costes y desea que Power BI refleje dichas actualizaciones, debe actualizar el almacén de entidades para el contenido de Power BI sobre el **análisis de la contabilidad de costes**. Una vez que complete la actualización del almacén de entidades desde Finance and Operations, deberá actualizar artefactos en PowerBI.com. Para obtener más información sobre cómo realizar una actualización del almacén de entidades, consulte [Actualizar almacén de entidades](power-bi-integration-entity-store.md#update-entity-store). El propietario del contenido de Power BI sobre el **análisis de la contabilidad de costes** también debe realizar una actualización del almacén de entidades si se concede acceso a nuevos usuarios a la jerarquía organizativa. Asimismo, el propietario debe agregar a los nuevos usuarios al rol **Controlador de objeto de coste** en PowerBI.com, de manera que se aplique la seguridad de nivel de fila para ellos.

## <a name="disabling-security"></a>Deshabilitar la seguridad
Asumimos que su organización desea restringir el acceso a los datos. Si, por algún motivo, se deshabilitarán los parámetros de seguridad al ejecutar la contabilidad de costes, el propietario debe agregar usuarios al rol **Contable de costes** en Power BI en su lugar. Si cambia la seguridad de un estado habilitado a un estado deshabilitado, es recomendable quitar usuarios del rol **Controlador de objeto de coste**. Y viceversa si vuelve a habilitar la seguridad. Los usuarios pueden pertenecer a ambos roles. El acceso común es la unión de ambos roles. En el caso del contenido de Power BI sobre el **análisis de la contabilidad de costes**, los usuarios con acceso común tiene acceso sin restricción a los datos. Si su objetivo es aplicar un acceso restringido, los usuarios deben asignarse solo al rol **Controlador de objeto de coste**. Estas actualizaciones de seguridad de nivel de fila tienen efecto de inmediato. Los usuarios afectados deben actualizar sus exploradores.

## <a name="additional-resources"></a>Recursos adicionales
Para obtener más información acerca de la seguridad de nivel de fila de Power BI, consulte [Gestionar la seguridad de su modelo en Power BI](https://powerbi.microsoft.com/en-us/documentation/powerbi-admin-rls/#manage-security-on-your-model).
