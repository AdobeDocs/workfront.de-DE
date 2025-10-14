---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Vorschau 1 und 2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit den Versionen R1.1 und R1.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 19. Januar 2017 in der Vorschau-Umgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# R1 Vorschau 1 und 2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit den Versionen R1.1 und R1.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 19. Januar 2017 in der Vorschau-Umgebung verfügbar gemacht.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [R1-Versionsaktivität - Übersicht](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Projekte, Aufgaben und Probleme aus dem Papierkorb wiederherstellen 

Workfront-Admins können jetzt Projekte, Aufgaben und Probleme wiederherstellen, die in den letzten 30 Tagen gelöscht wurden. Alle mit dem Projekt, der Aufgabe oder dem Problem verknüpften Informationen werden wiederhergestellt, einschließlich Dokumente und benutzerdefinierte Daten.

Neue Optionen sind auch verfügbar, um zu konfigurieren, was mit Stunden geschieht, die für ein Projekt, eine Aufgabe oder ein Problem protokolliert werden, das gelöscht wird. Weitere Informationen finden Sie unter [Auswirkungen auf Stunden konfigurieren, in denen ein Objekt gelöscht und wiederhergestellt wird](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Weitere Informationen zum Wiederherstellen von Objekten in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Informationen zum Anzeigen von Projekten, Aufgaben und Problemen, die kürzlich wiederhergestellt wurden, finden Sie unter [Wiederhergestelltes Element anzeigen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Genehmigungsdiagramm, das die vorherigen, aktuellen und künftigen Genehmigungsschritte visuell darstellt

Wenn jetzt eine Genehmigung für ein Projekt, eine Aufgabe oder ein Problem aussteht, wird ein Diagramm angezeigt. Das Genehmigungsdiagramm zeigt den aktuellen Schritt im Genehmigungsprozess (der noch aussteht) an und ermöglicht Ihnen außerdem, frühere und künftige Genehmigungsschritte schnell anzuzeigen, ohne zur Registerkarte Genehmigungen navigieren zu müssen.

Vor dieser Änderung waren Informationen zu Genehmigungsschritten nur auf der Registerkarte Genehmigungen innerhalb des Projekts, der Aufgabe oder des Problems verfügbar und wurden nur in einer Listenansicht und nicht in einer Diagrammansicht angezeigt. (Diese Informationen sind weiterhin auf der Registerkarte Genehmigungen verfügbar und unverändert.)

Bei Projekten werden die Genehmigungsinformationen in der Kopfzeile neben dem Projekttitel angezeigt. Bei Aufgaben und Problemen werden die Genehmigungsinformationen im rechten Bedienfeld angezeigt.

Weitere Informationen finden Sie unter [Genehmigen von &#x200B;](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Arbeit genehmigen](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Zu aktualisierende Objekte konfigurieren, für die die Genehmigung aussteht

Wenn für ein Projekt, eine Aufgabe oder ein Problem die Genehmigung aussteht, können Sie jetzt konfigurieren, ob die Benutzer:

* Bearbeiten Sie das benutzerdefinierte Formular eines Projekts, einer Aufgabe oder eines Problems, für das die Genehmigung aussteht.\
  Informationen zum Konfigurieren von Projekten, Aufgaben und Problemen, die bei ausstehender Genehmigung bearbeitet werden sollen, finden Sie unter [Konfigurieren globaler Genehmigungseinstellungen](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Probleme zu einem Projekt hinzufügen, dessen Genehmigung aussteht.\
  Informationen zum Konfigurieren von Projekten, damit Benutzer Probleme hinzufügen können, wenn das Projekt noch nicht genehmigt wurde, finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Bearbeiten von Aufgaben und Problemen innerhalb eines Projekts, das noch nicht genehmigt wurde.\
  Informationen zum Konfigurieren von Projekten, damit Benutzer Aufgaben und Probleme bearbeiten können, wenn die Genehmigung für das Projekt aussteht, finden [&#x200B; unter Systemweite Projektvoreinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Vor dieser Änderung konnten Projekte, Aufgaben und Probleme, für die die Genehmigung ausstand, nicht bearbeitet werden. Außerdem konnten Probleme nicht zu Projekten hinzugefügt werden, für die die Genehmigung ausstand, und Aufgaben und Probleme konnten nicht in Projekten bearbeitet werden, für die die Genehmigung ausstand.

## Zuweisen von Layout-Vorlagen zu Gruppen

Sie können jetzt Layoutvorlagen zu Gruppen zuweisen.

Vor dieser Änderung konnten Sie Benutzern, Teams und Aufgabengebieten Layoutvorlagen zuweisen. Das Zuweisen einer Layout-Vorlage zu Gruppen hat den niedrigsten Rang bei der Zuweisungspriorität der Layout-Vorlage. 

Weitere Informationen finden Sie unter „Erstellen und Verwalten von Layout-Vorlagen“.

## Änderungen an Benutzerbenachrichtigungen für die Massenbearbeitung

Die Funktionalität zur Massenbearbeitung der Einstellungen für Benutzer-E-Mail-Benachrichtigungen wurde geändert. Wenn Sie mehrere Benutzer auswählen, um deren Benachrichtigungs-E-Mail-Einstellungen zu bearbeiten, werden nur die spezifischen Benachrichtigungen geändert, die Sie aktualisieren, für alle ausgewählten Benutzer. Alle unveränderten E-Mail-Benachrichtigungseinstellungen bleiben für alle ausgewählten Benutzer gleich, auch wenn sie sich von Benutzer zu Benutzer unterscheiden. 

Vor dieser Änderung wurden die ausgewählten E-Mail-Benachrichtigungseinstellungen gespeichert und alle anderen unveränderten Benachrichtigungseinstellungen wurden beim Speichern der Änderungen deaktiviert. 

Weitere Informationen finden Sie unter „Benutzerbenachrichtigungseinstellungen stapelweise ändern“ in [Eigene E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Das Erscheinungsbild mehrerer E-Mail-Benachrichtigungen wurde aktualisiert

Das Erscheinungsbild der folgenden E-Mail-Benachrichtigungen wurde mit einer neuen Benutzeroberfläche aktualisiert:

* Problemzuweisung
* Datumsänderungen übernehmen
* Ein Projekt, an dem ich mitarbeite, ist jetzt aktiv.
* Genehmigungsentscheidung an Interessenten
* Vorgängeraufgaben-Fertigstellung für abhängige Aufgaben
* Ausstehende Genehmigung (Projekt, Aufgabe, Probleme)
* Statusänderung in Projekten, Aufgaben, Problemen

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht.    Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [Adobe Workfront-](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Neue E-Mail-Digest-Optionen für mehrere Benachrichtigungsbereiche

Für die folgenden Benachrichtigungsbereiche wurde die Option „Täglicher Digest“ hinzugefügt:

* Informationen über Projekte, an denen ich mitwirke
* Informationen zu &quot;Projekte, die von mir gesponsert werden&quot;
* Genehmigungsinformationen
* Informationen über mir zugewiesene Arbeiten
* Kommunikation

Weitere Informationen finden Sie unter [Adobe Workfront-](../../../../workfront-basics/using-notifications/wf-notifications.md).  Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können, da die Vorschau-Sandbox die E-Mail-Adressen für alle Benutzer löscht. 

## Gruppe öffentlich machen

Wenn Sie eine Gruppe öffentlich machen, können Sie diese Gruppe jetzt Benutzenden hinzufügen, ohne Gruppeneigentümer zu sein. Sie benötigen administrativen Benutzerzugriff, um Benutzer bearbeiten zu können.

Weitere Informationen zum Veröffentlichen einer Gruppe finden Sie im Abschnitt [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) in [Erstellen einer Gruppe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Freigeben der URL eines Objekts in der Mobile App 

Sie können jetzt die URL für die folgenden Objekte in der Workfront Mobile App freigeben:

* Projekte
* Aufgaben
* Probleme
* Arbeitszeit- tabellen
* Dokumente

Sie können eine URL eines Objekts in den folgenden Anwendungen freigeben:

* Textnachricht
* E-Mail
* Speicherlaufwerk (z. B. iCloud Drive)
* Andere installierte Anwendung (z. B. Notes, Facebook)
* Sie können einen Link zum -Objekt in die Zwischenablage kopieren und später in eine andere Anwendung einfügen. 

## Kontextbezogene Hilfe beim Setup

Alle Bereiche im Setup-Menü wurden mit einem Hilfesymbol in der oberen rechten Ecke des Bereichs aktualisiert. Dieses Symbol enthält einen Link zu einem Hilfeartikel zu diesem Bereich. Einige Abschnitte in den Setup-Bereichen wurden auch mit dem Hilfesymbol aktualisiert. 

## Präzisere Ausgabensätze hinzufügen

Jetzt können Sie beim Erstellen von Ausgabentypen genauere Ausgabensätze hinzufügen. Ausgabensätze können bis zu 4 Zeichen nach der Dezimalzahl enthalten (z. B. 1,0375). Dies bedeutet, dass alle Felder, die diese Rate verwenden, präziser sein können.

Vor dieser Änderung konnten Ausgabensätze nur bis zu 2 Zeichen nach der Dezimalzahl enthalten (z. B. 1,03).

Weitere Informationen zum Erstellen von Ausgabensätzen finden Sie unter [Erstellen benutzerdefinierter Ausgabentypen](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Aufzeichnung von Webinaren der R1-Vorschau 1 und 2

Dieses Webinar wurde am 19. Januar 2017 vom Workfront Release Readiness Team vorgestellt. Dieses Webinar konzentrierte sich auf die Versionsänderungen im Jahr 2017 und behandelte neue Funktionen, die in der Vorschau getestet werden können.
