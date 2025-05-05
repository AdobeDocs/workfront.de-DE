---
content-type: release-notes
keywords: Anmerkungen,vierteljährlich,aktualisieren
navigation-topic: product-releases
title: 21.1 Verbesserungen für Administratoren
description: Auf dieser Seite werden alle mit der Version 21.1 vorgenommenen Administrator-Verbesserungen für die Vorschau -Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 15. Februar 2021 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1 Verbesserungen für Administratoren

Auf dieser Seite werden alle mit der Version 21.1 vorgenommenen Administrator-Verbesserungen für die Vorschau -Umgebung beschrieben. Diese Verbesserungen werden in der Woche vom 15. Februar 2021 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 21.1 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Einführung einer neuen Zugriffsebenen-Einstellung für das Kopieren von Projekten

Um Ihnen als System-Admin mehr Kontrolle darüber zu geben, was Planende mit einem Projekt tun können, haben wir den Bearbeitungszugriff auf Projekte in der Zugriffsebene granularer gestaltet, indem eine neue Einstellung eingeführt wurde, mit der Sie die Möglichkeit haben, Projekte zu kopieren. Vor dieser Änderung hatten Benutzer, die Sie den Zugriff auf „Projekte bearbeiten“ aktiviert haben, automatisch Zugriff, um sie zu kopieren. Mit der neuen Funktion können Sie Benutzern Zugriff auf die Bearbeitung von Projekten gewähren, ohne diese unbedingt kopieren zu müssen, indem Sie die neue Kopiereinstellung deaktivieren.

Wenn Ihre Benutzerinnen und Benutzer vor dieser Änderung Zugriff auf Projekte bearbeiten in ihrer Zugriffsebene hatten, wird diese Einstellung automatisch aktiviert, wenn diese Funktion veröffentlicht wird.

Informationen zur Zugriffsebene „Plan“ finden Sie unter [Zugriff auf Projekte gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Informationen zum Kopieren eines Projekts finden Sie unter [Kopieren eines Projekts](../../../manage-work/projects/manage-projects/copy-project.md).

Diese Funktion ist jetzt in den [Administratorgrundlagen in der neuen Workfront-Version, Teil 1: Benutzerorganisation, Lernpfad ](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

## Wählen Sie in einem benutzerdefinierten Formular für ein Objekt alle Elemente in einem Dropdown-Feld mit Mehrfachauswahl aus

>[!NOTE]
>
>Diese Funktion ist derzeit nicht verfügbar, wenn Sie eine neue Anfrage senden.

Wenn Sie auf der Detailseite für ein Objekt ein Dropdown-Feld mit Mehrfachauswahl in einem benutzerdefinierten Formular ausfüllen, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Optionen auswählen müssen.

Informationen zum Bearbeiten von Daten in einem benutzerdefinierten Formular finden Sie unter [Bearbeiten von Informationen in benutzerdefinierten Formularfeldern](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Alle benutzerdefinierten Formularfelder für ein Objekt neu berechnen

Jetzt ist es einfacher, sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern für ein Objekt aktuell sind. Mit der neuen Menüoption Ausdrücke neu berechnen können Sie alle Daten in diesen Feldern schnell neu berechnen.

Dies ist besonders nützlich, nachdem jemand Daten in einem anderen Objekt bearbeitet hat, auf das ein berechnetes benutzerdefiniertes Feld in Ihrem -Objekt verweist.

Zuvor mussten Benutzende Problemumgehungen verwenden, um sicherzustellen, dass alle Daten in berechneten benutzerdefinierten Feldern aktuell waren. Beispielsweise bearbeiteten sie das -Objekt zusammen mit anderen -Objekten, um die für die Massenbearbeitung verfügbare Option „Neuberechnung“ zu verwenden.

Weitere Informationen finden Sie unter [Bearbeiten von Informationen in benutzerdefinierten Formularfeldern](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Voreinstellungen für Aufgaben und Probleme von Gruppenadministratoren entsperren

>[!NOTE]
>
>Bis zum 24. Juni 2021 war dies als Teil eines schrittweisen Rollouts nur für Kunden verfügbar, die die Möglichkeit haben, Projektvoreinstellungen für Gruppen zu entsperren. Jetzt ist es für alle Kunden verfügbar.

Adobe Workfront-Administratoren können Gruppenadministratoren nun mehr Autonomie geben, indem sie individuelle Aufgaben- und Problemvoreinstellungen freischalten. Wenn eine Voreinstellung entsperrt ist, können Gruppenadministratoren sie für ihre Gruppen konfigurieren, um die individuellen Anforderungen und internen Prozesse jeder Gruppe zu erfüllen.

Weitere Informationen finden Sie unter [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Diese Funktion ist jetzt in den Administrator[Grundlagen der neuen Workfront-Version, Teil 2: Projekteinrichtung, Lernpfad ](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

## Zugriffsebenen-Einstellungen für Portfolios und Programme separat konfigurieren

Jetzt ist es einfacher, den Benutzerzugriff auf Portfolios und Programme zu verwalten, da Sie deren Zugriffsebenen-Einstellungen separat konfigurieren können.

Zuvor wurden die Zugriffsebenen-Einstellungen für Portfolios und Programme kombiniert. Dies bedeutete, dass Sie die Zugriffseinstellungen für Programme nicht auf die gleiche Weise konfigurieren konnten wie für Portfolios, und das Gleiche galt für umgekehrte Einstellungen.

Informationen zum Konfigurieren einer Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Informationen zu den Zugriffseinstellungen, die Sie für Programme und Portfolios konfigurieren können, finden Sie unter [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Diese Funktion ist jetzt in den [Administratorgrundlagen in der neuen Workfront-Version, Teil 1: Benutzerorganisation, Lernpfad ](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

## Aktivieren aller Kontrollkästchen in einer Reihe beim Bearbeiten von Informationen in einem benutzerdefinierten Formular

>[!NOTE]
>
>Diese Funktion ist derzeit nicht verfügbar, wenn Sie eine neue Anfrage senden.

Wenn Sie auf der Detailseite für ein Objekt ein benutzerdefiniertes Formularfeld ausfüllen, das Kontrollkästchen enthält, können Sie auf Alle auswählen klicken, wenn Sie alle verfügbaren Kontrollkästchen auswählen müssen.

Diese Option wird nur angezeigt, wenn das Feld mehr als zwei Kontrollkästchen enthält.

Weitere Informationen finden Sie unter [Bearbeiten von Informationen in benutzerdefinierten Formularfeldern](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Konfigurieren der Workfront-E-Mail-Zulassungsliste

Um Ihre Daten besser zu schützen, können Sie jetzt eine E-Mail-Domain-Zulassungsliste verwenden, um:

* Steuern, wohin Workfront-E-Mails gesendet werden können, wenn sie in Workfront gespeicherte Berichte oder Dokumente enthalten
* E-Mail-Domains können in der E-Mail-Adresse gespeichert werden, die Benutzer in ihrem Benutzerprofil angeben können

Wenn Sie beispielsweise sensible Daten schützen möchten, z. B. einen Bericht, in dem Ihre gefährdeten Kunden aufgeführt sind, können Sie nur Ihre interne E-Mail-Domain oder Ihre Domains in die E-Mail-Zulassungsliste einbeziehen. Auf diese Weise können Benutzende diesen Bericht (oder einen anderen Workfront-Bericht) nicht an eine externe E-Mail-Adresse senden.

Weitere Informationen finden Sie im Abschnitt [Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) im Artikel [Konfigurieren der Firewall-Zulassungsliste auf die Zulassungsliste setzte ](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zuweisen eines Gruppenadministrators für eine Untergruppe

Um die Unabhängigkeit der verschiedenen Unternehmensebenen zu erleichtern, haben wir die Möglichkeit hinzugefügt, einer Untergruppe einen Gruppenadministrator zuzuweisen. Jetzt können Sie sicherstellen, dass Sie die Verwaltung von Untergruppen an die richtigen Personen delegieren.

Zuvor konnte nur eine Gruppe auf oberster Ebene Gruppenadministratoren haben, und diese Administratoren verwalteten alle Untergruppen unter der Gruppe auf oberster Ebene.

Weitere Informationen finden Sie im Abschnitt [Gruppenadministratoren für Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) im Artikel [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Diese Funktion ist jetzt in den [Administratorgrundlagen in der neuen Workfront-Version, Teil 1: Benutzerorganisation, Lernpfad ](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

## Konfigurieren von Ereignisbenachrichtigungen für Gruppen

>[!NOTE]
>
>Nur für Kunden verfügbar, die über die Möglichkeit verfügen, Projektvoreinstellungen für Gruppen zu entsperren, wenn ein schrittweiser Rollout erforderlich ist. Dazu gehören alle Kunden auf Cluster 4 und 6 und eine geringe Anzahl von Kunden auf anderen Clustern. Diese Anmerkung wird aktualisiert, sobald die Funktion für mehr Cluster verfügbar wird.

Workfront-Administratoren können Gruppenadministratoren nun mehr Autonomie geben, indem sie Ereignisbenachrichtigungen für ihre Gruppen der obersten Ebene konfigurieren können. Untergruppen übernehmen Ereignisbenachrichtigungskonfigurationen von ihrer übergeordneten Gruppe.

Zuvor konnten Ereignisbenachrichtigungen nur von einem Workfront-Administrator auf Systemebene konfiguriert werden, d. h. alle Gruppen mussten denselben Satz an Ereignisbenachrichtigungen verwenden.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Anzeigen und Konfigurieren von Ereignisbenachrichtigungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Diese Funktion ist jetzt in den [Administratorgrundlagen in der neuen Workfront-Version, Teil 1: Benutzerorganisation, Lernpfad ](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) Workfront One enthalten.

Diese Funktion ist jetzt in den E[Mail- und In-App-Benachrichtigungen im neuen Lernpfad von Workfront ](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) in Workfront One enthalten.

## Arbeiten mit Gruppenprojekten und Genehmigungsprozessen im Bereich Gruppen

Wenn Sie Gruppenadministrator sind, können Sie die Projekte und Genehmigungsprozesse Ihrer Gruppe einfach anzeigen und damit arbeiten, da sie jetzt im Bereich Gruppen aufgeführt sind. Auf der Hauptseite einer Gruppe haben Sie folgende Möglichkeiten:

* Klicken Sie im linken Menü auf Projekte , um die Projekte der Gruppe anzuzeigen und neue für die Gruppe zu erstellen. Wenn ein ausgewähltes Projekt für Sie freigegeben wurde, können Sie es mit den Schaltflächen in der Symbolleiste bearbeiten, exportieren, kopieren oder löschen.

  Weitere Informationen finden Sie unter [Erstellen und Ändern der Projekte einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Klicken Sie im linken Menü auf Validierungen , um alle mit der Gruppe verbundenen Validierungsprozesse anzuzeigen und zu verwalten.

  Weitere Informationen finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Diese Funktion ist auch für Workfront-Admins verfügbar.

## Anzahl der verwendeten und zugewiesenen Lizenzen in einer Gruppe anzeigen

Um zu bestimmen, wie gut Ihre Lizenzen verteilt werden, können Sie jetzt die Anzahl der Lizenzen anzeigen, die in einer Gruppe und allen untergeordneten Gruppen verwendet werden.

Wenn Sie eine Gruppe der obersten Ebene verwalten, können Sie sowohl die Anzahl der in einer Gruppe verwendeten Lizenzen (und deren Untergruppen) als auch die maximale Anzahl der für die Gruppe zugewiesenen Lizenzen anzeigen.

Weitere Informationen finden Sie unter [Anzeigen der Anzahl der zugeordneten und in einer Gruppe verwendeten Lizenzen in der neuen Adobe Workfront-](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

