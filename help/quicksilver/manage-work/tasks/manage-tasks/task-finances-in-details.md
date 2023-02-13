---
product-area: projects
navigation-topic: manage-tasks
title: Verwalten von Aufgabenfinanzen im Abschnitt "Aufgabendetails"
description: Verwalten von Aufgabenfinanzen im Abschnitt "Aufgabendetails"
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# Verwalten von Aufgabenfinanzen im Abschnitt &quot;Aufgabendetails&quot;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Sie können die Finanzinformationen einer Aufgabe anzeigen oder bearbeiten, indem Sie auf den Bereich Übersicht im Abschnitt Aufgabendetails zugreifen. Es gibt eine begrenzte Anzahl von Feldern, die Sie in diesem Bereich anzeigen oder bearbeiten können. Informationen zum Bearbeiten aller Finanzinformationen für eine Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Zugriff auf Finanzdaten oder höher anzeigen</p> <p>Sie müssen Zugriff auf Finanzdaten bearbeiten haben, um Finanzinformationen zu Aufgaben zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für die Aufgabe, die View Finance (oder höher) enthalten</p> <p>Sie müssen über Verwaltungsberechtigungen für die Aufgabe verfügen, die "Finanz bearbeiten"enthalten, um Finanzinformationen zu Aufgaben zu bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Bearbeiten von Aufgabenfinanzierungen im Abschnitt &quot;Aufgabendetails&quot;

1. Wechseln Sie zu einem Projekt, in dem Sie eine Aufgabe anzeigen möchten.

   >[!NOTE]
   >
   >Um eine Aufgabe zu finden, können Sie auch danach suchen und auf den Namen klicken, um auf die Aufgabe zuzugreifen. Weitere Informationen zum Suchen nach Objekten in Workfront finden Sie unter [Adobe Workfront durchsuchen](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Klicken **Aufgaben** im linken Bereich.
1. Klicken Sie auf den Namen einer Aufgabe, die Sie anzeigen möchten.
1. Klicken **Aufgabendetails**.
1. (Optional) Klicken Sie auf die **Alle reduzieren** rechts oben auf der Seite &quot;Aufgabendetails&quot;angezeigt.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator unsere Layout-Vorlage einrichtet, werden die Felder im Abschnitt &quot;Aufgabendetails&quot;möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klicken **Finanzen** , um die Finanzinformationen für die Aufgabe zu erweitern und anzuzeigen.

   Klicken Sie auf **Bearbeiten** icon ![](assets/edit-icon.png) in der oberen rechten Ecke des Bereichs Details klicken Sie auf **Finanzen**.

1. Bearbeiten Sie ein beliebiges Feld, das bearbeitet werden kann, indem Sie mit einem einzigen Klick auf das Feld klicken oder auf **+Hinzufügen** , um Informationen zu einem leeren Feld hinzuzufügen.
1. Überprüfen oder bearbeiten Sie die folgenden Informationen in der **Finanzen** area :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostenart</td> 
      <td> <p>Geben Sie den Kostentyp für die Aufgabe an. Auf diese Weise wird bestimmt, wie die Kosten der Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet werden. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p>Keine Kosten</p> </li> 
        <li> <p>Festgelegt pro Stunde </p> </li> 
        <li> <p> Benutzer pro Stunde </p> </li> 
        <li> <p> Stundensatz nach Funktion</p> </li> 
       </ul> <p>Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a> . Ihr Workfront-Administrator oder Gruppenadministrator wählt die Standardeinstellung für den Kostentyp für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Umsatztyp</td> 
      <td> <p>Geben Sie den Umsatztyp für die Aufgabe an. Auf diese Weise wird bestimmt, wie der Umsatz aus der Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet wird. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p> Nicht fakturierbar </p> </li> 
        <li> <p>Benutzer pro Stunde </p> </li> 
        <li> <p>Stundensatz nach Funktion </p> </li> 
        <li> <p>Festgelegt pro Stunde </p> </li> 
        <li> <p>Benutzer pro Stunde m/Obergrenze </p> </li> 
        <li> <p>Stundensatz nach Funktion m/Obergrenze </p> </li> 
        <li> <p>Benutzer pro Stunde plus festgelegt </p> </li> 
        <li> <p>Stundensatz nach Funktion plus fest </p> </li> 
        <li> <p>Festeinnahmen </p> </li> 
       </ul> <p>Weitere Informationen zur Umsatzverfolgung finden Sie unter<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Rechnungsstellung und Umsatz</a> . </p> <p>Ihr Workfront-Administrator oder Gruppenadministrator wählt die standardmäßige Einstellung "Umsatztyp"für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Weitere Informationen zum Festlegen der Projektstandards finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Systemweite Projektvoreinstellungen konfigurieren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Kosten</td> 
      <td> <p>Hierbei handelt es sich um eine Berechnung, die die Kosten der Aufgabe basierend auf den geplanten Stunden, dem Kostentyp und der Stundenrate für Benutzer oder Stellenrollen anzeigt. Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Kosten</td> 
      <td> <p> Hierbei handelt es sich um eine Berechnung, die die Kosten der Aufgabe basierend auf den tatsächlichen Stunden, dem Kostentyp und der Stundenrate für Benutzer oder Stellenrollen anzeigt. Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Einnahmen</td> 
      <td> <p>Dies ist eine Berechnung, die den Umsatz, der mit der Aufgabe verbunden ist, basierend auf den geplanten Stunden, dem Umsatztyp und der Stundenrate für Benutzer oder Stellenrollen anzeigt. Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächlicher Umsatz</td> 
      <td> <p>Dies ist eine Berechnung, die den Umsatz, der mit der Aufgabe verbunden ist, basierend auf den tatsächlichen Stunden, dem Umsatztyp und der Stundenrate für Benutzer oder Stellenrollen anzeigt. Weitere Informationen zu Tracking-Kosten finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten verfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>Dies sind Metriken zur Aufgabenleistung, die die Leistung Ihrer Aufgabe zu einem bestimmten Zeitpunkt anzeigen. Ihre Werte werden anhand der Leistungsindex-Methode des Projekts berechnet.<br>Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">CPI (Cost Performance Index) berechnen</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Berechnung des Zeitplan-Leistungsindex (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calculate Cost Schedule Performance Index (CSI)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung zum Abschluss (EAC)</td> 
      <td> <p>Dies ist eine Berechnung, die die Gesamtkosten Ihrer Aufgabe nach Abschluss anzeigt. Weitere Informationen über die Schätzung zum Zeitpunkt der Fertigstellung finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schätzung nach Abschluss berechnen (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie die Felder im Abschnitt Finanzen bearbeiten, klicken Sie auf **Speichern***Änderungen**.
