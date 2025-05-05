---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.3 an der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 10. August 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.3 an der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 10. August 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 20.3 verfügbaren Änderungen finden Sie unter [20.3 - Versionsübersicht](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Kalender über einen privaten Link freigeben

Um die Kalenderfreigabe in Workfront zu erleichtern, können Sie einen privaten Link freigeben, über den Benutzer direkt zum Kalender gelangen. Der Kalender muss für den Benutzer freigegeben sein und er muss sich anmelden, um ihn anzuzeigen.

Zuvor konnten Sie eine öffentliche URL freigeben, für deren Anzeige keine Anmeldung erforderlich war.

Weitere Informationen finden Sie unter [Freigeben eines Kalenderberichts](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Neuer Bereich „Entwürfe“ beim Erstellen von Anforderungen

Um Ihnen bei der Arbeit mit Anfragen mehr Flexibilität zu bieten, speichert Workfront jetzt automatisch jede Anfrage, die Sie erstellen, als Entwurf im neuen Entwurfsbereich. Wenn Sie nicht über alle Informationen verfügen, die zum Abschließen der neuen Anfrage erforderlich sind, können Sie sie als Entwurf hinterlassen, zu ihr zurückkehren und sie später abschließen. Workfront speichert eine Anfrage pro Warteschlangenthema im Bereich „Neue Entwürfe“. Die Anforderungsentwürfe können so lange gespeichert werden, wie Sie sie benötigen, bis Sie bereit sind, sie abzuschließen und zu übermitteln. Sie können den Bereich „Entwürfe“ im linken Bereich auch mithilfe einer Layout-Vorlage entfernen oder neu positionieren.

Weitere Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Workfront-Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Wenn Ihnen in der Vorschau-Version eine benutzerdefinierte Layout-Vorlage zugewiesen wurde, müssen Sie den Bereich „Entwürfe“ Ihrer Anfragen hinzufügen, indem Sie Ihre Layout-Vorlage ändern.

## Elemente in der Arbeitszeittabelle ein- oder ausblenden

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar

Um Arbeitszeittabellen mit mehreren Elementen einfach verwalten zu können, können Sie jetzt alle Elemente mit einem Klick ein- oder ausblenden.

Zuvor mussten Sie auf jedes Element einzeln klicken.

Weitere Informationen finden Sie unter [Zeit erfassen](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Tatsächliche Termine in Workfront-Kalendern ignorieren

>[!NOTE]
>
>Diese Funktion wurde am 5. Juni 2020 in der Vorschau-Umgebung veröffentlicht. Sie wird am 19. Juni 2020 in der Produktionsumgebung verfügbar sein.

Damit Sie besser steuern können, wie Objekte in Kalenderberichten angezeigt werden, können Sie festlegen, dass tatsächliche Datumsangaben ignoriert werden, selbst wenn sie verfügbar sind.

Zuvor verwendete der Kalender automatisch tatsächliche Daten, sobald sie verfügbar waren.

Weitere Informationen finden Sie unter [Übersicht über Kalenderberichte](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Verwenden benutzerdefinierter Datumsfelder in Kalenderberichten

>[!NOTE]
>
>Diese Funktion wurde am 29. Mai 2020 in der Vorschau-Umgebung veröffentlicht. Sie wird am 12. Juni 2020 in der Produktionsumgebung verfügbar sein.

Um Ihre tägliche Arbeit mit Kalendern besser visualisieren und verwalten zu können, stehen jetzt benutzerdefinierte Datumsfelder als Datumsoption zur Verfügung.

Zuvor konnten Sie Ihren Kalender nur mit projizierten, geplanten Terminen verwalten, wenn keine tatsächlichen Termine verfügbar waren.

Weitere Informationen finden Sie unter [Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (oder wenn Sie Workfront Classic verwenden, finden Sie [Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

## E-Mail-Änderungen

**Änderungen ausgehender E-Mails:** Alle E-Mails von Workfront stammen von notifications@my.workfront.com. Dazu gehören automatisierte Warnhinweise und die Kommunikation zwischen Benutzenden.

Zuvor konnten Systemadministratoren im Bereich „E-Mail-Setup“ eine benutzerdefinierte E-Mail-Adresse hinzufügen.

**POP-Antwortänderungen für eingehende E-Mails:** Systemadministratoren können jetzt keinen benutzerdefinierten POP-E-Mail-Server mehr für eingehende E-Mail-Antworten auf Benachrichtigungen konfigurieren.

Weitere Informationen finden Sie unter [E-Mail-Spoofing und POP-Antwort-E-Mail-Änderungen](https://experienceleague.adobe.com/de/docs/workfront/using/home).

## DomainKeys Identified Mail (DKIM) ist jetzt in ausgehenden Workfront-E-Mails enthalten

Alle ausgehenden E-Mails enthalten eine E-Mail-Authentifizierungstechnik (DKIM). Diese DKIM-Signatur ist für den Endbenutzer nicht sichtbar, ermöglicht jedoch die Validierung auf Serverebene und stärkt unser bestehendes Authentifizierungs-Framework.

## Aktualisierungen der Registrierung in der neuen Workfront-Version

Um die Benutzerregistrierung in der neuen Workfront-Version überschaubarer zu gestalten, haben Gruppenadministratoren jetzt Zugriff auf die Registrierung und das Aufheben der Registrierung von Benutzenden, die zu den von ihnen verwalteten Gruppen gehören.

Es gibt jetzt auch einen Link Benutzerdetails , der die folgenden Benutzerinformationen anzeigt:

* Name
* Aufgabengebiet
* E-Mail-Adresse
* Profilbild

## Neu für Administratoren: Brand Workfront für bestimmte Gruppen, Teams, Aufgabengebiete und Benutzer

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar

Jetzt können Sie eine Layout-Vorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Aufgabengebiete und Benutzende zu ändern, die über ein eigenes Branding verfügen.

Weitere Informationen finden Sie unter [Branding Ihrer Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Gruppenadministratoren können Genehmigungsprozesse erstellen und verwalten

Um eine größere Autonomie und Kontrolle über die Workflows ihrer Gruppen zu ermöglichen, kann ein Gruppenadministrator jetzt auf den Bereich Genehmigungsprozess unter Einrichten zugreifen und Genehmigungsprozesse für eine Gruppe erstellen und bearbeiten, die er verwaltet. Diese Genehmigungsprozesse basieren auf den Status dieser Gruppe.

Um sicherzustellen, dass Gruppenadministratoren nicht versehentlich Genehmigungsprozesse bearbeiten, die im gesamten System verwendet oder von anderen Gruppen erstellt werden, können sie nur auf die Genehmigungsprozesse zugreifen, die mit den von ihnen verwalteten Gruppen verknüpft sind.

Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Für Administratoren: Die Seite Neue Gruppen erleichtert die Erstellung und Verwaltung von Gruppen.

Gruppenadministratoren können jetzt, da alles, was sie benötigen, auf der neuen Seite Gruppen angezeigt wird, Gruppen einfacher verwalten. Es ist nicht mehr erforderlich, zwischen verschiedenen Überlagerungsfeldern und Setup-Seiten zu navigieren, um Gruppen zu erstellen und zu ändern.

Im Folgenden finden Sie die wichtigsten Highlights:

* Gruppendetails: Zeigen Sie grundlegende Informationen über die Gruppe an und bearbeiten Sie sie, z. B. den Namen der Gruppe, ihre Beschreibung und die Namen von Gruppenadministratoren. Zudem erfahren Sie, ob die Gruppe öffentlich oder privat ist.
* Liste der Gruppenmitglieder: Zeigen Sie alle Gruppenmitglieder an und verwenden Sie die neue Symbolleiste, um Mitgliedschaften schnell hinzuzufügen, zu entfernen, zu exportieren, zu aktivieren und zu deaktivieren. Sie können auch die Profile der Mitglieder bearbeiten und ihnen Kommentare zur Aktualisierung senden.
* Feld „Gruppenadministrator“ in der Kopfzeile: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, können Sie schnell ein Gruppenmitglied als Administrator der Gruppe zuweisen oder die Zuweisung aufheben. Dies können Sie auch in der Liste der Gruppenmitglieder mithilfe der neuen Spalte „Gruppenrolle“ tun.
* Untergruppenliste: Anzeigen, Bearbeiten, Kopieren, Exportieren und Löschen der Untergruppen in einer von Ihnen verwalteten Gruppe.
* Statusliste : Zeigen Sie die Status Ihrer Gruppe an und verwalten Sie sie.

Weitere Informationen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Neu für Admins: Bis zu 14 Ebenen von Untergruppen erstellen

Um die Organisation Ihrer Workfront-Gruppen entsprechend Ihrer Organisationshierarchie zu erleichtern, haben wir die Anzahl der Untergruppen, die Sie innerhalb einer Gruppe erstellen können, von 3 auf 14 erhöht.

Weitere Informationen finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Neu für Admins: Neue Setup-Seitenleiste

>[!NOTE]
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar

Die linke Seitenleiste im Setup ist jetzt schneller und einfacher zu verwenden und nutzt das grundlegende Layout und die Funktionalität, die Sie bereits kennen. Neben einem moderneren Look-and-Feel gibt es noch etwas Neues:

* Ein neuer cremefarbener Hintergrund in der Seitenleiste erleichtert die Unterscheidung vom Rest des Setup-Bereichs.
* Die Symbole in der Seitenleiste sind etwas größer, und einige wurden neu gestaltet, um klarer vorzuschlagen, was die Option tut.
* Mehr vertikaler Abstand zwischen Seitenleisten-Elementen erleichtert deren Lesbarkeit.
* Sie können die Seitenleiste ausblenden, wenn Sie im Hauptbereich mehr Platz benötigen, um sie anzuzeigen und auszuführen (z. B. um zusätzliche Spalten anzuzeigen). Außerdem können Sie die Seitenleiste wieder erweitern, wenn Sie Funktionsnamen anzeigen möchten.
* Während die Seitenleiste ausgeblendet ist, werden nur die Symbole für die einzelnen Funktionen angezeigt. Um die Unterelemente unter einem Hauptseitenleistenelement anzuzeigen, bewegen Sie den Mauszeiger über das zugehörige Symbol, um sie in einem Flyout-Menü anzuzeigen. Bewegen Sie beispielsweise den Mauszeiger über das Symbol Prozesse , um ein Menü mit Genehmigungen und Meilensteinpfaden anzuzeigen.
* Die beiden Kickstarts (Datenimport und -export) sind mit einem Klick verfügbar. Sie wurden unter „System“ aus verschoben, um sie auf der Hauptebene der Seitenleiste anzuzeigen.

Weitere Informationen zur Verwendung des Bereichs Setup finden Sie unter [Administration und Setup](../../../administration-and-setup/administration-and-setup.md).

## Cluster-Nummer in Kundeninformationsbereich einschließen

Als Workfront-Administrator können Sie die Cluster-Nummer jetzt einfach in Workfront finden, ohne zusätzliche Zeit und Mühe darauf verwenden zu müssen, sie von unserem Support-Team zu erhalten. Wir haben im Bereich „Kundeninformationen“ von „Setup“ ein Feld „Cluster-Setup“ hinzugefügt.

Weitere Informationen zum Bereich „Kundeninformationen“ finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Base64-Codierung für Ereignisabonnements

Das Feld base64encoding ist ein optionales Feld, das verwendet wird, um die Base64-Codierung von Payloads von Ereignisabonnements zu aktivieren. Wenn eine Anfrage mit dem Feld base64Encoding gestellt wird, das auf „true“ gesetzt ist, werden die newState- und oldState-Objekte in der Payload als Base64-Codierungszeichenfolgen bereitgestellt. Diese Funktion kann nützlich sein, wenn Ihr Netzwerk so konfiguriert ist, dass Sonderzeichen in Ereignisabonnements nicht zulässig sind.

Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md).

## Möglichkeit zum Erstellen doppelter Ereignisabonnements entfernt

Um den Versand doppelter Nachrichten zu verhindern, können Sie keine doppelten Abonnements mehr erstellen. Darüber hinaus wurden alle zuvor erstellten doppelten Abonnements entfernt.

Weitere Informationen finden Sie unter [FAQs - Ereignisabonnements](../../../wf-api/general/event-subs-faq.md).
