---
title: Crear, aprobar y publicar trabajos en Attract
description: "Este tema describe los elementos de un trabajo en Attract. También se explica cómo crear un trabajo."
author: josaw
manager: AnnBe
ms.date: 12/21/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-365-talent
ms.technology: 
ms.search.form: 
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent, Core
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.search.industry: 
ms.author: josaw
ms.search.validFrom: 2018-10-24
ms.dyn365.ops.version: Talent October 2018 update
ms.translationtype: HT
ms.sourcegitcommit: 95031534c43dc0578e258bc3e5376c429d72b0ab
ms.openlocfilehash: 6c5daa4050d63303f1ac10c24901e5b1182cb62b
ms.contentlocale: es-es
ms.lasthandoff: 12/23/2018

---

# <a name="create-approve-and-post-jobs-in-attract"></a>Crear, aprobar y publicar trabajos en Attract

[!include [banner](includes/banner.md)]

Este tema describe los elementos de un trabajo en Microsoft Dynamics 365 for Talent: Attract. También se explica cómo crear un trabajo.

## <a name="job-creation"></a>Creación de trabajos

Las administraciones, los reclutadores, y los administradores de contratación pueden crear trabajos. Al crear un trabajo, se le pedirá que seleccione su rol en el proceso: administrador o reclutador de contratación. Tras seleccionar un rol, se le pedirá que seleccione una plantilla de proceso. Si selecciona **Omitir**, se usa la plantilla predeterminada. Para obtener más información acerca de las plantillas de proceso, consulte [Crear una plantilla de proceso en Attract](./process-templates-attract.md).

Un trabajo en Attract tiene detalles del trabajo, un equipo de contratación, un proceso de contratación, propuestas de empleo, y análisis.

## <a name="job-details"></a>Detalles del trabajo

La pestaña **Detalles del trabajo** contiene detalles sobre las responsabilidades y los atributos de trabajo. Los campos para el puesto, la descripción, y la ubicación del trabajo son necesarios. Los demás campos son opcionales.

De forma predeterminada, el campo **Número de vacantes** se establece en **1**. Sin embargo, se puede cambiar este valor. Cuando una oferta se ha preparado para un trabajo, el valor del campo **Número de vacantes disponibles** disminuye.

Si se ha activado la gestión del puesto en el Centro de administración, la búsqueda **Actualizar puestos** está disponible. Esta búsqueda lee la entidad JobPosition en el Common Data Service para las aplicaciones y devuelve una lista de puestos que se pueden seleccionar para el trabajo. Si el número de puestos que selecciona supera el número de puestos vacantes, se mostrará una advertencia. También recibe una advertencia si un puesto se utiliza en varios trabajos.

> [!NOTE]
> La gestión de puestos está disponible con el complemento de contratación completa.

En función de los valores de la actividad de la oferta del proceso de contratación, se puede usar dos veces un número de puesto en una oferta. Para obtener más información, consulte [Proceso de contratación](./activities-attract.md).

Attract incluye un conjunto predeterminado de **Aptitudes**. Estas aptitudes se muestran como sugerencias a medida que escribe. Puede agregar más aptitudes especificando el nuevo texto de aptitud en el campo y después presionando Intro.

Attract incluye un conjunto predeterminado de **Funciones de trabajo**. Puede agregar hasta tres funciones de trabajo más especificando la nueva función de trabajo en el campo y después presionando Intro.

Attract incluye un conjunto predeterminado de **Sector de la empresa**. Puede agregar hasta tres sectores de empresas más especificando el nuevo sector de empresa en el campo y después presionando Intro.

## <a name="hiring-team"></a>Equipo de contratación

La pestaña **Equipo de contratación** contiene la lista de personas que están implicadas en el trabajo. Cuando se agregan usuarios a un equipo de contratación, deben asignárseles un rol en el equipo de contratación. El rol determina los datos a los que los usuarios tienen acceso y las notificaciones que reciben. Los roles que se pueden seleccionar son **Reclutador**, **Administrador de contratación**, **delegado**, y **Entrevistador**. Para más información sobre los privilegios de los roles, consulte la documentación "Administración de roles". Los reclutadores y los administradores de contratación pueden designar uno o más delegados para trabajar en su nombre. Para obtener más información sobre los delegados, consulte [La seguridad y la gestión de roles en Attract](./security-attract.md).

El equipo de contratación se puede actualizar después de activar el trabajo.

## <a name="process"></a>Proceso

La información predeterminada sobre el proceso de contratación se basa en la plantilla de proceso que se activó cuando el trabajo se creó. Si una plantilla específica no se activó en ese momento, se usa la plantilla predeterminada. Al definir el proceso de contratación, puede agregar o quitar las distintas etapas, salvo las etapas Cliente potencial, Solicitud y Oferta. Aunque la etapa de cliente potencial no se pueda quitar, puede desactivarse. Dentro de cada etapa, puede agregar o quitar una o varias actividades predefinidas.

Para obtener más información sobre las actividades que se pueden agregar al proceso de contratación, consulte [Actividades de proceso de contratación en Attract](./activities-attract.md).

> [!NOTE]
> El proceso de contratación no se puede actualizar después de activar el trabajo.

## <a name="postings"></a>Registros

Después de que se active un trabajo, este se puede registrar. Solo los reclutadores y los administradores pueden registrar trabajos. El trabajo se puede registrar en Talent Careers (un sitio de carreras de Microsoft Dynamics 365 for Talent) o LinkedIn. 

> [!NOTE]
> Existen tres elementos importantes que hay que tener en cuenta sobre el proceso de oferta de empleo en LinkedIn.
> 1. Los trabajos enviados a LinkedIn se registran como trabajos de "listas limitadas”. Los trabajos de listas limitadas no se pueden promocionar por todo el sitio de LinkedIn. Si desea promocionar trabajos de listas limitadas enviados a LinkedIn desde Attract, debe trabajar con LinkedIn para habilitar el “ajuste de trabajo”. Consulte los vínculos siguientes y póngase en contacto con el soporte de LinkedIn para obtener más detalles.
>
>    [Listas limitadas y registros de trabajos premium para el ajuste de trabajo](https://www.linkedin.com/help/recruiter/answer/79049/limited-listings-vs-premium-job-slots-for-job-wrapping)
>
>    [Preguntas más frecuentes de ajuste de trabajo](https://www.linkedin.com/help/recruiter/answer/79050/job-wrapping-frequently-asked-questions)
>
> 1. Al registrar trabajos en LinkedIn, Attract pasa el nombre de la organización Microsoft 365 con el trabajo. LinkedIn vincula los trabajos a una empresa en el lado de LinkedIn basándose en el nombre de la organización que se pasa. Si su trabajo se muestra con la empresa errónea en LinkedIn, compruebe que su nombre de la organización de Microsoft 365 coincide con el nombre de la empresa en LinkedIn.  
>
>    [Cambio de dirección de contacto y más](https://docs.microsoft.com/en-us/office365/admin/manage/change-address-contact-and-more)
>
>    Si tiene problemas después de que este paso, contacte con el soporte de LinkedIn. 
> 
> 1. Puede tardar hasta 24 horas que los trabajos enviados a LinkedIn estén visibles para candidatos de dentro de LinkedIn, como consecuencia del proceso de registro actual de trabajos por lotes de LinkedIn.

El equipo de Attract trabaja continuamente para asociarse con los agregadores tableros de trabajo. Esta lista se expandirá con el tiempo.

Para obtener más información acerca de registros de trabajo, consulte [La funcionalidad del sitio de carreras en Attract](./career-site.md).

> [!NOTE]
> La funcionalidad de registro de trabajo está disponible únicamente con el complemento de contratación completa de Attract.

## <a name="activate"></a>Activar

Después de que se active un trabajo, este se puede registrar, y se le pueden agregar los clientes potenciales y los candidatos. La opción para agregar clientes potenciales a un trabajo se establece en la actividad del cliente potencial en el proceso de contratación.

> [!NOTE]
> El proceso de contratación no se puede actualizar después de activar el trabajo.

## <a name="prospects-and-applicants"></a>Clientes potenciales y candidatos

La opción para agregar clientes potenciales a un trabajo se establece en la [Actividad del cliente potencial](./activities-attract.md#prospect-activity) en el proceso de contratación. Esta opción debe ser establecida antes de activar el trabajo. Después de que se active un trabajo, se le pueden agregar los clientes potenciales y los candidatos.

## <a name="approvals"></a>Aprobaciones

Los trabajos de Attract pueden ser enviados para su aprobación. No todos los trabajos requieren aprobación. El requisito se establece en el nivel de la plantilla. De forma predeterminada, las aprobaciones se desactivan en la plantilla. Para configurar aprobaciones, vaya a una plantilla de proceso, y establezca el campo **Aprobación** en Valor predeterminado. A continuación seleccione dicha plantilla al crear el trabajo.

Una vez guardado un trabajo, puede ser enviado para su aprobación. En la tabla siguiente se muestran los estados de un documento que utiliza aprobaciones.

| Estado   | Comunidad autónoma                                                               |
|----------|---------------------------------------------------------------------|
| Borrador    | Se ha guardado el trabajo, pero no se ha enviado a un flujo de trabajo. |
| Pendientes  | El trabajo se envió a aprobadores.                            |
| Aprobados | Se ha aprobado el trabajo, pero no se ha activado.            |
| Rechazados | Se ha rechazado el trabajo, y no se puede activar.               |
| Activas   | Se ha aprobado y se ha activado el trabajo.                            |

En la lista de trabajos, puede filtrar por los estados de trabajo.

Las aprobaciones se pueden enviar a cualquier usuario de Microsoft Azure Active Directory (Azure AD) de la empresa. Las aprobaciones se envían en paralelo a todas las personas que aparecen como aprobadores. Después de que se apruebe un trabajo, este se puede activar.

Las personas que figuran como aprobadores recibirán una notificación en Attract para informarles de que tienen un elemento por aprobar. También aparecerá un elemento de aprobación en la sección **Asignadas a usted** en el panel. Una vez que alguien acepte o aprueebe un trabajo, el equipo de contratación recibirá una notificación. Finalmente, el equipo de contratación recibirá una notificación cuando se apruebe el trabajo.

## <a name="create-a-job"></a>Creación de un trabajo

Siga estos pasos para crear un trabajo.

1. Vaya a **Trabajos**.
2. Seleccione **Nuevo**.
3. En el campo **Cargo**, especifique el puesto. En el campo **Rol**, escriba su rol.
4. En el campo **Plantilla**, seleccione una plantilla. De forma alternativa, seleccione **Omitir**. Si se selecciona **Omitir**, la plantilla se usará la plantilla marcada como predeterminada.

    Si el documento pasa con un proceso de aprobación, seleccione una plantilla donde el campo **Proceso de aprobación** se establece en **Predeterminado**.

5. En la ficha **Detalles**, especifique la información detallada del trabajo. Los campos **Título**, **Descripción del trabajo** y **Ubicación** son necesarios.
6. Seleccione **Guardar**.
7. En la pestaña **Equipo de contratación**, agregue un administrador, un reclutador, o un entrevistador de contratación.
8. Seleccione **Guardar**.
9. En la pestaña **proceso**, agregue o quite etapas como sea necesario:

    - Para agregar una etapa, seleccione **+ Nueva etapa**.
    - Para quitar una etapa, mantenga el puntero del mouse sobre la etapa que desea quitar, y seleccione el botón de papelera que aparece.

        > [!NOTE]
        > Las etapas de candidatos potenciales, solicitud u oferta no se pueden eliminar.

10. Agregue o quite actividades como sea necesario:

    - Para agregar una actividad, arrástrela desde la lista de la derecha a la etapa adecuada. De forma alternativa, haga doble clic en la actividad, y luego seleccione la etapa a la que la agregará.
    - Para quitar una actividad, expanda la actividad, y seleccione el botón de papelera en el encabezado de la actividad.

11. Seleccione **Guardar**.
12. Si ha seleccionado usar un proceso de aprobación, siga estos pasos:

    1. Seleccione **+ Agregar aprobador**y, a continuación, especifique un usuario que tenga una cuenta Azure AD. Puede agregar varios aprobadores.
    2. Seleccione **Enviar a aprobadores**.

    El campo **Estado del trabajo** del trabajo se establece en **Pendiente**. Una vez que el valor de **Estado del trabajo** cambia a **Aprobado**, el trabajo se puede activar.

13. Para activar el trabajo, seleccione **Activar**.
14. Para registrar el trabajo, vaya a **Registros** y, a continuación, seleccione **Registrar ahora** en el sitio de carreras de Talent o en LinkedIn.
