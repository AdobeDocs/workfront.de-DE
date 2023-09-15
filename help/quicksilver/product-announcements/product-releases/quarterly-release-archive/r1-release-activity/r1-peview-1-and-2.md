---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Vorschau 1 und 2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit den R1.1- und R1.2-Versionen verfügbar sind. Die Funktionalität auf dieser Seite wurde am 19. Januar 2017 in der Vorschau-Umgebung bereitgestellt.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 2%

---

# R1 Vorschau 1 und 2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit den R1.1- und R1.2-Versionen verfügbar sind. Die Funktionalität auf dieser Seite wurde am 19. Januar 2017 in der Vorschau-Umgebung bereitgestellt.

Eine Liste aller in R1 vorgenommenen Änderungen finden Sie unter [Übersicht über die Release-Aktivität R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Wiederherstellen von Projekten, Aufgaben und Problemen aus dem Papierkorb 

Workfront-Administratoren können jetzt Projekte, Aufgaben und Probleme wiederherstellen, die innerhalb der letzten 30 Tage gelöscht wurden. Alle mit dem Projekt, der Aufgabe oder dem Problem verknüpften Informationen, einschließlich Dokumenten und benutzerdefinierten Daten, werden wiederhergestellt.

Es stehen auch neue Optionen zur Konfiguration von Stunden zur Verfügung, die mit einem Projekt, einer Aufgabe oder einem Problem protokolliert werden, das gelöscht wird. Weitere Informationen finden Sie unter [Konfigurieren der Auswirkungen auf die Stunden, in denen ein Objekt gelöscht und wiederhergestellt wird](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Weitere Informationen zum Wiederherstellen von Objekten in Workfront finden Sie unter [Gelöschte Elemente wiederherstellen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Informationen zum Anzeigen von Projekten, Aufgaben und Problemen, die kürzlich wiederhergestellt wurden, finden Sie unter [Wiederhergestelltes Element anzeigen](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Genehmigungsdiagramm zeigt visuelle Darstellung der vorherigen, aktuellen und künftigen Genehmigungsschritte

Wenn nun eine Genehmigung für ein Projekt, eine Aufgabe oder ein Problem aussteht, wird ein Diagramm angezeigt. Das Genehmigungsdiagramm zeigt den aktuellen Schritt im Genehmigungsprozess (der ausstehend ist) und ermöglicht es Ihnen, schnell die vorherigen und künftigen Genehmigungsschritte anzuzeigen, ohne zur Registerkarte Genehmigungen zu navigieren.

Vor dieser Änderung waren Informationen zu Validierungsschritten nur auf der Registerkarte Validierungen des Projekts, der Aufgabe oder des Problems verfügbar und wurden nur in einer Listenansicht und nicht in einer Diagrammansicht angezeigt. (Diese Informationen sind weiterhin verfügbar und bleiben im Tab Genehmigungen unverändert.)

Bei Projekten werden die Genehmigungsinformationen in der Kopfzeile neben dem Projekttitel angezeigt. Bei Aufgaben und Problemen werden die Validierungsinformationen im rechten Bereich angezeigt.

Weitere Informationen finden Sie unter [Validierung der Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Validierung der Arbeit](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Zu aktualisierende Objekte konfigurieren, die noch nicht genehmigt wurden

Wenn die Genehmigung eines Projekts, einer Aufgabe oder eines Problems aussteht, können Sie jetzt konfigurieren, ob Benutzer:

* Bearbeiten Sie das benutzerdefinierte Formular eines Projekts, einer Aufgabe oder eines Problems, für das die Genehmigung aussteht.\
  Informationen zum Konfigurieren von Projekten, Aufgaben und Problemen, die bei ausstehender Genehmigung bearbeitet werden sollen, finden Sie unter [Globale Genehmigungseinstellungen konfigurieren](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Fügen Sie einem Projekt, für das die Genehmigung aussteht, Probleme hinzu.\
  Informationen dazu, wie Sie Projekte so konfigurieren, dass Benutzer Probleme hinzufügen können, wenn das Projekt noch nicht genehmigt wurde, finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Bearbeiten Sie Aufgaben und Probleme in einem Projekt, für das die Genehmigung aussteht.\
  Informationen dazu, wie Sie Projekte so konfigurieren, dass Benutzer Aufgaben und Probleme bearbeiten können, wenn das Projekt noch nicht genehmigt ist, finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Vor dieser Änderung konnten Projekte, Aufgaben und Probleme, die noch nicht genehmigt wurden, nicht bearbeitet werden. Außerdem konnten Probleme nicht zu Projekten hinzugefügt werden, für die eine Genehmigung aussteht, und Aufgaben und Probleme konnten nicht in Projekten bearbeitet werden, für die eine Genehmigung aussteht.

## Zuweisen von Layoutvorlagen zu Gruppen

Sie können nun Layoutvorlagen Gruppen zuweisen.

Vor dieser Änderung können Sie Benutzern, Teams und Auftragsprofilen Layoutvorlagen zuweisen. Das Zuweisen einer Layoutvorlage zu Gruppen hat bei der Zuweisungspriorität von Layoutvorlagen den niedrigsten Rang. 

Weitere Informationen finden Sie unter &quot;Erstellen und Verwalten von Layoutvorlagen&quot;.

## Änderungen an Massenbearbeitungs-Benutzerbenachrichtigungen

Die Funktion wurde bei der Massenbearbeitung von E-Mail-Benachrichtigungseinstellungen für Benutzer geändert. Wenn Sie mehrere Benutzer auswählen, um ihre Benachrichtigungs-E-Mail-Einstellungen zu bearbeiten, werden nur die spezifischen Benachrichtigungen, die Sie aktualisieren, für alle ausgewählten Benutzer geändert. Alle unveränderten E-Mail-Benachrichtigungseinstellungen bleiben für alle ausgewählten Benutzer gleich, auch wenn sie sich von Benutzer zu Benutzer unterscheiden. 

Vor dieser Änderung wurden die von Ihnen ausgewählten E-Mail-Benachrichtigungseinstellungen gespeichert und alle anderen unveränderten Benachrichtigungseinstellungen beim Speichern der Änderungen deaktiviert. 

Weitere Informationen finden Sie unter &quot;Ändern der Einstellungen für Benutzerbenachrichtigungen in Stapeln&quot;in [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aktualisiertes Erscheinungsbild mehrerer E-Mail-Benachrichtigungen

Das Erscheinungsbild der folgenden E-Mail-Benachrichtigungen wurde mit einer neuen Benutzeroberfläche aktualisiert:

* Zuweisung eines Problems
* Änderungen am Zustimmungsdatum
* Ein Projekt, an dem ich mitarbeite, ist jetzt aktiv.
* Genehmigungsentscheidung für interessierte Parteien
* Fertigstellung einer vorherigen Aufgabe für Aufgabenabhängigkeiten
* Ausstehende Genehmigung (Projekt, Aufgabe, Probleme)
* Statusänderung bei Projekten, Aufgaben, Problemen

Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können, da die Vorschau-Sandbox die E-Mail-Adressen aller Benutzer löscht.    Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie unter [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Neue E-Mail-Digest-Optionen für mehrere Benachrichtigungsbereiche

In den folgenden Benachrichtigungsbereichen wurde die Option &quot;Tägliche Zusammenfassung&quot;hinzugefügt:

* Informationen zu Projekten, die ich verwende
* Informationen zu &quot;Projekte, die von mir gesponsert werden&quot;
* Genehmigungsinformationen
* Informationen über mir zugewiesene Arbeiten
* Kommunikation

Weitere Informationen finden Sie unter [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md).  Denken Sie daran, die mit Ihrem Konto verknüpfte E-Mail-Adresse zu aktualisieren, um diese Funktion testen zu können, da die Vorschau-Sandbox die E-Mail-Adressen aller Benutzer löscht. 

## Als Gruppe veröffentlichen

Wenn Sie eine Gruppe öffentlich machen, können Sie diese Gruppe jetzt Benutzern hinzufügen, ohne Gruppeninhaber zu sein. Sie müssen über Administratorrechte für Benutzer verfügen, um Benutzer bearbeiten zu können.

Weitere Informationen zum Veröffentlichen einer Gruppe finden Sie unter [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) Abschnitt in [Gruppe erstellen](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## URL eines Objekts in der Mobile App freigeben 

Sie können die URL jetzt für die folgenden Objekte in der mobilen Workfront-App freigeben:

* Projekte
* Aufgaben
* Probleme
* Arbeitszeittabellen
* Dokumente

Sie können eine URL eines Objekts in den folgenden Anwendungen freigeben:

* Textnachricht
* E-Mail
* Speicherlaufwerk (z. B. iCloud Drive)
* Eine andere installierte Anwendung (z. B. Notizen, Facebook)
* Sie können einen Link zum Objekt in die Zwischenablage kopieren und später in eine andere Anwendung einfügen. 

## Kontextbezogene Hilfe bei der Einrichtung

Alle Bereiche im Menü &quot;Einrichtung&quot;wurden mit einem Hilfesymbol in der oberen rechten Ecke des Bereichs aktualisiert. Dieses Symbol enthält einen Link zu einem Hilfe-Site-Artikel zu diesem Bereich. Einige Abschnitte in den Einrichtungsbereichen wurden ebenfalls mit dem Hilfesymbol aktualisiert. 

## Hinzufügen präziserer Ausgabensätze

Jetzt können Sie bei der Erstellung von Ausgabetypen genauere Ausgabenraten hinzufügen. Die Ausgabenzahlen können bis zu 4 Zeichen nach der Dezimalstelle enthalten (z. B. 1.0375). Das bedeutet, dass alle Felder, die diese Rate verwenden, präziser sein können.

Vor dieser Änderung konnten die Ausgabenraten nur bis zu 2 Zeichen nach der Dezimalstelle (z. B. 1,03) enthalten.

Weitere Informationen zur Erstellung von Ausgabenraten finden Sie unter [Benutzerdefinierte Ausgabentypen erstellen](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1 Vorschau 1 und 2 Release Webinar-Aufzeichnung

Dieses Webinar wurde vom Workfront Release Readiness Team am 19. Januar 2017 vorgestellt. Dieses Webinar konzentrierte sich auf die Änderungen der Version 2017 und umfasste neue Funktionen, die in der Vorschau getestet werden können.
