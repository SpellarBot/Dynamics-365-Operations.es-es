---
title: "Administración y creación de categorías de productos"
description: "En este tema se describen las mejoras que se han realizado en la experiencia de gestión de las categorías de productos al por menor. Estas mejoras permiten a los encargados de comercialización tener una correlación entre la jerarquía de producto y los detalles del producto liberado."
author: ashishmsft
manager: AnnBe
ms.date: 09/01/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.search.scope: 
ms.search.region: Global
ms.author: asharchw
ms.search.validFrom: 2017-09-01
ms.dyn365.ops.version: 
ms.translationtype: HT
ms.sourcegitcommit: 6b9afb40b68b672514c083d99efbc9bd098dd561
ms.openlocfilehash: b158ff5b277c125e0aa158c071007ed8a0f25482
ms.contentlocale: es-es
ms.lasthandoff: 10/03/2017

---

# <a name="product-category-management-and-creation"></a><span data-ttu-id="d828b-104">Administración y creación de categorías de productos</span><span class="sxs-lookup"><span data-stu-id="d828b-104">Product category management and creation</span></span>

[!include[banner](./includes/banner.md)]

<span data-ttu-id="d828b-105">Gracias a las mejoras que se han realizado en la experiencia de gestión en el caso de las categorías de productos al por menor, permiten a los gestores de comercialización (TMA) tener una correlación entre la jerarquía de productos y los detalles del producto liberado.</span><span class="sxs-lookup"><span data-stu-id="d828b-105">Enhancements that have been made to the management experience for Retail product categories let merchandising managers have a correlation between Retail product hierarchy and released product details.</span></span> <span data-ttu-id="d828b-106">Para ver estos mejoras, en el área de trabajo **Categoría y gestión de productos**, seleccione **Jerarquía del producto al por menor** para abrir la página **Nueva estructura de la categoría de producto al por menor**.</span><span class="sxs-lookup"><span data-stu-id="d828b-106">To view these enhancements, in the **Category & product management**  workspace, select **Retail product hierarchy** to open the **New structure of Retail product category** page.</span></span> 

<span data-ttu-id="d828b-107">En versiones anteriores, las propiedades del producto se dividían en propiedades básicas de producto y propiedades de producto al por menor, en función del ámbito de su aplicabilidad.</span><span class="sxs-lookup"><span data-stu-id="d828b-107">In previous releases, product properties were divided into Basic product properties and Retail product properties, based on the scope of their applicability.</span></span> <span data-ttu-id="d828b-108">Las propiedades de producto al por menor eran *globales*</span><span class="sxs-lookup"><span data-stu-id="d828b-108">Retail product properties were *global*.</span></span> <span data-ttu-id="d828b-109">Es decir, para una propiedad dada del producto, el mismo valor se comparte en todas las entidades jurídicas.</span><span class="sxs-lookup"><span data-stu-id="d828b-109">In other words, for a given product property, the same value is shared across all legal entities.</span></span> <span data-ttu-id="d828b-110">Las propiedades básicas de producto eran *específicas de cada entidad jurídica*.</span><span class="sxs-lookup"><span data-stu-id="d828b-110">Basic product properties were *legal entity–specific*.</span></span> <span data-ttu-id="d828b-111">Esto es, que la propiedad dada de un producto puede ser diferente entre entidades jurídicas, en función de los requisitos empresariales individuales.</span><span class="sxs-lookup"><span data-stu-id="d828b-111">In other words, a given product property might differ across legal entities, based on individual business requirements.</span></span>

<span data-ttu-id="d828b-112">Con estas mejoras en las propiedades de producto en la categoría de producto al por menor, continuamos separando los campos en función de su aplicabilidad dentro de un grupo, para así reflejar la estructura del formulario de detalles del producto liberado.</span><span class="sxs-lookup"><span data-stu-id="d828b-112">With these enhancements, for product properties in the Retail product category, we continue to separate the fields, based on their applicability within a group, to reflect the released product details form structure.</span></span>

<span data-ttu-id="d828b-113">Puede elegir si quiere gestionar las propiedades específicas de todas las entidades jurídicas o gestionarlas según una entidad jurídica específica.</span><span class="sxs-lookup"><span data-stu-id="d828b-113">You can switch between managing legal-entity specific properties across all legal entities and managing them for a specific legal entity.</span></span> <span data-ttu-id="d828b-114">Simplemente seleccione **Ver o editar los detalles de todas las entidades jurídicas** o **Ver o editar los detalles de una entidad jurídica específica** como sea necesario.</span><span class="sxs-lookup"><span data-stu-id="d828b-114">Just select **View/Edit for all legal entities** or **View/Edit for a specific legal entity** as you require.</span></span>

<span data-ttu-id="d828b-115">Los gestores de marketing también pueden definir los valores predeterminados de un conjunto adicional de propiedades de producto en el nivel de una categoría individual.</span><span class="sxs-lookup"><span data-stu-id="d828b-115">Merchandising managers can also define default values for an additional set of product properties at the level of an individual category.</span></span> <span data-ttu-id="d828b-116">Un producto hereda estos valores de propiedades, en función de su asociación con una categoría a la hora de crear el producto.</span><span class="sxs-lookup"><span data-stu-id="d828b-116">These property values are inherited by a product, based on their association with a category at the time of product creation.</span></span>

## <a name="select-properties-to-update-products-from-the-retail-product-category-form"></a><span data-ttu-id="d828b-117">Seleccionar las propiedades adecuadas para actualizar productos desde el formulario de categoría de productos al por menor</span><span class="sxs-lookup"><span data-stu-id="d828b-117">Select properties to update products from the Retail product category form</span></span>

<span data-ttu-id="d828b-118">Puede usar las propiedades de agrupación lógicas para seleccionar qué propiedades actualizadas deben relacionarse con los productos asociados.</span><span class="sxs-lookup"><span data-stu-id="d828b-118">You can use logical grouping properties to select which updated product properties should be pushed to associated products.</span></span>

<span data-ttu-id="d828b-119">Los encargados comercialización pueden modificar estas propiedades de producto heredadas para cada producto, y así poder cumplir con los requisitos empresariales individuales.</span><span class="sxs-lookup"><span data-stu-id="d828b-119">Merchandising managers can modify these inherited product properties for each product, to meet individual business requirements.</span></span>
