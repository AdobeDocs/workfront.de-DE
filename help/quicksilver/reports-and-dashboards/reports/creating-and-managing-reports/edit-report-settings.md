---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Berichteinstellungen bearbeiten
description: Sie können die Einstellungen eines Berichts bearbeiten, um festzulegen, wie der Bericht für andere Benutzer angezeigt wird oder um festzulegen, nach welchen Informationen Benutzer gefragt werden können, bevor sie den Bericht ausführen.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 6%

---

# Berichteinstellungen bearbeiten

<!-- Audited: 11/2024 -->

Sie können die Einstellungen eines Berichts bearbeiten, um festzulegen, wie der Bericht für andere Benutzer angezeigt wird oder um festzulegen, nach welchen Informationen Benutzer gefragt werden können, bevor sie den Bericht ausführen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Schritte

1. Beginnen Sie mit der Erstellung eines Berichts, indem Sie das **Hauptmenü** > **Berichte** aufrufen und dann das Objekt Ihres Berichts auswählen.

   Oder

   Öffnen Sie einen vorhandenen Bericht und klicken Sie dann auf **Berichtaktionen** > **Bearbeiten**.

1. Klicken Sie oben rechts im ReportBuilder auf **Berichtseinstellungen** .
1. Konfigurieren Sie die folgenden Berichtseinstellungen:

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
      <td>Geben Sie eine Erklärung an, die den Zweck und die Verwendung des Berichts beschreibt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Führen Sie diesen Bericht mit den Zugriffsrechten von aus.</td> 
      <td>Wählen Sie den Benutzer aus, dessen Zugriffsberechtigungen dieser Bericht bei der Anzeige für andere Benutzer verwenden soll. Weitere Informationen zum Ausführen eines Berichts mit den Zugriffsrechten eines anderen Benutzers finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ausführen und Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn der Bericht geladen wird, zeigen Sie die</td> 
      <td>Wählen Sie die Standardregisterkarte aus, die für alle Benutzer beim Laden des Berichts angezeigt wird.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wenn der Bericht in ein Dashboard geladen wird, zeigen Sie ... Elemente an</td> 
      <td>Geben Sie an, wie viele Elemente für alle Benutzer angezeigt werden, wenn der Bericht in ein Dashboard geladen wird. Der Standardwert ist 15 Elemente und die maximale Anzahl von Elementen ist 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigen des Ressourcenrasters auf der Registerkarte "Details"</td> 
      <td> <p>(Nur Benutzerbericht) Wählen Sie diese Option aus, um das Ressourcenraster auf der Registerkarte Details des Berichts anzuzeigen.</p> <p>Hinweis: Beim Anwenden der Ansicht "Ressourcenraster"auf einen Benutzerbericht zeigt der Bericht nur Projekte an, die sich im aktuellen Status befinden. Wenn Sie Projekte in einem anderen Status anzeigen möchten, können Sie die Registerkarte "Benutzerauslastung"im Bereich "Personen"der globalen Navigationsleiste verwenden und dort die Ansicht "Ressourcenraster"anwenden. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigen einer speziellen Ansicht auf der Registerkarte "Details"</td> 
      <td>(Nur Projektbericht) Geben Sie den Ansichtstyp an, der Benutzern angezeigt wird, wenn sie auf diese Informationen auf der Registerkarte Details zugreifen. Sie können beispielsweise eine Meilenstein- oder Gantt-Ansicht auswählen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diesen Bericht standardmäßig in einer Balkendiagrammansicht anzeigen.</td> 
      <td>(Nur Projektbericht und Aufgabenbericht) Wählen Sie diese Option, damit die Gantt-Ansicht automatisch aktiviert wird, wenn Benutzer die Registerkarte Details in diesem Bericht anzeigen.<br>Weitere Informationen zum Anzeigen des Gantt-Diagramms in Projekt- und Aufgabenberichten finden Sie im Abschnitt "Anzeigen von Aufgabeninformationen in der Projektliste Gantt-Diagramm"im Artikel <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Anzeigen von Informationen im Gantt-Diagramm </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ansichtänderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer die Ansicht beim Ausführen des Berichts ändern können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenänderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer die Gruppe bei Ausführung des Berichts ändern können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filteränderung im Bericht zulassen</td> 
      <td>Wählen Sie diese Option aus, damit Benutzer den Filter beim Ausführen des Berichts ändern können.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Berichtaufforderungen** , um alle Eingabeaufforderungen für den Bericht einzurichten.\
   Weitere Informationen zum Hinzufügen von Eingabeaufforderungen zu einem Bericht finden Sie im Artikel [Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Fertig,** und dann auf **Speichern + Schließen**.

## Weitere Informationen

Siehe auch:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Erste Schritte mit Berichten](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Verwenden der integrierten Adobe Workfront-Berichte](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
