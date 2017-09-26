--- 
title: "Configurar directivas para jerarquías de categorías de compras"
description: "Use este procedimiento para configurar las reglas para solicitar productos en una categoría."
author: mkirknel
manager: AnnBe
ms.date: 08/25/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f01d88149074b37517d00f03d8f55e1199a5198f
ms.openlocfilehash: 5ad4c448077ef9cf40555d39bb69c3ba8e2bce1e
ms.contentlocale: es-es
ms.lasthandoff: 07/27/2017

---
# <a name="set-up-policies-for-procurement-category-hierarchies"></a>Configurar directivas para jerarquías de categorías de compras

[!include[task guide banner](../../includes/task-guide-banner.md)]

Use este procedimiento para configurar las reglas para solicitar productos en una categoría. Las reglas se definen para una directiva de compras específica. La regla de acceso de categorías controla a qué categorías de compras tendrán acceso los empleados al crear una solicitud. Cuando se está creando una solicitud, la directiva de compra y regla de acceso de categoría que se deben aplicar se determinan por la entidad jurídica y la unidad operativa a las que pertenece el empleado. Puede utilizar este procedimiento en la empresa de datos de demostración USMF. Esta tarea la realizará normalmente un director de compras.


## <a name="find-the-procurement-policy"></a>Encuentre la directiva de compras
1. Vaya a Adquisición y abastecimiento > Configuración > Directivas > Directivas de compra.
2. Haga clic en el vínculo en la directiva de USMF de la directiva de compras.
    * Esta es la política a la que agregará una regla. Debe ser una directiva activa.  

## <a name="create-a-category-access-rule"></a>Crear una regla de acceso de categorías
1. Seleccione la Regla de directivas de acceso a categorías.
    * Si el botón Crear regla de directivas aparece atenuado, se debe a que ya hay una regla de directivas activa para el acceso de categorías. Compruebe los campos Vigencia y Fecha de vencimiento para determinar cuál es, después selecciónelo y haga clic en Regla de directivas de jubilación. Si el botón Crear regla de directivas está disponible, no necesita hacer nada.  
2. Haga clic en Crear regla de directivas.
3. En el campo Fecha de vigencia, especifique una fecha y una hora.
    * El tiempo no se debe superponer con otra regla que ya esté activa.  
    * Seleccione una categoría a la que se aplicará la regla. Anote qué categoría es, ya que la necesitará más adelante. Al seleccionar una categoría, sus categorías principales también se agregará a la lista Categorías seleccionadas.  
    * Si desea que la regla se aplique a todas las subcategorías de la categoría seleccionada, active la casilla Incluir subcategorías.  
4. Haga clic en Agregar.
    * Si establece la opción Incluir regla principal en Sí, la regla de directivas que se defina para una categoría principal también se asigna a sus categorías secundarias si no se ha definido ninguna regla de directivas para las categorías secundarias.  
5. Haga clic en Aceptar

## <a name="create-a-category-policy-rule"></a>Cree una regla de directivas de categoría.
1. Seleccione la Regla de directivas de categorías
    * Si el botón Crear regla de directivas aparece atenuado, seleccione la regla de directivas activa y, a continuación, haga clic en Regla de directivas de jubilación.  
2. Haga clic en Crear regla de directivas.
3. En el campo Fecha de vigencia, especifique una fecha y una hora.
4. Haga clic en Agregar.
5. Seleccione la misma categoría que utilizó para la regla de acceso de categorías.
6. En el campo Selección de proveedores, seleccione una opción.
    * Seleccione una regla para controlar qué tipo de proveedores se pueden seleccionar para la categoría al crear solicitudes.  
7. Haga clic en Cerrar.
    * Las reglas de directivas que ha definido han sido para solicitudes de tipo Consumo. Si deseara definir directivas para solicitudes del tipo Reabastecimiento, crearía una regla para el tipo Regla de directivas llamada “Regla de directivas de acceso de categorías de reabastecimiento”.  

