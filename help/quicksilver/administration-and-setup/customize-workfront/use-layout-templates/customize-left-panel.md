---
title: Anpassen des linken Bereichs mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In einer Layoutvorlage können Sie anpassen, was Benutzer im linken Bedienfeld in Adobe Workfront sehen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

# Anpassen des linken Bedienfelds mithilfe einer Layoutvorlage

<!--Audited: 10/2024-->

In einer Layoutvorlage können Sie anpassen, was Benutzer im linken Bedienfeldbereich in [!DNL Adobe Workfront] sehen.

Sie können beispielsweise bestimmen, welche der folgenden Elemente Benutzern im linken Bereich angezeigt werden, wenn Sie eine Aufgabe anzeigen:

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>An der Bestellung und Sichtbarkeit vorgenommene Änderungen werden in der Mobile App übernommen.

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassen des linken Bereichs für einen Bereich in [!DNL Workfront]:

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie auf den Abwärtspfeil ![](assets/dropdown-arrow.png) unter **[!UICONTROL Anpassen, was Benutzer sehen]**, und klicken Sie dann auf den Namen eines Objekttyps oder eines Bereichs [!DNL Workfront] , dessen linker Bereich Sie anpassen möchten.

   Die Objekttypen und [!DNL Workfront] -Bereiche, deren linker Bereich Sie anpassen können, sind in der folgenden Tabelle aufgeführt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Objekttyp oder Bereich [!DNL Workfront]</th> 
      <th>Wenn Benutzer auf Folgendes klicken..</th> 
      <th>Abschnitte im linken Bereich, die Benutzern angezeigt werden, nachdem Sie sie in der Layoutvorlage angezeigt haben:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Projekt]</td> 
      <td>Der Name eines Projekts</td> 
      <td>[!UICONTROL Aufgaben], [!UICONTROL Projektdetails], [!UICONTROL Geschäftsfall], [!UICONTROL Updates], [!UICONTROL Dokumente], [!UICONTROL Probleme], [!UICONTROL Risiken], [!UICONTROL Validierungen], [!UICONTROL Grundlinien], [!UICONTROL Abrechnungsraten], [!UICONTROL Abrechnung], Aufzeichnungen Ausgaben!UICONTROL, [!UICONTROL Stunden], [!UICONTROL Workload Balancer], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics], [!UICONTROL CONTROL Planning]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Der Name einer Aufgabe</td> 
      <td> [!UICONTROL Aktualisierungen], [!UICONTROL Dokumente], [!UICONTROL Aufgabendetails], [!UICONTROL Unteraufgabe], [!UICONTROL Probleme], [!UICONTROL Stunden], [!UICONTROL Genehmigungen], [!UICONTROL Ausgaben], [!UICONTROL Vorgänger]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problem]</td> 
      <td>Der Name eines Problems</td> 
      <td> [!UICONTROL Aktualisierungen], [!UICONTROL Dokumente], [!UICONTROL Problemdetails], [!UICONTROL Stunden], [!UICONTROL Genehmigungen]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Der Name eines Portfolios</td> 
      <td>[!UICONTROL Projekte], [!UICONTROL Programme], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio] [!UICONTROL Optimierung], [!UICONTROL Dokumente], [!UICONTROL Updates], [!UICONTROL Planung]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Programm]</td> 
      <td>Der Name eines Programms</td> 
      <td>[!UICONTROL Projekte], [!UICONTROL Programmdetails], [!UICONTROL Updates], [!UICONTROL Dokumente], [!UICONTROL Planung]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Vorlage]</td> 
      <td>Der Name einer Projektvorlage</td> 
      <td>[!UICONTROL Vorlagenaufgaben], [!UICONTROL Vorlagendetails], [!UICONTROL Aktualisierungen], [!UICONTROL Dokumente], [!UICONTROL Risiken], [!UICONTROL Ausgaben], [!UICONTROL Personen], [!UICONTROL Genehmigungen], [!UICONTROL Abrechnungsraten], [!UICONTROL Warteschlangendetails], [!UICONTROL Routing Rules],!UICONTROL Warteschlangenthema], [!UICONTROL Themengruppe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Vorlagenaufgabe]</td> 
      <td>Der Name einer Vorlagenaufgabe</td> 
      <td>[!UICONTROL Aktualisierungen], [!UICONTROL Dokumente], [!UICONTROL Vorlagenaufgaben], [!UICONTROL Unteraufgaben], [!UICONTROL Ausgaben], [!UICONTROL Genehmigungen], [!UICONTROL Vorgänger]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Rechnungsdatensatz]</td> 
      <td>Der Name eines Abrechnungsdatensatzes für ein Projekt</td> 
      <td>[!UICONTROL Rechnungsdatensätze], [!UICONTROL Rechnungsstunden], [!UICONTROL Abrechenbare Ausgaben], [!UICONTROL Festeinnahmen]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projekte]</td> 
      <td>Projekte <img src="assets/projects-in-main-menu.png"> im [!UICONTROL Hauptmenü] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projekte]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Anforderungen]</td> 
      <td>Der Name einer Anforderung</td> 
      <td>[!UICONTROL Neue Anfrage], [!UICONTROL Gesendete Anfragen], [!UICONTROL Alle Anfragen], [!UICONTROL Entwürfe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Der Name eines Dashboards</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b>HINWEIS</b>: Wenn Sie benutzerdefinierte Registerkarten für den Bereich [!UICONTROL Berichte] mit einer Layout-Vorlage in [!DNL Adobe Workfront Classic] erstellt haben, werden diese am unteren Rand dieser Liste angezeigt. Benutzer werden im Bereich [!UICONTROL Dashboards] unten im linken Bereich angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Der Name eines Scrum-Teams</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>HINWEIS:</strong> Das Element <strong>[!UICONTROL Aktuelle Iteration]</strong> wird nur dann im linken Bereich angezeigt, wenn bei der Iteration mindestens eine Aufgabe oder ein Problem vorliegt.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>Der Name eines Kanban-Teams</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban Board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Wasserfallteam]</td> 
      <td>Der Name eines Wasserfallteams</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>Der Name einer Iteration</td> 
      <td>[!UICONTROL Meldungen], [!UICONTROL Probleme], [!UICONTROL Meldungsboard], [!UICONTROL Übersicht], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   *Ihr Unternehmen muss eine zusätzliche Lizenz für Workfront Planning erwerben, um diesen Bereich zum linken Bereich von Projekten, Portfolios und Programmen hinzufügen zu können. Weitere Informationen finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md)


1. Führen Sie in der Liste **[!UICONTROL Linker Bereich]** einen der folgenden Schritte aus, um zu bestimmen, welche Benutzer im linken Bereich für den ausgewählten [!DNL Workfront] -Bereich oder Objekttyp angezeigt werden:

   * Klicken Sie auf die Symbole **Anzeigen** ![](assets/add-secondary-nav-item.png) oder **Ausblenden** ![](assets/delete-secondary-nav-item.png) , um Abschnitte im linken Bereich ein- oder auszublenden. Sie können keine Elemente ausblenden, die kein Symbol **Einblenden** oder **Ausblenden** aufweisen.

   * Ziehen Sie Elemente ![](assets/move-icon---dots.png) in die Reihenfolge, um sie im linken Bereich zu ändern.

   >[!NOTE]
   >
   >Die folgenden Elemente in der Dropdownliste **[!UICONTROL Anpassen, was Benutzer sehen]** beziehen sich auf andere Bereiche als den linken Bereich:
   >* [!UICONTROL Listen]
   >* [!UICONTROL Bedienfeld &quot;Zusammenfassung&quot;]
   >* [!UICONTROL Startseite]
   >* [!UICONTROL Branding]
   > 
   >Informationen zum Anpassen der zusätzlichen Bereiche finden Sie in den folgenden Artikeln:
   >
   >* [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Passen Sie das Bedienfeld [!UICONTROL Zusammenfassung] mithilfe einer Layoutvorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Passen Sie die Startseite mit einer Layoutvorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Adobe markieren [!DNL Workfront] mit einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Optional) Wenn Sie ein Element des linken Bedienfelds hinzufügen möchten, das mit einem der Dashboards Ihres Unternehmens verknüpft ist, klicken Sie auf **[!UICONTROL Benutzerspezifischen Abschnitt hinzufügen]**, geben Sie einen **[!UICONTROL Titel des benutzerdefinierten Abschnitts]** für das Element ein und fügen Sie dann das Dashboard hinzu.

   Dashboard-Elemente werden unten im linken Bereich angezeigt. Benutzer sehen den Titel des benutzerdefinierten Abschnitts, den Sie neben dem Dashboard-Element eingeben, wenn sie im linken Bereich den Mauszeiger darüber bewegen.

   >[!NOTE]
   >
   >Benutzer können benutzerdefinierte Dashboard-Elemente zu ihrem eigenen linken Bereich hinzufügen. Wenn Sie benutzerdefinierte Dashboard-Elemente zu einer Layoutvorlage hinzufügen, werden Ihre Elemente zusätzlich zu den von ihnen hinzugefügten Elementen angezeigt, ohne sie zu überschreiben oder zurückzusetzen. Dies gilt auch, wenn Sie Benutzer einer neuen Layoutvorlage mit benutzerdefinierten Dashboard-Elementen zuweisen. Informationen dazu, wie Benutzer das linke Bedienfeld anpassen können, finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Weitere Informationen zu Dashboards finden Sie unter [Dashboards](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.

   >[!TIP]
   >
   >Sie können jederzeit auf [!UICONTROL **Speichern**] klicken, um Ihren Fortschritt zu speichern, wodurch der Layout-Vorlagen-Editor geschlossen wird, und die Vorlage später weiter ändern.
