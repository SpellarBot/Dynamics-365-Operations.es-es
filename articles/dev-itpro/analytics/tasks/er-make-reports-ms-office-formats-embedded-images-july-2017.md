--- 
title: "Crear informes en formatos de Microsoft Office con imágenes insertadas para informes electrónicos (ER) (Parte 1)"
description: "En los pasos siguientes se explica cómo un usuario con rol de \"Administrador de sistema\" o \"Desarrollador de informes electrónicos\" puede diseñar configuraciones de informe electrónico (ER) para generar documentos electrónicos en formatos de MS Office (Excel y Word) que contienen imágenes incrustadas."
author: NickSelin
manager: AnnBe
ms.date: 06/13/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 93a40f36e38ef5ea393cf429ad9244b56504bbfc
ms.contentlocale: es-es
ms.lasthandoff: 09/29/2017

---
# <a name="make-reports-in-microsoft-office-formats-with-embedded-images-for-electronic-reporting-er--part-1"></a><span data-ttu-id="8f807-103">Crear informes en formatos de Microsoft Office con imágenes insertadas para informes electrónicos (ER) (Parte 1)</span><span class="sxs-lookup"><span data-stu-id="8f807-103">Make reports in Microsoft Office formats with embedded images for electronic reporting (ER)  (Part 1)</span></span> 

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="8f807-104">En los pasos siguientes se explica cómo un usuario con rol de "Administrador de sistema" o "Desarrollador de informes electrónicos" puede diseñar configuraciones de informe electrónico (ER) para generar documentos electrónicos en formatos de MS Office (Excel y Word) que contienen imágenes incrustadas.</span><span class="sxs-lookup"><span data-stu-id="8f807-104">The following steps explain how a user playing either ‘System administrator’ or ‘Electronic reporting developer’ role can design Electronic reporting (ER) configurations to generate electronic documents in MS office formats (Excel and Word) containing embedded images.</span></span>

<span data-ttu-id="8f807-105">En este ejemplo, usará configuraciones de ER creadas para una empresa de ejemplo "Litware, Inc".</span><span class="sxs-lookup"><span data-stu-id="8f807-105">In this example, you will use created ER configurations for sample company, ‘Litware, Inc.’.</span></span>  <span data-ttu-id="8f807-106">Para completar estos pasos, primero debe completar los pasos de la guía de tareas "ER crea informes en los formatos de MS Office con imágenes incrustadas (Parte 2: Revisar configuraciones)”.</span><span class="sxs-lookup"><span data-stu-id="8f807-106">To complete these steps, you must first complete the steps in the “ER Make reports in MS Office formats with embedded images (Part 2: Review configurations)” task guide.</span></span> <span data-ttu-id="8f807-107">Estos pasos se pueden llevar a cabo en la empresa "USMF".</span><span class="sxs-lookup"><span data-stu-id="8f807-107">These steps can be performed in ‘USMF’ company.</span></span>


## <a name="run-format-with-initial-model-mapping"></a><span data-ttu-id="8f807-108">Ejecutar formato con asignación de modelo inicial</span><span class="sxs-lookup"><span data-stu-id="8f807-108">Run format with initial model mapping</span></span>
1. <span data-ttu-id="8f807-109">Vaya a Gestión de efectivo y de banco > Cuentas bancarias > Cuentas bancarias.</span><span class="sxs-lookup"><span data-stu-id="8f807-109">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
2. <span data-ttu-id="8f807-110">Use un filtro rápido para filtrar por el campo Cuenta bancaria, por el valor ''USMF OPER".</span><span class="sxs-lookup"><span data-stu-id="8f807-110">Use the Quick Filter to filter on the Bank account field with a value of 'USMF OPER'.</span></span>
3. <span data-ttu-id="8f807-111">En el panel de acciones, haga clic en Configurar.</span><span class="sxs-lookup"><span data-stu-id="8f807-111">On the Action Pane, click Set up.</span></span>
4. <span data-ttu-id="8f807-112">Haga clic en Comprobar.</span><span class="sxs-lookup"><span data-stu-id="8f807-112">Click Check.</span></span>
5. <span data-ttu-id="8f807-113">Haga clic en Imprimir prueba.</span><span class="sxs-lookup"><span data-stu-id="8f807-113">Click Print test.</span></span>
    * <span data-ttu-id="8f807-114">Ejecute el formato para probar.</span><span class="sxs-lookup"><span data-stu-id="8f807-114">Run the format for testing purposes.</span></span>  
6. <span data-ttu-id="8f807-115">Seleccione Sí en el campo Formato de cheque negociable.</span><span class="sxs-lookup"><span data-stu-id="8f807-115">Select Yes in the Negotiable check format field.</span></span>
7. <span data-ttu-id="8f807-116">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="8f807-116">Click OK.</span></span>
    * <span data-ttu-id="8f807-117">Revise el resultado creado.</span><span class="sxs-lookup"><span data-stu-id="8f807-117">Review the created output.</span></span> <span data-ttu-id="8f807-118">Tenga en cuenta que el logotipo de la empresa se mostrará en el informe junto con la firma de la persona autorizada.</span><span class="sxs-lookup"><span data-stu-id="8f807-118">Note that the company logo is presented in the report as well as the authorized person’s signature.</span></span> <span data-ttu-id="8f807-119">La imagen de firma se obtiene en el campo del tipo de datos “Contenedor” del registro de diseño de cheques que está asociado a la cuenta bancaria seleccionada.</span><span class="sxs-lookup"><span data-stu-id="8f807-119">The signature image is taken from the field of the ‘Container’ data type of the cheque layout record which is associated with the selected bank account.</span></span>  
8. <span data-ttu-id="8f807-120">Expanda la sección Copias.</span><span class="sxs-lookup"><span data-stu-id="8f807-120">Expand the Copies section.</span></span>
9. <span data-ttu-id="8f807-121">Haga clic en Editar.</span><span class="sxs-lookup"><span data-stu-id="8f807-121">Click Edit.</span></span>
10. <span data-ttu-id="8f807-122">En el campo de marca de agua, introduzca "Imprimir marca de agua como Anulada".</span><span class="sxs-lookup"><span data-stu-id="8f807-122">In the Watermark field, enter 'Print watermark as Void'.</span></span>
    * <span data-ttu-id="8f807-123">Cambie la configuración del diseño de la marca de agua para mostrar el texto de la marca de agua en la generación de documentos en un elemento de forma de Excel.</span><span class="sxs-lookup"><span data-stu-id="8f807-123">Change the watermark layout setting to show the watermark text in generating document in an Excel shape element.</span></span>  
11. <span data-ttu-id="8f807-124">Haga clic en Imprimir prueba.</span><span class="sxs-lookup"><span data-stu-id="8f807-124">Click Print test.</span></span>
12. <span data-ttu-id="8f807-125">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="8f807-125">Click OK.</span></span>
    * <span data-ttu-id="8f807-126">Revise el resultado creado.</span><span class="sxs-lookup"><span data-stu-id="8f807-126">Review the created output.</span></span> <span data-ttu-id="8f807-127">Tenga en cuenta que la marca de agua se mostrará en el informe creado de acuerdo a la opción de selección.</span><span class="sxs-lookup"><span data-stu-id="8f807-127">Note that the watermark is shown in the created report in accordance to the selection option.</span></span>  
13. <span data-ttu-id="8f807-128">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-128">Close the page.</span></span>
14. <span data-ttu-id="8f807-129">En el panel Acción, haga clic en Administrar pagos.</span><span class="sxs-lookup"><span data-stu-id="8f807-129">On the Action Pane, click Manage payments.</span></span>
15. <span data-ttu-id="8f807-130">Haga clic en Cheques.</span><span class="sxs-lookup"><span data-stu-id="8f807-130">Click Checks.</span></span>
16. <span data-ttu-id="8f807-131">Haga clic en Mostrar filtros.</span><span class="sxs-lookup"><span data-stu-id="8f807-131">Click Show filters.</span></span>
17. <span data-ttu-id="8f807-132">Aplique los filtros siguientes: escriba un valor de filtro de "381","385","389" en el campo "Número de cheque” con el operador de filtro “es uno de”.</span><span class="sxs-lookup"><span data-stu-id="8f807-132">Apply the following filters: Enter a filter value of "381","385","389" on the "Check number" field using the "is one of" filter operator.</span></span>
18. <span data-ttu-id="8f807-133">En la lista, marque todas las filas.</span><span class="sxs-lookup"><span data-stu-id="8f807-133">In the list, mark all rows.</span></span>
19. <span data-ttu-id="8f807-134">Haga clic en Imprimir copia de cheque.</span><span class="sxs-lookup"><span data-stu-id="8f807-134">Click Print check copy.</span></span>
    * <span data-ttu-id="8f807-135">Ejecute el formato para reimprimir los cheques seleccionados.</span><span class="sxs-lookup"><span data-stu-id="8f807-135">Run the format to re-print the selected cheques.</span></span>  
    * <span data-ttu-id="8f807-136">Revise el resultado creado.</span><span class="sxs-lookup"><span data-stu-id="8f807-136">Review the created output.</span></span> <span data-ttu-id="8f807-137">Observe que se han vuelto a imprimir los cheques seleccionados.</span><span class="sxs-lookup"><span data-stu-id="8f807-137">Note that the selected cheques have been re-printed.</span></span> <span data-ttu-id="8f807-138">El logotipo de la empresa y las etiquetas no se imprimen ya que se muestran en el formulario preimpreso.</span><span class="sxs-lookup"><span data-stu-id="8f807-138">The company logo and labels are not printed out since they are presented on the pre-printed form.</span></span>  

## <a name="modify-the-mapping-of-the-imported-data-model"></a><span data-ttu-id="8f807-139">Modificar la asignación del modelo de datos importado</span><span class="sxs-lookup"><span data-stu-id="8f807-139">Modify the mapping of the imported data model</span></span>
1. <span data-ttu-id="8f807-140">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-140">Close the page.</span></span>
2. <span data-ttu-id="8f807-141">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-141">Close the page.</span></span>
3. <span data-ttu-id="8f807-142">Vaya a Administración de la organización > Informes electrónicos > Configuraciones.</span><span class="sxs-lookup"><span data-stu-id="8f807-142">Go to Organization administration > Electronic reporting > Configurations.</span></span>
4. <span data-ttu-id="8f807-143">En el árbol, seleccione "Modelo para cheques".</span><span class="sxs-lookup"><span data-stu-id="8f807-143">In the tree, select 'Model for cheques'.</span></span>
5. <span data-ttu-id="8f807-144">Haga clic en Diseñador.</span><span class="sxs-lookup"><span data-stu-id="8f807-144">Click Designer.</span></span>
6. <span data-ttu-id="8f807-145">Haga clic en Asignar modelo a origen de datos.</span><span class="sxs-lookup"><span data-stu-id="8f807-145">Click Map model to datasource.</span></span>
7. <span data-ttu-id="8f807-146">Haga clic en Diseñador.</span><span class="sxs-lookup"><span data-stu-id="8f807-146">Click Designer.</span></span>
    * <span data-ttu-id="8f807-147">Cambiaremos el enlace del elemento de la firma del modelo de datos para obtener la imagen de firma a partir del archivo que se ha adjuntado al registro del diseño de cheques que está asociado a la cuenta bancaria seleccionada.</span><span class="sxs-lookup"><span data-stu-id="8f807-147">We will change the binding of the data model’s signature item to get the signature image from the file that has been attached to the cheque layout record which is associated with the selected bank account.</span></span>  
8. <span data-ttu-id="8f807-148">Desactive Mostrar detalles.</span><span class="sxs-lookup"><span data-stu-id="8f807-148">Turn Show details off.</span></span>
9. <span data-ttu-id="8f807-149">En el árbol, expanda "Diseño".</span><span class="sxs-lookup"><span data-stu-id="8f807-149">In the tree, expand 'layout'.</span></span>
10. <span data-ttu-id="8f807-150">En el árbol, expanda "Diseño\firma".</span><span class="sxs-lookup"><span data-stu-id="8f807-150">In the tree, expand 'layout\signature'.</span></span>
11. <span data-ttu-id="8f807-151">En el árbol, seleccione "diseño\firma\imagen = cuentadecheque."<Relaciones".DiseñoChequeBancario.Firma1Bmp'.</span><span class="sxs-lookup"><span data-stu-id="8f807-151">In the tree, select 'layout\signature\image = chequesaccount.'<Relations'.BankChequeLayout.Signature1Bmp'.</span></span>
12. <span data-ttu-id="8f807-152">En el árbol, expanda "cuentadecheque".</span><span class="sxs-lookup"><span data-stu-id="8f807-152">In the tree, expand 'chequesaccount'.</span></span>
13. <span data-ttu-id="8f807-153">En el árbol, expanda "cuentadecheque\<Relaciones".</span><span class="sxs-lookup"><span data-stu-id="8f807-153">In the tree, expand 'chequesaccount\<Relations'.</span></span>
14. <span data-ttu-id="8f807-154">En el árbol, expanda "cuentadecheque\<Relaciones\DiseñodeChequeBancario".</span><span class="sxs-lookup"><span data-stu-id="8f807-154">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout'.</span></span>
15. <span data-ttu-id="8f807-155">En el árbol, expanda "cuentadecheque\<Relaciones\DiseñodeChequeBancario\<Relaciones".</span><span class="sxs-lookup"><span data-stu-id="8f807-155">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout\<Relations'.</span></span>
16. <span data-ttu-id="8f807-156">En el árbol, expanda "cuentadecheque\<Relaciones\DiseñodeChequeBancario\<Relaciones\<Documentos'.</span><span class="sxs-lookup"><span data-stu-id="8f807-156">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents'.</span></span>
17. <span data-ttu-id="8f807-157">En el árbol, seleccione 'cuentadecheque\<Relaciones\DiseñodeChequeBancario\<Relaciones\<Documentos\obtenerContenidodeArchivocomoContenedor()'.</span><span class="sxs-lookup"><span data-stu-id="8f807-157">In the tree, select 'chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents\getFileContentAsContainer()'.</span></span>
18. <span data-ttu-id="8f807-158">Haga clic en Enlazar.</span><span class="sxs-lookup"><span data-stu-id="8f807-158">Click Bind.</span></span>
19. <span data-ttu-id="8f807-159">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="8f807-159">Click Save.</span></span>
20. <span data-ttu-id="8f807-160">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-160">Close the page.</span></span>
21. <span data-ttu-id="8f807-161">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-161">Close the page.</span></span>
22. <span data-ttu-id="8f807-162">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-162">Close the page.</span></span>
23. <span data-ttu-id="8f807-163">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-163">Close the page.</span></span>

## <a name="run-format-using-the-adjusted-model-mapping"></a><span data-ttu-id="8f807-164">Ejecutar formato con la asignación de modelo ajustado</span><span class="sxs-lookup"><span data-stu-id="8f807-164">Run format using the adjusted model mapping</span></span>
1. <span data-ttu-id="8f807-165">Vaya a Gestión de efectivo y de banco > Cuentas bancarias > Cuentas bancarias.</span><span class="sxs-lookup"><span data-stu-id="8f807-165">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
2. <span data-ttu-id="8f807-166">Use el filtro rápido para buscar registros.</span><span class="sxs-lookup"><span data-stu-id="8f807-166">Use the Quick Filter to find records.</span></span> <span data-ttu-id="8f807-167">Por ejemplo, filtre por el campo Cuenta bancaria, con un valor de 'USMF OPER'.</span><span class="sxs-lookup"><span data-stu-id="8f807-167">For example, filter on the Bank account field with a value of 'USMF OPER'.</span></span>
3. <span data-ttu-id="8f807-168">En el panel de acciones, haga clic en Configurar.</span><span class="sxs-lookup"><span data-stu-id="8f807-168">On the Action Pane, click Set up.</span></span>
4. <span data-ttu-id="8f807-169">Haga clic en Comprobar.</span><span class="sxs-lookup"><span data-stu-id="8f807-169">Click Check.</span></span>
5. <span data-ttu-id="8f807-170">Haga clic en Imprimir prueba.</span><span class="sxs-lookup"><span data-stu-id="8f807-170">Click Print test.</span></span>
6. <span data-ttu-id="8f807-171">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="8f807-171">Click OK.</span></span>
    * <span data-ttu-id="8f807-172">Revise el resultado creado.</span><span class="sxs-lookup"><span data-stu-id="8f807-172">Review the created output.</span></span> <span data-ttu-id="8f807-173">Tenga en cuenta que la imagen de los datos adjuntos de la gestión de documentos se muestra como la firma de una persona autorizada.</span><span class="sxs-lookup"><span data-stu-id="8f807-173">Note that the image from the Document Management attachment is presented as the signature of an authorized person.</span></span>  

## <a name="use-ms-word-document-as-a-template-in-the-imported-format"></a><span data-ttu-id="8f807-174">Use el documento de MS Word como plantilla en el formato importado</span><span class="sxs-lookup"><span data-stu-id="8f807-174">Use MS Word document as a template in the imported format</span></span>
1. <span data-ttu-id="8f807-175">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-175">Close the page.</span></span>
2. <span data-ttu-id="8f807-176">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-176">Close the page.</span></span>
3. <span data-ttu-id="8f807-177">Vaya a Administración de la organización > Informes electrónicos > Configuraciones.</span><span class="sxs-lookup"><span data-stu-id="8f807-177">Go to Organization administration > Electronic reporting > Configurations.</span></span>
4. <span data-ttu-id="8f807-178">En el árbol, expanda "Modelo para cheques".</span><span class="sxs-lookup"><span data-stu-id="8f807-178">In the tree, expand 'Model for cheques'.</span></span>
5. <span data-ttu-id="8f807-179">En el árbol, seleccione "Modelo para cheques\Formato de impresión de cheques".</span><span class="sxs-lookup"><span data-stu-id="8f807-179">In the tree, select 'Model for cheques\Cheques printing format'.</span></span>
6. <span data-ttu-id="8f807-180">Haga clic en Diseñador.</span><span class="sxs-lookup"><span data-stu-id="8f807-180">Click Designer.</span></span>
7. <span data-ttu-id="8f807-181">Haga clic en Archivos adjuntos.</span><span class="sxs-lookup"><span data-stu-id="8f807-181">Click Attachments.</span></span>
8. <span data-ttu-id="8f807-182">Haga clic Eliminar.</span><span class="sxs-lookup"><span data-stu-id="8f807-182">Click Delete.</span></span>
9. <span data-ttu-id="8f807-183">Haga clic en Sí.</span><span class="sxs-lookup"><span data-stu-id="8f807-183">Click Yes.</span></span>
10. <span data-ttu-id="8f807-184">Haga clic en Nuevo.</span><span class="sxs-lookup"><span data-stu-id="8f807-184">Click New.</span></span>
11. <span data-ttu-id="8f807-185">Haga clic en Archivo.</span><span class="sxs-lookup"><span data-stu-id="8f807-185">Click File.</span></span>
    * <span data-ttu-id="8f807-186">Haga clic en Examinar y seleccione el archivo “Cheque template Word.docx" descargado previamente.</span><span class="sxs-lookup"><span data-stu-id="8f807-186">Click Browse and select the downloaded in advance ‘Cheque template Word.docx’ file.</span></span>  
12. <span data-ttu-id="8f807-187">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-187">Close the page.</span></span>
13. <span data-ttu-id="8f807-188">En el campo Plantilla, especifique o seleccione un valor.</span><span class="sxs-lookup"><span data-stu-id="8f807-188">In the Template field, enter or select a value.</span></span>
14. <span data-ttu-id="8f807-189">Haga clic en Guardar.</span><span class="sxs-lookup"><span data-stu-id="8f807-189">Click Save.</span></span>
15. <span data-ttu-id="8f807-190">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-190">Close the page.</span></span>
16. <span data-ttu-id="8f807-191">Haga clic en Editar.</span><span class="sxs-lookup"><span data-stu-id="8f807-191">Click Edit.</span></span>
17. <span data-ttu-id="8f807-192">Seleccione Sí en el campo Borrador de ejecución.</span><span class="sxs-lookup"><span data-stu-id="8f807-192">Select Yes in the Run Draft field.</span></span>
18. <span data-ttu-id="8f807-193">Cierre la página.</span><span class="sxs-lookup"><span data-stu-id="8f807-193">Close the page.</span></span>
19. <span data-ttu-id="8f807-194">Vaya a Gestión de efectivo y de banco > Cuentas bancarias > Cuentas bancarias.</span><span class="sxs-lookup"><span data-stu-id="8f807-194">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
20. <span data-ttu-id="8f807-195">Use un filtro rápido para filtrar por el campo Cuenta bancaria, por el valor ''USMF OPER".</span><span class="sxs-lookup"><span data-stu-id="8f807-195">Use the Quick Filter to filter on the Bank account field with a value of 'USMF OPER'.</span></span>
21. <span data-ttu-id="8f807-196">Haga clic en Comprobar.</span><span class="sxs-lookup"><span data-stu-id="8f807-196">Click Check.</span></span>
22. <span data-ttu-id="8f807-197">Haga clic en Imprimir prueba.</span><span class="sxs-lookup"><span data-stu-id="8f807-197">Click Print test.</span></span>
23. <span data-ttu-id="8f807-198">Haga clic en Aceptar</span><span class="sxs-lookup"><span data-stu-id="8f807-198">Click OK.</span></span>
    * <span data-ttu-id="8f807-199">Revise el resultado creado.</span><span class="sxs-lookup"><span data-stu-id="8f807-199">Review the created output.</span></span> <span data-ttu-id="8f807-200">Tenga en cuenta que el resultado se ha generado como documento de MS Word con las imágenes incrustadas que presentan el logotipo de la empresa, la firma de una persona autorizada y el texto seleccionado de la marca de agua.</span><span class="sxs-lookup"><span data-stu-id="8f807-200">Note that the output has been generated as a MS Word document with embedded images presenting the company logo, the signature of an authorized person and the selected text of the watermark.</span></span>  

