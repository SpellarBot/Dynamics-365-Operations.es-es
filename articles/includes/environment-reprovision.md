<span data-ttu-id="6022d-101">Al copiar una base de datos entre entornos, deberá ejecutar la herramienta de reaprovisionamiento de entornos antes de que la base de datos que se copió sea completamente funcional, con el fin de asegurarse de que todos los componentes de Retail se actualizaron.</span><span class="sxs-lookup"><span data-stu-id="6022d-101">When copying a database between environments, you will need to run the environment re-provisioning tool before the copied database is fully functional, to ensure that all Retail components are up-to-date.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6022d-102">Es recomendable ejecutar este procedimiento tanto si usa los componentes Retail como si no, ya que la función Retail se incluye en todos los entornos.</span><span class="sxs-lookup"><span data-stu-id="6022d-102">We recommend that you run this procedure whether you are using Retail components or not, because Retail functionality is included in all environments.</span></span> 

<span data-ttu-id="6022d-103">Antes de continuar, debe asegurarse de cumplir los siguientes requisitos previos:</span><span class="sxs-lookup"><span data-stu-id="6022d-103">Before you continue, you must make sure that the following prerequisites are met:</span></span>
1. <span data-ttu-id="6022d-104">Si se está actualizando a la versión de julio de 2017 (también conocida como 7.2) 7.2.11792.56024, aplique las siguientes revisiones de la aplicación X++ en el entorno de destino antes de ejecutar la actualización de datos en ese entorno.</span><span class="sxs-lookup"><span data-stu-id="6022d-104">If you are upgrading to the July 2017 release (also known as 7.2) 7.2.11792.56024, apply the following application X++ hotfixes in the destination environment before running the data upgrade in that environment.</span></span> <span data-ttu-id="6022d-105">Estos impedirán que se produzcan varios errores durante la actualización de datos:</span><span class="sxs-lookup"><span data-stu-id="6022d-105">These will prevent various errors occurring during the data upgrade:</span></span>

    - <span data-ttu-id="6022d-106">KB 4036156 - actualización menor de versión de Retail - "la secuencia numérica de variante no está establecida".</span><span class="sxs-lookup"><span data-stu-id="6022d-106">KB 4036156 - Retail minor version upgrade - 'Variant number sequence is not set.'</span></span> <span data-ttu-id="6022d-107">Este paquete de revisiones también incluye KB 4035399 y KB 4035751.</span><span class="sxs-lookup"><span data-stu-id="6022d-107">This fix package also includes KB 4035399 and KB 4035751.</span></span> <span data-ttu-id="6022d-108">Tenga en cuenta que para usar este paquete debe tener como mínimo la Platform Update 9.</span><span class="sxs-lookup"><span data-stu-id="6022d-108">Note that you must have a minimum of Platform Update 9 to use this package.</span></span> <span data-ttu-id="6022d-109">Si no está seguro, instale los últimos binarios.</span><span class="sxs-lookup"><span data-stu-id="6022d-109">If you are unsure, install the latest binaries.</span></span>
    
2. <span data-ttu-id="6022d-110">Si está actualizando desde Microsoft Dynamics AX 2012, instale las correcciones siguientes de la aplicación X++ en el entorno de destino antes de ejecutar la actualización de datos:</span><span class="sxs-lookup"><span data-stu-id="6022d-110">If you are upgrading from Microsoft Dynamics AX 2012, install the following application X++ fixes in the destination environment before you run the data upgrade:</span></span>
    - <span data-ttu-id="6022d-111">KB 4033183 - La actualización no minorista de Dynamics AX 2012 R2 o Dynamics AX 2012 R3 Pre-CU8 falla con Objeto no encontrado para dbo.RETAILTILLLAYOUTZONE.</span><span class="sxs-lookup"><span data-stu-id="6022d-111">KB 4033183 - Dynamics AX 2012 R2 or Dynamics AX 2012 R3 Pre-CU8 non-retail upgrade fails with Object not found for dbo.RETAILTILLLAYOUTZONE.</span></span>
    - <span data-ttu-id="6022d-112">KB 4040692 - La actualización de Dynamics AX 2012 R3 a Microsoft Dynamics 365 for Operations 7.2 falla por el índice duplicado RetailSalesLine en SalesLineIdx.</span><span class="sxs-lookup"><span data-stu-id="6022d-112">KB 4040692 - Dynamics AX 2012 R3 to Microsoft Dynamics 365 for Operations 7.2 upgrade fails on RetailSalesLine duplicate index on SalesLineIdx.</span></span>
    - <span data-ttu-id="6022d-113">KB 4035490 - Degradación de rendimiento con la actualización del script GeneralJournalAccountEntry MainAccount.</span><span class="sxs-lookup"><span data-stu-id="6022d-113">KB 4035490 - Performance issue with GeneralJournalAccountEntry MainAccount field upgrade script.</span></span>


<span data-ttu-id="6022d-114">Siga estos pasos para ejecutar la herramienta de reaprovisionamiento del entorno.</span><span class="sxs-lookup"><span data-stu-id="6022d-114">Follow these steps to run the Environment reprovisioning tool.</span></span>

1. <span data-ttu-id="6022d-115">En la biblioteca del activo compartido, seleccione **Paquete implementable del software**.</span><span class="sxs-lookup"><span data-stu-id="6022d-115">In the Shared asset library, select **Software deployable package**.</span></span>
2. <span data-ttu-id="6022d-116">Descargue la herramienta de reaprovisionamiento del entorno.</span><span class="sxs-lookup"><span data-stu-id="6022d-116">Download the Environment reprovisioning tool.</span></span>
3. <span data-ttu-id="6022d-117">En la biblioteca del activo para su proyecto, seleccione **Paquete implementable del software**.</span><span class="sxs-lookup"><span data-stu-id="6022d-117">In the asset library for your project, select **Software deployable package**.</span></span>
4. <span data-ttu-id="6022d-118">Seleccionar **Nuevo** para crear un paquete nuevo.</span><span class="sxs-lookup"><span data-stu-id="6022d-118">Select **New** to create a new package.</span></span>
5. <span data-ttu-id="6022d-119">Especifique un nombre y descripción para el paquete.</span><span class="sxs-lookup"><span data-stu-id="6022d-119">Enter a name and description for the package.</span></span> <span data-ttu-id="6022d-120">Puede usar **Herramienta de reaprovisionamiento de entorno** como el nombre del paquete.</span><span class="sxs-lookup"><span data-stu-id="6022d-120">You can use **Environment reprovisioning tool** as the package name.</span></span>
6. <span data-ttu-id="6022d-121">Cargue el paquete que ha descargado antes.</span><span class="sxs-lookup"><span data-stu-id="6022d-121">Upload the package that you downloaded earlier.</span></span>
7. <span data-ttu-id="6022d-122">En la página **Detalles del entorno** para su entorno de destino, seleccione **Mantener** > **Aplicar las actualizaciones**.</span><span class="sxs-lookup"><span data-stu-id="6022d-122">On the **Environment details** page for your target environment, select **Maintain** > **Apply updates**.</span></span>
8. <span data-ttu-id="6022d-123">Seleccione la herramienta de reaprovisionamiento del entorno que cargó antes y a continuación seleccione **Aplicar** para aplicar el paquete.</span><span class="sxs-lookup"><span data-stu-id="6022d-123">Select the Environment reprovisioning tool that you uploaded earlier, and then select **Apply** to apply the package.</span></span>
9. <span data-ttu-id="6022d-124">Supervisar el progreso del paquete de implementación.</span><span class="sxs-lookup"><span data-stu-id="6022d-124">Monitor the progress of the package deployment.</span></span> 

<span data-ttu-id="6022d-125">Para más información acerca de cómo aplicar un paquete implementable, consulte [Aplicar un paquete implementable](../deployment/create-apply-deployable-package.md).</span><span class="sxs-lookup"><span data-stu-id="6022d-125">For more information about how to apply a deployable package, see [Apply a deployable package](../deployment/create-apply-deployable-package.md).</span></span> <span data-ttu-id="6022d-126">Para más información acerca de cómo aplicar manualmente un paquete implementable, consulte [Instalar un paquete implementable](../deployment/install-deployable-package.md).</span><span class="sxs-lookup"><span data-stu-id="6022d-126">For more information about how to manually apply a deployable package, see [Install a deployable package](../deployment/install-deployable-package.md).</span></span>