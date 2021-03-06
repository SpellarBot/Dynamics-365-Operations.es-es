---
title: Funcionalidad de ventas del centro de llamadas
description: Este tema proporciona una visión general de la funcionalidad de ventas de centro de asistencia telefónica en Microsoft Dynamics 365 for Retail.
author: josaw1
manager: AnnBe
ms.date: 04/03/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailMCRChannelDetailPage, MCROrderParameters
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 16361
ms.assetid: c8ed2ba4-8d06-4d99-9728-2a83e6d95ca9
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: 8b78762ce70b318e1f77e1e49ffaa7b72f01667f
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "363163"
---
# <a name="call-center-sales-functionality"></a>Funcionalidad de ventas del centro de llamadas

[!include [banner](includes/banner.md)]

En Dynamics 365 for Retail, un centro de llamadas es un tipo de canal minorista que se puede definir en la aplicación. La definición de un canal específico para sus entidades de centro de asistencia telefónica permite que el sistema vincule valores predeterminados específicos de datos y los valores predeterminados del procesamiento del pedido a los pedidos de ventas creados por un usuario del canal de centro de llamadas.

Las características del centro de asistencia telefónica incluyen precio y promociones al por menor avanzados, catálogos, tarjetas regalo, programas de fidelidad, y vales. Se saca provecho de los pedidos de centro de asistencia telefónica en función de su aplicación de punto de venta (POS) para admitir escenarios de cumplimiento de pedidos transcanales.

Es importante tener en cuenta que mientras que el módulo de centro de asistencia telefónica se utiliza en otras sectores que no son de ventas al por menor, la versión actual de la aplicación de centro de asistencia telefónica de Dynamics 365 for Retail no se ha optimizado para su uso en escenarios interempresariales (B2B) de procesamiento de pedidos o los escenarios donde los pedidos tengan una gran cantidad de líneas de ventas. Se recomienda que los usuarios que desean utilizar el centro de asistencia telefónica para el procesamiento del pedido fuera del procesamiento de transacciones típico de directo a consumidor, tomen el tiempo adecuado para probar y validar que la habilitación de la función del centro de asistencia telefónica va a cubrir las necesidades funcionales y de rendimiento.

Además de admitir la creación de pedidos, el módulo de centro de asistencia telefónica también proporciona una aplicación de servicio al cliente convivial que hace más fácil que los usuarios localicen cuentas de cliente y revisen todos los datos y atributos relacionados de pedido de cliente. La pantalla de servicio al cliente está diseñada para permitir que un usuario pueda obtener acceso rápidamente a los datos relacionados con el pedido que le permitirán atender la mayoría de consultas más habituales relacionadas con pedidos recibidos de clientes.

Esta página ofrece vínculos a la documentación pertinente relacionada con la configuración, y el uso funcional de las características del centro de asistencia telefónica de Dynamics 365 for Retail.

## <a name="configure-the-call-center"></a>Configure el centro de llamadas

[Configurar opciones de procesamiento de pedidos](set-up-order-processing-options.md)

## <a name="configure-order-processing"></a>Configurar el procesamiento de pedidos

[Configurar alertas de fraude](set-up-fraud-alerts.md)

[Retenciones de pedidos manuales](work-with-order-holds.md)

## <a name="configure-payment-processing"></a>Configurar procesamiento de pagos

[Métodos de pago en un centro de llamadas](work-with-payments.md)

## <a name="configure-delivery-modes"></a>Configurar modos de entrega

[Configurar modos y cargos de entrega del centro de llamadas](configure-call-center-delivery.md)

## <a name="configure-direct-marketing"></a>Configurar marketing directo

[Catálogos de centros de llamadas](call-center-catalogs.md)

[Configurar análisis de RFM](set-up-rfm-analysis.md)

## <a name="configure-continuity-programs"></a>Configurar programas de continuidad

[Configurar un programa de continuidad para un centro de llamadas](set-up-continuity-program.md)
