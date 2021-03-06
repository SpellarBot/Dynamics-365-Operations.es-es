---
title: Contenido de administración de créditos y cobros de Power BI
description: Este tema describe lo que se incluye en el contenido en Power BI de Administración de créditos y cobros. Explica cómo obtener acceso a los informes de Power BI y proporciona información acerca del modelo de datos y las entidades que se utilizan para generar el contenido.
author: ShivamPandey-msft
manager: AnnBe
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustomerCollectionManagerWorkspace
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: a80a180623d1cca77c633f12bcd92a088e089ee5
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "325190"
---
# <a name="credit-and-collections-management-power-bi-content"></a>Contenido de administración de créditos y cobros de Power BI

[!include [banner](../includes/banner.md)]

Este tema describe lo que se incluye en el contenido **Administración de créditos y cobros** de Microsoft Power BI. Explica cómo obtener acceso a los informes Power BI y proporciona información acerca del modelo de datos y las entidades que se utilizan para generar el contenido.

## <a name="overview"></a>Información general

El contenido en Power BI de **Administración de créditos y cobros** se creó para los administradores de créditos y cobros y los empleados de cobros. Proporciona métricas clave de créditos y cobros, como las ventas de los días pendientes, saldos vencidos, exposición crediticia y los clientes que sobrepasan su límite de crédito. Usa datos transaccionales y ofrece las vistas globales de créditos y cobros en todas las empresas. También proporciona un desglose por empresa, grupo de clientes y cliente.

Este contenido en Power BI consta de 10 páginas de informe:

- Dos páginas de visión general (una página para la visión general de créditos y una página para la visión general de cobros)
- Ocho páginas de detalles que proporcionan detalles de las métricas de crédito y de cobros que vienen desglosadas y articuladas en distintas dimensiones

Todos los importes se muestran en la divisa del sistema. Puede establecer la divisa del sistema en la página **Parámetros del sistema** .

De forma predeterminada, se muestran los datos sobre créditos y cobros para la empresa actual. Para ver los datos en todas las empresas, asigne el deber **CustCollectionsBICrossCompany** al rol.

## <a name="accessing-the-power-bi-content"></a>Acceso al contenido de Power BI
El contenido de Power BI **Administración de créditos y cobros** se muestra en el área de trabajo **Crédito y cobros de clientes**.

## <a name="reports-that-are-included-in-the-power-bi-content"></a>Informes que se incluyen en el contenido de Power BI

El contenido en Power BI de **CustCollectionsBICrossCompany** incluye un informe compuesto por un conjunto de métricas. Estas métricas se visualizan como gráficos, mosaicos y tablas. La tabla siguiente proporciona una visión general de las visualizaciones en el contenido de **CustCollectionsBICrossCompany** en Power BI.

| Página de informes                 | Visualización |
|-----------------------------|---------------|
| Visión general de los cobros        | <ul><li>Actividad de cliente vencida</li><li>Clientes sobre límite de crédito</li><li>30 días de DSO</li><li>Casos abiertos</li><li>Promedio de días para cerrar el caso</li><li>Actividades abiertas</li><li>Promedio de días para cerrar las actividades</li><li>Abrir notas de interés</li><li>Abrir cartas de cobro</li><li>Cliente en espera</li><li>Ventas en espera</li><li>Saldos vencidos</li><li>Importes de estado de cobro</li><li>Importes de código de cobro</li><li>Motivo de cancelación</li><li>Saldo vencido por región</li><li>Pagos previstos</li></ul> |
| Visión general de crédito             | <ul><li>Actividad de cliente vencida</li><li>Límite de crédito frente a saldo pendiente</li><li>Cuadrícula de clientes sobre límite de crédito</li><li>Clientes sobre límite de crédito por empresa</li><li>Crédito utilizado frente a límite de crédito total</li><li>Límite de crédito frente a crédito usado por región</li><li>Clientes por clasificación crediticia</li></ul> |
| Límite de crédito                | <ul><li>Límite de crédito</li><li>Detalles de límite de crédito</li><li>Límite de crédito por cliente</li><li>Límite de crédito por grupo de clientes</li><li>Límite de crédito por clasificación crediticia por empresa</li><li>Límite de crédito frente a crédito usado por región</li></ul> |
| Clientes sobre límite de crédito | <ul><li>Clientes sobre límite de crédito</li><li>Detalle de clientes sobre límite de crédito</li><li>Clientes sobre límite de crédito por empresa</li><li>Cliente sobre límite de crédito por grupo de clientes</li><li>Clientes sobre límite de crédito por región</li></ul> |
| Actividad de cliente vencida          | <ul><li>Actividad de cliente vencida</li><li>Detalles sobre cliente vencido</li><li>Cliente vencido por empresa</li><li>Cliente vencido por grupo de clientes</li><li>Cliente vencido por región</li></ul> |
| Saldos vencidos               | <ul><li>Saldos vencidos</li><li>Detalles de saldos vencidos</li><li>Saldos vencidos por empresa</li><li>Saldos vencidos por grupo de clientes</li></ul> |
| Pagos previstos           | <ul><li>Pagos previstos</li><li>Detalles de pagos previstos</li><li>Pagos previstos por empresa</li><li>Pagos previstos por grupo de clientes</li><li>Pagos previstos por región</li></ul> |
| Cancelaciones                  | <ul><li>Cancelaciones por región</li><li>Detalles de las cancelaciones</li><li>Cancelaciones por cuenta principal</li><li>Cancelaciones por empresa</li><li>Cancelaciones por grupo de clientes</li><li>Cancelaciones por región</li></ul> |
| Estado de cobros          | <ul><li>Con conflicto</li><li>Compromiso de pago roto</li><li>Compromiso de pago</li><li>Detalles de estado de cobros</li><li>Importes de estado de cobro</li><li>Casos abiertos</li><li>Actividades abiertas</li></ul> |
| Cartas de cobros         | <ul><li>Importes por código de cobro</li><li>Detalles de importes por código de cobro</li><li>Importe de cartas de cobro por empresa</li><li>Importe de carta de cobro por grupo de clientes</li><li>Importe de carta de cobro por región</li></ul> |

Los gráficos y los iconos en todos estos informes se pueden filtrar y anclar al panel de información. Para obtener más información acerca de cómo filtrar y anclar en Power BI, consulte [Crear y configurar un panel de información](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-4-2-create-configure-dashboards/). También puede usar la funcionalidad subyacente de exportación de datos para exportar los datos subyacente que se resume en una visualización.

## <a name="understanding-the-data-model-and-entities"></a>Comprensión del modelo de datos y de las entidades

Los datos siguientes se usan para rellenar las páginas de informes en el contenido en Power BI de **Administración de crédito y cobros**. Estos datos se representan como medidas agregadas que se realizan en el almacén de la entidad. El almacén de la entidad es una base de datos de Microsoft SQL Server que se optimiza para el análisis. Para obtener más información, consulte [Visión general de la integración de Power BI con el almacén de entidades](../../dev-itpro/analytics/power-bi-integration-entity-store.md).


|                   Entidad                    |      Medidas agregadas clave      |             Origen de datos              |                           Campo                            |                                    Descripción                                     |
|---------------------------------------------|--------------------------------------|--------------------------------------|------------------------------------------------------------|------------------------------------------------------------------------------------|
| CustCollectionsBIActivitiesAverageCloseTime | NumOfActivities, AveragecClosedTime  |            smmActivities             | AverageOfChildren(AverageClosedTime) Count(ActivityNumber) |     El recuento de actividades cerradas y tiempo promedio para cerrar esas actividades.     |
|       CustCollectionsBIActivitiesOpen       |            ActivityNumber            |            smmActivities             |                   Count(ActivityNumber)                    |                           El recuento de las actividades abiertas.                            |
|        CustCollectionsBIAgedBalances        |             AgedBalances             |  CustCollectionsBIAgedBalancesView   |                 Sum(SystemCurrencyBalance)                 |                             La suma de saldos vencidos.                              |
|        CustCollectionsBIBalancesDue         |         SystemCurrencyAmount         |   CustCollectionsBIBalanceDueView    |                 Sum(SystemCurrencyAmount)                  |                           Los importes que vencidos.                            |
|    CustCollectionsBICaseAverageCloseTIme    |  NumOfCases, CaseAverageClosedTime   |      CustCollectionsCaseDetail       | AverageOfChildren(CaseAverageClosedTime) Count(NumOfCases) |        El recuento de casos cerrados y el promedio para cerrar esos casos.        |
|         CustCollectionsBICasesOpen          |                CaseId                |      CustCollectionsCaseDetail       |                       Count(CaseId)                        |                              El recuento de los casos abiertos.                              |
|      CustCollectionsBICollectionLetter      |         CollectionLetterNum          |       CustCollectionLetterJour       |                 Count(CollectionLetterNum)                 |                       El recuento de cartas de cobro abiertas.                        |
|   CustCollectionsBICollectionLetterAmount   |       CollectionLetterAmounts        | CustCollectionsBIAccountsReceivables |                 Sum(SystemCurrencyAmount)                  |                     El saldo de cartas de cobro registradas.                      |
|      CustCollectionsBICollectionStatus      |       CollectionStatusAmounts        | CustCollectionsBIAccountsReceivables |                 Sum(SystemCurrencyAmount)                  |                El saldo de las transacciones con estado de cobro.                 |
|           CustCollectionsBICredit           | CreditExposed, AmountOverCreditLimit |     CustCollectionsBICreditView      |       Sum(CreditExposed), Sum(AmountOverCreditLimit)       | La suma de exposición crediticia y los importes que los clientes que superan su límite de crédito. |
|         CustCollectionsBICustOnHold         |               Bloqueado                |      CustCollectionsBICustTable      |                       Count(Blocked)                       |                     El número de clientes que están en espera.                      |
|            CustCollectionsBIDSO             |                DSO30                 |       CustCollectionsBIDSOView       |                  AverageOfChildren(DSO30)                  |                        Ventas diarias pendientes para 30 días.                         |
|      CustCollectionsBIExpectedPayment       |           ExpectedPayment            | CustCollectionsBIExpectedPaymentView |                 Sum(SystemCurrencyAmounts)                 |                 La suma de pagos previstos en el año próximo.                 |
|        CustCollectionsBIInterestNote        |             InterestNote             |           CustInterestJour           |                    Count(InterestNote)                     |                El número de notas de interés que se crearon.                |
|        CustCollectionsBISalesOnHold         |               SalesId                |              SalesTable              |                       Count(SalesId)                       |                 El número pedidos de venta totales que están en espera.                 |
|          CustCollectionsBIWriteOff          |            WriteOffAmount            |    CustCollectionsBIWriteOffView     |                 Sum(SystemCurrencyAmount)                  |                La suma de transacciones que se han cancelado.                 |

