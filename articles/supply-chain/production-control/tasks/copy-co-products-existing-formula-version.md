---
title: Copiar coproductos de una versión de fórmula existente
description: Este procedimiento muestra cómo copiar coproductos derivados de una versión de fórmula existente a otra versión de fórmula diferente para un producto liberado.
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: EcoResProductDetailsExtended, BOMConsistOf, PmfFormulaCoBy, BOMRouteCopyDialog
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 179c12da0c2ddc7b5e2f2fdddd21168eac121811
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "319256"
---
# <a name="copy-co-products-from-an-existing-formula-version"></a>Copiar coproductos de una versión de fórmula existente

[!include [task guide banner](../../includes/task-guide-banner.md)]

Este procedimiento muestra cómo copiar coproductos derivados de una versión de fórmula existente a otra versión de fórmula diferente para un producto liberado. Es un requisito previo que haya al menos una versión de fórmula asociada a coproductos. La empresa de datos de demostración USP2 se utiliza para crear este procedimiento.


## <a name="find-a-released-product"></a>Buscar un producto liberado
1. Vaya a Productos emitidos.
2. Haga clic en Mostrar filtros.
    * Está a punto de agregar el tipo de producción de campo en el cuadro de diálogo de filtro.  
3. Haga clic en el campo Agregar un filtro para agregar el campo Tipo de producción.
    * En el siguiente paso, necesita especificar manualmente la fórmula en el campo Tipo de producción antes de seleccionar Aplicar. Esto establece el filtro en la lista de productos emitidos.  
4. Especifique manualmente la fórmula en el campo Tipo de producción.
5. Haga clic en Aplicar.

## <a name="select-a-released-product"></a>Seleccionar un producto liberado
1. En la lista, busque y seleccione el registro deseado.
2. Haga clic en Versiones de fórmula.
    * En el panel de acciones Ingeniería, haga clic en Versiones de fórmula.  

## <a name="copy-co-products"></a>Copiar coproductos
1. En el panel de acciones, haga clic en Versión de fórmula.
2. Haga clic en Productos conjuntos.
3. Haga clic en Copiar.
4. En el campo Número de artículo, especifique o seleccione un valor.
5. En el campo Versión de fórmula, especifique o seleccione un valor.
6. Haga clic en Aceptar
7. Cierre la página.

