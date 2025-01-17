---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fehlerbehandlung in Adobe Workfront Fusion auslösen
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Behandlung von Auslösefehlern in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Problemumgehung für `throw` konfigurieren](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einigen Fällen empfiehlt es sich, die Ausführung des Szenarios mit der [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)- oder [Commit](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit)-Phase zu stoppen oder die Verarbeitung einer Route zu stoppen und sie optional in der Warteschlange der unvollständigen Ausführungen zu speichern.

Derzeit können die Anweisungen zur Fehlerbehandlung nicht außerhalb des Bereichs einer [Route für Fehlerhandler](../../workfront-fusion/errors/error-handling.md#error) verwendet werden und [!DNL Adobe Workfront Fusion] bietet kein Modul, das es Ihnen ermöglichen würde, einfach bedingte Fehler zu erzeugen (Fehler auszulösen).

Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Informationen zu Anweisungen zur Fehlerbehandlung finden Sie unter [Anweisungen zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Problemumgehung für Throw

Um einen Fehler bedingt auszulösen, können Sie ein Modul so konfigurieren, dass es optional während seines Vorgangs fehlschlägt. Eine Möglichkeit besteht darin, das Modul [!UICONTROL JSON] > [!UICONTROL Parse JSON] zu verwenden (siehe [JSON-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md)), das so konfiguriert ist, dass es optional einen Fehler auslöst (in diesem Fall BundleValidationError):

Anschließend können Sie eine der Anweisungen zur Fehlerbehandlung an die Route für die Fehlerbehandlung anhängen an:

* Erzwingen, dass die Szenarioausführung angehalten wird und die Rollback-Phase ausgeführt wird: [!UICONTROL Rollback]
* Erzwingt, dass die Ausführung des Szenarios beendet wird und die Commit-Phase durchführt: [!UICONTROL Commit]
* Verarbeitung einer Route stoppen: [!UICONTROL Ignorieren]
* Stoppen Sie die Verarbeitung einer Route und speichern Sie sie in der Warteschlange des Ordners für unvollständige Ausführungen: [!UICONTROL break]

Das folgende Beispiel zeigt die Verwendung der [!DNL Rollback]-Direktive:

![](assets/rollback-directive-350x175.png)
