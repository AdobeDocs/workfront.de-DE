---
title: Gewähren des vollständigen Administratorzugriffs für einen Benutzer
description: Sie können Benutzenden vollständigen administrativen Zugriff auf Workfront gewähren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 1%

---

# Gewähren des vollständigen Administratorzugriffs für einen Benutzer

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihre Organisation in die Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Anweisungen zum Gewähren des vollständigen Administratorzugriffs in der Adobe Admin Console finden Sie unter [Verwalten von Systemadministratoren in der Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>Eine Liste der Verfahren, die sich je nachdem unterscheiden, ob Ihr Unternehmen Adobe Admin Console verwendet hat, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Als Adobe Workfront-Administrator können Sie einen anderen Workfront-Administrator erstellen, indem Sie ihm die Zugriffsebene „Systemadministrator“ zuweisen. Ein Benutzer mit dieser Zugriffsebene hat vollen administrativen Zugriff auf alle Elemente in Workfront, einschließlich der Elemente, die er nicht selbst erstellt hat.

>[!NOTE]
>
>Dies unterscheidet sich von der Verwendung einer Zugriffsebene, um Benutzenden administrativen Zugriff auf bestimmte Bereiche des Systems zu gewähren. Weitere Informationen finden Sie unter:
>
>* [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Zugriff eines Workfront-Administrators vs. Zugriff eines Planbenutzers mit Administratorrechten](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) in diesem Artikel
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Gewähren des vollständigen Systemadministratorzugriffs für einen einzelnen Benutzer

{{step-1-to-users}}

1. Klicken Sie auf den Namen des Benutzers, dem Sie Administratorrechte gewähren möchten.
1. Klicken Sie auf **Mehr**-![](assets/more-icon.png) rechts neben dem Benutzernamen und dann auf **Bearbeiten**.

   Das **Person bearbeiten** wird angezeigt.
1. Klicken Sie **linken** auf „Zugriff“.
1. Wählen Sie in **Dropdown** Liste „Zugriffsebene“ die Zugriffsebene **Systemadministrator** aus.

   Abhängig von den Änderungen in Ihrem System kann sich der Name dieser Zugriffsebene geändert haben.

1. Klicken Sie **Änderungen speichern.**

   Der Benutzer verfügt jetzt über vollständige Systemadministratorrechte im System.

## Zugriff eines Workfront-Administrators im Vergleich zum Zugriff eines Planbenutzers mit Administratorrechten  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

Die beiden folgenden Tabellen zeigen den Unterschied zwischen den Zugriffsrechten einer Benutzerin oder eines Benutzers mit einer Workfront-Systemadministrator-Zugriffsebene und denen einer Benutzerin oder eines Benutzers mit einer Planlizenz mit einigen Administratorrechten.

Workfront-Admins können alle Objekte im System anzeigen (unabhängig davon, wer sie erstellt hat), neue erstellen und vorhandene ändern oder löschen. Sie haben vollen Zugriff auf alle Objekte im System.

Benutzer mit einer Planlizenz, die Funktionen in einem Bereich bearbeiten können, haben vollen Zugriff auf die Funktionen in diesem Bereich.

>[!NOTE]
>
>Benutzende mit einer Planlizenz, die als Gruppenadministratoren bezeichnet sind, können einige der Aktionen ausführen, die für Workfront-Administratoren zulässig sind. Sie dürfen diese Aktionen nur für die von ihnen verwalteten Gruppen, deren Untergruppen und die Benutzenden in diesen Gruppen und Untergruppen ausführen. Weitere Informationen finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Zugang zum Setup-Bereich](#access-to-the-setup-area)
* [Zugriff auf Objekte](#access-to-objects)

### Zugang zum Setup-Bereich {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Bereich/Objekt</th> 
   <th>Workfront-Administrator </th> 
   <th>Benutzer mit Plan-Lizenz und einigen Administratorrechten</th> 
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
   <td>Projektvoreinstellungen: Prioritäten</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Schweregrade</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Projektvoreinstellungen: Wechselkurse</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Prozesse: Genehmigungen</td> 
   <td> <p>Vollständiger Zugriff</p> </td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Prozesse: Meilensteinpfade</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Benutzerdefinierte Formulare</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Benutzerdefinierte Formulare verwalten, die sie erstellt haben, oder benutzerdefinierte Formulare verwalten, die für sie freigegeben wurden.</p> <p>Hängen Sie benutzerdefinierte Formulare, die sie erstellt haben oder die für sie freigegeben wurden, an Objekte an, für die sie Berechtigungen verwalten oder beitragen.</p> </td> 
  </tr> 
  <tr> 
   <td>Papierkorb: Zuletzt gelöscht</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Benutzende, die Gruppenadministratoren sind, können Projekte, die von ihnen verwalteten Gruppen zugewiesen wurden, sowie Aufgaben, Probleme oder Dokumente, die mit diesen Projekten verknüpft sind, wiederherstellen.</p> </td> 
  </tr> 
  <tr> 
   <td>Papierkorb: Zuletzt wiederhergestellt</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Benutzende, die Gruppenadministratoren sind, können die Elemente sehen, die sie kürzlich wiederhergestellt haben.</td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiete</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Vorhandene Aufgabengebiete ändern, aber nicht löschen.</p> <p>Neue Aufgabengebiete hinzufügen.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Teams.</p> <p>Hinzufügen vorhandener Teams zu Benutzern beim Erstellen oder Bearbeiten von Benutzern.</p> </td> 
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
   <td> <p>Wenn der Administratorzugriff für ihre Gruppe auf der Zugriffsebene aktiviert und sie als Gruppenadministrator ernannt sind, können sie sich als Benutzer in der Gruppe, die sie verwalten, und in ihren Untergruppen anmelden. Sie können sich nicht als Systemadministrator anmelden.<br>Weitere Informationen zur Aktivierung des Administratorzugriffs für Gruppen für Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Zeitpläne</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Bearbeitung von Zeitplänen.</p> <p>Zugriff zum Hinzufügen vorhandener Zeitpläne zu anderen Benutzern auf Benutzerebene. </p> </td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle und Stunden: Arbeitszeittabellen-Profile</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff zum Zuweisen vorhandener Arbeitszeittabellen-Profile zu Benutzern auf Benutzerebene.</p> <p>Benutzende, die Gruppenadministratoren sind, können Arbeitszeittabellen-Profile für die von ihnen verwalteten Gruppen und deren Untergruppen erstellen. </p> </td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle und Stunden: Stundentypen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff zum Zuweisen von Stundentypen zu Benutzern auf Benutzerebene.</p> </td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle und Stunden: Voreinstellungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: Ereignisbenachrichtigungen</td> 
   <td>Alle aktivieren/deaktivieren</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: Erinnerungsnachrichten</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Benachrichtigungen: E-Mail-Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Bearbeitung von E-Mail-Vorlagen.</p> <p>Zugriff zum Hinzufügen vorhandener E-Mail-Vorlagen zu Erinnerungsnachrichten.</p> </td> 
  </tr> 
  <tr> 
   <td>E-Mail: automatische Erinnerungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>E-Mail: Einladungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zur Bearbeitung von E-Mail-Einladungen.</p> <p>Zugriff zum erneuten Senden von E-Mail-Einladungen an nicht registrierte Benutzer nur über die Registerkarte Personen .</p> </td> 
  </tr> 
  <tr> 
   <td>E-Mail: Setup</td> 
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
   <td> <p>Vollständiger Zugriff zum Ändern aller Zugriffsebenen.</p> <p>Die Zugriffsebenen „Systemadministrator“ und „Externe Benutzer“ können standardmäßig nicht geändert werden.</p> </td> 
   <td> <p>Kein Zugriff zur Bearbeitung von Zugriffsebenen.</p> <p>Weisen Sie anderen Benutzern eine Zugriffsebene zu, die kleiner oder gleich der Zugriffsebene der anderen Benutzer auf Benutzerebene ist.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Layout-Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Zugriff, um anderen Benutzern vorhandene Layout-Vorlagen auf Benutzerebene zuzuweisen. </p> <p>Benutzende, die als Gruppenadministratoren bestimmt sind, können Layout-Vorlagen für von ihnen verwaltete Gruppen und Untergruppen erstellen.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Aktualisierungs-Feeds</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Änderung von Aktualisierungs-Feeds.</p> <p>Zugriff zum Hinzufügen von Feldern, die bei der Bearbeitung von benutzerdefinierten Forms in den Aktualisierungs-Feeds verfolgt werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Filter</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf das Erstellen von Filtern im Bereich „Setup“.</p> <p>Zugriff zum Erstellen neuer Filter in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Ansichten</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Ansichten im Bereich „Setup“.</p> <p>Zugriff zum Erstellen neuer Ansichten in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Schnittstelle: Gruppierungen</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff zum Erstellen von Gruppierungen im Bereich „Setup“.</p> <p>Zugriff zum Erstellen neuer Gruppierungen in einer Liste von Objekten.</p> </td> 
  </tr> 
  <tr> 
   <td>Benutzeroberfläche: Listensteuerelemente</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Cloud-Anbieter</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Konfiguration von Cloud-Anbietern.</p> <p>Zugriff auf das Verknüpfen von Dokumenten mit und von Cloud-Anbietern über die Registerkarte Dokumente , nachdem die Cloud-Anbieter in Workfront integriert wurden.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Metadatenzuordnung</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>Dokumente: SharePoint-Integration</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Konfiguration einer SharePoint-Integration.</p> <p>Zugriff auf den Link von Dokumenten zu und von SharePoint über die Registerkarte Dokumente , nachdem die SharePoint-Integration mit Workfront konfiguriert wurde.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokumente: Benutzerdefinierte Integration</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Kein Zugriff auf die Konfiguration einer benutzerdefinierten Integration.</p> <p>Zugriff auf Verknüpfungen von Dokumenten zu und von Drittanbietern über die Registerkarte Dokumente , nachdem die Drittanbieter mit Workfront integriert wurden.</p> </td> 
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
   <td>System: Benutzer für SSO aktualisieren</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Kickstarts</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kein Zugriff</td> 
  </tr> 
  <tr> 
   <td>System: Diagnose</td> 
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
   <th>Benutzer mit Plan-Lizenz und einigen Administratorrechten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kalender</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Kalender verwalten, die sie erstellen und für die sie Kalender freigegeben haben.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Erstellte Dashboards verwalten und für sie freigegebene Dashboards.</td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Dokumente verwalten, die hochgeladen oder für sie freigegeben werden.</td> 
  </tr> 
  <tr> 
   <td>Probleme</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Probleme verwalten, die sie erstellen oder die für sie freigegeben wurden.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Portfolios verwalten, die sie erstellen oder die sie mit ihnen teilen. </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Programme verwalten, die sie erstellen, oder Programme, die für sie freigegeben werden.</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Projekte verwalten, die sie erstellen oder für die sie freigegeben wurden.</td> 
  </tr> 
  <tr> 
   <td>Berichte</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Berichte verwalten, die sie erstellen, oder Berichte verwalten, die für sie freigegeben werden. Anzeigen, Kopieren und Bearbeiten von Systemberichten.</td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Aufgaben verwalten, die sie erstellen oder für die sie freigegeben haben</td> 
  </tr> 
  <tr> 
   <td>Vorlagen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vorlagen verwalten, die sie erstellen oder für sie freigegeben haben</td> 
  </tr> 
  <tr> 
   <td>Arbeitszeit- tabellen</td> 
   <td>Vollständiger Zugriff</td> 
   <td>Vollständiger Zugriff</td> 
  </tr> 
  <tr> 
   <td>Benutzende</td> 
   <td>Vollständiger Zugriff</td> 
   <td> <p>Eingeschränkter Zugriff</p> <p>Sie können Benutzenden, für die sie kein Gruppenadministrator sind, oder Gruppen, die nicht öffentlich sind, keine Gruppen zuweisen.</p> <p>Benutzenden kann keine Zugriffsebene zugewiesen werden, die höher ist als die eigene Zugriffsebene.</p> <p>Wenn der Administratorzugriff für ihre Gruppe auf der Zugriffsebene aktiviert ist und sie als Gruppenadministrator für eine Gruppe vorgesehen sind, können sie das Kennwort für zurücksetzen und sich als Benutzer in der Gruppe, die sie verwalten, und in ihren Untergruppen anmelden. Sie können das Kennwort von nicht zurücksetzen und sich nicht als Systemadministrator anmelden.<br>Weitere Informationen zur Aktivierung des Administratorzugriffs für Gruppen für Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
