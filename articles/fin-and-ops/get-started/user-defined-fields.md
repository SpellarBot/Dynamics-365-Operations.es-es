---
title: Crear y trabajar con campos personalizados
description: Este tema muestra cómo Microsoft Dynamics 365 for Finance and Operations permite a algunos usuarios crear campos personalizados para adaptar la aplicación para que se ajuste a su negocio.
author: jasongre
manager: AnnBe
ms.date: 07/16/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: SysCustomFieldManageFields
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: jasongre
ms.search.validFrom: 2018-1-31
ms.dyn365.ops.version: Platform update 13
ms.openlocfilehash: 18402579789c17de7b46dd7a013b3b6327ea5d4f
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "348029"
---
# <a name="create-and-work-with-custom-fields"></a>Crear y trabajar con campos personalizados

[!include [banner](../includes/banner.md)]

Aunque Microsoft Dynamics 365 for Finance and Operations proporciona un amplio conjunto de campos disponibles de inmediato para gestionar una amplia gama de procesos empresariales, algunas veces es necesaria una empresa que realice un seguimiento de la información adicional en el sistema. Para tener en cuenta esta necesidad, Finance and Operations le permite crear campos personalizados para adaptar la aplicación para que se ajuste a su negocio, siempre que disponga de permisos para la característica.

La capacidad de agregar campos personalizados está disponible en la actualización de plataforma 13 y versiones posteriores.

Este vídeo muestra lo sencillo que es agregar un campo personalizado a una página: [Cómo agregar campos personalizados en Dynamics 365 for Finance and Operations](https://www.youtube.com/watch?v=gWSGZI9Vtnc).

## <a name="creating-custom-fields"></a>Crear campos personalizados

Una vez identificada la información adicional cuyo seguimiento desea realizar en la aplicación, puede crear el campo personalizado en la tabla apropiada y exponer ese campo nuevo en una página.

Los siguientes pasos describen el proceso para crear un campo personalizado y colocar ese campo en un formulario.

1. Vaya al formulario en el que es necesario el nuevo campo.
2. Puesto que el objetivo final es exponer el campo personalizado en un formulario, el punto de entrada para crear campos personalizados existe dentro de la experiencia de personalización. Abra la barra de herramientas de personalización seleccionando **Opciones** y, a continuación, **Personalizar este formulario**.
3. Haga click en **Insertar** y, a continuación, en **Campo**.
4. Seleccione la región del formulario en la que desea exponer el nuevo campo. Tras la selección, el cuadro de diálogo **Insertar campos** mostrará una lista de campos existentes que se pueden insertar en la región seleccionada del formulario.
5. Asegúrese de que el campo en el que está interesado no existe en la lista. Si existe, simplemente puede seleccionar ese campo en la lista y hacer clic en **Insertar**.
6. Haga clic en el botón **Crear nuevo campo** encima de la lista para iniciar el proceso de crear un campo personalizado. Se abrirá el cuadro de diálogo **Crear nuevo campo**.

    Si no ve el botón **Crear nuevo campo**, no dispone de los permisos necesarios para usar esta función.

7. En el cuadro de diálogo **Crear nuevo campo**, especifique la siguiente información.

    1. Seleccione la tabla de la base de datos si debe agregarse este campo. Tenga en cuenta que solo aparecerán las tablas personalizadas compatibles en la lista desplegable. Consulte la siguiente sección para obtener detalles técnicos sobre las tablas compatibles.
    2. Seleccione el tipo de datos para el nuevo campo. Los tipos de datos disponibles son casilla de verificación, fecha, fecha y hora, decimal, número, lista de selección y texto.

        - Si elige el tipo de datos del texto, también puede especificar la longitud máxima del texto que se puede especificar en este campo.
        - Si elige el tipo de datos de la lista de selección, también puede seleccionar el conjunto de valores válidos para el campo.

    3. Proporcione un nombre, una etiqueta y un texto de ayuda para el campo. El nombre corresponde al nombre de campo físico en la base de datos, mientras que la etiqueta y el texto de ayuda son el texto utilizado para representar este campo en la interfaz de usuario.

8. Si este es el único campo que necesita crear para este formulario, haga clic en **Guardar**. Si necesita crear campos adicionales, haga clic en **Guardar y nuevo** y vuelva al paso 7. Tenga en cuenta que actualmente hay un límite de **20 campos personalizados por tabla**.
9. Dejar el cuadro de diálogo **Crear nuevo campo** le devolverá al cuadro de diálogo **Insertar campos** . Cualquier campo personalizado recién agreado se marcará automáticamente en la lista de campos que se insertará en el formulario.
10. Haga clic en **Insertar** para insertar los campos marcados en la región seleccionada del formulario.
11. **Opcional:** habilite el modo **Mover** de la barra de herramientas de personalización para mover los campos nuevos a su ubicación deseada en la región seleccionada. Consulte [Personalizar la experiencia del usuario](personalize-user-experience.md) para obtener más información sobre cómo usar las diversas capacidades de personalización para optimizar un formulario para su uso personal.

## <a name="sharing-custom-fields-with-other-users"></a>Compartir campos personalizados con otros usuarios

Después de crear un campo personalizado y exponerlo en un formulario, puede que desee proporcionar esta vista de página actualizada que incluye el nuevo campo a otros usuarios en el sistema. Esto se puede realizar de dos formas distintas mediante las capacidades de personalización de producto:

- La ruta recomendada es a través del administrador del sistema, que puede insertar una personalización a todos los usuarios o un subconjunto de usuarios. Consulte [Personalizar la experiencia del usuario](personalize-user-experience.md) para obtener más detalles.
- Como alternativa, puede exportar los cambios (llamados *personalizaciones*), enviarlos a uno o varios usuarios y hacer que cada uno de estos usuarios importe los cambios. La opción **Gestionar** en la barra de herramientas de personalización le permite exportar e importar personalizaciones.

## <a name="managing-custom-fields"></a>Gestionar campos personalizados

La gestión de todos los campos personalizados en el sistema se puede lograr a través de la página **Campos personalizados** en el módulo de administración del sistema. Esta página permite a los usuarios acceder muchas capacidades, entre las que se incluyen:

- Ver una lista de todos los campos personalizados en el sistema.
- Edición limitada de campos personalizados existentes.
- Eliminar campos personalizados.
- Exponer campos personalizados en entidades de datos.
- Proporcionar traducciones de etiquetas de campo personalizadas y texto de ayuda.

### <a name="viewing-all-custom-fields"></a>Ver todos los campos personalizados

La página **Campos personalizados** proporciona visibilidad a todos los campos personalizados que se han definido en el sistema. Seleccione simplemente la tabla que le interese, y la página se actualizará para mostrar una lista de los campos personalizados asociados a esa tabla. Elegir un campo personalizado de la lista le permitirá ver todos los detalles sobre el campo.

### <a name="editing-custom-fields"></a>Editar campos personalizados

Una vez creado un campo personalizado, solo se pueden modificar determinados fragmentos de información sobre el campo personalizado en la página **Campos personalizados** .

*Puede* modificar estos atributos:

- Etiqueta
- Texto de ayuda
- Longitud, para Campos de texto

*No puede* editar los siguientes atributos:

- Nombre del campo
- Tipo de datos

Además, para los campos de la lista de selección, se puede reordenar el conjunto de valores válidos para el campo personalizado, y se pueden agregar nuevos valores; sin embargo, los valores existentes para el campo de la lista de selección no se pueden eliminar. Recuerde hacer clic en **Aplicar cambios** cuando termine de editar campos para una tabla determinada para que se guarden los cambios.

### <a name="exposing-custom-fields-on-data-entities"></a>Exponer campos personalizados en entidades de datos

También puede ser importante permitir que los campos personalizados estén visibles en entidades de datos. Las entidades de datos se utilizan en la característica [Abrir en Office](../../dev-itpro/office-integration/office-integration.md), así como para los escenarios de importación/exportación de datos.

Siga estos tres pasos para exponer un campo personalizado en una entidad de datos:

1. Seleccione el campo personalizado en el formulario **Campos personalizados** .
2. Expanda la sección **Entidades** para ver el conjunto de entidades relevantes.
3. Haga clic en el botón **Editar**.
4. Modifique el campo **Habilitado** que se va a seleccionar para cada entidad que debe exponer este campo.
5. Haga clic en **Aplicar cambios** para guardar sus selecciones.

### <a name="allowing-custom-fields-to-be-displayed-in-other-languages"></a>Permitir que los campos personalizados se muestren en otros idiomas

Dado que es posible que los usuarios necesiten acceder a una variedad de idiomas, la página **Campos personalizados** proporciona un mecanismo para permitir la etiqueta y el texto de ayuda para que un campo personalizado se traduzca a otros idiomas.

Los siguientes pasos describen el proceso para traducir campos personalizados en otros idiomas:

1. Seleccione el campo personalizado en la página **Campos personalizados** .
2. Seleccione el botón **Traducciones** en el panel de acciones. Se abrirá un menú desplegable con las traducciones existentes para este campo.
3. El menú desplegable **Idioma** muestra el conjunto de idiomas para los que ya se han proporcionado traducciones.

    Si desea editar una traducción existente, seleccione el idioma deseado desde el menú y modifique los valores para la etiqueta y el texto de ayuda.

    De lo contrario, haga clic en el botón **Agregar idioma**, seleccione el idioma deseado desde el menú y, a continuación, proporcione valores traducidos para la etiqueta y el texto de ayuda.

4. Cuando haya terminado, haga clic en **Aceptar**.

### <a name="deleting-custom-fields"></a>Eliminar campos personalizados

En raras ocasiones, puede decidir si un campo personalizado ya no es neceasario. Si esto ocurre, un administrador del sistema puede optar por eliminar el campo de la página **Campos personalizados**. Para ello, asegúrese de que se selecciona el campo correcto, haga clic en **Eliminar**, haga clic en **Sí** para confirmar la eliminación y finalmente haga clic en **Aplicar cambios**.

> [!NOTE]
> Esta acción no se puede deshacer y dará lugar a los datos asociados al campo que se eliminará permanentemente de la base de datos.

## <a name="appendix"></a>Apéndice

### <a name="who-can-create-custom-fields"></a>¿Quién puede crear campos personalizados?

Como elemento de protección para el sistema, solo los administradores del sistema pueden crear campos personalizados de forma predeterminada. Sin embargo, estos usuarios avanzados que la organización considera necesario pueden obtener derechos para crear campos personalizados por un administrador del sistema mediante el rol de seguridad **Usuario avanzado de personalización de tiempo de ejecución**. Los usuarios sin este rol de seguridad no podrán crear campos personalizados, pero si podrán ver e interactuar con los campos personalizados agregados por otros usuarios en el sistema.

### <a name="what-tables-support-custom-fields"></a>¿Qué tablas admiten campos personalizados?

Por motivos rendimiento y técnicos, solo las tablas que cumplen las siguientes condiciones permiten actualmente que se agreguen campos personalizados.

- La tabla debe etiquetarse como uno de estos grupos:

    - Grupo
    - WorksheetHeader
    - Principal
    - Varios
    - Parámetro
    - Referencia
    - TransactionHeader

- La tabla no puede extenderse a otra tabla.
- La tabla no puede marcarse como una tabla del sistema.
- La tabla no puede ser una tabla temporal.
