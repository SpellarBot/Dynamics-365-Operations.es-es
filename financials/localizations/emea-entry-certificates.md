---
title: Certificados de entrada de la UE
description: "Este artículo proporciona información acerca de los certificados de entrada en la Unión Europea (UE)."
author: ShylaThompson
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: CustEntryCertificateJour_W, CustParameters, CustTable, SalesTable
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 11464
ms.assetid: e2240f55-cc9a-4ba4-ad50-2d919bca3b7f
ms.search.region: Austria, Belgium, Czech Republic, Denmark, Estonia, Finland, France, Germany, Hungary, Ireland, Italy, Latvia, Lithuania, Netherlands, Poland, Spain, Sweden, United Kingdom
ms.author: mrolecki
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 6bb98cc72c2ec0c1551412dd39d5bea3ce10e2cd
ms.openlocfilehash: a951b1f0159ef61704fb772d81ab6a9bc1c80589
ms.lasthandoff: 03/31/2017


---

# <a name="eu-entry-certificates"></a>Certificado de entrada de la UE

[!include[banner](../includes/banner.md)]


Este artículo proporciona información acerca de los certificados de entrada en la Unión Europea (UE).

Puede realizar las tareas siguientes para un certificado de entrada de la Unión Europea (UE):

-   Crear y emitir un certificado de entrada de la UE junto con un albarán o una factura de cliente para la entrega de artículos o servicios en los países o regiones de la UE.
-   Recibir el certificado de entrada de la UE firmado por un cliente de la UE.
-   Cargar el certificado de entrada de la UE firmado que se recibe del cliente o de un tercero que es responsable de entregar los artículos al cliente.
-   Asociar el certificado de entrada de la UE cargado con una factura de cliente.
-   Actualizar el estado del certificado de entrada de la UE cargado.

## <a name="prerequisites"></a>Requisitos previos
La tabla siguiente muestra los requisitos previos que deben cumplirse antes de comenzar.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Categoría</th>
<th>Requisito previo</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>País o región</td>
<td>La dirección principal de la entidad jurídica debe estar en un estado miembro de la Unión Europea.</td>
</tr>
<tr class="even">
<td>Tareas de configuración relacionadas</td>
<td><ul>
<li>En la página <strong>Parámetros de clientes</strong>, seleccione las opciones <strong>Habilitar administración de certificados de entrada</strong> y <strong>Habilitar emisión de certificados de entrada</strong>.</li>
<li>En la página <strong>Clientes</strong>, en la ficha desplegable <strong>Factura y entrega</strong>, seleccione <strong>Se necesita certificado de entrada</strong> para indicar que un certificado de entrada de la UE es obligatorio para el cliente. Seleccione la opción <strong>Emitir certificado de entrada</strong> para emitir un certificado de entrada de la UE para la entidad jurídica del cliente.</li>
<li>En la página <strong>Parámetros de clientes</strong>, seleccione un código de secuencia numérica para la referencia <strong>Certificado de entrada</strong>.</li>
</ul></td>
</tr>
<tr class="odd">
<td>Transacciones relacionadas</td>
<td><ul>
<li>Cree una cuenta de cliente.</li>
<li>Cree un pedido de ventas.</li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="creating-registering-and-uploading-an-eu-entry-certificate"></a>Creación, registro y carga de un certificado de entrada de la UE
Puede crear un certificado de entrada de la UE de forma automática o manual. Un certificado de entrada de la UE se crea y se imprime automáticamente al registrar un albarán o una factura para un cliente mediante a través de la página **Registro del albarán** o la página **Registro de factura**. Para crear manualmente o reimprimir un certificado de entrada de la UE para una factura de cliente, use la página **Diario de facturas**. También, puede usar la página **Diario de certificado de entrada** para especificar detalles acerca de un certificado de entrada de la UE emitido por un tercero.

### <a name="creating-an-eu-entry-certificate-automatically-or-manually"></a>Creación de un certificado de entrada de la UE de forma automática o manual

Puede crear un certificado de entrada de la UE automáticamente usando un albarán en la página **Todos los pedidos de ventas** o mediante una factura en la página **Pedido de venta**. Para crear manualmente un certificado de entrada de la UE, puede usar una factura en la página **Diario de facturas**. Sin embargo, debe cambiar el estado de certificado de la factura antes de crear manualmente un certificado de entrada de la UE.

### <a name="registering-an-eu-entry-certificate"></a>Registro de un certificado de entrada de la UE

Si se requiere un registro, puede usar la página **Diario de certificado de entrada** para registrar una entrada de la UE emitido por un tercero.

### <a name="uploading-a-received-eu-entry-certificate"></a>Carga de un certificado de entrada de la UE recibido

Utilice la página **Archivos adjuntos** para cargar un certificado de entrada de la UE firmado por un cliente de la UE. Después de que se carga el certificado, puede asociarlo con una factura como prueba de la entrega de los artículos. Se requiere esta prueba si debe emitir una factura que no incluya el Impuesto sobre el valor añadido (IVA) y también se usa durante la auditoría.

### <a name="optional-updating-the-certification-status-and-printing-status-of-an-invoice"></a>Opcional: Actualización del estado de impresión y certificación de una factura

Puede actualizar el estado de certificación de entrada y el estado de impresión de una factura de cliente mediante la página **Diario de facturas**.

## <a name="technical-information-for-system-administrators"></a>Información técnica para administradores del sistema
Si no tiene acceso a las páginas que se usan para completar esta tarea, póngase en contacto con el administrador del sistema y proporcione la información que se indica en la tabla siguiente.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Categoría</th>
<th>Requisito previo</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Roles y responsabilidades de seguridad</td>
<td>Para configurar y crear certificados de entrada de la UE para artículos o servicios, debe ser miembro de un rol de seguridad que incluya las siguientes responsabilidades:
<ul>
<li><strong>Funcionario de clientes</strong> (CustInvoiceAccountsReceivableClerk)</li>
<li><strong>Representante de servicio al cliente</strong> (TradeCustomerServiceRepresentative)</li>
<li><strong>Funcionario de ventas</strong> (TradeSalesClerk)</li>
<li><strong>Funcionario de envío</strong> (InventShippingClerk)</li>
</ul></td>
</tr>
</tbody>
</table>





