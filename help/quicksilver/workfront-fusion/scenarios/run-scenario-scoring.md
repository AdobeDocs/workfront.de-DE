---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ausführen des Szenario-Scoring-Experten in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Ausführen des Szenario-Scoring-Experten in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Den Szenario-Scoring-Experten ausführen](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/run-scenario-scoring.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Der Szenario-Scoring-Experte kann Ihnen dabei helfen sicherzustellen, dass Ihr Szenario so konfiguriert ist, dass es den Best Practices entspricht. Er prüft Ihr Szenario und gibt Empfehlungen für dessen Struktur und Organisation.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und -integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

Ausführen des Szenario-Scoring-Experten

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Szenario“ im linken Bedienfeld.
1. Wählen Sie das Szenario aus, in dem Sie den Szenario-Scoring-Experten ausführen möchten.
1. Klicken Sie auf eine beliebige Stelle im Szenario, um den Szenario-Editor aufzurufen.
1. Klicken Sie auf das Symbol „Szenario![Bewertungsexperte](assets/scoring-expert-icon.png) unten im Bildschirm.

   Das Expertengremium für Szenario-Bewertung wird geöffnet.
1. Klicken Sie **Auswerten**.

Der Szenario-Scoring-Experte gibt einen Score von 10 zurück und zeigt an, welche Prüfungen bestanden oder fehlgeschlagen sind. Wenn eine Prüfung fehlgeschlagen ist, gibt der Szenario-Scoring-Experte Empfehlungen, wie sichergestellt werden kann, dass das Szenario diese Prüfungen erfüllt.

![Szenario-Bewertung](assets/scenario-score.png)

## Szenario-Scoring-Prüfungen

Der Szenario-Scoring-Experte verwendet die folgenden Prüfungen:

* Das Szenario muss benannt werden.
* Alle Module müssen beschriftet sein.
* Das Szenario muss nach einem festgelegten Zeitplan ausgeführt werden.

  Anweisungen finden Sie unter [Planen eines Szenarios](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* Die Größe des Szenario-Blueprints muss unter 5 MB liegen.

  Weitere Informationen finden Sie unter [Leistungs-Schutzmechanismen von Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Wenn ein Workfront Instant Trigger-Modul verwendet wird, muss es gefiltert werden.

  Anweisungen finden Sie unter [Ereignisabonnementfilter im Modul  [!DNL Workfront] > [!UICONTROL Ereignisse ]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).

