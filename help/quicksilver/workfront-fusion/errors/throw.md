---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Umgang mit Throw-Fehlern in Adobe Workfront Fusion
description: In einigen Fällen können Sie die Ausführung des Szenarios zwangsweise stoppen, gefolgt von der Rollback- oder der Zustellphase, oder die Verarbeitung einer Route stoppen und optional in der Ansichtswarteschlange speichern und unvollständige Ausführungen in Adobe Workfront Fusion auflösen.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Umgang mit Throw-Fehlern in [!DNL Adobe Workfront Fusion]

In einigen Fällen können Sie die Ausführung des Szenarios mit anschließender [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) - oder [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) -Phase erzwingen oder die Verarbeitung einer Route stoppen und sie optional in der Warteschlange unvollständiger Ausführungen speichern.

Derzeit können die Richtlinien zur Fehlerbehebung nicht außerhalb des Bereichs einer [Fehler-Handler-Route](../../workfront-fusion/errors/error-handling.md#error) verwendet werden und [!DNL Adobe Workfront Fusion] bietet kein Modul, mit dem Sie einfach bedingt Fehler (Auswerfen) generieren können.

Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Informationen zu Richtlinien zur Fehlerbehebung finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Problemumgehung für Throw

Um einen Fehler bedingt auszulösen, können Sie ein Modul so konfigurieren, dass es während des Vorgangs optional versehentlich fehlschlägt. Eine Möglichkeit besteht darin, das Modul [!UICONTROL JSON] > [!UICONTROL JSON analysieren] zu verwenden (siehe [JSON-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md)), das so konfiguriert ist, dass optional ein Fehler ausgegeben wird (in diesem Fall BundleValidationError):

Anschließend können Sie eine der Anweisungen zur Fehlerbehebung an die Fehlerbehebungsroute anhängen an:

* Setzen Sie die Ausführung des Szenarios zum Anhalten und Ausführen der Rollback-Phase auf: [!UICONTROL Rollback]
* Setzen Sie die Ausführung des Szenarios zum Anhalten und Ausführen der Commitphase: [!UICONTROL Bestätigen]
* Beenden Sie die Verarbeitung einer Route: [!UICONTROL Ignorieren]
* Beenden Sie die Verarbeitung einer Route und speichern Sie sie in der Warteschlange des Ordners für unvollständige Ausführungen: [!UICONTROL Break]

Das folgende Beispiel zeigt die Verwendung der Anweisung [!DNL Rollback] :

![](assets/rollback-directive-350x175.png)
