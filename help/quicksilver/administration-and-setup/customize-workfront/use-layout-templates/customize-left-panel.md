---
title: Anpassen des linken Bedienfelds mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In einer Layout-Vorlage können Sie anpassen, was Benutzende im linken Bereich in Adobe Workfront sehen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# Anpassen des linken Bedienfelds mithilfe einer Layout-Vorlage

<!--Audited: 10/2024-->

In einer Layout-Vorlage können Sie anpassen, was Benutzende im gesamten Bereich des linken Bedienfelds sehen [!DNL Adobe Workfront].

Sie können beispielsweise bestimmen, welches der folgenden Elemente Benutzern im linken Bereich beim Anzeigen einer Aufgabe angezeigt wird:

![Linker Bereich für Branding](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Änderungen an der Bestellung und der Sichtbarkeit werden in der Mobile App übernommen.

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>Beliebig</p>
   <p>Das Hinzufügen benutzerdefinierter Programme zum Hauptmenü ist nur für Organisationen verfügbar, die für Adobe App Builder lizenziert sind.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Passen Sie das linke Bedienfeld für einen Bereich in [!DNL Workfront] an:

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie auf den Abwärtspfeil ![Abwärtspfeil](assets/dropdown-arrow.png) unter **[!UICONTROL Anpassen, was Benutzer sehen]** und klicken Sie dann auf den Namen eines Objekttyps oder [!DNL Workfront] Bereichs, dessen linker Bereich angepasst werden soll.

   Die Objekttypen und [!DNL Workfront] Bereiche, deren linker Bereich angepasst werden kann, sind in der folgenden Tabelle aufgeführt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Objekttyp oder [!DNL Workfront]</th> 
      <th>Wenn Benutzer auf Folgendes klicken…</th> 
      <th>Abschnitte im linken Bereich, die Benutzenden angezeigt werden, nachdem sie in der Layout-Vorlage angezeigt wurden:</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL-Projekt]</td> 
      <td>Der Name eines Projekts</td> 
      <td>[!UICONTROL Aufgaben], [!UICONTROL Projektdetails], [!UICONTROL Business Case], [!UICONTROL Updates], [!UICONTROL Dokumente], [!UICONTROL Probleme], [!UICONTROL Risiken], [!UICONTROL Genehmigungen], [!UICONTROL Baselines], [!UICONTROL Abrechnungssätze], [!UICONTROL Abrechnungssätze], [!UICONTROL Ausgaben], [!UICONTROL Stunden], [!UICONTROL Workload Balancer], [!UICONTROL Personen], [!UICONTROL Auslastung], [!UICONTROL Auslastung], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group], [!UICONTROL Metrics], [!UICONTROL Planning]*, [!UICONTROL Custom Application]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Aufgabe]</td> 
      <td>Der Name einer Aufgabe</td> 
      <td> [!UICONTROL-Aktualisierungen], [!UICONTROL-Dokumente], [!UICONTROL-Aufgabendetails], [!UICONTROL-Unteraufgabe], [!UICONTROL-Probleme], [!UICONTROL-Stunden], [!UICONTROL-Genehmigungen], [!UICONTROL-Ausgaben], [!UICONTROL-Vorgänger], [!UICONTROL-benutzerdefinierte Anwendung]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problem]</td> 
      <td>Der Name eines Problems</td> 
      <td> [!UICONTROL-Aktualisierungen], [!UICONTROL-Dokumente], [!UICONTROL-Problemdetails], [!UICONTROL-Stunden], [!UICONTROL-Genehmigungen], [!UICONTROL-benutzerdefinierte Anwendung]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Der Name eines Portfolios</td> 
      <td>[!UICONTROL-Projekte], [!UICONTROL-Programme], [!UICONTROL Portfolio-Details], [!UICONTROL Portfolio] [!UICONTROL-Optimierung], [!UICONTROL-Dokumente], [!UICONTROL-Updates], [!UICONTROL Planning]*, [!UICONTROL Custom Application]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL-Programm]</td> 
      <td>Der Name eines Programms</td> 
      <td>[!UICONTROL-Projekte], [!UICONTROL-Programmdetails], [!UICONTROL-Updates], [!UICONTROL-Dokumente], [!UICONTROL Planning]*, [!UICONTROL Custom Application]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL-Vorlage]</td> 
      <td>Der Name einer Projektvorlage</td> 
      <td>[!UICONTROL Vorlagenaufgaben], [!UICONTROL Vorlagendetails], [!UICONTROL Updates], [!UICONTROL Dokumente], [!UICONTROL Risiken], [!UICONTROL Ausgaben], [!UICONTROL Personen], [!UICONTROL Genehmigungen], [!UICONTROL Abrechnungssätze], [!UICONTROL Warteschlangendetails], [!UICONTROL Routing-Regeln], [!UICONTROL Warteschlangenthema], [!UICONTROL Themengruppe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Vorlagenaufgabe]</td> 
      <td>Der Name einer Vorlagenaufgabe</td> 
      <td>[!UICONTROL-Aktualisierungen], [!UICONTROL-Dokumente], [!UICONTROL-Vorlagenaufgabendetails], [!UICONTROL-Teilaufgaben], [!UICONTROL-Ausgaben], [!UICONTROL-Genehmigungen], [!UICONTROL-Vorgänger]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Rechnungsnachweis]</td> 
      <td>Der Name eines Rechnungsnachweises für ein Projekt</td> 
      <td>[!UICONTROL Rechnungsnachweis-Details], [!UICONTROL Fakturierbare Stunden], [!UICONTROL Fakturierbare Ausgaben], [!UICONTROL Feste Einnahmen]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL-Projekte]</td> 
      <td>Im [!UICONTROL-Hauptmenü] <img src="assets/projects-in-main-menu.png"> Projekte <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL-Projekte]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL-Anforderungen]</td> 
      <td>Der Name einer Anfrage</td> 
      <td>[!UICONTROL Neue Anfrage], [!UICONTROL Gesendete Anfragen], [!UICONTROL Alle Anfragen], [!UICONTROL Entwürfe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Der Name eines Dashboards</td> 
      <td>[!UICONTROL Eigene Dashboards], [!UICONTROL Freigegebene Dashboards], [!UICONTROL Alle Dashboards]<p><b>HINWEIS</b>: Wenn Sie benutzerdefinierte Registerkarten für den Bereich [!UICONTROL Berichte] mithilfe einer Layout-Vorlage in [!DNL Adobe Workfront Classic] erstellt haben, werden sie unten in dieser Liste angezeigt. Für Benutzer werden sie unten im linken Bereich im Bereich [!UICONTROL Dashboards] angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum-Team]</td> 
      <td>Der Name eines Scrum-Teams</td> 
      <td><p>[!UICONTROL-Iterationen], [!UICONTROL Aktuelle Iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL-Aktualisierungen], [!UICONTROL-Teameinstellungen]</p> <p><strong>HINWEIS:</strong> Das Element <strong>[!UICONTROL Aktuelle Iteration]</strong> wird im linken Bereich nur angezeigt, wenn mindestens eine Aufgabe oder ein Problem bei der Iteration vorliegt.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban-Team]</td> 
      <td>Der Name eines Kanban-Teams</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban-Board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team-Einstellungen]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall-Team]</td> 
      <td>Der Name eines Waterfall-Teams</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>Der Name einer Iteration</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Probleme], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
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

   *Ihr Unternehmen muss eine zusätzliche Lizenz für Workfront Planning erwerben, um diesen Bereich dem linken Bereich von Projekten, Portfolios und Programmen hinzufügen zu können. Weitere Informationen finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md)

   **Benutzerdefinierte Programme müssen separat erstellt werden, bevor sie als Hauptmenüoptionen verfügbar werden. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Programms für Workfront mit Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).


1. Führen Sie in der **[!UICONTROL Linker Bereich]** einen der folgenden Schritte aus, um zu bestimmen, was Benutzende im linken Bereich für den ausgewählten [!DNL Workfront] Bereich oder Objekttyp sehen werden:

   * Klicken Sie auf **Anzeigen** ![Symbol anzeigen](assets/add-secondary-nav-item.png) oder **Ausblenden** ![Symbol ausblenden](assets/delete-secondary-nav-item.png), um Abschnitte im linken Bereich ein- oder auszublenden. Sie können keine Elemente ausblenden, die kein Symbol **Anzeigen** oder **Ausblenden** aufweisen.

   * Ziehen Sie Elemente ![Symbol Verschieben](assets/move-icon---dots.png), um ihre Reihenfolge im linken Bedienfeld zu ändern.

   >[!NOTE]
   >
   >Die folgenden Elemente in der **[!UICONTROL Anpassen, was Benutzer sehen]** Dropdown-Liste beziehen sich auf andere Bereiche als den linken Bereich:
   >* [!UICONTROL Listen]
   >* [!UICONTROL Bedienfeld Zusammenfassung]
   >* [!UICONTROL Startseite]
   >* [!UICONTROL Branding]
   > 
   >Informationen zum Anpassen der zusätzlichen Bereiche finden Sie in den folgenden Artikeln:
   >
   >* [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Passen Sie den [!UICONTROL Zusammenfassungsbereich] mithilfe einer Layout-Vorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Passen Sie die Startseite mithilfe einer Layout-Vorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Marke Adobe [!DNL Workfront] mit einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Optional) Wenn Sie ein Element im linken Bedienfeld hinzufügen möchten, das mit einem der Dashboards Ihres Unternehmens verknüpft ist, klicken Sie auf **[!UICONTROL Benutzerdefinierten Abschnitt hinzufügen]** und geben Sie einen **[!UICONTROL benutzerdefinierten Abschnittstitel]** für das Element ein. Fügen Sie dann das Dashboard hinzu.

   Dashboard-Elemente werden am unteren Rand des linken Bedienfelds angezeigt. Benutzern wird der benutzerdefinierte Abschnittstitel angezeigt, den Sie neben dem Dashboard-Element eingeben, wenn sie den Mauszeiger darüber im linken Bedienfeld bewegen.

   >[!NOTE]
   >
   >Benutzer können benutzerdefinierte Dashboard-Elemente zu ihrem eigenen linken Bedienfeld hinzufügen. Wenn Sie einer Layout-Vorlage benutzerdefinierte Dashboard-Elemente hinzufügen, werden Ihre Elemente zusätzlich zu den hinzugefügten Elementen angezeigt, ohne sie zu überschreiben oder zurückzusetzen. Dies gilt auch, wenn Sie Benutzende einer neuen Layout-Vorlage mit benutzerdefinierten Dashboard-Elementen zuweisen. Informationen zum Anpassen des linken Bedienfelds durch Benutzende finden Sie unter [Erstellen benutzerdefinierter Registerkarten oder Abschnitte](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Weitere Informationen zu Dashboards finden Sie unter [Dashboards](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **[!UICONTROL Speichern]**.

   >[!TIP]
   >
   >Sie können jederzeit auf [!UICONTROL **Speichern**] klicken, um Ihren Fortschritt zu speichern. Dadurch wird der Layout-Vorlageneditor geschlossen und die Vorlage später weiter geändert.
