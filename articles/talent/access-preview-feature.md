---
title: Obtener acceso a las características de vista previa de Talent
description: Este tema describe cómo un administrador puede habilitar las características de vista previa, y enumera las características que se habilitan actualmente para la vista previa.
author: andreabichsel
manager: AnnBe
ms.date: 04/17/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Talent, Core
ms.custom: 7521
ms.assetid: 3b953d5f-6325-4c9e-8b9b-6ab0458a73f8
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2018-04-30
ms.dyn365.ops.version: AX 7.1.0, Talent April 2018 update
ms.openlocfilehash: 060a36185641d5bb7912631b7c857c5c4331c8b7
ms.sourcegitcommit: 608e68b603afef9eb98d8fb25e90109c2473ef87
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "856333"
---
# <a name="access-preview-features-in-talent"></a>Obtener acceso a las características de vista previa de Talent

[!include[banner](../includes/banner.md)]

Como parte de nuestro desarrollo continuo de las capacidades del producto, deseamos que los clientes experimenten las nuevas características lo más rápidamente posible. Los administradores pueden ver y utilizar características de vista previa en los entornos. Estas características casi están preparadas para la disponibilidad general y han pasado por un amplio proceso de pruebas. Simplemente estamos buscando una ronda final de comentarios de clientes y de validación antes de que las lancemos al mercado en general.

Este tema describe cómo un administrador puede habilitar las características de vista previa, y enumera las características que están habilitadas actualmente para la vista previa. Esta lista se actualizará a medida que se pongan nuevas características a disposición de todos y a medida que se lancen nuevas características para probarlas previamente. No se da ninguna notificación cuando las nuevas características se lanzan para obtener una vista previa. Los usuarios solo comenzarán a ver las características.

## <a name="enable-or-disable-preview-features"></a>Habilitar o deshabilitar las funciones de vista previa

Puede usar la configuración **Funciones de vista previa** del centro de gestión de Microsoft Dynamics 365 for Talent para habilitar o deshabilitar las características de vista previa. De forma predeterminada, la configuración está desactivada. La acción de habilitar o deshabilitar las características de vista previa es específica del entorno.

> [!IMPORTANT]
> Si activa la configuración **Funciones de vista previa** , habilita las características de vista preliminar para todos los usuarios de la organización que se encuentran en dicho entorno. Si desactiva la configuración, deshabilita las características de vista previa y hace que no sean accesibles a los usuarios. Las funciones de vista previa tienen compatibilidad limitada en Talent. Es posible que apliquen menos medidas de privacidad y de seguridad, y no se incluyen en el contrato de nivel de servicio de Talent. No debe utilizar características de vista preliminar para procesar datos personales (es decir, toda información que pueda identificarle), o para procesar otros datos sujetos a requisitos de conformidad legales o administrativos.

### <a name="enable-or-disable-preview-features-for-your-organization"></a>Habilitar o deshabilitar funciones de vista preliminar para su organización

#### <a name="attract"></a>Atraer

1. Iniciar sesión en Microsoft Dynamics 365 for Talent: Attract.
2. En el menú **Configuración** (el símbolo de engranaje) en la esquina superior derecha, seleccione **Configuración de administrador**.
3. En la pestaña **Administración de características** , seleccione la opción que está al lado de **Características de vista previa** para que se vuelva azul.
4. Puede controlar opcionalmente funciones individuales habilitando o deshabilitando características específicas en esta página.
5. Actualice al explorador para empezar a ver las nuevas características. (Cualquier usuario que ya haya iniciado sesión verá las características la siguiente vez que inicie sesión, o puede actualizar al explorador para ver las características inmediatamente.)

#### <a name="core-hr"></a>Core HR

1. Inicie sesión en Talent. El espacio de trabajo de recursos humanos básico se abrirá. En él podrá completar los pasos restantes. 
2. Seleccione **Administración del sistema \> Parámetros del sistema de enlaces**.
3. En la **Página de los parámetros del sistema**, en la pestaña **Funciones de vista previa**, establezca la opción **Habilitar modo de vista previa para todos los usuarios** en **Sí** para que las características de vista previa estén disponibles.

> [!NOTE]
> Para deshabilitar las características de vista previa, siga los mismos pasos básicos. Cuando deshabilita las características de vista previa, estas se vuelven inaccesibles para sus usuarios, y pueden producirse errores en los procesos asociados a las características.

## <a name="features-that-are-currently-in-preview"></a>Características que están actualmente en vista previa

### <a name="attract"></a>Atraer

- **Candidatos relevantes en un trabajo** los reclutadores y los administradores de contratación pueden ver fácilmente qué candidatos pueden ser los más relevantes para el trabajo entre todos los candidatos. Se muestran los 5 candidatos más aptos en función de la relevancia de su currículum/perfil en relación con la descripción del trabajo.
- **Trabajos relevantes** Ahora los candidatos ven una lista de otros trabajos que son relevantes para ellos en función de su currículum/perfil y las descripciones de trabajo.  Esto se muestra actualmente a los candidatos una vez que aplican una sugerencia para otras oportunidades.
- **Compatibilidad de EEO/OFCCP** Los nuevos tipos de actividad habilitan el uso de un formulario predefinido para la recopilación de Oportunidad de Igualdad de Empleo (EEO) y los datos de la Oficina de Programas de Cumplimiento de Contratos Federales (OFCCP) del candidato.  Este es un formulario predefinido y no es editable.

    > [!NOTE]
    > Los trabajos que se registran son visibles solo para los clientes que se suscriben a uno o más productos de la lista de trabajos de LinkedIn. De lo contrario, los clientes ven un trabajo solo si lo buscan explícitamente. Hay un retraso cuando los trabajos se envían a LinkedIn. Un trabajo puede tardar algunas horas en aparecer después de que haya enviado publicado desde Attract.

- **Aplicación de candidato** Los candidatos internos y externos podrán presentarse directamente desde la página de trabajo en el sitio de Proyectos profesionales.
- **Administración de la propuesta** – Los usuarios podrán crear cartas a partir de plantillas que incluyen marcadores de posición. A medida que los candidatos avanzan a la etapa de propuesta, los reclutadores y los administradores de contratación pueden usar la herramienta de oferta para preparar la propuesta formal de un candidato a través de plantillas, enviar la propuesta para la aprobación interna y, finalmente, enviar la oferta al candidato para la firma. Se agregarán muchas nuevas capacidades a la herramienta de la propuesta a medida que se avance, y la función de vista previa se actualizará con estas capacidades cuando estemos listos para lanzarlas al mercado para obtener una vista previa.

### <a name="core-hr"></a>Core HR

- **Inscripción abierta** La inscripción abierta a las prestaciones da a los empleados una experiencia simple, de autoservicio, para seleccionar sus prestaciones. Los administradores de Recursos humanos (HR) pueden configurar el proceso de inscripción de prestaciones abierto de su organización, y la experiencia de inscripción de los empleados, mediante una solución orientada fácil de seguir.

## <a name="feedback"></a>Realimentación

Independientemente de si los comentarios son positivos o negativos, deseamos que nos haga llegar sus comentarios sobre el uso de las características de la vista previa. Recomendamos que publique con regularidad sus comentarios en los sitios siguientes cuando use estas características u otras.

- [Comunidad](https://community.dynamics.com/enterprise/f/759?pi53869=0&category=Talent) – Este sitio es un gran recurso en el que los usuarios pueden discutir los casos de uso, hacer preguntas, y obtener ayuda de la comunidad.
- Use los sitios siguientes para sugerir ideas de producto. Infórmenos sobre las características que desea ver en el producto, así como los cambios que crea que deben realizarse en las características existentes.

    - [Atraer ideas](https://powerusers.microsoft.com/t5/Ideas-for-Attract/idb-p/Attract)
    - [Core HR](https://powerusers.microsoft.com/t5/Ideas-for-Human-Resources/idb-p/HumanResources)

No incluya los datos personales (información que podría identificarlo) en los envíos de comentarios o de revisión del producto. La información que se obtiene se puede analizar más, pero no se usará para responder a solicitudes, de acuerdo con las leyes aplicables de privacidad. La información personal obtenida por separado en estos programas está sujeta a la [Declaración de privacidad de Microsoft](https://privacy.microsoft.com/privacystatement).

> [!TIP]
> Marque este tema, y consúltelo a menudo para mantenerse actualizado sobre características nuevas de vista previa a medida que las lanzamos al mercado.
