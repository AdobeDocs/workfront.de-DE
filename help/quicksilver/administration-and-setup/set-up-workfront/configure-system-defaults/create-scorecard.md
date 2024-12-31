---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Scorecard erstellen
description: Eine Scorecard misst, wie gut ein Projekt den zuvor festgelegten Kriterien eines Portfolios entspricht. Eine Scorecard spiegelt häufig die Mission, die Werte und die strategischen Ziele eines Unternehmens wider. Portfolio-Manager definieren in der Regel die Scorecard-Fragen und -Antworten, um sicherzustellen, dass sie bei der Priorisierung und Auswahl des Projekts aussagekräftig und wertvoll sind.  [!DNL Adobe Workfront]  erstellt die Scorecards anhand der Empfehlungen von Portfolio-Managern.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---

# Scorecard erstellen

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Eine Scorecard misst, wie gut ein Projekt den zuvor festgelegten Kriterien eines Portfolios entspricht. Eine Scorecard spiegelt oft die Mission, die Werte und die strategischen Ziele eines Unternehmens wider.

Portfolio-Manager definieren in der Regel die Scorecard-Fragen und -Antworten, um sicherzustellen, dass sie bei der Priorisierung und Auswahl des Projekts aussagekräftig und wertvoll sind. Ein [!DNL Adobe Workfront] erstellt die Scorecards anhand der Empfehlungen von Portfolio-Managern.

Die für eine Scorecard ausgewählten Fragen und Antworten müssen quantifizierbar sein, damit ein Alignment-Wert zum Vergleich verschiedener Projekte bereitgestellt werden kann.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Aktuell: [!UICONTROL Business] oder höher</p> 
   Oder
   <p>Neu: [!UICONTROL Prime] oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   Oder
   <p>Neu: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scorecard erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Scorecards]** und dann auf **[!UICONTROL Neue Scorecard]**, um den Scorecard Builder zu starten und eine Scorecard zu erstellen.

1. Geben Sie einen **[!UICONTROL Scorecard-Namen]** und eine **[!UICONTROL Beschreibung]** an.

   Der Name wird angezeigt, wenn Sie die Scorecard mit dem Projekt verknüpfen. Die Beschreibung wird neben dem Scorecard-Namen in der Scorecard-Liste angezeigt.

1. Klicken Sie auf **[!UICONTROL Dropdown-Menü]** Frage hinzufügen“, um den Abschnitt [!UICONTROL Scorecard-]&quot; zu öffnen, und geben Sie dann die folgenden Informationen für Ihre Frage an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Frage]</td> 
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

1. Klicken Sie **[!UICONTROL Speichern]** wenn Sie alle Informationen eingegeben haben.

   Diese erstellen die Scorecard, und Projektmanager können sie jetzt an ihren Projekt-Business-Case anhängen.

## Scorecard auf ein Projekt anwenden

Ein Benutzer mit [!UICONTROL Verwalten]-Berechtigungen für ein Projekt kann eine Scorecard auf ein Projekt anwenden, nachdem die Scorecard vom [!DNL Workfront]-Administrator erstellt wurde.

Eine Scorecard wird einem Projekt beim Erstellen eines Business Case für das Projekt hinzugefügt. Weitere Informationen zum Hinzufügen einer Scorecard zu einem Projekt finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
