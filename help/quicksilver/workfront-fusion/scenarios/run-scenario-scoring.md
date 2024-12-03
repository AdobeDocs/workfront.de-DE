---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ausführen des Szenario-Scoring-Experten in Adobe Workfront Fusion
description: Der Scoring-Experte für Szenarien kann Ihnen dabei helfen sicherzustellen, dass Ihr Szenario so konfiguriert ist, dass Best Practices befolgt werden. Es überprüft Ihr Szenario und gibt Empfehlungen für seine Struktur und Organisation.
author: Becky
feature: Workfront Fusion
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 2b455fb2d3892c6bb796aa7ea57a60c861c3d599
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Ausführen des Szenario-Scoring-Experten in Adobe Workfront Fusion

Der Scoring-Experte für Szenarien kann Ihnen dabei helfen sicherzustellen, dass Ihr Szenario so konfiguriert ist, dass Best Practices befolgt werden. Es überprüft Ihr Szenario und gibt Empfehlungen für seine Struktur und Organisation.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

Ausführen des Szenario-Scoring-Experten

1. Klicken Sie im linken Bereich auf die Registerkarte **[!UICONTROL Szenario]** .
1. Wählen Sie das Szenario aus, in dem Sie den Scoring-Experten für Szenarien ausführen möchten.
1. Klicken Sie auf eine beliebige Stelle des Szenarios, um den Szenario-Editor aufzurufen.
1. Klicken Sie unten auf dem Bildschirm auf das Symbol &quot;Szenario-Scoring-Experte&quot;![Scenario Scoring Expert](assets/scoring-expert-icon.png) .

   Das Bedienfeld &quot;Szenario-Scoring-Experte&quot;wird geöffnet.
1. Klicken Sie auf **Evaluate**.

Der Szenario-Scoring-Experte gibt einen Wert von 10 zurück und zeigt an, welche Prüfungen bestanden oder fehlgeschlagen sind. Wenn eine Prüfung fehlgeschlagen ist, gibt der Scoring-Expert Empfehlungen dazu, wie sichergestellt werden kann, dass das Szenario diese Prüfungen erfüllt.

![Szenario-Ergebnis](assets/scenario-score.png)

## Prüfungen der Szenario-Scoring

Der Scoring-Experte für Szenarien verwendet die folgenden Prüfungen:

* Das Szenario muss einen Namen haben.
* Alle Module müssen beschriftet werden.
* Das Szenario muss nach einem festgelegten Zeitplan ausgeführt werden.

  Anweisungen finden Sie unter [Planen eines Szenarios](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* Die Blueprint-Größe des Szenarios muss unter 5 MB liegen.

  Weitere Informationen finden Sie unter [Schutzmechanismen für die Leistung von Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Wenn ein Workfront-Instant-Trigger-Modul verwendet wird, muss es gefiltert werden.

  Anweisungen finden Sie unter [Ereignisabonnementfilter im Modul  [!DNL Workfront] > [!UICONTROL Ereignisse beobachten]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).

