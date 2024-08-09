---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Scorecard erstellen
description: Eine Scorecard misst, wie gut ein Projekt mit den zuvor festgelegten Kriterien eines Portfolios übereinstimmt. Eine Scorecard spiegelt oft die Aufgaben, Werte und strategischen Ziele einer Organisation wider. Portfolio-Manager definieren in der Regel die Scorecard-Fragen und -Antworten, um sicherzustellen, dass sie bei der Priorisierung und Auswahl von Projekten sinnvoll und wertvoll sind. Ein [!DNL Adobe Workfront] Administrator erstellt die Scorecards anhand der Empfehlungen von Portfoliomanagern.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Scorecard erstellen

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Eine Scorecard misst, wie gut ein Projekt mit den zuvor festgelegten Kriterien eines Portfolios übereinstimmt. Eine Scorecard spiegelt oft die Mission, Werte und strategischen Ziele einer Organisation wider.

Portfolio-Manager definieren in der Regel die Scorecard-Fragen und -Antworten, um sicherzustellen, dass sie bei der Priorisierung und Auswahl des Projekts sinnvoll und wertvoll sind. Ein [!DNL Adobe Workfront] -Administrator erstellt die Scorecards auf der Grundlage der Empfehlungen von Portfoliomanagern.

Die für eine Scorecard gewählten Fragen und Antworten müssen quantifizierbar sein, um einen Ausrichtungswert für den Vergleich verschiedener Projekte zu bieten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Aktuell: [!UICONTROL Business] oder höher</p> 
   Oder
   <p>Neu: [!UICONTROL Prime] oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   Oder
   <p>Neu: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

+++

## Scorecard erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Scorecards]** und dann auf **[!UICONTROL Neue Scorecard]** , um den Scorecard Builder zu starten und eine Scorecard zu erstellen.

1. Geben Sie einen **[!UICONTROL Scorecard-Namen]** und eine **[!UICONTROL Beschreibung]** an.

   Der Name wird angezeigt, wenn Sie die Scorecard mit dem Projekt verknüpfen. Die Beschreibung wird neben dem Scorecard-Namen in der Scorecard-Liste angezeigt.

1. Klicken Sie auf das Dropdownmenü **[!UICONTROL Frage hinzufügen]** , um den Abschnitt [!UICONTROL Scorecard-Frage] zu öffnen, und geben Sie dann die folgenden Informationen für Ihre Frage an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Frage]</td> 
      <td>Geben Sie die Frage ein, die Sie in die Scorecard aufnehmen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Geben Sie die für diese Frage möglichen Maximalpunkte ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Punkte]</td> 
      <td>Wählen Sie diese Option aus, um anzugeben, dass [!DNL Workfront] von den insgesamt möglichen Punkten abgezogen werden soll. Negative Werte können nicht zu den höchstmöglichen Punkten einer Scorecard hinzugefügt werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anzeigetyp]</td> 
      <td>Wählen Sie <strong>[!UICONTROL Wert(0-100)]</strong> aus, wenn Sie ein numerisches Feld in der Scorecard anzeigen möchten, in dem Benutzer einen beliebigen Wert zwischen 0 und 100 angeben können.<p>Oder wählen Sie <strong>[!UICONTROL Dropdown]</strong> oder <strong>[!UICONTROL Optionsfelder]</strong> aus, um eine Antwort zu erstellen, die Benutzer mithilfe dieses Steuerelements angeben können. Klicken Sie auf <strong>[!UICONTROL Antwort hinzufügen]</strong> und geben Sie dann den <strong>[!UICONTROL Wert]</strong> in Prozentpunkten für diese Antwort ein, falls sie erfüllt ist. Wenn Sie 100 % auswählen, wird die Anzahl der für diese Frage zugewiesenen Punkte vollständig erreicht. Wenn Sie angeben möchten, dass diese Antwort nur einen Teil der Gesamtanzahl der für diese Frage zugewiesenen Punkte enthält, wählen Sie einen niedrigeren Prozentwert aus. Wenn Ihre Frage beispielsweise bei 10 Punkten bewertet wird und Sie möchten, dass diese Antwort 5 dieser Punkte enthält, wählen Sie 50 % für Ihren Wert.</p>
      <p>Wählen Sie <strong>[!UICONTROL Default]</strong> aus, wenn Sie angeben möchten, dass diese Antwort die Standardantwort ist.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Frage hinzufügen]** , um Ihrer Scorecard weitere Fragen und Antworten hinzuzufügen, indem Sie dieselben Schritte ausführen.

   >[!NOTE]
   >
   >Sie können die Fragen in Ihrer Scorecard neu anordnen, indem Sie die Fragen in die richtige Reihenfolge ziehen und dort ablegen.

1. Klicken Sie auf **[!UICONTROL Speichern]** , wenn Sie mit der Eingabe aller Informationen fertig sind.

   Diese erstellen die Scorecard und Projektmanager können sie nun an ihren Projekt-Geschäftsfall anhängen.

## Anwenden einer Scorecard auf ein Projekt

Ein Benutzer mit [!UICONTROL Verwaltung] -Berechtigungen für ein Projekt kann eine Scorecard auf ein Projekt anwenden, nachdem die Scorecard vom [!DNL Workfront] -Administrator erstellt wurde.

Im Rahmen der Erstellung eines Geschäftsszenarios für das Projekt wird einem Projekt eine Scorecard hinzugefügt. Weitere Informationen zum Hinzufügen einer Scorecard zu einem Projekt finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in  [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
