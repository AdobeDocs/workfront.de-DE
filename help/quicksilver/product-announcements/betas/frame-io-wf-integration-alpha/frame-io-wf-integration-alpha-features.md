---
content-type: reference
navigation-topic: betas
title: '„Native Integration von Adobe Workfront und Frame.io: Beta-Funktionen“'
description: Geplante Funktionen für die native Beta-Integration von Adobe Workfront und Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: b7a0fe333f0d8f17bc2d6c612d8cff6ee484c935
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Beta-Version der nativen Integration von Adobe Workfront und Frame.io: Funktionen und Tests

Mit dieser Integration möchten wir es Kreativen ermöglichen, in ihrem bevorzugten Tool (CC oder Frame.io) zu bleiben, um Inhalte zu erstellen und Peer Reviews durchzuführen. Gleichzeitig koordinieren die Projektmanager die Arbeit und initialisieren und überwachen den formalen Überprüfungsprozess innerhalb von Workfront. Nutzen Sie dazu die Vorteile beider Lösungen: die neuen Dokumentgenehmigungen von Workfront für die Verwaltung von Inhaltsgenehmigungen in Verbindung mit den von Frame.io bereitgestellten Funktionen zur Inhaltsüberprüfung. Zusammen bilden die neuen Dokumentgenehmigungen und Frame.io unsere neue End-to-End-Inhaltsüberprüfungs- und -genehmigungserfahrung. 

Weitere Informationen zur Funktionsweise der Betaversion und zu den Möglichkeiten zur Teilnahme finden Sie unter [Integration von Adobe Workfront und Frame.io - Beta-Version: Übersicht](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Falls Sie auf diese Seiten gestoßen sind, ohne dass Ihr Unternehmen an diesem Beta-Programm teilgenommen hat, sollten Sie die Informationen hier mit Vorsicht behandeln und sich an Ihren Workfront- oder Frame.io-Administrator wenden, um weitere Informationen zu erhalten.
>

## Demo-Video

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Einfaches Testszenario

Um die neuen Funktionen des Beta-Programms einfach testen zu können, haben wir ein neues Frame.io-Testkonto erstellt und es mit einer neuen Gruppe namens verbunden `Frame.io testing` in Ihrer bestehenden Workfront-Vorschau- oder Sandbox-Umgebung.

Um die Funktion zu testen, melden Sie sich bei Ihrer Workfront-Vorschau- oder Sandbox-Instanz an und führen Sie die folgenden Schritte aus:

1. **Koordinatoren:** Erstellen Sie in Workfront ein Projekt mit dem `Frame.io testing` Gruppe, die als Projektgruppe zugewiesen ist.

1. **Koordinatoren:** Markieren Sie in Workfront die Aufgaben, für die Kreativarbeit erforderlich ist, als Frame-aktiviert (in „Aufgabendetails„) und weisen Sie ihr Ihre Kreativen zu (weisen Sie sich auch selbst zu, wenn Sie den gesamten Workflow testen möchten).

>[!NOTE]
>
>Teilaufgaben können nicht als Frame aktiviert markiert werden.
>

1. **Koordinatoren:** Laden Sie Ihre kreative Zusammenfassung hoch und ändern Sie den Projektstatus in „Aktuell„.

1. **Kreative:** Überprüfen Sie Ihre E-Mails auf eine Einladung zum neu erstellten Frame.io-Projekt

1. **Kreative:** Klicken Sie in der Einladungs-E-Mail auf die Schaltfläche „Projekt beitreten„, um am Frame.io-Projekt teilzunehmen, den Creative Brief innerhalb des Projekts zu lesen und mit der Inhaltserstellung in Ihrem Creative Cloud-Tool Ihrer Wahl zu beginnen.

1. **Kreative:** Laden Sie die erstellten Assets in Frame.io hoch und fügen Sie sie dem verknüpften Workfront-Projekt hinzu, indem Sie eine der zugewiesenen Frame-aktivierten Aufgaben auswählen. Wählen Sie die Option aus, um die Aufgabe als abgeschlossen zu markieren.

1. **Koordinatoren:** Suchen Sie in Workfront die verknüpften Frame.io-Assets in der Frame-aktivierten Aufgabe und überprüfen Sie, ob der Aufgabenstatus in „Abgeschlossen“ geändert wurde.

1. **Koordinatoren:** Weisen Sie dem verknüpften Frame.io-Asset Validierungsverantwortliche bzw. genehmigende Personen zu. Weisen Sie sich auch selbst als genehmigende Person zu, wenn Sie den gesamten Workflow testen möchten. (Weitere Informationen zum Zuweisen von Reviews/Genehmigern finden Sie unter [Hinzufügen zusätzlicher genehmigender Personen oder Prüfer zu einem Dokument](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Stakeholder:** Zeigen Sie in Workfront Ihre Genehmigungsanfrage auf der Startseite, in den Dokumentdetails oder in der empfangenen E-Mail-Benachrichtigung an. Öffnen Sie das Asset im Viewer Frame.io, hinterlassen Sie einen Kommentar mit Feedback und treffen Sie eine Entscheidung.

1. **Koordinatoren:** In Workfront können Sie die von den Stakeholdern erstellten Kommentare im Abschnitt „Aktualisierungen“ des mit Frame.io verbundenen Dokuments sowie die Entscheidung im Abschnitt „Genehmigung“ oder im Bereich „Dokumentzusammenfassung“ anzeigen.

1. **Kreative:** Beachten Sie in Frame.io die allgemeine Genehmigungsentscheidung, die für Ihre Assets getroffen wurde.

1. **Kreative:** Wenden Sie in Frame.io die angeforderten Änderungen an, indem Sie die aktualisierte Version zum Versionsstapel des verbundenen Assets hinzufügen.

1. **Koordinatoren:** Weisen Sie innerhalb von Workfront der neu hochgeladenen Version genehmigende Personen/Prüfer zu und überwachen Sie den Fortschritt, bis diese die Genehmigung erhält.

## Detailliertes Testszenario

Für Teilnehmer, die zusätzliche Funktionen testen möchten, haben wir ein stärker involviertes Testszenario erstellt. Eine Anleitung für dieses detaillierte Testszenario können Sie hier herunterladen: [Anleitung für das detaillierte Testszenario in WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Funktionspläne

Nachstehend finden Sie Informationen zu den wichtigsten Anwendungsfällen, die wir ansprechen möchten, und zu den Funktionen, die wir derzeit planen. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Aufzählungszeichen unter einem **„Potenzielle Verbesserungen bei zukünftigen Versionen“** Abhängig vom Beta-Feedback und unseren sich weiterentwickelnden Entwicklungsplänen kann der Header in einer zukünftigen Version enthalten sein oder nicht.
>

### Workfront-Administratoren können eine Verbindung zwischen Workfront-Gruppen und Frame.io-Konten einrichten

* Innerhalb von Workfront können Sie eine Workfront-Gruppe mit einem Frame.io-Konto verbinden

* In Frame.io wird ein neues Frame.io-Team erstellt, das die verbundene Workfront-Gruppe repräsentiert (beachten Sie, dass diese Funktion nur für Kunden aktiviert wurde, die die Integration in der Produktionsumgebung verwenden. Kunden, die noch immer Tests in Sandbox oder Vorschau durchführen, müssen die Verbindung vom Adobe-Team konfigurieren.)

**Mögliche Verbesserungen in zukünftigen Versionen:**

* Trennen von Workfront-Gruppen von einem Frame.io-Konto

* Verbinden einer Workfront-Gruppe mit einem vorhandenen Frame.io-Team

### Projektkoordinatoren können konfigurieren, welche Workfront-Projekte an Frame.io gesendet werden, und die zugewiesenen Kreativen in Workfront dem Projekt in Frame.io hinzufügen lassen

* Möglichkeit, Workfront-Projekte durch Zuweisen einer mit Frame verbundenen Gruppe als Frame.io zu markieren

* Möglichkeit zum Umschalten von Aufgaben innerhalb von Workfront-Projekten als Frame-Aufgaben, wodurch wiederum Aufgabenordner innerhalb von Frame.io erstellt werden

* Wenn einem Workfront-Projekt eine Frame-verbundene Gruppe und mindestens eine Frame-fähige Aufgabe zugewiesen sind und der Workfront-Projektstatus auf „Aktuell“ gesetzt ist, wird ein entsprechendes verknüpftes Projekt in Frame erstellt. Workfront-zugewiesene Benutzende werden zum Frame-Projekt hinzugefügt und von Frame.io erhält sie eine E-Mail-Benachrichtigung

   * Benutzende und Teams, die Frame-aktivierten Workfront-Aufgaben zugewiesen wurden, werden dem Frame.io-Projekt als Mitarbeiter hinzugefügt und benachrichtigt (bei der Projekterstellung und später)

* Dokumente (Creative Briefs), die dem Projekt und den Frame-aktivierten Aufgaben hinzugefügt wurden, werden an das Frame.io-Projekt (innerhalb des entsprechenden Arbeitsordners) übertragen, wenn das Projekt erstellt wird (Trigger: Projektstatus auf „Aktuell“ festgelegt)

   * Es wird empfohlen, die Anzahl der zu einem Projekt hinzugefügten Dokumente zu begrenzen, bevor sie in Ihren Creative Briefs aktiv werden, um zu vermeiden, dass mehrere unnötige Dokumente an Frame.io gesendet werden

   * Dokumente/Aufgaben, die nach der ersten Projektsynchronisierung hinzugefügt wurden, werden nicht an Frame.io gepusht, sondern nur Benutzer/Teams

**Mögliche Verbesserungen in zukünftigen Versionen:**

* Frame-aktivierte Aufgaben können in Projektvorlagen konfiguriert werden

* Uploads neuer Versionen in Creative Briefs werden an Frame gesendet.

* Optimierte Projektsynchronisierung (Trennen von Projekten, Neusynchronisierung von Projekten und Dokumenten usw.)

### In Frame.io können Kreative erstellte Assets zur formellen Überprüfung an das Workfront-Projekt senden

* Möglichkeit, ein einzelnes Frame.io-Asset mit einem WF-Projekt oder einer Aufgabe zu verbinden. In Workfront wird ein Asset-Verweis erstellt

* Beim Hochladen neuer Versionen in Frame.io wird automatisch eine neue Dokumentversion in Workfront für Connected Assets erstellt

* Möglichkeit, die referenzierten Workfront-Aufgaben aus Frame.io als abgeschlossen zu markieren

* Falls das verbundene Workfront-Dokument gelöscht wird, bleibt es in Frame.io und kann mit derselben oder einer anderen Projektaufgabe erneut verbunden werden

**Mögliche Verbesserungen in zukünftigen Versionen:**

* Möglichkeit, mehrere Frame.io-Assets gleichzeitig an Workfront zu senden

* Zeitprotokollierung für Workfront-Projekt/-Aufgabe in Frame.io

### Projektkoordinatoren können den formalen Genehmigungsprozess Dokumenten zuweisen, die über Frame.io verknüpft sind

* Workfront-Benutzende und -Teams können zu neuen Dokumentgenehmigungen für mit Frame.io verbundene Dokumente hinzugefügt werden

* Wenn die Freigabe eines Benutzers/Teams in einem Frame-fähigen Dokument aufgehoben wird, verlieren diese auch ihren Zugriff auf das Asset im Frame.io-Viewer

**Mögliche Verbesserungen in zukünftigen Versionen:**

* Mehrere Assets als eine Überprüfung senden

* Massenzuweisung von Genehmigern/Validierern zu Workfront-Dokumenten

### Stakeholder können ihre Überprüfung und Genehmigung in Frame.io Viewer durchführen.

* Stakeholder werden benachrichtigt und können das mit dem Frame verbundene Dokument im Frame.io-Viewer anzeigen

* Auf Frame.io Viewer kann von verschiedenen Stellen in Workfront aus zugegriffen werden, z. B. von der Dokumentliste, Dokumentdetails, Workfront-Startseite

* Möglichkeit, die vorhandenen Überprüfungs- und Kommentierungsfunktionen zu nutzen, die vom Frame.io-Viewer bereitgestellt werden, der mit dem Workfront-Aktualisierungsverlauf synchronisiert wird

* Möglichkeit, innerhalb des Frame.io-Viewers eine neue Dokumentengenehmigungsentscheidung zu treffen
