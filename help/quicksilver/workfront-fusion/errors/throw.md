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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Umgang mit Fehlermeldungen in [!DNL Adobe Workfront Fusion]

In einigen Fällen können Sie die Ausführung des Szenarios erzwingen, gefolgt von [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) oder [Bestätigen](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) -Phase oder zum Beenden der Verarbeitung einer Route und optional deren Speicherung in der Warteschlange unvollständiger Ausführungen.

Derzeit können die Richtlinien zur Fehlerbehebung nicht außerhalb des Anwendungsbereichs eines [Fehler-Handler-Route](../../workfront-fusion/errors/error-handling.md#error) und [!DNL Adobe Workfront Fusion] bietet kein Modul an, das es Ihnen ermöglicht, leicht bedingte (Auswurffehler) zu erzeugen.

Informationen zu unvollständigen Ausführungen finden Sie unter [Unvollständige Ausführungen in Adobe Workfront Fusion anzeigen und auflösen](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Informationen zu Richtlinien zur Fehlerbehebung finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Problemumgehung für Throw

Um einen Fehler bedingt auszulösen, können Sie ein Modul so konfigurieren, dass es während des Vorgangs optional versehentlich fehlschlägt. Eine Möglichkeit besteht darin, die [!UICONTROL JSON] > [!UICONTROL Parse JSON] -Modul (siehe [JSON-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md)), konfiguriert, um optional einen Fehler auszulösen (in diesem Fall BundleValidationError ):

Anschließend können Sie eine der Anweisungen zur Fehlerbehebung an die Fehlerbehebungsroute anhängen an:

* Setzen Sie die Ausführung des Szenarios zum Anhalten und Durchführen der Rollback-Phase auf: [!UICONTROL Rollback]
* Setzen Sie die Ausführung des Szenarios zum Anhalten und Ausführen der Commit-Phase auf: [!UICONTROL Bestätigen]
* Verarbeitung einer Route stoppen: [!UICONTROL Ignorieren]
* Beenden Sie die Verarbeitung einer Route und speichern Sie sie in der Warteschlange des Ordners mit unvollständigen Ausführungen: [!UICONTROL Break]

Das folgende Beispiel zeigt die Verwendung der [!DNL Rollback] Richtlinie:

![](assets/rollback-directive-350x175.png)
