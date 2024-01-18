---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3. Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.3 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 10. August 2020 bereitgestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3. Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 20.3 der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Produktionsumgebung in der Woche vom 10. August 2020 bereitgestellt.

Eine Liste aller in Version 20.3 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Kalender mit einem privaten Link freigeben

Um die Freigabe von Kalendern in Workfront zu erleichtern, können Sie einen privaten Link freigeben, über den Benutzer direkt zum Kalender gelangen. Der Kalender muss für den Benutzer freigegeben werden und muss sich anmelden, um ihn anzuzeigen.

Zuvor konnten Sie eine öffentliche URL freigeben, für die keine Anmeldung erforderlich war.

Weitere Informationen finden Sie unter [Kalenderberichte freigeben](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Neuer Entwurfsbereich beim Erstellen von Anforderungen

Um Ihnen mehr Flexibilität beim Arbeiten mit Anforderungen zu geben, speichert Workfront jetzt automatisch alle von Ihnen erstellten Anforderungen als Entwurf im neuen Entwurfsbereich. Wenn Sie nicht über alle zum Abschließen der neuen Anforderung erforderlichen Informationen verfügen, können Sie sie als Entwurf hinterlassen, später erneut darauf zugreifen und abschließen. Workfront speichert eine Anforderung pro Warteschlangenthema im neuen Bereich &quot;Entwürfe&quot;. Die Entwurfsanfragen können so lange gespeichert werden, wie Sie sie benötigen, bis Sie sie abschließen und übermitteln können. Sie können den Bereich &quot;Entwürfe&quot;auch mithilfe einer Layout-Vorlage im linken Bereich entfernen oder neu positionieren.

Weitere Informationen zum Erstellen von Anforderungen finden Sie unter [Erstellen und Senden von Workfront-Anforderungen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Wenn Sie in der Vorschau-Version eine benutzerdefinierte Layout-Vorlage zugewiesen haben, müssen Sie den Bereich &quot;Entwürfe&quot;Ihrer Anforderungen hinzufügen, indem Sie Ihre Layout-Vorlage ändern.

## Ein- oder Ausblenden von Elementen auf dem Zeitblatt

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Um die einfache Verwaltung von Timesheets mit mehreren Elementen zu erleichtern, können Sie jetzt alle Elemente durch Klicken auf eine Schaltfläche erweitern oder reduzieren.

Zuvor musste jedes Element einzeln angeklickt werden.

Weitere Informationen finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Tatsächliche Daten in Workfront-Kalendern ignorieren

>[!NOTE]
>
>Diese Funktion wurde am 5. Juni 2020 in der Vorschau-Umgebung veröffentlicht. Es wird am 19. Juni 2020 in der Produktionsumgebung verfügbar sein.

Um Ihnen mehr Kontrolle darüber zu geben, wie Objekte in Kalenderberichten angezeigt werden, können Sie die tatsächlichen Daten ignorieren, selbst wenn sie verfügbar sind.

Zuvor verwendete der Kalender automatisch die tatsächlichen Daten, sobald sie verfügbar waren.

Weitere Informationen finden Sie unter [Kalenderberichte - Übersicht](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Verwenden benutzerdefinierter Datumsfelder in Kalenderberichten

>[!NOTE]
>
>Diese Funktion wurde am 29. Mai 2020 in der Vorschau-Umgebung veröffentlicht. Es wird am 12. Juni 2020 in der Produktionsumgebung verfügbar sein.

Um Ihre tägliche Arbeit mit Kalendern besser zu visualisieren und zu verwalten, stehen jetzt benutzerdefinierte Datumsfelder als Datumsoption zur Verfügung.

Zuvor konnten Sie Ihren Kalender nur mit projizierten, geplanten Datumsangaben verwalten.

Weitere Informationen finden Sie unter [Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (oder wenn Sie Workfront Classic verwenden, finden Sie unter [Verwenden benutzerdefinierter Datumsfelder in einem Kalenderbericht](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## E-Mail-Änderungen

**Ausgehende E-Mail-Änderungen:** Alle E-Mails von Workfront werden von notifications@my.workfront.com stammen. Dies umfasst automatisierte Warnungen und die Kommunikation zwischen Benutzern und Benutzern.

Zuvor konnten Systemadministratoren im Bereich E-Mail-Einrichtung eine benutzerdefinierte E-Mail-Adresse hinzufügen.

**Änderungen an der POP-Antwort der eingehenden E-Mail:** Systemadministratoren können keinen benutzerdefinierten POP-E-Mail-Server mehr für eingehende E-Mail-Antworten auf Benachrichtigungen konfigurieren.

Weitere Informationen finden Sie unter [E-Mail-Spoofing- und POP-Antwort-E-Mail-Änderungen](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM) ist jetzt in ausgehenden Workfront-E-Mails enthalten

In allen ausgehenden E-Mails wird eine E-Mail-Authentifizierungstechnik (DKIM) eingesetzt. Diese DKIM-Signatur ist für den Endbenutzer nicht sichtbar, ermöglicht jedoch die Validierung auf Serverebene und stärkt unser vorhandenes Authentifizierungs-Framework.

## Aktualisierungen der Anmeldung für das neue Workfront-Erlebnis

Damit die Benutzereinanmeldung in der neuen Workfront besser verwaltet werden kann, haben Gruppenadministratoren jetzt Zugriff auf die Möglichkeit, Benutzer, die zu den von ihnen verwalteten Gruppen gehören, zu registrieren und die Registrierung aufzuheben.

Es gibt jetzt auch einen Link Benutzerdetails , der die folgenden Benutzerinformationen anzeigt:

* Name
* Auftragsrolle
* E-Mail-Adresse
* Profilbild

## Neu für Administratoren: Brand Workfront für bestimmte Gruppen, Teams, Jobrollen und Benutzer

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Jetzt können Sie eine Layout-Vorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Jobrollen und Benutzer mit ihrem eigenen Branding zu ändern.

Weitere Informationen finden Sie unter [Markieren Sie Ihre Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Gruppenadministratoren können Genehmigungsprozesse erstellen und verwalten

Um mehr Autonomie und Kontrolle über die Workflows ihrer Gruppen zu ermöglichen, kann ein Gruppenadministrator jetzt auf den Bereich Validierungsprozess unter Einrichtung zugreifen und Validierungsprozesse für eine von ihm verwaltete Gruppe erstellen und bearbeiten. Diese Genehmigungsprozesse basieren auf den Status dieser Gruppe.

Um sicherzustellen, dass Gruppenadministratoren nicht versehentlich Validierungsprozesse bearbeiten, die im gesamten System verwendet werden oder von anderen Gruppen erstellt werden, können sie nur auf die Validierungsprozesse zugreifen, die den von ihnen verwalteten Gruppen zugeordnet sind.

Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Für Administratoren: Neue Seite &quot;Gruppen&quot;erleichtert die Erstellung und Verwaltung von Gruppen

Gruppenadministratoren können Gruppen jetzt einfacher verwalten, da sich alles, was sie benötigen, auf der neuen Seite &quot;Gruppen&quot;befindet. Es ist nicht mehr erforderlich, zwischen verschiedenen Überlagerungsfeldern und Einrichtungsseiten zu navigieren, um Gruppen zu erstellen und zu ändern.

Hier sind die wichtigsten Highlights:

* Gruppendetails: Zeigen Sie grundlegende Informationen zur Gruppe an und bearbeiten Sie sie, z. B. den Namen der Gruppe, die Beschreibung, die Namen der Gruppenadministratoren und ob die Gruppe öffentlich oder privat ist.
* Liste der Gruppenmitglieder: Zeigen Sie alle Gruppenmitglieder an und verwenden Sie die neue Symbolleiste, um schnell Mitgliedschaften hinzuzufügen, zu entfernen, zu exportieren, zu aktivieren und zu deaktivieren. Sie können auch die Profile der Mitglieder bearbeiten und ihnen Aktualisierungskommentare senden.
* Gruppenadministrator-Feld in der Kopfzeile: Wenn Sie eine von Ihnen verwaltete Gruppe anzeigen, weisen Sie ein Gruppenmitglied schnell als Administrator der Gruppe zu oder heben Sie die Zuweisung auf. Sie können dies auch in der Liste der Gruppenmitglieder in der neuen Spalte Gruppenrolle tun.
* Liste der Untergruppen: Zeigen Sie die Untergruppen in einer von Ihnen verwalteten Gruppe an, bearbeiten Sie sie, kopieren, exportieren und löschen Sie sie.
* Statusliste: Zeigen Sie die Status Ihrer Gruppe an und verwalten Sie sie.

Weitere Informationen finden Sie unter [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Neu für Administratoren: Erstellen Sie bis zu 14 Ebenen von Untergruppen

Um die Organisation Ihrer Workfront-Gruppen an Ihre Organisationshierarchie anzupassen, haben wir die Ebenen der Untergruppen, die Sie in einer Gruppe erstellen können, von 3 auf 14 erhöht.

Weitere Informationen finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Neu für Administratoren: Neue Sidebar &quot;Einstellungen&quot;

>[!NOTE]
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Die linke Seitenleiste unter Einrichtung ist jetzt schneller und einfacher zu verwenden und nutzt das grundlegende Layout und die Funktionalität, die Sie bereits kennen. Neben einem moderneren Look-and-Feel ist hier das Neue:

* Ein neuer weißer Hintergrund in der Seitenleiste erleichtert die Unterscheidung vom Rest des Einrichtungsbereichs.
* Die Symbole in der Seitenleiste sind etwas größer und einige werden neu gestaltet, um klarer vorzuschlagen, was die Option bewirkt.
* Ein größerer vertikaler Abstand zwischen Seitenleisten-Elementen erleichtert deren Lesbarkeit.
* Sie können die Seitenleiste ausblenden, wenn Sie Platz im Hauptbereich benötigen, um mehr zu sehen und zu tun, z. B. die Anzeige zusätzlicher Spalten. Außerdem können Sie die Seitenleiste erneut erweitern, wenn Sie Funktionsnamen sehen möchten.
* Während die Seitenleiste ausgeblendet ist, sehen Sie nur die Symbole für jede Funktion. Um die Unterelemente unter einem Haupt-Seitenleistenelement anzuzeigen, halten Sie den Mauszeiger über das Symbol, um sie in einem Flyout-Menü anzuzeigen. Bewegen Sie beispielsweise den Mauszeiger über das Symbol Prozesse , um ein Menü mit Genehmigungen und Meilensteinpfaden anzuzeigen.
* Sie können die beiden Kick-Starts-Optionen (Daten importieren und Daten exportieren) mit einem Klick schneller aufrufen. Sie wurden von unter System zur Anzeige auf der Hauptebene der Seitenleiste verschoben.

Informationen zur Verwendung des Einrichtungsbereichs finden Sie unter [Administration und Einrichtung](../../../administration-and-setup/administration-and-setup.md).

## Hinzufügen der Cluster-Nummer im Bereich &quot;Kundeninformationen&quot;

Als Workfront-Administrator können Sie jetzt die Cluster-Nummer in Workfront einfach finden, ohne zusätzliche Zeit und Mühe darauf verwenden zu müssen, sie von unserem Support-Team zu erhalten. Im Bereich &quot;Kundeninformationen&quot;der Einrichtung wurde das Feld Cluster-Setup hinzugefügt.

Informationen zum Bereich &quot;Kundeninformationen&quot;finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Base64-Kodierung für Ereignisanmeldungen

Das Feld base64Encoding ist ein optionales Feld, das verwendet wird, um die Base64-Kodierung von Payloads für Ereignisabonnements zu aktivieren. Wenn eine Anfrage mit dem base64Encoding -Feld auf true gestellt wird, werden die Objekte newState und oldState in der Payload als Base64-Kodierungszeichenfolgen bereitgestellt. Diese Funktion kann nützlich sein, wenn Ihr Netzwerk so konfiguriert ist, dass Sonderzeichen in Ereignisanmeldungen nicht zulässig sind.

Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../../wf-api/general/event-subs-api.md).

## Die Möglichkeit zur Erstellung doppelter Ereignisanmeldungen wurde entfernt

Um den Versand doppelter Nachrichten zu verhindern, können Sie keine doppelten Abonnements mehr erstellen. Darüber hinaus wurden alle zuvor erstellten doppelten Abonnements entfernt.

Weitere Informationen finden Sie unter [Häufig gestellte Fragen - Ereignisabos](../../../wf-api/general/event-subs-faq.md).
