---
title: "Espacio de trabajo móvil Aprobaciones de facturas"
description: "Este tema proporciona información sobre del espacio de trabajo móvil Aprobaciones de facturas. Este espacio de trabajo proporciona una lista de facturas que se le han asignado a través del proceso de flujo de trabajo del encabezado de factura de proveedor."
author: abruer
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: Core, Operations, UnifiedOperations
ms.search.region: Global
ms.author: abruer
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: 70f3e0fe53fc0b1daa471a7022f5659d09caa867
ms.contentlocale: es-es
ms.lasthandoff: 06/13/2017

---

# Espacio de trabajo móvil Aprobaciones de facturas
<a id="invoice-approvals-mobile-workspace" class="xliff"></a>

[!include[banner](../includes/banner.md)]

Este tema proporciona información sobre del espacio de trabajo móvil **Aprobaciones de facturas**. Este espacio de trabajo proporciona una lista de facturas que se le han asignado a través del proceso de flujo de trabajo del encabezado de factura de proveedor. 

Este espacio de trabajo móvil se debe usar con la aplicación móvil Microsoft Dynamics 365 for Unified Operations.

## Información general
<a id="overview" class="xliff"></a>

El espacio de trabajo móvil **Aprobaciones de facturas** permite a los empleados y directores de proveedores ver las facturas que se les han asignado como parte del proceso de flujo de trabajo del encabezado de factura de proveedor. Puede ver la información de la factura e incluso los detalles de la línea y la distribución, que le ayudarán a tomar decisiones informadas de aprobación. En el espacio de trabajo, puede tomar medidas para mover la factura por el proceso de flujo de trabajo. 

## Requisitos previos
<a id="prerequisites" class="xliff"></a>

Para poder usar este espacio de trabajo móvil, antes debe satisfacer los siguientes requisitos previos:

<table>
<thead>
<tr class="header">
<th>Requisito previo</th>
<th>Función</th>
<th>Descripción</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Microsoft Dynamics 365 for Finance and Operations, Enterprise Edition, actualización de julio 2017, deben haberse implementando en la organización.</td>
<td>Administrador del sistema</td>
<td>Consulte <a href="../deployment/deploy-demo-environment.md">Implementar un entorno de demostración</a>.
</td>
</tr>
<tr class="even">
<td>El espacio de trabajo móvil <strong>Aprobaciones de facturas</strong> debe publicarse.</td>
<td>Administrador del sistema</td>
<td>Consulte <a href="/dynamics365/unified-operations/dev-itpro/mobile-apps/publish-mobile-workspace">Publicar un espacio de trabajo móvil</a>.</td>
</tr>
</tbody>
</table>

## Descargar e instalar la aplicación móvil
<a id="download-and-install-the-mobile-app" class="xliff"></a>

Descargue e instale la aplicación móvil Dynamics 365 for Unified Operations:

-   [Para teléfonos Android](https://go.microsoft.com/fwlink/?linkid=850662)
-   [Para iPhones](https://go.microsoft.com/fwlink/?linkid=850663)

## Iniciar sesión en la aplicación móvil
<a id="sign-in-to-the-mobile-app" class="xliff"></a>

1.  Inicie la aplicación en su dispositivo móvil.
2.  Escriba la dirección URL de Microsoft Dynamics 365.
3.  La primera vez que se inicie sesión, se le solicitará su nombre de usuario y contraseña. Escriba sus credenciales.
4.  Tras iniciar sesión, se mostrarán los espacios de trabajo disponibles para su empresa. Tenga en cuenta que si el administrador del sistema publica un nuevo espacio de trabajo más tarde, tendrá que actualizar la lista de espacios de trabajo móviles.

    [![Toque la pantalla para actualizar](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)

## Aprobar facturas mediante el espacio de trabajo móvil Aprobaciones de facturas
<a id="approve-invoices-by-using-the-invoice-approvals-mobile-workspace" class="xliff"></a>
1.  En el dispositivo móvil, seleccione el espacio de trabajo **Aprobaciones de facturas**.
2.  Seleccione la factura que le ha sido asignada por el proceso de flujo de trabajo del encabezado de factura de proveedor.
3.  En la página **Detalles de la factura**, revise la información de encabezado de factura, como la información del proveedor y la fecha.
4.  Seleccione una línea de la factura para ver su información más detallada en la vista **Detalles de línea de factura**.
5.  En la vista **Detalles de línea de factura**, seleccione la **Distribuciones** para mostrar las distribuciones de la línea. Aquí puede ver la contabilidad para la línea de factura. La información que se muestra incluye las dimensiones financieras y la cuenta principal.
6.  En la página **Detalles de línea de factura**, seleccione la **Distribuciones** para mostrar todas las distribuciones. Aquí puede ver la contabilidad para la toda la factura. La información que se muestra incluye las dimensiones financieras y las cuentas principales. 
7.  Seleccione **Datos adjuntos** para ver las notas o los archivo que están asociadas a la factura.
8.  En la página **Detalles de la factura**, seleccione la acción del flujo de trabajo adecuado para completar el proceso de revisión.
9.  Seleccione **Listo**.
