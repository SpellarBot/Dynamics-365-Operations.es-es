---
title: Informes de gastos y varios aprobadores
description: En este tema se proporciona información sobre los informes de gastos que requieren la aprobación de más de una persona.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1483de5405895d60f0cb302ab622758b2b05d2ca
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "362427"
---
# <a name="expense-reports-and-multiple-approvers"></a>Informes de gastos y varios aprobadores

[!include [banner](../includes/banner.md)]

En función de las directivas de aprobación de gastos de su organización, puede que más de una persona tenga que aprobar un informe de gastos que haya enviado un empleado. Cuando configura el proceso de flujo de trabajo para la aprobación del informe de gastos, puede agregar elementos de flujo de trabajo que incluyan las tareas o los pasos para uno o varios aprobadores del informe de gastos. Por ejemplo, puede solicitar que todos los informes de gastos los apruebe en primer lugar el director del empleado que envió el informe y, a continuación, el coordinador de proveedores.

Si decide solicitar varios aprobadores del informe de gastos, puede agregar elementos de flujo de trabajo de una de las siguientes formas:

- Agregue un elemento de aprobación que tenga un paso. Por ejemplo, el paso puede requerir que un informe de gastos se asigne a un grupo de usuarios y que lo apruebe el 50 por ciento de los miembros del grupo de usuarios.
- Agregue un elemento de aprobación que tenga varios pasos. Por ejemplo, el elemento de aprobación puede tener los siguientes pasos:

    1. El director del empleado que envió el informe de gastos lo aprueba.
    2. El funcionario de proveedores comprueba las recepciones y los artículos del informe de gastos.
    3. El propietario de presupuesto aprueba el informe de gastos.

- Agregue varios elementos de aprobación, cada uno que tenga un paso. Por ejemplo, puede agregar un elemento de aprobación individual para cada uno de los siguientes pasos:

    1. El director del empleado aprueba el informe de gastos.
    2. El propietario de presupuesto aprueba el informe de gastos.
