---
title: Precio base y acuerdos comerciales
description: Este procedimiento le muestra la creación de acuerdos comerciales de precios de venta específicos de canal.
author: josaw1
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PriceDiscGroup, RetailStoreTable, RetailChannelPriceGroup, EcoResProductDetailsExtended, PriceDiscAdmTable, PriceDiscAdm
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4830ac553318cfbb3cb74395d1662e74dff75290
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "320429"
---
# <a name="base-price-and-trade-agreements"></a>Precio base y acuerdos comerciales

[!include[task guide banner](../includes/task-guide-banner.md)]

Este procedimiento le muestra la creación de acuerdos comerciales de precios de venta específicos de canal. Este procedimiento usa la empresa de datos de demostración USRT.

1. Vaya a Venta minorista y comercio > Precios y descuentos > Grupos de precios > Todos los grupos de precios.
    * Los grupos de precios son la manera en que los acuerdos comerciales se asignan a los canales específicos. El uso de grupos de precios para asignar acuerdos comerciales a un canal permite precios específicos de canal.  
2. Haga clic en Nuevo.
3. En el campo Grupos de precios, escriba un valor.
4. En el campo Nombre, escriba un valor.
5. Haga clic en Guardar.
6. Cierre la página.
7. Vaya a Venta minorista y comercio > Canales > Tiendas > Todas las tiendas minoristas.
8. En la lista, seleccione "Nueva York"
9. En el panel de acciones, haga clic en Tienda.
10. Haga clic en Grupos de precios.
11. Haga clic en Nuevo.
12. En el campo Grupos de precios, haga clic en el botón desplegable para abrir la búsqueda.
13. En la lista, busque y seleccione el registro deseado.
14. Haga clic en Guardar.
15. Cierre la página.
16. Cierre la página.
17. Vaya a Venta minorista y comercio > Productos y categorías > Productos liberados por categoría.
18. En la lista, haga clic en el vínculo de la fila seleccionada.
19. Haga clic en Editar.
20. Alterne la expansión de la sección Vender.
21. En el campo Precio, escriba un número.
    * Este precio se usa si no se encuentra ningún acuerdo comercial aplicable.  
22. Haga clic en Guardar.
23. En el panel de acciones, haga clic en Vender.
24. Haga clic en Crear acuerdos comerciales.
25. Haga clic en Nuevo.
26. En el campo Nombre, haga clic en el botón desplegable para abrir la búsqueda.
27. En la lista, seleccione "Venta minorista".
    * En los datos de demostración, el nombre de diario "Venta minorista" tiene la relación predeterminado de "Precio (ventas)". Esto significa que todas las nuevas líneas creadas se asignarán de forma predeterminada a los acuerdos comerciales de precio de ventas.  
28. Haga clic en Líneas.
29. En el campo Código de cuenta, seleccione "Grupo".
30. En el campo Selección de cuentas, haga clic en el botón desplegable para abrir la búsqueda.
31. En la lista, busque y seleccione el registro deseado.
    * Esto completará Vincular el grupo de precios a un cana al Acuerdo comercial.  
32. En el campo Relación de artículos, escriba un valor.
33. En el campo Importe en divisa, escriba un número.
34. Active o desactive la casilla Buscar siguiente.
    * Cuando Buscar siguiente se establezca en "Sí", el motor de precios continuará buscando acuerdos comerciales aplicables con un precio de venta menor. Cuando Buscar siguiente se establezca en "No", el motor de precios detendrá la búsqueda y usará el acuerdo comercial.  
35. Haga clic en Registrar.
36. Haga clic en Aceptar
37. Cierre la página.
38. En el panel de acciones, haga clic en Vender.
39. Haga clic en Precio de ventas.

