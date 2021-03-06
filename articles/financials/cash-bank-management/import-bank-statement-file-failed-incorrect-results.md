---
title: Solución de problemas de la importación de archivos de extractos bancarios
description: Es importante que el archivo de extracto bancario del banco coincida con el diseño admitido por Microsoft Dynamics 365 for Finance and Operations. Debido a los estrictos estándares para extractos bancarios, la mayoría de las integraciones funcionarán correctamente. Sin embargo, a veces, el archivo de extracto no se puede importar o tiene resultados incorrectos. Normalmente, estos problemas son originados por pequeñas diferencias en el archivo de extracto bancario. En este artículo se explica cómo corregir estas diferencias y resolver los problemas.
author: ShylaThompson
manager: AnnBe
ms.date: 01/11/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankStatementFormat
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 141273
ms.assetid: 3ee2f32b-02aa-420b-8990-e6aa5fc6bda3
ms.search.region: global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a4006bf35673e3bb61bcf11619ecc68d295f29eb
ms.sourcegitcommit: 0f530e5f72a40f383868957a6b5cb0e446e4c795
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/29/2019
ms.locfileid: "324454"
---
# <a name="bank-statement-file-import-troubleshooting"></a>Solución de problemas de la importación de archivos de extractos bancarios

[!include [banner](../includes/banner.md)]

Es importante que el archivo de extracto bancario del banco coincida con el diseño admitido por Microsoft Dynamics 365 for Finance and Operations. Debido a los estrictos estándares para extractos bancarios, la mayoría de las integraciones funcionarán correctamente. Sin embargo, a veces, el archivo de extracto no se puede importar o tiene resultados incorrectos. Normalmente, estos problemas son originados por pequeñas diferencias en el archivo de extracto bancario. En este artículo se explica cómo corregir estas diferencias y resolver los problemas.

<a name="what-is-the-error"></a>¿Qué es el error?
------------------

Tras intentar importar un archivo de extracto bancario, vaya al historial de trabajos de administración de datos y sus detalles de ejecución para encontrar el error. El error puede resultar de ayuda al señalar la instrucción, el saldo o la línea de extracto. Sin embargo, es poco probable que proporcione suficiente información para ayudarle a identificar el campo o el elemento que está ocasionando el problema.

## <a name="what-are-the-differences"></a>¿Cuáles son las diferencias?
Compare la definición del diseño de archivos de banco con la definición de importación de Finance and Operations y observe los posibles diferencias en los campos y elementos. Compare el archivo de extracto bancario con el archivo de muestra relacionado de Finance and Operations. En los archivos ISO20022 las diferencia se verán fácilmente.

## <a name="transformations"></a>Transformaciones
Normalmente, el cambio se debe realizar en una de tres transformaciones. Cada transformación se escribe para un estándar específico.

| Nombre del recurso                                         | Nombre de archivo                          |
|-------------------------------------------------------|------------------------------------|
| BankStmtImport\_BAI2CSV\_to\_BAI2XML\_xslt            | BAI2CSV-to-BAI2XML.xslt            |
| BankStmtImport\_ISO20022XML\_to\_Reconciliation\_xslt | ISO20022XML-to-Reconciliation.xslt |
| BankStmtImport\_MT940TXT\_to\_MT940XML\_xslt          | MT940TXT-to-MT940XML.xslt          |

## <a name="debugging-transformations"></a>Depuración de transformaciones
### <a name="adjust-the-bai2-and-mt940-files"></a>Ajustar los archivos BAI2 y MT940

Los archivos BAI2 y MT940 son archivos basados en texto y requieren un ajuste para habilitar la depuración del Lenguaje de transformación basado en hojas de estilo (XSLT). El programa realiza este ajuste cuando se importa un archivo.

1.  Cree un archivo XML y copie el siguiente texto en él.

        <Batch><![CDATA[PASTESTATEMENTFILEHERE
        ]]></Batch>

2.  Copie el contenido del archivo de extracto bancario y péguelo en el archivo XML de modo que reemplace **PASTESTATEMENTFILEHERE**.

### <a name="debug-the-xslt"></a>Depurar XSLT

Para obtener más información, vea <https://msdn.microsoft.com/en-us/library/ms255605.aspx>.

1.  Iniciar Microsoft Visual Studio.
2.  Crear una aplicación de consola.
3.  Abra el XSLT adecuado.
4.  Haga clic en el XLST y su página de propiedades.
5.  Establezca la entrada en la ubicación del archivo del extracto bancario.
6.  Defina una ubicación y un nombre de archivo para la salida.
7.  Establezca los puntos de interrupción necesarios.
8.  En el menú, haga clic en **XML** &gt; **Iniciar depuración de XSLT**.

### <a name="format-the-xslt-output"></a>Aplicar formato a la salida de XSLT

Cuando se ejecuta la transformación, crea un archivo de salida que pueda ver en Visual Studio. Use Ctrl+A, Ctrl+K y Ctrl+D para dar formato rápidamente al archivo de salida.

### <a name="adjust-the-transformation"></a>Ajustar la transformación

Ajuste la transformación para obtener el elemento o el campo adecuado en el archivo de extracto bancario. A continuación, asigne ese campo o artículo al elemento de Finance and Operations adecuado.

### <a name="debitcredit-indicator"></a>Indicador de débito o crédito

A veces, los débitos se pueden importar como créditos y los créditos se pueden importar como débitos. Para resolver este problema, debe cambiar el XSLT adecuado. Si los extractos bancarios proceden de varios bancos, asegúrese de que todos usen el mismo enfoque de débito/crédito o cree transformaciones independientes.

-   Plantilla GetAmountCreditDebitIndicator de BAI2XML-to-Reconciliation.xlst
-   Plantilla GetCreditDebit de ISO20022XML-to-Reconcilation.xslt
-   Plantilla GetCreditDebitIndicator de MT940XML-to-Reconcilation.xslt

## <a name="examples-of-bank-statement-formats-and-technical-layouts"></a>Ejemplos de diseños técnicos y formatos de extracto bancario
En la tabla siguiente se muestran ejemplos de las definiciones de diseño técnico para los archivos de importación de conciliación bancaria avanzados y tres archivos de ejemplo de extracto bancario relacionados. Puede descargar los archivos de ejemplo y los diseños técnicos aquí: https://mbs.microsoft.com/customersource/northamerica/AX/learning/documentation/how-to-articles/exofbankstfotechlayouts  


| Definición de diseño técnico                             | Archivo de ejemplo de extracto bancario          |
|---------------------------------------------------------|--------------------------------------|
| DynamicsAXMT940Layout                                   | MT940StatementExample                |
| DynamicsAXISO20022Layout                                | ISO20022StatementExample             |
| DynamicsAXBAI2Layout                                    | BAI2StatementExample                 |





