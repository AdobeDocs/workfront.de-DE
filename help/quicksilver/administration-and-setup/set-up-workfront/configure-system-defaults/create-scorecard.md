---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Scorecard erstellen
description: Eine Scorecard misst, wie gut ein Projekt den zuvor festgelegten Kriterien eines Portfolios entspricht. Eine Scorecard spiegelt häufig die Mission, die Werte und die strategischen Ziele eines Unternehmens wider. Portfolio-Manager definieren in der Regel die Scorecard-Fragen und -Antworten, um sicherzustellen, dass sie bei der Priorisierung und Auswahl des Projekts aussagekräftig und wertvoll sind.  [!DNL Adobe Workfront]  erstellt die Scorecards anhand der Empfehlungen von Portfolio-Managern.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 05512c4cfdc094e90abea471b5356337955119be
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 1%

---

# Scorecard erstellen

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen werden nach einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar sein. </span>

<span class="preview">Weitere Informationen finden Sie unter [Modernisierung der ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)</span>

Eine Scorecard misst, wie gut ein Projekt den zuvor festgelegten Kriterien eines Portfolios entspricht. Eine Scorecard spiegelt oft die Mission, die Werte und die strategischen Ziele eines Unternehmens wider.

Als Portfolio-Manager können Sie die Scorecard-Fragen und -Antworten definieren, um sicherzustellen, dass sie bei der Priorisierung und Auswahl des Projekts aussagekräftig und wertvoll sind.

Als [!DNL Adobe Workfront] können Sie Scorecards auf der Grundlage der Empfehlungen von Portfolio-Managern erstellen.

Die für eine Scorecard ausgewählten Fragen und Antworten müssen quantifizierbar sein, damit ein Alignment-Wert zum Vergleich verschiedener Projekte bereitgestellt werden kann.

Sie können eine Scorecard wie folgt erstellen:

* Neu
* Durch Kopieren einer vorhandenen

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie benötigen den folgenden Zugriff:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Neu: [!UICONTROL Prime] oder höher</p>
   <p>Aktuell: [!UICONTROL Business] oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scorecard komplett neu erstellen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Scorecards]** und dann auf **[!UICONTROL Neue Scorecard]**.

   <span class="preview">Das Feld **Neue Scorecard** wird geöffnet.</span>

   <span class="preview">![Neues Scorecard-Feld](assets/new-scorecard-350x173.png)</span>

1. Geben Sie einen **[!UICONTROL Scorecard-Namen]** und eine **[!UICONTROL Beschreibung]** an.

   Der Name wird angezeigt, wenn Sie die Scorecard mit dem Projekt verknüpfen. Die Beschreibung wird neben dem Scorecard-Namen in der Scorecard-Liste angezeigt.

1. Klicken Sie auf **[!UICONTROL Dropdown-Menü]** Frage hinzufügen“, um den Abschnitt [!UICONTROL Scorecard-]&quot; zu öffnen, und geben Sie dann die folgenden Informationen für Ihre Frage an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL -Frage]</td> 
      <td>Geben Sie die Frage ein, die Sie in die Scorecard aufnehmen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Geben Sie die maximal möglichen Punkte für diese Frage ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Punkte]</td> 
      <td>Wählen Sie diese Option, um anzugeben, dass [!DNL Workfront] von der Gesamtzahl der möglichen Punkte subtrahieren soll. Negative Scores können nicht zu den maximal möglichen Punkten einer Scorecard hinzugefügt werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anzeigetyp]</td> 
      <td>Wählen Sie <strong>[!UICONTROL Value(0-100)]</strong>, wenn Sie ein numerisches Feld in der Scorecard anzeigen möchten, in dem Benutzer einen beliebigen Wert zwischen 0-100 angeben können.<p>Oder wählen Sie <strong>[!UICONTROL Dropdown]</strong> oder <strong>[!UICONTROL Optionsschaltflächen]</strong> aus, um eine Antwort zu erstellen, die Benutzer mithilfe dieses Steuerelements angeben können. Klicken Sie auf <strong>[!UICONTROL Antwort hinzufügen]</strong> und geben Sie dann die <strong>[!UICONTROL Value]</strong> in Prozentpunkten für diese Antwort ein, falls sie erfüllt ist. Wenn Sie 100 % auswählen, wird die Anzahl der für diese Frage zugewiesenen Punkte vollständig erreicht. Wenn Sie angeben möchten, dass diese Antwort nur einen Teil der gesamten Punktzahl für diese Frage enthält, wählen Sie einen niedrigeren Prozentwert aus. Wenn Ihre Frage beispielsweise mit 10 Punkten bewertet wird und Sie möchten, dass diese Antwort 5 dieser Punkte enthält, wählen Sie 50 % für Ihren Wert.</p>
      <p>Wählen Sie <strong>[!UICONTROL Default]</strong>, wenn Sie angeben möchten, dass dies die Standardantwort ist.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **[!UICONTROL Frage hinzufügen]**, um Ihrer Scorecard weitere Fragen und Antworten hinzuzufügen, indem Sie die gleichen Schritte ausführen.

   >[!NOTE]
   >
   >Sie können die Fragen in Ihrer Scorecard neu anordnen, indem Sie sie per Drag-and-Drop in die richtige Reihenfolge ziehen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Dadurch wird die Scorecard erstellt und Projektmanager können sie jetzt an ihren Projekt-Business-Case anhängen.

## Kopieren einer vorhandenen Scorecard

Sie können eine Scorecard durch Kopieren und Bearbeiten einer vorhandenen Scorecard erstellen.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL linken]** auf „Scorecards“.
1. Wählen Sie eine Scorecard in der Liste aus und klicken Sie dann oben in der Scorecard **Liste auf** Kopieren![Symbol „Scorecard ](assets/copy-scorecard-icon.png) kopieren“.

   <span class="preview">Das Feld **Scorecard kopieren** wird geöffnet.</span>

   <span class="preview">![Scorecard-Feld kopieren](assets/copy-scorecard-box.png)</span>

1. Geben Sie die folgenden Informationen an:

   * **Scorecard**: Aktualisieren Sie den Namen der Scorecard.  Standardmäßig wird der Name automatisch im folgenden Format aktualisiert:

     `Original scorecard name (Copy)`
   * **Beschreibung**: Geben Sie zusätzliche Informationen zur Scorecard ein.
1. Klicken Sie auf **Speichern**.

   Dadurch wird eine neue Scorecard mit denselben Informationen wie bei der ursprünglichen Scorecard erstellt. Projektmanager können ihn jetzt ihrem Projekt-Business-Case zuordnen.

## Scorecard auf ein Projekt anwenden

Ein Benutzer mit [!UICONTROL Verwalten]-Berechtigungen für ein Projekt kann eine Scorecard auf ein Projekt anwenden, nachdem die Scorecard vom [!DNL Workfront]-Administrator erstellt wurde.

Eine Scorecard wird einem Projekt beim Erstellen eines Business Case für das Projekt hinzugefügt. Weitere Informationen zum Hinzufügen einer Scorecard zu einem Projekt finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


