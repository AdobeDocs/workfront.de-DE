---
title: Gewähren eines vollen Administratorzugriffs
description: Sie können Benutzern uneingeschränkten Administratorzugriff auf Workfront gewähren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '1583'
ht-degree: 1%

---

# Gewähren eines vollen Administratorzugriffs

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Gewähren des uneingeschränkten Administratorzugriffs in der Adobe Admin Console finden Sie unter [Verwalten von Systemadministratoren in der Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator können Sie einen anderen Workfront-Administrator erstellen, indem Sie ihm die Zugriffsebene &quot;Systemadministrator&quot;zuweisen. Ein Benutzer mit dieser Zugriffsebene hat vollen Administratorzugriff auf alles in Workfront, einschließlich der Elemente, die er selbst nicht erstellt hat.

>[!NOTE]
>
>Dies unterscheidet sich von der Verwendung einer Zugriffsebene, um Benutzern Administratorzugriff auf bestimmte Bereiche des Systems zu gewähren. Weitere Informationen finden Sie unter folgenden Themen:
>
>* [Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Zugriff eines Workfront-Administrators auf einen Planbenutzer mit Administratorrechten](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in diesem Artikel
>

## Zugriffsanforderungen

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="#" class="MCXref xref selected">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vollständigen Systemadministratorzugriff für einen einzelnen Benutzer gewähren

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Benutzer** ![](assets/users-icon-in-main-menu.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf den Namen des Benutzers, dem Sie Administratorrechte gewähren möchten.
1. Klicken Sie auf das Menü Mehr ![](assets/more-icon.png) und dann auf **Bearbeiten**.

1. Klicken Sie im angezeigten Feld **Person bearbeiten** auf **Zugriff**.

1. Wählen Sie in der Dropdownliste **Zugriffsstufe** die Zugriffsstufe **Systemadministrator** aus.

   Abhängig von den in Ihrem System vorgenommenen Änderungen hat sich der Name dieser Zugriffsebene möglicherweise geändert.

1. Klicken Sie auf **Änderungen speichern.**

   Der Benutzer verfügt jetzt über vollständige Systemadministratorrechte im System.

## Zugriff eines Workfront-Administrators auf einen Planbenutzer mit Administratorrechten im Vergleich  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Die beiden folgenden Tabellen zeigen den Unterschied zwischen den Zugriffsrechten eines Benutzers mit Workfront-Administrator-Zugriffsstufe und denen eines Benutzers mit einer Planungslizenz mit einigen Administratorrechten.

Workfront-Administratoren können alle Objekte im System anzeigen (unabhängig davon, wer sie erstellt hat), neue erstellen und vorhandene ändern oder löschen. Sie haben vollen Zugriff auf alle Objekte im System.

Benutzer mit einer Planungslizenz, die Funktionen in einem Bereich bearbeiten können, haben vollen Zugriff auf die Funktionalität in diesem Bereich.

>[!NOTE]
>
>Benutzer mit einer Planungslizenz, die als Gruppenadministratoren benannt sind, können einige der für Workfront-Administratoren zulässigen Aktionen ausführen. Sie dürfen diese Aktionen nur für die von ihnen verwalteten Gruppen, deren Untergruppen und die Benutzer in diesen Gruppen und Untergruppen durchführen. Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Zugriff auf den Einrichtungsbereich](#access-to-the-setup-area)
* [Zugriff auf Objekte](#access-to-objects)

### Zugriff auf den Einrichtungsbereich {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich/Objekt</th> 
   <th>Workfront-Administrator </th> 
   <th>Benutzer mit einer Planungslizenz und einigen Administratorrechten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projektvoreinstellungen: Projekte</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Aufgaben und Probleme</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Status</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Projektpräferenzen: Prioritäten</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Schwerpunkte</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Wechselkurse</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Prozesse: Validierungen</td> 
   <td> <p>Vollständiger Zugriff</p> </td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Prozesse: Milestone-Pfade</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Formulare</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Verwalten Sie benutzerdefinierte Formulare, die sie erstellt haben, oder benutzerdefinierte Formulare, die für sie freigegeben wurden.</p> <p>Hängen Sie benutzerdefinierte Formulare, die sie erstellt haben, oder benutzerdefinierte Formulare, die für sie freigegeben sind, an Objekte an, die sie verwalten oder für die sie Berechtigungen erteilen.</p> </td> 
  </tr> 
  <tr> 
   <td>Papierkorb: Kürzlich gelöscht</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Benutzer, die Gruppenadministratoren sind, können Projekte wiederherstellen, die Gruppen zugewiesen sind, die sie verwalten, sowie Aufgaben, Probleme oder Dokumente, die mit diesen Projekten verknüpft sind.</p> </td> 
  </tr> 
  <tr> 
   <td>Papierkorb: kürzlich wiederhergestellt</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Benutzer, die Gruppenadministratoren sind, können die Elemente sehen, die sie kürzlich wiederhergestellt haben.</td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiete</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Vorhandene Auftragsrollen können geändert, aber nicht gelöscht werden.</p> <p>Fügen Sie neue Auftragsrollen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Erstellung von Teams.</p> <p>Fügen Sie Benutzern vorhandene Teams bei der Erstellung oder Bearbeitung von Benutzern hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>Gruppen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Gruppen.</p> <p>Nur Gruppenadministratoren können Gruppenmitgliedschaften, Untergruppen und Gruppenstatus für die von ihnen verwalteten Gruppen verwalten. </p> </td> 
  </tr> 
  <tr> 
   <td>Firmen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Anmelden als</td> 
   <td>Vollständiger Zugriff </td> 
   <td> <p>Wenn der Gruppenverwaltungszugriff auf der Zugriffsebene aktiviert ist und sie als Gruppenadministrator benannt sind, kann er sich als Benutzer in der Gruppe, die er verwaltet, und in den Untergruppen anmelden. Sie können sich nicht als Systemadministrator anmelden.<br>Weitere Informationen zum Aktivieren des Gruppenadministrationszugriffs für Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Zeitpläne</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Bearbeiten von Zeitplänen.</p> <p>Zugriff auf das Hinzufügen vorhandener Zeitpläne zu anderen Benutzern auf Benutzerebene. </p> </td> 
  </tr> 
  <tr> 
   <td>Datenblatt und Stunden: Datenblatt-Profile</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff auf die Zuweisung vorhandener Timesheet-Profile zu Benutzern auf Benutzerebene.</p> <p>Benutzer, die Gruppenadministratoren sind, können für die von ihnen verwalteten Gruppen und deren Untergruppen Timesheet-Profile erstellen. </p> </td> 
  </tr> 
  <tr> 
   <td>Datenblatt und Stunden: Stunden</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff zur Zuweisung von Stündungstypen an Benutzer auf Benutzerebene.</p> </td> 
  </tr> 
  <tr> 
   <td>Zeitblatt und Stunden: Voreinstellungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: Ereignisbenachrichtigungen</td> 
   <td>Alle aktivieren/deaktivieren</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: Erinnerung</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: E-Mail-Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zur Bearbeitung von E-Mail-Vorlagen.</p> <p>Zugriff auf das Hinzufügen vorhandener E-Mail-Vorlagen zu Erinnerungsbenachrichtigungen.</p> </td> 
  </tr> 
  <tr> 
   <td>E-Mail: Automatische Erinnerungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Email: Einladungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zur Bearbeitung von E-Mail-Einladungen.</p> <p>Zugriff zum erneuten Senden von E-Mail-Einladungen an abgemeldete Benutzer nur über den Tab Personen .</p> </td> 
  </tr> 
  <tr> 
   <td>E-Mail: Einrichtung</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Vollständiger Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Ausgabentypen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Risikotypen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Zugriffsebenen</td> 
   <td> <p>Vollständiger Zugriff zur Änderung aller Zugriffsebenen.</p> <p>Die Zugriffsebenen "Systemadministrator"und "Externer Benutzer"können standardmäßig nicht geändert werden.</p> </td> 
   <td> <p>Kein Zugriff zur Bearbeitung von Zugriffsebenen.</p> <p>Weisen Sie anderen Benutzern eine Zugriffsstufe zu, die auf Benutzerebene kleiner oder gleich den entsprechenden ist.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Layout-Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff auf die Zuweisung vorhandener Layout-Vorlagen für andere Benutzer auf Benutzerebene. </p> <p>Benutzer, die als Gruppenadministratoren festgelegt wurden, können Layoutvorlagen für von ihnen verwaltete Gruppen und Untergruppen erstellen.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Feeds aktualisieren</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Ändern von Aktualisierungs-Feeds.</p> <p>Zugriff auf das Hinzufügen von Feldern, die bei der Bearbeitung des benutzerdefinierten Forms in den Update-Feeds verfolgt werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>Schnittstelle: Filter</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Filtern im Bereich "Einrichtung".</p> <p>Zugriff zum Erstellen neuer Filter in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Ansichten</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Ansichten im Bereich "Einrichtung".</p> <p>Zugriff zum Erstellen neuer Ansichten in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Gruppierungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf das Erstellen von Gruppierungen im Bereich Einrichtung .</p> <p>Zugriff zum Erstellen neuer Gruppierungen in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Listen-Steuerelemente</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Cloud-Anbieter</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zur Konfiguration von Cloud-Anbietern.</p> <p>Zugriff auf Verknüpfungsdokumente von und zu Cloud-Anbietern über die Registerkarte "Dokumente", nachdem Cloud-Anbieter in Workfront integriert wurden.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Metadatenzuordnung</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Dokumente: SharePoint-Integration</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Konfigurieren einer SharePoint-Integration.</p> <p>Zugriff auf Verknüpfungsdokumente von und zu SharePoint über die Registerkarte Dokumente , nachdem die SharePoint-Integration mit Workfront konfiguriert wurde.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Benutzerdefinierte Integration</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Konfigurieren einer benutzerdefinierten Integration.</p> <p>Zugriff auf Verknüpfungsdokumente von und zu Drittanbietern über die Registerkarte Dokumente , nachdem die Drittanbieter in Workfront integriert wurden.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Kundeninformationen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Aktualisieren von Benutzern für SSO</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Start</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Voreinstellungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
 </tbody> 
</table>

### Zugriff auf Objekte {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich/Objekt</th> 
   <th>Workfront-Administrator </th> 
   <th>Benutzer mit einer Planungslizenz und einigen Administratorrechten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kalender</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie die von ihnen erstellten Kalender und die für sie freigegebenen Kalender.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie Dashboards, die sie erstellen, und Dashboards, die für sie freigegeben sind.</td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie Dokumente, die sie hochladen, oder Dokumente, die für sie freigegeben wurden.</td> 
  </tr> 
  <tr> 
   <td>Probleme</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie Probleme, die sie erstellen, oder Probleme, die für sie freigegeben wurden.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie die von ihnen erstellten Portfolios oder die für sie freigegebenen Portfolios. </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie Programme, die sie erstellen, oder Programme, die für sie freigegeben sind.</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie von ihnen erstellte Projekte oder Projekte, die für sie freigegeben wurden.</td> 
  </tr> 
  <tr> 
   <td>Berichte</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten Sie von ihnen erstellte Berichte oder Berichte, die für sie freigegeben wurden. Systemberichte anzeigen, kopieren und bearbeiten.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Verwalten von Aufgaben, die sie erstellen, oder Aufgaben, die für die</td> 
  </tr> 
  <tr> 
   <td>Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vorlagen verwalten, die sie erstellen oder Vorlagen, die für sie freigegeben wurden</td> 
  </tr> 
  <tr> 
   <td>Arbeitszeit- tabellen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Benutzende</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Eingeschränkter Zugriff</p> <p>Sie können keine Gruppen Benutzern zuweisen, für die sie kein Gruppenadministrator sind, oder nicht öffentlichen Gruppen.</p> <p>Sie können Benutzern keine Zugriffsstufe zuweisen, die höher ist als ihre eigene Zugriffsstufe.</p> <p>Wenn der Gruppenverwaltungszugriff auf der Zugriffsebene aktiviert ist und sie als Gruppenadministrator für eine Gruppe bestimmt sind, können sie das Kennwort zurücksetzen und sich als Benutzer in der Gruppe, die sie verwalten, und in ihren Untergruppen anmelden. Sie können das Kennwort von nicht zurücksetzen oder sich als Systemadministrator anmelden.<br>Weitere Informationen zum Aktivieren des Gruppenadministrationszugriffs für Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
