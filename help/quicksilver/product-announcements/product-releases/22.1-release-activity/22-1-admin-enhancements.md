---
title: 22.1 Verbesserungen für Administratoren
description: 22.1 Verbesserungen für Administratoren
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# 22.1 Verbesserungen für Administratoren

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit Version 22.1 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 17. Januar 2022.

Eine Liste aller in Version 22.1 verfügbaren Änderungen finden Sie in der Übersicht über die Version [22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Dokument-Downloads, die im Bereich Aktualisierungen protokolliert sind

Damit Benutzerinnen und Benutzer Downloads von Dokumenten verfolgen können, die sie in Workfront speichern, protokolliert das System jetzt einen Eintrag im Bereich Aktualisierungen für ein Dokument, wenn es von jemandem heruntergeladen wird.

>[!NOTE]
>
>Es wird empfohlen, diese Funktion in der Vorschau für ein neu hochgeladenes Dokument zu testen.

Informationen dazu, wie Workfront automatische Aktualisierungen von Objekten protokolliert, finden Sie unter [Vom System verfolgte Aktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Gewähren von Zugriff für Teams, die Zugriffsebenen verwenden

Ein neuer Abschnitt im Bereich Zugriffsebenen bietet Ihnen detailliertere Steuerelemente zum Verwalten des Zugriffs Ihrer Benutzer auf Teams. Jetzt können Sie festlegen, wer Teams erstellen, bearbeiten und anzeigen kann.

Dies ändert nichts am bestehenden Zugriff Ihrer Benutzer auf Teams.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Gruppenzuordnung jetzt in Blueprints verfügbar

Einige Blueprints enthalten jetzt Gruppen, die Sie vor der Installation der Blueprint anpassen können. Sie können eine Gruppe im Blueprint einer vorhandenen Gruppe in Ihrer Workfront-Instanz zuordnen oder bei Bedarf eine neue Gruppe erstellen.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Formatierungsaktualisierungen im Bereich Benutzerdefinierte Forms

Der benutzerdefinierte Forms-Bereich hat ein neues Erscheinungsbild, das ihn mit vielen anderen Bereichen der neuen Workfront-Version auf den neuesten Stand bringt.

## Viele Verbesserungen beim Erstellen von berechneten benutzerdefinierten Feldern

Das Erstellen berechneter benutzerdefinierter Felder ist jetzt mit diesen Ergänzungen im neuen Berechnungs-Editor viel einfacher:

* Sie können den Mauszeiger über einen beliebigen Ausdruck in Ihrer Berechnung bewegen, um Informationen darüber anzuzeigen, einschließlich einer Beschreibung, eines Beispiels für dessen Verwendung und eines Links zu weiteren Informationen in einem Hilfeartikel.
* Jeder hinzugefügte Ausdruck ist farbcodiert, je nach Typ. Dadurch können Sie Ihre Ausdrücke leichter erkennen und ihren Typ sofort erkennen.
* Zeilennummern helfen Ihnen, Funktionen in einer langen Berechnung zu identifizieren und zu referenzieren.
* Wenn Sie mit der Eingabe eines Ausdrucks oder Feldnamens beginnen, wird eine Liste der verfügbaren Elemente angezeigt, sodass Sie den gewünschten auswählen können. Und wenn Sie eine offene Klammer eingeben, wird die schließende Klammer automatisch hinzugefügt.
* Sie können das Ergebnis Ihrer Berechnung mit einem vorhandenen Objekt in der Vorschau anzeigen, ohne den Berechnungs-Editor zu verlassen.

Außerdem können Sie in den anpassbaren „Anweisungen“ über dem Text für ein berechnetes benutzerdefiniertes Feld die Formel des Felds anzeigen oder ausblenden. Dies ist nützlich, wenn Sie der Meinung sind, dass die Benutzer, die das benutzerdefinierte Formular ausfüllen werden, diese Informationen nicht benötigen.

## Anzeigen von Auditprotokollinformationen zu Status und Unternehmen

Sie können jetzt einfacher eine Fehlerbehebung bei Vorfällen durchführen, die Status und Unternehmen betreffen, indem Sie Informationen dazu im Bereich Audit-Protokolle im Setup anzeigen.

Beispiel:

* Sie können feststellen, wer einen Status umbenannt, gesperrt oder ausgeblendet hat und wann dies der Fall war.
* Sie können herausfinden, wer einige Mitglieder oder Aufgabengebiete aus einem Unternehmen entfernt hat und wann.

Informationen zum Anzeigen von Administratorprotokollinformationen finden Sie unter [Anzeigen und Exportieren von Administratorprotokollen](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprints - Unternehmenszuordnung und andere Verbesserungen

Die folgenden Blueprints-Verbesserungen sind jetzt verfügbar:

* Einige Blueprints umfassen jetzt Unternehmen, die Sie vor der Installation der Blueprint anpassen können. Sie können ein Unternehmen in der Blueprint einem bestehenden Unternehmen in Ihrer Workfront-Instanz zuordnen oder bei Bedarf ein neues Unternehmen erstellen.
* Ein neuer Blueprint-Typ, Organisationsstruktur , ist jetzt verfügbar. Einige Blueprints enthalten Elemente aus mehreren Typen (z. B. Projektvorlage und Organisationsstruktur). Sie können auf der Katalogseite nach Blueprint-Typ filtern.
* Die Abschnitte „Installationsvoreinstellungen“ und „Vorlageneigentümerschaft“ auf der Konfigurationsseite wurden aus Gründen der Einfachheit in „Vorlagenvoreinstellungen“ zusammengefasst.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Einfache Verwaltung von Unternehmensmitgliedschaften

Im Bereich Firmen erleichtert eine aktualisierte Symbolleiste das Hinzufügen vorhandener Workfront-Benutzender zu einer Firma und das Entfernen von Firmenmitgliedern.

Zuvor waren diese Aktionen nur im Feld Firma bearbeiten verfügbar.

Die aktualisierte Symbolleiste enthält auch alle Aktionen, die in der vorherigen Symbolleiste verfügbar waren, z. B. das Bearbeiten der Benutzerprofilinformationen von Mitgliedern und deren Deaktivierung im System.

Weitere Informationen finden Sie unter [Verwalten von Unternehmensmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Auswählen von Ausdrücken und Feldern im neuen Fenster für berechnete Felder

Wir machen es weiterhin einfacher, ein berechnetes Feld in einem benutzerdefinierten Formular zu erstellen. Wenn Sie nun auf Maximieren klicken, um den neuen Berechnungs-Editor zu öffnen, können Sie die benötigten Ausdrücke und Felder suchen und auswählen.

## Gruppen können ihre eigenen Arbeitszeittabellen- und Stundeneinstellungen konfigurieren

>[!NOTE]
>
>Diese Funktion war ursprünglich als Teil eines schrittweisen Rollouts nur für Kunden auf Cluster 4 als Teil der Version 21.4 verfügbar. Diese Funktion ist ab dem 8. November 2021 für alle verbleibenden Cluster in Produktion verfügbar.

In einem großen Unternehmen müssen einige Gruppen möglicherweise die Arbeitszeittabellen- und Stundeneinstellungen unabhängig voneinander konfigurieren, um sie an ihre spezifischen Workflows anzupassen, anstatt die von einem Administrator auf Systemebene konfigurierten Einstellungen zu übernehmen. Jetzt können Workfront-Administratoren eine Arbeitszeittabelle und Stundenvoreinstellungen für alle Gruppen im System entsperren, sodass sie sie selbst konfigurieren können.

Diese Funktion wurde kürzlich für Projektvoreinstellungen sowie für Aufgaben- und Problemvoreinstellungen hinzugefügt.

Informationen dazu, wie Workfront-Admins eine Arbeitszeittabelle und Stundeneinstellungen entsperren, finden Sie im Abschnitt [Arbeitszeittabelle und Stundeneinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Arbeitszeittabelle und Stundeneinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen dazu, wie Gruppenadmins die Einstellungen für entsperrte Aufgaben und Probleme für eine Gruppe konfigurieren, finden [ unter „Arbeitszeittabelle und Stundeneinstellungen für eine Gruppe konfigurieren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Wählen Sie mehrere Benachrichtigungen aus, die Sie für Gruppen entsperren oder erneut sperren möchten

E-Mail-Benachrichtigungen für Gruppen können jetzt schneller und einfacher entsperrt oder erneut gesperrt werden. Jetzt können Sie mehrere Benachrichtigungen auswählen, Ihre Auswahl überprüfen, um sicherzustellen, dass sie korrekt sind, und dann auf die neue Schaltfläche Entsperren oder Sperren klicken, die in der Symbolleiste angezeigt wird.

Zuvor mussten Sie Benachrichtigungen einzeln entsperren und erneut sperren. Workfront verfügt derzeit über 95 Benachrichtigungen. Es hat also eine Weile gedauert, bis Sie diese für alle oder viele von ihnen einrichten mussten.

Weitere Informationen finden Sie unter [Konfiguration von Ereignisbenachrichtigungen für alle Gruppen entsperren oder sperren](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Für Gruppenadministratoren: Einfachere Auswahl einer Ersatzgruppe, wenn eine Gruppe gelöscht wird

Beim Löschen einer Gruppe erleichtern zwei Verbesserungen im Feld Gruppe löschen die Auswahl der Ersatzgruppe, bei der die Benutzer, Arbeitselemente und Untergruppen der gelöschten Gruppe erhalten bleiben sollen:

* Sie können den Namen der Gruppe eingeben, um sie schnell zu finden. Zuvor gab es nur eine Dropdown-Liste, die Sie nicht eingeben konnten. Dies war für Organisationen mit vielen Gruppen problematisch, da Sie durch die Liste scrollen mussten, um die gewünschte Gruppe zu finden. Außerdem hatte die Dropdown-Liste eine Elementbegrenzung, sodass es möglich war, dass die gewünschte Gruppe nicht angezeigt wurde.
* Sie können das Symbol Neue Informationen verwenden, um sicherzustellen, dass Sie die gewünschte Ersatzgruppe auswählen. Wenn Sie den Mauszeiger über das Symbol bewegen, wird eine QuickInfo mit Informationen über die Gruppe angezeigt, wie z. B. die Hierarchie der darüber liegenden Gruppen und die Namen der Administratoren.

Weitere Informationen finden Sie unter [Gruppe löschen](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Größerer Bereich zum Erstellen berechneter Felder

Jetzt ist es einfacher, komplexe berechnete Felder in einem benutzerdefinierten Formular zu erstellen. Klicken Sie auf die neue Schaltfläche Maximieren , um ein großes Bearbeitungsfenster für die Erstellung Ihrer Berechnung zu öffnen. Wenn Sie fertig sind, klicken Sie auf Minimieren , um mit der Arbeit an Ihrem benutzerdefinierten Formular fortzufahren.

## Hinzufügen benutzerdefinierter Formulare zu Gruppen

Benutzerdefinierte Formulare werden jetzt für das Gruppenobjekt unterstützt. Dies erleichtert es Gruppen in Ihrer Organisation, Informationen zu erfassen und freizugeben, die ihren spezifischen Anforderungen und Workflows entsprechen. Benutzer können Folgendes für eine Gruppe tun, genau wie für andere Workfront-Objekte:

* Erstellen eines benutzerdefinierten Formulars
* Benutzerdefiniertes Formular anhängen
* Speichern benutzerdefinierter Formulardaten
* Entfernen eines benutzerdefinierten Formulars
* Bearbeiten Sie benutzerdefinierte Daten aus Listen und im neuen Workfront-Erlebnis über die Seite Gruppe .

Informationen zu benutzerdefinierten Formularen finden Sie unter [Benutzerdefinierte Formulare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Erstellen von OAuth2-Apps zur Integration von Programmen mit Workfront

Jetzt können Sie Workfront mit anderen Programmen integrieren, für die Workfront keine integrierte Integration bietet. Durch Erstellen einer OAuth2-App für die Anwendung, mit der Sie eine Integration durchführen möchten, können Sie dieser Anwendung den Zugriff auf Workfront ermöglichen, wobei Sie wissen, dass Ihre Daten durch das sichere, dem Industriestandard entsprechende OAuth2-Authentifizierungsprotokoll geschützt sind.

Zuvor konnten Sie nur über integrierte Integrationen, Workfront Fusion oder die Workfront-API mit anderen Programmen integrieren.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Verbesserungen der Benutzeroberfläche im Bereich Unternehmen

Im Bereich Firmen im Setup erleichtern neue Bestätigungsnachrichten und geringfügige redaktionelle Änderungen die Verwaltung der Firmenmitgliedschaft. Beispielsweise lautet der Abschnittsname „Personen“ im linken Bereich jetzt „Firmenmitglieder“.

Informationen zur Verwaltung von Unternehmensmitgliedschaften finden Sie unter [Verwalten von Unternehmensmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
