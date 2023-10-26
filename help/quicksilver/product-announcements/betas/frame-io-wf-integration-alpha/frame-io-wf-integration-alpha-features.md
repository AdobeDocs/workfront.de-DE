---
content-type: reference
navigation-topic: betas
title: 'Alpha: Funktionen der nativen Integration von Adobe Workfront und Frame.io'
description: Geplante Funktionen für die native Adobe Workfront- und Frame.io-Integration - Alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Alpha: Funktionen der nativen Integration von Adobe Workfront und Frame.io

## Anwendungsbeispiele und Funktionstests

Mit dieser Integration möchten wir es Kreativen ermöglichen, in ihrem bevorzugten Tool (CC oder Frame.io) zu bleiben, um ihre Inhaltserstellung und Peer Reviews durchzuführen, während Projektmanager die Arbeit koordinieren und den formalen Review-Prozess innerhalb von Workfront initialisieren und überwachen können. Dies lässt sich erreichen, indem die besten beider Lösungen genutzt werden: die neuen Dokumentgenehmigungen von Workfront für die Verwaltung von Inhaltsgenehmigungen in Verbindung mit den Inhaltsüberprüfungsfunktionen von Frame.io. Insgesamt werden die neuen Dokumentgenehmigungen und Frame.io unser neues durchgängiges Inhalts-Review- und Genehmigungs-Erlebnis bilden. 

Weitere Informationen zur Funktionsweise des Alpha-Alphabets und zur Teilnahme finden Sie unter [Adobe Workfront- und Frame.io-Integration - Alpha: Übersicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Falls Sie auf diese Seiten gestoßen sind, ohne dass Ihr Unternehmen an diesem Alpha-Programm teilnimmt, wenden Sie sich bitte an Ihren Workfront- oder Frame.io-Administrator, um weitere Informationen zu erhalten.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Funktionspläne

Im Folgenden finden Sie Informationen zu den wichtigsten Anwendungsfällen, die wir behandeln möchten, sowie zu den Funktionen, die wir derzeit geplant haben. <!--, along with documentation to get you started testing.-->


### Workfront-Administratoren können eine Verbindung zwischen Workfront-Gruppen und Frame.io-Konten herstellen

* _In Workfront können Sie eine Workfront-Gruppe mit einem Frame.io-Konto verbinden_

* Ein neues Frame.io-Team wird in Frame.io erstellt, das die verbundene Workfront-Gruppe darstellt.

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Trennen einer Workfront-Gruppe von einem Frame.io-Konto

* Verbinden einer Workfront-Gruppe mit einem vorhandenen Frame.io-Team

### Projektkoordinatoren können konfigurieren, welche Workfront-Projekte an Frame.io gesendet werden, und die zugewiesenen Creatives in Workfront zum Projekt in Frame.io hinzufügen.

* Möglichkeit, Workfront-Projekte durch Zuweisen einer Frame-verbundenen Gruppe als Frame.io zu markieren

* _Verbesserung: Möglichkeit, Aufgaben in Workfront-Projekten als Frame-Aufgaben umzuschalten, wodurch wiederum Aufgabenordner in Frame.io erstellt werden_

* Wenn ein Workfront-Projektstatus auf &quot;Aktuell&quot;festgelegt ist, wird ein entsprechendes vernetztes Projekt in Frame erstellt, mit Workfront verknüpfte Benutzer werden zum Frame-Projekt hinzugefügt und ihnen wird von Frame.io aus eine E-Mail-Benachrichtigung gesendet

   * Alle Workfront-Projektmitglieder (Benutzer und Teams) werden als Mitwirkende zum Frame.io-Projekt hinzugefügt (bei der Projekterstellung und späteren).

   * _Änderung: Benutzer und Teams, die Frame-aktivierten Workfront-Aufgaben zugewiesen sind, werden als Mitwirkende zum Frame.io-Projekt hinzugefügt und benachrichtigt (bei der Projekterstellung und später)_

* Dokumente (Creative Briefs), die zu projektbezogenen und Frame-aktivierten Aufgaben hinzugefügt wurden, werden beim Erstellen des Projekts in das Frame.io-Projekt (innerhalb des entsprechenden Arbeitsordners) verschoben (Trigger: Projektstatus auf &quot;Aktuell&quot;).

   * Es wird empfohlen, die Anzahl der Dokumente zu begrenzen, die Ihrem Projekt hinzugefügt werden, bevor Sie nur für kreative Briefs aktiv werden. So können Sie vermeiden, dass mehrere unnötige Dokumente an Frame.io gesendet werden.

* _Verbesserung: Benutzer/Teams, die explizit von einer Frame-aktivierten Workfront-Aufgabe nicht zugewiesen wurden, werden aus dem Frame.io-Projekt entfernt_

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Frame-aktivierte Aufgaben können für Projektvorlagen konfiguriert werden

* Neue Versionen von Uploads in kreative Briefs werden an Frame gesendet

* Optimierte Projektsynchronisierung (Trennen von Projekten, Neusynchronisieren von Projekten und Dokumenten usw.)

### In Frame.io können kreative Assets zur formalen Überprüfung an das Workfront-Projekt gesendet werden

* Möglichkeit, einzelne Frame.io-Assets mit einem WF-Projekt oder einer Aufgabe zu verbinden. Eine Asset-Referenz wird in Workfront erstellt.

* Neue Versionen in Frame.io erstellen automatisch eine neue Dokumentversion in Workfront für verbundene Assets

* _Verbesserung: Möglichkeit, die referenzierten Workfront-Aufgaben aus Frame.io als abgeschlossen zu markieren_

* _Verbesserung: Wenn das verbundene Workfront-Dokument gelöscht wird, bleibt es in Frame.io und kann mit derselben oder anderen Projektaufgabe erneut verbunden werden_

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Möglichkeit, mehrere Frame.io-Assets gleichzeitig an Workfront zu senden

* Zeitprotokollierung mit Workfront-Projekt/-Aufgabe aus Frame.io

### Projektkoordinatoren können den von Frame.io verknüpften Dokumenten den formalen Genehmigungsprozess zuweisen.

* Workfront-Benutzer und -Teams können neuen Dokumentgenehmigungen für mit Frame.io verbundene Dokumente hinzugefügt werden

* _Verbesserung: Wenn die Freigabe eines Benutzers/Teams für ein Dokument mit aktiviertem Frame aufgehoben wird, verliert er auch seinen Zugriff auf das Asset im Frame.io-Viewer_

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Senden mehrerer Assets als einzelne Überprüfung

* Massen-Zuweisung von Genehmigern/Validierern zu Workfront-Dokumenten

### Stakeholder können ihre Überprüfung und Genehmigung im Frame.io Viewer durchführen

* Interessengruppen werden benachrichtigt und können das Dokument mit Frame-Verbindung im Frame.io-Viewer anzeigen

* Der Zugriff auf den Frame.io-Viewer erfolgt über verschiedene Stellen in Workfront, z. B. Dokumentliste, Dokumentdetails, Workfront-Startseite

* Möglichkeit zur Nutzung der vorhandenen Reviews- und Kommentarfunktionen, die vom Frame.io-Viewer bereitgestellt werden und mit dem Workfront-Update-Stream synchronisiert werden

* _Möglichkeit, im Frame.io-Viewer eine neue Entscheidung über die Dokumentgenehmigung zu treffen_

### In Frame.io werden Kreative über die Gesamtentscheidung informiert, die für das verbundene Frame.io-Asset getroffen wurde.

* _Verbesserung: Der Gesamtstatus der Dokumentgenehmigung wird auf dem Asset in Frame.io angezeigt_

### Projektkoordinatoren können endgültige Assets an AEM senden

* _Verbesserung: Frame-verbundene Dokumente, einschließlich Metadaten, können mit dem vorhandenen Workfront + AEM Asset CS-Connector an AEM gesendet werden_