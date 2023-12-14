---
content-type: reference
navigation-topic: betas
title: 'Alpha: Funktionen der nativen Integration von Adobe Workfront und Frame.io'
description: Geplante Funktionen für die native Adobe Workfront- und Frame.io-Integration - Alpha
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 4ab78cff65141636e9e2c95526d68face1f278ba
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 0%

---

# Alpha: Funktionen und Tests der nativen Integration von Adobe Workfront und Frame.io

Mit dieser Integration möchten wir es Kreativen ermöglichen, in ihrem bevorzugten Tool (CC oder Frame.io) zu bleiben, um ihre Inhaltserstellung und Peer Reviews durchzuführen, während Projektmanager die Arbeit koordinieren und den formalen Review-Prozess innerhalb von Workfront initialisieren und überwachen können. Dies lässt sich erreichen, indem die besten beider Lösungen genutzt werden: die neuen Dokumentgenehmigungen von Workfront für die Verwaltung von Inhaltsgenehmigungen in Verbindung mit den Inhaltsüberprüfungsfunktionen von Frame.io. Insgesamt werden die neuen Dokumentgenehmigungen und Frame.io unser neues durchgängiges Inhalts-Review- und Genehmigungs-Erlebnis bilden. 

Weitere Informationen zur Funktionsweise des Alpha-Alphabets und zur Teilnahme finden Sie unter [Adobe Workfront- und Frame.io-Integration - Alpha: Übersicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)

>[!NOTE]
>
>Falls Sie auf diese Seiten gestoßen sind, ohne dass Ihr Unternehmen an diesem Alpha-Programm teilnimmt, wenden Sie sich bitte an Ihren Workfront- oder Frame.io-Administrator, um weitere Informationen zu erhalten.
>

## Grundlegendes Testszenario

Damit Sie die neuen Funktionen des Alpha-Programms einfach testen können, haben wir ein neues Frame.io-Testkonto erstellt und mit einer neuen Gruppe namens `Frame.io alpha testing` in Ihrer vorhandenen Workfront-Vorschau- oder Sandbox-Umgebung.

Um die Funktion zu testen, melden Sie sich bei Ihrer Workfront-Vorschau- oder Sandbox-Instanz an und führen Sie die folgenden Schritte aus:

1. **Koordinatoren:** Erstellen Sie in Workfront ein Projekt mit der `Frame.io alpha testing` als Projektgruppe zugewiesen wurde.

1. **Koordinatoren:** Markieren Sie in Workfront die Aufgaben, für die kreative Arbeit erforderlich ist, als &quot;frame-fähig&quot;(in Aufgabendetails) und weisen Sie ihr Ihre kreativen Inhalte zu (weisen Sie sich selbst zu, wenn Sie den gesamten Workflow testen möchten).

>[!NOTE]
>
>Unteraufgaben können nicht als Frame aktiviert markiert werden.
>

1. **Koordinatoren:** Laden Sie Ihre Kreativbeschreibung hoch und ändern Sie den Projektstatus in &quot;Aktuell&quot;.

1. **Kreative:** Prüfen Sie Ihre E-Mails auf eine Einladung zum neu erstellten Frame.io-Projekt

1. **Kreative:** Klicken Sie in der Einladungs-E-Mail auf die Schaltfläche &quot;Projekt beitreten&quot;, um dem Projekt Frame.io beizutreten, überprüfen Sie die Kreativbeschreibung innerhalb des Projekts und beginnen Sie mit der Inhaltserstellung in Ihrem gewünschten Creative Cloud-Tool.

1. **Kreative:** Laden Sie die erstellten Assets in Frame.io hoch und fügen Sie sie zum verknüpften Workfront-Projekt hinzu, indem Sie eine der zugewiesenen Frame-aktivierten Aufgaben auswählen. Wählen Sie die Option aus, um die Aufgabe als abgeschlossen zu markieren.

1. **Koordinatoren:** Suchen Sie in Workfront die verknüpften Frame.io-Assets in der Frame-aktivierten Aufgabe und vergewissern Sie sich, dass der Status der Aufgabe in &quot;Abgeschlossen&quot;geändert wurde.

1. **Koordinatoren:** Weisen Sie dem verknüpften Frame.io-Asset Reviewer/Genehmiger zu. Weisen Sie sich auch als Genehmiger zu, wenn Sie den gesamten Workflow testen möchten. (Weitere Informationen zum Zuweisen von Überprüfungen/Genehmigern finden Sie unter [Hinzufügen zusätzlicher Genehmiger oder Validierer zu einem Dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Interessenträger:** Zeigen Sie Ihre Genehmigungsanfrage in Workfront in Startseite, Dokumentdetails oder in der erhaltenen E-Mail-Benachrichtigung an. Öffnen Sie das Asset im Frame.io-Viewer, lassen Sie einen Kommentar mit Feedback und treffen Sie eine Entscheidung.

1. **Koordinatoren:** Sehen Sie sich in Workfront die von den Interessenträgern erstellten Kommentare im Abschnitt Updates des Dokuments mit Frame.io an, sowie die Entscheidung im Bereich Genehmigung oder in der Dokumentzusammenfassung.

1. **Kreative:** Beachten Sie in Frame.io die globale Genehmigungsentscheidung, die für Ihre Assets getroffen wurde.

1. **Kreative:** Wenden Sie in Frame.io die angeforderten Änderungen an, indem Sie die aktualisierte Version zum Versionsstapel des verbundenen Assets hinzufügen.

1. **Koordinatoren:** Weisen Sie in Workfront Genehmiger/Validierer der neu hochgeladenen Version zu und überwachen Sie den Fortschritt, bis die Abmeldung erreicht ist.

## Detailliertes Testszenario

Für Teilnehmer, die zusätzliche Funktionen testen möchten, haben wir ein stärker involviertes Testszenario erstellt. Eine Anleitung für dieses detaillierte Testszenario können Sie hier herunterladen: [WF + Frame.io - Anleitung zum detaillierten Testszenario](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## Funktionspläne

Im Folgenden finden Sie Informationen zu den wichtigsten Anwendungsfällen, die wir behandeln möchten, sowie zu den Funktionen, die wir derzeit geplant haben. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Aufzählungszeichen unter einem **&quot;Potenzielle Verbesserungen in zukünftigen Versionen&quot;** -Kopfzeile kann in einer zukünftigen Version enthalten sein oder auch nicht, je nach Alpha-Feedback und unseren sich entwickelnden Entwicklungsplänen.
>

### Workfront-Administratoren können eine Verbindung zwischen Workfront-Gruppen und Frame.io-Konten herstellen

* In Workfront können Sie eine Workfront-Gruppe mit einem Frame.io-Konto verbinden

* In Frame.io wird ein neues Frame.io-Team erstellt, das die verbundene Workfront-Gruppe repräsentiert (Bitte beachten Sie, dass diese Funktion nur für Kunden aktiviert wurde, die die Integration in der Produktionsumgebung verwenden. Bei Kunden, die noch auf Sandbox oder Vorschau testen, wird die Verbindung vom Adobe-Team konfiguriert.)

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Trennen einer Workfront-Gruppe von einem Frame.io-Konto

* Verbinden einer Workfront-Gruppe mit einem vorhandenen Frame.io-Team

### Projektkoordinatoren können konfigurieren, welche Workfront-Projekte an Frame.io gesendet werden, und die zugewiesenen Creatives in Workfront zum Projekt in Frame.io hinzufügen.

* Möglichkeit, Workfront-Projekte durch Zuweisen einer Frame-verbundenen Gruppe als Frame.io zu markieren

* Möglichkeit, Aufgaben innerhalb von Workfront-Projekten als Frame-Aufgaben umzuschalten, wodurch wiederum Aufgabenordner in Frame.io erstellt werden

* Wenn einem Workfront-Projekt eine Gruppe mit Frame-Anschluss zugewiesen ist und mindestens eine Aufgabe mit Frame-Unterstützung zugewiesen ist, wird bei der Festlegung des Workfront-Projektstatus auf Aktuell ein entsprechendes verbundenes Projekt in Frame erstellt, dem Frame-Projekt von Workfront zugewiesene Benutzer hinzugefügt und ihnen von Frame.io aus eine E-Mail-Benachrichtigung gesendet

   * Benutzer und Teams, die Frame-aktivierten Workfront-Aufgaben zugewiesen sind, werden als Mitwirkende zum Frame.io-Projekt hinzugefügt und benachrichtigt (bei der Projekterstellung und später)

* Dokumente (Creative Briefs), die zu projektbezogenen und Frame-aktivierten Aufgaben hinzugefügt wurden, werden beim Erstellen des Projekts in das Frame.io-Projekt (innerhalb des entsprechenden Arbeitsordners) verschoben (Trigger: Projektstatus auf &quot;Aktuell&quot;).

   * Es wird empfohlen, die Anzahl der Dokumente zu begrenzen, die Ihrem Projekt hinzugefügt werden, bevor Sie nur für kreative Briefs aktiv werden. So können Sie vermeiden, dass mehrere unnötige Dokumente an Frame.io gesendet werden.

   * Dokumente/Aufgaben, die nach der ersten Projektsynchronisierung hinzugefügt wurden, werden nicht an Frame.io gesendet, sondern nur Benutzer/Teams

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Frame-aktivierte Aufgaben können für Projektvorlagen konfiguriert werden

* Neue Versionen von Uploads in kreative Briefs werden an Frame gesendet

* Optimierte Projektsynchronisierung (Trennen von Projekten, Neusynchronisieren von Projekten und Dokumenten usw.)

### In Frame.io können kreative Assets zur formalen Überprüfung an das Workfront-Projekt gesendet werden

* Möglichkeit, einzelne Frame.io-Assets mit einem WF-Projekt oder einer Aufgabe zu verbinden. Eine Asset-Referenz wird in Workfront erstellt.

* Neue Versionen in Frame.io erstellen automatisch eine neue Dokumentversion in Workfront für verbundene Assets

* Möglichkeit, die referenzierten Workfront-Aufgaben in Frame.io als abgeschlossen zu markieren

* Wenn das verbundene Workfront-Dokument gelöscht wird, bleibt es in Frame.io und kann mit derselben oder anderen Projektaufgabe erneut verbunden werden

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Möglichkeit, mehrere Frame.io-Assets gleichzeitig an Workfront zu senden

* Zeitprotokollierung mit Workfront-Projekt/-Aufgabe aus Frame.io

### Projektkoordinatoren können den von Frame.io verknüpften Dokumenten den formalen Genehmigungsprozess zuweisen.

* Workfront-Benutzer und -Teams können neuen Dokumentgenehmigungen für mit Frame.io verbundene Dokumente hinzugefügt werden

* Wenn die Freigabe eines Benutzers/Teams für ein Dokument mit aktiviertem Frame aufgehoben wird, verliert der Benutzer auch seinen Zugriff auf das Asset im Frame.io-Viewer

**Potenzielle Verbesserungen in zukünftigen Versionen:**

* Senden mehrerer Assets als einzelne Überprüfung

* Massen-Zuweisung von Genehmigern/Validierern zu Workfront-Dokumenten

### Stakeholder können ihre Überprüfung und Genehmigung im Frame.io Viewer durchführen

* Interessengruppen werden benachrichtigt und können das Dokument mit Frame-Verbindung im Frame.io-Viewer anzeigen

* Der Zugriff auf den Frame.io-Viewer erfolgt über verschiedene Stellen in Workfront, z. B. Dokumentliste, Dokumentdetails, Workfront-Startseite

* Möglichkeit zur Nutzung der vorhandenen Reviews- und Kommentarfunktionen, die vom Frame.io-Viewer bereitgestellt werden und mit dem Workfront-Update-Stream synchronisiert werden

* Möglichkeit, im Frame.io-Viewer eine neue Entscheidung über die Dokumentgenehmigung zu treffen
