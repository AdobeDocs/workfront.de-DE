---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Berichteinstellungen bearbeiten
description: Sie können die Einstellungen eines Berichts bearbeiten, um festzulegen, wie er für andere Benutzer angezeigt wird oder welche Art von Informationen die Benutzer vor Ausführung des Berichts anfordern können.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 7%

---

# Berichteinstellungen bearbeiten

<!-- Audited: 11/2024 -->

Sie können die Einstellungen eines Berichts bearbeiten, um festzulegen, wie er für andere Benutzer angezeigt wird oder welche Art von Informationen die Benutzer vor Ausführung des Berichts anfordern können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
 <td> <p>Verwalten von Berechtigungen für einen Bericht</p></td>  
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anleitungsschritte

1. Beginnen Sie mit der Erstellung eines Berichts, indem Sie **Hauptmenü** > **Berichte** wechseln und dann das Objekt Ihres Berichts auswählen.

   Oder

   Öffnen Sie einen vorhandenen Bericht und klicken Sie auf **Berichtsaktionen** > **Bearbeiten**.

1. Klicken **oben rechts** Report Builder auf „Berichteinstellungen“.
1. Konfigurieren Sie die folgenden Berichteinstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Berichttitel</td> 
      <td>Geben Sie einen Titel für den Bericht an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Erklärung an, die den Zweck und die Verwendungszwecke des Berichts beschreibt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diesen Bericht ausführen mit Zugriffsrechten von</td> 
      <td>Wählen Sie den Benutzer aus, dessen Zugriffsrechte Sie für diesen Bericht verwenden möchten, wenn er für andere Benutzer angezeigt wird. Weitere Informationen zum Ausführen eines Berichts mit den Zugriffsrechten eines anderen Benutzers finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Bericht ausführen und mit den Zugriffsrechten eines anderen Benutzers bereitstellen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Laden des Berichts Folgendes anzeigen</td> 
      <td>Wählen Sie die Standardregisterkarte aus, die für alle Benutzer beim Laden des Berichts angezeigt wird.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn der Bericht auf einem Dashboard geladen wird, Elemente anzeigen …</td> 
      <td>Geben Sie die Anzahl der Elemente an, die für alle Benutzer angezeigt werden, wenn der Bericht in einem Dashboard geladen wird. Der Standardwert ist 15 Elemente und die maximale Anzahl von Elementen ist 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenraster-Ansicht auf der Registerkarte „Details“ anzeigen</td> 
      <td> <p>(Nur Benutzerbericht) Wählen Sie diese Option aus, um das Ressourcenraster auf der Registerkarte Details des Berichts anzuzeigen.</p> <p>Hinweis: Beim Anwenden der Ressourcenraster -Ansicht auf einen Benutzerbericht zeigt der Bericht nur Projekte an, die sich im aktuellen Status befinden. Wenn Sie Projekte mit einem anderen Status anzeigen möchten, können Sie die Registerkarte „Benutzerauslastung“ im Bereich „Personen“ der globalen Navigationsleiste verwenden und dort die Ansicht „Ressourcenraster“ anwenden. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spezielle Ansicht auf der Registerkarte „Details“ anzeigen</td> 
      <td>(Nur Projektbericht) Geben Sie den Ansichtstyp an, den Benutzer sehen, wenn sie auf diese Informationen auf der Registerkarte „Details“ zugreifen. Sie können beispielsweise eine Meilenstein- oder Gantt-Ansicht auswählen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diesen Bericht standardmäßig in einer Balkendiagrammansicht anzeigen.</td> 
      <td>(Nur Projektbericht und Aufgabenbericht) Wählen Sie diese Option, um die Gantt-Ansicht automatisch zu aktivieren, wenn Benutzer die Registerkarte „Details“ in diesem Bericht anzeigen.<br>Weitere Informationen zum Anzeigen des Gantt-Diagramms in Projektberichten und Aufgabenberichten finden Sie im Abschnitt „Aufgabeninformationen in der Projektliste anzeigen Gantt-Diagramm“ im Artikel <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Informationen in der Gantt-Diagramm-</a> anzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ansichtänderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer die Ansicht ändern können, wenn sie den Bericht ausführen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenänderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer beim Ausführen des Berichts die Gruppe ändern können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filteränderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer den Filter beim Ausführen des Berichts ändern können.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Eingabeaufforderungen**, um Eingabeaufforderungen für den Bericht einzurichten.\
   Weitere Informationen zum Hinzufügen von Eingabeaufforderungen zu einem Bericht finden Sie im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Fertig** und dann auf **Speichern + schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Erste Schritte mit Berichten](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Verwenden von integrierten Adobe Workfront-Berichten](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
