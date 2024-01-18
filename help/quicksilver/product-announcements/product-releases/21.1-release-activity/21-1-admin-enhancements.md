---
content-type: release-notes
keywords: notes,vierteljährlich,update
navigation-topic: product-releases
title: 21.1 Verbesserungen für Administratoren
description: Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 21.1 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1 Verbesserungen für Administratoren

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 21.1 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche des 15. Februar 2021 verfügbar sein.

Eine Liste aller in Version 21.1 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Einführung neuer Einstellungen für die Zugriffsebene für das Kopieren von Projekten

Damit Sie als Systemadministrator mehr Kontrolle darüber haben, was Planer mit einem Projekt tun können, haben wir den Bearbeitungszugriff auf Projekte auf Zugriffsebene detaillierter gestaltet, indem eine neue Einstellung eingeführt wurde, mit der Sie die Möglichkeit zum Kopieren von Projekten aktivieren oder deaktivieren können. Vor dieser Änderung hatten Benutzer, die den Zugriff von Benutzern auf Projekte bearbeiten aktiviert hatten, automatisch Zugriff auf das Kopieren. Mit der neuen Funktion können Sie jemandem Zugriff auf Projekte gewähren, ohne notwendigerweise darauf zugreifen zu müssen, indem Sie die neue Einstellung Kopieren deaktivieren.

Wenn Ihre Benutzer vor dieser Änderung Zugriff auf Projekte bearbeiten in ihrer Zugriffsebene hatten, wird diese Einstellung automatisch aktiviert, wenn diese Funktion veröffentlicht wird.

Informationen zur Zugriffsebene des Plans finden Sie unter [Projektzugriff gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Informationen zum Kopieren eines Projekts finden Sie unter [Projekt kopieren](../../../manage-work/projects/manage-projects/copy-project.md).

Diese Funktion ist jetzt im [Administratorgrundlagen im neuen Workfront-Erlebnis, Teil 1: Benutzerorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Lernpfad auf Workfront One.

## Wählen Sie in einem benutzerdefinierten Formular für ein Objekt alle Elemente in einem Dropdown-Feld mit Mehrfachauswahl aus

>[!NOTE]
>
>Diese Funktion ist derzeit nicht verfügbar, wenn Sie eine neue Anforderung senden.

Wenn Sie auf der Detailseite für ein Objekt ein Dropdown-Feld mit mehreren Auswahlen in einem benutzerdefinierten Formular ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Optionen auswählen müssen.

Informationen zum Bearbeiten von Daten in einem benutzerdefinierten Formular finden Sie unter [Informationen in benutzerdefinierten Formularfeldern bearbeiten](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Neuberechnen aller benutzerdefinierten Formularfelder für ein Objekt

Jetzt ist es einfacher sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern für ein Objekt aktuell sind. Mit der neuen Menüoption Ausdrücke neu berechnen können Sie schnell alle Daten in diesen Feldern neu berechnen.

Dies ist besonders nützlich, wenn jemand Daten in einem anderen Objekt bearbeitet, auf das in einem berechneten benutzerdefinierten Feld in Ihrem Objekt verwiesen wird.

Zuvor mussten Benutzer Umgehungslösungen verwenden, um sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern aktuell waren. Beispielsweise bearbeiteten sie das Objekt zusammen mit anderen Objekten, um die Neuberechnungsoption zu verwenden, die für die Massenbearbeitung verfügbar ist.

Weitere Informationen finden Sie unter [Informationen in benutzerdefinierten Formularfeldern bearbeiten](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Entsperren von Aufgaben- und Problemeinstellungen für Gruppenadministratoren

>[!NOTE]
>
>Bis zum 24. Juni 2021 war dies im Rahmen eines stufenweisen Rollouts nur für Kunden verfügbar, die Projektvoreinstellungen für Gruppen entsperren können. Jetzt ist sie für alle Kunden verfügbar.

Adobe Workfront-Administratoren können Gruppenadministratoren jetzt mehr Autonomie gewähren, indem sie einzelne Aufgaben entsperren und Voreinstellungen festlegen. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen so konfigurieren, dass sie den individuellen Anforderungen und internen Prozessen jeder Gruppe gerecht werden.

Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Diese Funktion ist jetzt im [Administratorgrundlagen im neuen Workfront-Erlebnis, Teil 2: Projekteinrichtung](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) Lernpfad auf Workfront One.

## Einstellungen für Zugriffsebene separat für Portfolios und Programme konfigurieren

Jetzt ist es einfacher, den Benutzerzugriff auf Portfolios und Programme zu verwalten, da Sie die Einstellungen für die Zugriffsebene separat konfigurieren können.

Zuvor wurden die Einstellungen für die Zugriffsebene für Portfolios und Programme kombiniert. Dies bedeutet, dass Sie die Zugriffseinstellungen für Programme nicht konfigurieren konnten, ohne sie für Portfolios auf die gleiche Weise zu konfigurieren, und das Gleiche galt umgekehrt.

Informationen zum Konfigurieren einer Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Informationen zu den Zugriffseinstellungen, die Sie für Programme und Portfolios konfigurieren können, finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Diese Funktion ist jetzt im [Administratorgrundlagen im neuen Workfront-Erlebnis, Teil 1: Benutzerorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Lernpfad auf Workfront One.

## Auswählen aller Kontrollkästchen in einer Reihe beim Bearbeiten von Informationen in einem benutzerdefinierten Formular

>[!NOTE]
>
>Diese Funktion ist derzeit nicht verfügbar, wenn Sie eine neue Anforderung senden.

Wenn Sie auf der Detailseite für ein Objekt ein Feld mit benutzerdefiniertem Formular mit Kontrollkästchen ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Kontrollkästchen auswählen müssen.

Diese Option wird nur angezeigt, wenn das Feld mehr als zwei Kontrollkästchen enthält.

Weitere Informationen finden Sie unter [Informationen in benutzerdefinierten Formularfeldern bearbeiten](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Konfigurieren Ihrer Workfront-E-Mail-Zulassungsliste

Um Ihre Daten besser zu schützen, können Sie jetzt eine E-Mail-Domain-Zulassungsliste für folgende Zwecke verwenden:

* Steuern, wohin Workfront-E-Mails gehen können, wenn sie in Workfront gespeicherte Berichte oder Dokumente enthalten
* E-Mail-Domains steuern können sich in der E-Mail-Adresse befinden, die Benutzer in ihrem Benutzerprofil angeben können.

Wenn Sie beispielsweise sensible Daten schützen möchten, z. B. einen Bericht, der Ihre risikobehafteten Kunden auflistet, können Sie nur Ihre interne E-Mail-Domäne oder Domänen in die E-Mail-Zulassungsliste aufnehmen. Auf diese Weise können Benutzer diesen Bericht (oder einen anderen Workfront-Bericht) nicht an eine externe E-Mail-Adresse senden.

Weitere Informationen finden Sie im Abschnitt . [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) im Artikel [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zuweisen eines Gruppenadministrators für eine Untergruppe

Um die unabhängige Funktionsweise der Ebenen Ihres Unternehmens zu vereinfachen, haben wir die Möglichkeit hinzugefügt, einen Gruppenadministrator einer Untergruppe zuzuweisen. Nun können Sie sicherstellen, dass Sie die Verwaltung von Untergruppen an die richtigen Personen delegieren.

Zuvor konnte nur eine Gruppe der obersten Ebene Gruppenadministratoren haben, und diese Administratoren haben alle Untergruppen unterhalb der Gruppe der obersten Ebene verwaltet.

Weitere Informationen finden Sie im Abschnitt . [Gruppenadministratoren für Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) im Artikel [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Diese Funktion ist jetzt im [Administratorgrundlagen im neuen Workfront-Erlebnis, Teil 1: Benutzerorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Lernpfad auf Workfront One.

## Ereignisbenachrichtigungen für Gruppen konfigurieren

>[!NOTE]
>
>Verfügbar als Teil eines schrittweisen Rollouts nur für Kunden, die Projektvoreinstellungen für Gruppen entsperren können. Dies schließt alle Kunden mit Cluster 4 und 6 sowie eine geringe Anzahl von Kunden mit anderen Clustern ein. Diese Anmerkung wird aktualisiert, sobald die Funktion für weitere Cluster verfügbar ist.

Workfront-Administratoren können nun Gruppenadministratoren mehr Autonomie gewähren, indem sie ihnen die Möglichkeit geben, Ereignisbenachrichtigungen für ihre Top-Level-Gruppen zu konfigurieren. Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen von ihrer obersten übergeordneten Gruppe.

Zuvor waren Ereignisbenachrichtigungen nur von einem Workfront-Administrator auf Systemebene konfigurierbar, was bedeutet, dass alle Gruppen denselben Satz von Ereignisbenachrichtigungen verwenden mussten.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Diese Funktion ist jetzt im [Administratorgrundlagen im neuen Workfront-Erlebnis, Teil 1: Benutzerorganisation](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Lernpfad auf Workfront One.

Diese Funktion ist jetzt im [E-Mail- und In-App-Benachrichtigungen im neuen Workfront-Erlebnis](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) Lernpfad auf Workfront One.

## Arbeiten mit Gruppenprojekten und Genehmigungsprozessen im Bereich &quot;Gruppen&quot;

Wenn Sie Gruppenadministrator sind, können Sie die Projekte und Genehmigungsprozesse Ihrer Gruppe einfach anzeigen und verwenden, nachdem sie im Bereich Gruppen aufgelistet sind. Auf der Hauptseite einer Gruppe haben Sie folgende Möglichkeiten:

* Klicken Sie im linken Menü auf Projekte , um die Projekte der Gruppe anzuzeigen und neue für die Gruppe zu erstellen. Wenn ein ausgewähltes Projekt für Sie freigegeben wurde, können Sie es mithilfe der Schaltflächen in der Symbolleiste bearbeiten, exportieren, kopieren oder löschen.

  Weitere Informationen finden Sie unter [Erstellen und Ändern von Gruppenprojekten](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Klicken Sie im linken Menü auf Validierungen , um alle mit der Gruppe verknüpften Validierungsprozesse anzuzeigen und zu verwalten.

  Weitere Informationen finden Sie unter [Validierungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Diese Funktion steht auch Workfront-Administratoren zur Verfügung.

## Anzahl der in einer Gruppe verwendeten und zugewiesenen Lizenzen anzeigen

Um festzustellen, wie gut Ihre Lizenzen verteilt sind, können Sie jetzt die Anzahl der Lizenzen anzeigen, die in einer Gruppe verwendet werden, sowie alle Untergruppen darunter.

Wenn Sie eine Gruppe der obersten Ebene verwalten, können Sie sowohl die Anzahl der in einer Gruppe verwendeten Lizenzen (und deren Untergruppen) als auch die maximale Anzahl der der Gruppe zugewiesenen Lizenzen anzeigen.

Weitere Informationen finden Sie unter [Anzahl der einer Gruppe zugewiesenen und verwendeten Lizenzen im neuen Adobe Workfront-Erlebnis anzeigen](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

