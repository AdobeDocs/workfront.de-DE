---
product-area: projects
navigation-topic: manage-tasks
title: Verwalten der Aufgabenfinanzen im Abschnitt Aufgabendetails
description: Verwalten der Aufgabenfinanzen im Abschnitt Aufgabendetails
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 4%

---

# Verwalten der Aufgabenfinanzen im Abschnitt Aufgabendetails

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Sie können die Finanzinformationen einer Aufgabe anzeigen oder bearbeiten, indem Sie auf den Bereich Übersicht des Abschnitts Aufgabendetails zugreifen. Es gibt eine begrenzte Anzahl von Feldern, die Sie in diesem Bereich anzeigen oder bearbeiten können. Informationen zum Bearbeiten aller Finanzinformationen für eine Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Aufgaben bearbeiten</p> <p>Zugriff auf Finanzdaten anzeigen oder höher</p> <p>Sie müssen Bearbeitungszugriff auf Finanzdaten haben, um Finanzinformationen zu Aufgaben bearbeiten zu können</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für die Aufgabe, die View Finance oder höher enthalten</p> <p>Sie müssen über Verwaltungsberechtigungen für die Aufgabe verfügen, die „Finanzen bearbeiten“ enthalten, um Finanzinformationen zu Aufgaben zu bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Aufgabenfinanzen im Abschnitt „Aufgabendetails“ bearbeiten

1. Wechseln Sie zu einem Projekt, in dem Sie eine Aufgabe anzeigen möchten.

   >[!NOTE]
   >
   >Um eine Aufgabe zu finden, können Sie auch danach suchen und auf den Namen klicken, um auf die Aufgabe zuzugreifen. Weitere Informationen zum Suchen nach Objekten in Workfront finden Sie unter [Adobe Workfront durchsuchen](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Klicken Sie **linken** auf „Aufgaben“.
1. Klicken Sie auf den Namen einer Aufgabe, die Sie anzeigen möchten.
1. Klicken Sie **Aufgabendetails**.
1. (Optional) Klicken Sie auf **Symbol „Alle** reduzieren“ oben rechts auf der Seite „Aufgabendetails“.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layout-Vorlage einrichtet, werden die Felder im Abschnitt Aufgabendetails möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Klicken Sie **Finanzen**, um die Finanzinformationen für die Aufgabe zu erweitern und anzuzeigen.

   Klicken Sie auf **Bearbeiten**-Symbol ![](assets/edit-icon.png) in der oberen rechten Ecke des Abschnitts Details und dann auf **Finanzen**.

1. Bearbeiten Sie alle Felder, die bearbeitet werden können, indem Sie einfach auf das Feld klicken oder auf **+Hinzufügen** klicken, um einem leeren Feld Informationen hinzuzufügen.
1. Überprüfen oder bearbeiten Sie die folgenden Informationen im Bereich **Finanzen** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kostenart</td> 
      <td> <p>Geben Sie den Kostentyp für die Aufgabe an. Dadurch wird bestimmt, wie die Kosten der Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet werden. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p>Keine Kosten</p> </li> 
        <li> <p>Festgelegt pro Stunde </p> </li> 
        <li> <p> Benutzer pro Stunde </p> </li> 
        <li> <p> Stundensatz nach Funktion</p> </li> 
       </ul> <p>Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a> . Ihr Workfront-Administrator oder ein Gruppenadministrator wählt die Standardkostenart für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Informationen zum Festlegen von Projektstandards finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Projektvoreinstellungen</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Umsatztyp</td> 
      <td> <p>Geben Sie den Umsatztyp für die Aufgabe an. Dadurch wird bestimmt, wie der Umsatz für die Aufgabe basierend auf der Anzahl der Stunden für die Aufgaben berechnet wird. </p> <p>Wählen Sie aus den folgenden Optionen aus: </p> 
       <ul> 
        <li> <p> Nicht fakturierbar </p> </li> 
        <li> <p>Benutzer pro Stunde </p> </li> 
        <li> <p>Stundensatz nach Funktion </p> </li> 
        <li> <p>Festgelegt pro Stunde </p> </li> 
        <li> <p>Benutzende pro Stunde mit Begrenzung </p> </li> 
        <li> <p>Stundensatz nach Funktion mit Begrenzung </p> </li> 
        <li> <p>Benutzer pro Stunde plus festgelegt </p> </li> 
        <li> <p>Stundensatz nach Funktion plus fest </p> </li> 
        <li> <p>Festeinnahmen </p> </li> 
       </ul> <p>Weitere Informationen zur Umsatzverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Übersicht über Abrechnung und Umsatz</a> . </p> <p>Ihr Workfront-Administrator oder Gruppenadministrator wählt die Standardeinstellung für den Umsatztyp für die Aufgaben in Ihrem System oder Ihrer Gruppe aus. Informationen zum Festlegen von Projektstandards finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Konfigurieren von systemweiten Projektvoreinstellungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Kosten</td> 
      <td> <p>Dies ist eine Berechnung, die die Kosten der Aufgabe basierend auf den geplanten Stunden, dem Kostentyp und dem Stundensatz für Benutzer oder Aufgabengebiete anzeigt. Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Istkosten</td> 
      <td> <p> Diese Berechnung zeigt die Kosten der Aufgabe basierend auf den tatsächlichen Stunden, dem Kostentyp und dem Stundensatz für Benutzer oder Aufgabengebiete an. Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Einnahmen</td> 
      <td> <p>Hierbei handelt es sich um eine Berechnung, die den mit der Aufgabe verbundenen Umsatz basierend auf den geplanten Stunden, dem Umsatztyp und dem Stundensatz für Benutzer oder Aufgabengebiete anzeigt. Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Einnahmen</td> 
      <td> <p>Hierbei handelt es sich um eine Berechnung, die den mit der Aufgabe verbundenen Umsatz basierend auf den tatsächlichen Stunden, dem Umsatztyp und dem Stundensatz für Benutzer oder Aufgabengebiete anzeigt. Weitere Informationen zur Kostennachverfolgung finden Sie unter <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Kosten nachverfolgen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>Dies sind Leistungsmetriken, die zeigen, wie Ihre Aufgabe zu einem bestimmten Zeitpunkt funktioniert. Ihre Werte werden auf Grundlage der Leistungsindexmethode des Projekts berechnet.<br>Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Kostenentwicklungsindex (Cost Performance Index, CPI) berechnen</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Planleistungsindex (SPI)-</a> berechnen </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Kostenplan-Leistungsindex (CSI) berechnen</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung bei Abschluss (EAC)</td> 
      <td> <p>Dies ist eine Berechnung, die die Gesamtkosten Ihrer Aufgabe bei Abschluss anzeigt. Weitere Informationen zur Schätzung bei Abschluss finden Sie unter <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schätzung bei Abschluss berechnen (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie die Felder im Abschnitt Finanzen bearbeiten, klicken Sie auf **Speichern**&#x200B;**Änderungen**.
