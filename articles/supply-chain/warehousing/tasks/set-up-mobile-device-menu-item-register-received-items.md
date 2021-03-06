---
title: Configurar un elemento de menú del dispositivo móvil para registrar los artículos recibidos
description: Esta tarea se centra en la configuración de un elemento de menú de dispositivo móvil.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSRFMenuItem, WHSRFMenu
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 3cab7eced20111b82afabe69b6f994333b16209a
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "318060"
---
# <a name="set-up-a-mobile-device-menu-item-to-register-received-items"></a>Configurar un elemento de menú del dispositivo móvil para registrar los artículos recibidos

[!include [task guide banner](../../includes/task-guide-banner.md)]

Esta tarea se centra en la configuración de un elemento de menú de dispositivo móvil. Este elemento de menú se usa para el registro de la recepción de los artículos pedidos mediante pedidos de compra. 

Puede usar esta guía en la empresa de datos de demostración USMF. Este procedimiento va destinado al encargado de almacén.


## <a name="create-a-mobile-device-menu-item"></a>Crear un elemento de menú del dispositivo móvil
1. Vaya a Gestión de almacenes > Configurar > Dispositivo móvil > Elementos de menú del dispositivo móvil.
2. Haga clic en Nuevo.
3. En el campo Nombre del elemento de menú, escriba un valor.
    * Este es el identificador único para este elemento de menú del dispositivo móvil. Por ejemplo, podría escribir “Mi registro de pedidos de compra”.  
4. En el campo Título, escriba un valor.
    * Este es el título, que se mostrará al usuario en el dispositivo móvil. Por ejemplo, podría escribir “Registro de pedidos de compra”.  
5. En el campo Modo, seleccione Trabajo.
    * El registro de las cantidades disponibles recibidas para una línea de pedido de compra creará el trabajo para mover los artículos del área de recepción al inventario. El trabajo no se crea hasta que no se registran los artículos.  Por tanto, deje la opción Usar trabajo existente establecida en No.  
6. Expanda o contraiga la sección General.
7. En el campo Proceso de creación de trabajo, seleccione "Recepción de artículo del pedido de compra".
    * Una línea de pedido de compra se debe identificar de manera exclusiva para que la cantidad disponible se pueda registrar en el almacén. En esta situación, el dispositivo móvil registrará el número del pedido de compra y el código del artículo, y esto permitirá al sistema identificar la línea del pedido de compra. Se creará trabajo de ubicación y se podrá seleccionar por otro trabajador.    El método de creación de trabajo que seleccione determina qué campos están disponibles en la ficha desplegable General.  
    * Si selecciona la opción Usar datos predeterminados, se habilita el botón Datos predeterminados. Aquí puede seleccionar campos para mostrar los datos que un trabajador necesita normalmente en su trabajo diario, de manera que se muestren estos valores en el dispositivo móvil.  
    * El parámetro Agrupar por matrícula de entidad de almacén funciona junto con el grupo de secuencias de unidades que se asigna al artículo que se está recibiendo. Puede especificar si los recibos de menos o más de un pallet se deben agrupar en una matrícula de entidad de almacén o dividirse en una matrícula de entidad de almacén independiente para cada unidad.  
    * Si selecciona la opción Generar matrícula de entidad de almacén, esto genera una matrícula de entidad de almacén única basada en la selección de la secuencia numérica.   
    * Puede seleccionar la plantilla que se usará al crear el trabajo. Por ejemplo, si registra un artículo para un pedido de compra, el trabajo de ubicación se generará en función de la plantilla de trabajo. Si no selecciona una plantilla de trabajo aquí, el sistema asignará una plantilla basada en los criterios de consulta que están asociados a las plantillas.  
    * Si los códigos de disposición se muestran en el dispositivo móvil, los trabajadores pueden evaluar el estado o la calidad de los artículos, y seleccionar el código apropiado. Las reglas del código de disposición determinan si los artículos estarán disponibles para otros procesos de almacén. Las reglas también determinan qué directiva de ubicación se usa para el trabajo creado.   
    * Si seleccione la opción Códigos de disposición de lote, los trabajadores pueden evaluar el estado o la calidad de un lote y seleccionar el código de disposición apropiado.  Las reglas que se establecen en el código de disposición de lote determinan si el lote estará disponible para otros procesos de almacén.  
    * Si selecciona la opción Imprimir etiquetas, se imprimirá automáticamente una etiqueta de matrícula de entidad de almacén cuando se reciban los artículos.  
8. Haga clic en Guardar.
9. Cierre la página.

## <a name="add-the-menu-item-to-a-mobile-device-menu"></a>Agregar el elemento de menú a un menú de dispositivo móvil
1. Vaya a Gestión de almacenes > Configurar > Dispositivo móvil > Menú del dispositivo móvil.
2. Use el filtro rápido para filtrar el campo Nombre con un valor de "entrada".
3. Haga clic en Editar.
4. En el árbol, seleccione "En el árbol, seleccione el elemento de menú que ha creado antes".
    * Seleccione el elemento de menú que ha creado anteriormente.  
5. Haga clic en la flecha que apunta a la derecha.
6. Haga clic en Guardar.
7. Cierre la página.

