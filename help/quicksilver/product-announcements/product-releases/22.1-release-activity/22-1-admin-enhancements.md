---
title: 22.1 Verbesserungen für Administratoren
description: 22.1 Verbesserungen für Administratoren
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 22.1 Verbesserungen für Administratoren

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 22.1 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 17. Januar 2022.

Eine Liste aller in Version 22.1 verfügbaren Änderungen finden Sie unter [22.1 - Versionsübersicht](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Dokumentdownloads, die im Bereich Updates protokolliert wurden

Um Ihren Benutzern zu helfen, Downloads von Dokumenten zu verfolgen, die sie in Workfront speichern, protokolliert das System jetzt einen Eintrag im Bereich Updates für ein Dokument, wenn ein Benutzer es herunterlädt.

>[!NOTE]
>
>Es wird empfohlen, diese Funktion in der Vorschau für ein neu hochgeladenes Dokument zu testen.

Informationen dazu, wie Workfront automatische Aktualisierungen von Objekten protokolliert, finden Sie unter [Vom System getrackte Aktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Gewähren des Zugriffs auf Teams über Zugriffsebenen

Ein neuer Abschnitt im Bereich Zugriffsebenen bietet Ihnen detailliertere Steuerelemente für die Verwaltung des Zugriffs Ihrer Benutzer auf Teams. Jetzt können Sie bestimmen, wer Teams erstellen, bearbeiten und anzeigen kann.

Dadurch wird der vorhandene Zugriff Ihrer Benutzer auf Teams nicht geändert.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Gruppenzuordnung jetzt in Blueprints verfügbar

Einige Blueprints enthalten jetzt Gruppen, die Sie anpassen können, bevor Sie den Blueprint installieren. Sie können eine Gruppe im Blueprint einer vorhandenen Gruppe in Ihrer Workfront-Instanz zuordnen oder bei Bedarf eine neue Gruppe erstellen.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Formatierungsaktualisierungen im Bereich &quot;Benutzerdefinierte Forms&quot;

Der Bereich &quot;Benutzerdefinierte Forms&quot;hat ein neues Erscheinungsbild, das ihn mit vielen anderen Bereichen des neuen Workfront-Erlebnisses auf den neuesten Stand bringt.

Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Viele Verbesserungen beim Erstellen von berechneten benutzerdefinierten Feldern

Das Erstellen berechneter benutzerdefinierter Felder ist jetzt mit diesen Hinzufügungen im neuen Berechnungs-Editor viel einfacher:

* Sie können den Mauszeiger über einen beliebigen Ausdruck in Ihrer Berechnung bewegen, um Informationen dazu anzuzeigen, einschließlich einer Beschreibung, eines Beispiels für dessen Verwendung und eines Links zu weiteren Informationen in einem Hilfeartikel.
* Jeder hinzugefügte Ausdruck ist je nach Typ farbcodiert. Dies erleichtert das Auffinden von Ausdrücken und die sofortige Erkennung ihrer Art.
* Mithilfe von Zeilennummern können Sie Funktionen in einer langen Berechnung identifizieren und referenzieren.
* Wenn Sie mit der Eingabe eines Ausdrucks oder Feldnamens beginnen, wird eine Liste der verfügbaren Elemente angezeigt, damit Sie den gewünschten eingeben können. Wenn Sie eine offene Klammer eingeben, wird die schließende Klammer automatisch hinzugefügt.
* Sie können das Ergebnis Ihrer Berechnung mithilfe eines vorhandenen Objekts in der Vorschau anzeigen, ohne den Berechnungs-Editor verlassen zu müssen.

Außerdem können Sie im anpassbaren Text &quot;Anweisungen&quot;für ein berechnetes benutzerdefiniertes Feld die Formel des Felds ein- oder ausblenden. Dies ist nützlich, wenn Sie glauben, dass die Benutzer, die das benutzerdefinierte Formular ausfüllen, diese Informationen nicht benötigen.

Weitere Informationen zum Erstellen eines berechneten benutzerdefinierten Felds finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Audit-Protokollinformationen zu Status und Unternehmen anzeigen

Sie können jetzt einfacher Probleme mit Statusangaben und Unternehmen beheben, indem Sie Informationen dazu im Bereich Auditprotokolle unter Einrichtung anzeigen.

Beispiel:

* Sie können feststellen, wer einen Status umbenannt, gesperrt oder ausgeblendet hat und wann er dies getan hat.
* Sie können herausfinden, wer einige Mitglieder oder Stellenrollen aus einem Unternehmen entfernt hat und wann sie dies getan haben.

Informationen zum Anzeigen von Auditprotokollinformationen finden Sie unter [Audit-Protokolle anzeigen und exportieren](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprints-Unternehmenszuordnung und andere Verbesserungen

Die folgenden Blueprints-Verbesserungen sind jetzt verfügbar:

* Einige Blueprints beinhalten jetzt Unternehmen, die Sie anpassen können, bevor Sie den Blueprint installieren. Sie können ein Unternehmen im Blueprint einem bestehenden Unternehmen in Ihrer Workfront-Instanz zuordnen oder bei Bedarf ein neues Unternehmen erstellen.
* Ein neuer Blueprint-Typ, die Organisationsstruktur, ist jetzt verfügbar. Einige Blueprints enthalten Elemente von mehreren Typen (z. B. Projektvorlage und Organisationsstruktur). Sie können auf der Katalogseite nach Blueprint-Typ filtern.
* Die Abschnitte &quot;Install Preferences&quot; und &quot;Template Ownership&quot; auf der Konfigurationsseite wurden zur Vereinfachung in &quot;Template Preferences&quot; kombiniert.

Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../../administration-and-setup/blueprints/configure-template-package.md).

## Verwaltung von Firmenmitgliedschaften einfacher

Im Bereich &quot;Unternehmen&quot;ermöglicht eine aktualisierte Symbolleiste das einfache Hinzufügen vorhandener Workfront-Benutzer zu einem Unternehmen und das Entfernen von Unternehmensmitgliedern.

Zuvor waren diese Aktionen nur im Feld Unternehmen bearbeiten verfügbar.

Die aktualisierte Symbolleiste enthält auch alle Aktionen, die in der vorherigen Symbolleiste verfügbar waren, z. B. das Bearbeiten der Benutzerprofilinformationen der Mitglieder und das Deaktivieren dieser Informationen im System.

Weitere Informationen finden Sie unter [Verwalten von Firmenmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Ausdrücke und Felder im Fenster des neuen berechneten Felds auswählen

Wir machen es weiterhin einfacher, ein berechnetes Feld in einem benutzerdefinierten Formular zu erstellen. Wenn Sie nun auf Maximieren klicken, um den neuen Berechnungs-Editor zu öffnen, können Sie die benötigten Ausdrücke und Felder suchen und auswählen.

Weitere Informationen finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Gruppen können ihre eigenen Voreinstellungen für das Zeitblatt und die Stunde konfigurieren

>[!NOTE]
>
>Diese Funktion war ursprünglich nur als Teil eines schrittweisen Rollouts für Kunden auf Cluster 4 als Teil der Version 21.4 verfügbar. Diese Funktion ist für alle verbleibenden Cluster in der Produktion ab dem 8. November 2021 verfügbar.

In einer großen Organisation müssen einige Gruppen möglicherweise die Voreinstellungen für das Zeitblatt und die Stunde unabhängig voneinander konfigurieren, um ihren individuellen Workflows anzupassen, anstatt die von einem Administrator auf Systemebene konfigurierten Voreinstellungen zu übernehmen. Jetzt können Workfront-Administratoren für alle Gruppen im System die Voreinstellungen für ein Zeitblatt und eine Stunde aufheben, damit sie es selbst konfigurieren können.

Diese Möglichkeit wurde kürzlich auch für Projektvoreinstellungen sowie für Aufgaben- und Problemeinstellungen hinzugefügt.

Informationen dazu, wie ein Workfront-Administrator die Voreinstellung für ein Zeitblatt und eine Stunde freischaltet, finden Sie im Abschnitt . [Zeitblatt- und Stundenvoreinstellungen für Gruppen entsperren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) im Artikel [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Informationen dazu, wie ein Gruppenadministrator entsperrte Aufgaben konfiguriert und die Voreinstellungen für eine Gruppe ausgibt, finden Sie unter [Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Auswählen mehrerer Benachrichtigungen, die Sie für Gruppen entsperren oder erneut sperren möchten

E-Mail-Benachrichtigungen für Gruppen lassen sich jetzt schneller und einfacher entsperren oder erneut sperren. Jetzt können Sie mehrere Benachrichtigungen auswählen, Ihre Auswahl überprüfen, um sicherzustellen, dass sie korrekt sind, und dann auf die neue Schaltfläche Entsperren oder Sperren klicken, die in der Symbolleiste angezeigt wird.

Zuvor mussten Sie Benachrichtigungen einzeln entsperren und erneut sperren. Workfront verfügt derzeit über 95 Benachrichtigungen. Dies hat also eine Weile gedauert, wenn Sie dies für alle oder viele davon tun mussten.

Weitere Informationen finden Sie unter [Entsperren oder Sperren der Konfiguration von Ereignisbenachrichtigungen für alle Gruppen](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Für Gruppenadministratoren: Einfachere Auswahl einer Ersatzgruppe beim Löschen einer Gruppe

Wenn Sie eine Gruppe löschen, können Sie mit zwei Verbesserungen im Feld Gruppe löschen die Ersatzgruppe einfacher auswählen, für die Sie die Benutzer, Arbeitselemente und Untergruppen der gelöschten Gruppe beibehalten möchten:

* Sie können damit beginnen, den Namen der Gruppe einzugeben, um sie schnell zu finden. Zuvor gab es nur eine Dropdown-Liste, in die Sie nicht eingeben konnten. Dies war für Organisationen mit vielen Gruppen problematisch, da Sie durch die Liste blättern mussten, um die gewünschte Gruppe zu finden. Außerdem hatte die Dropdown-Liste eine Elementbegrenzung, sodass die gewünschte Gruppe möglicherweise nicht angezeigt wurde.
* Sie können das neue Infosymbol verwenden, um sicherzustellen, dass Sie die gewünschte Ersatzgruppe auswählen. Wenn Sie den Mauszeiger über das Symbol bewegen, wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und die Namen der Administratoren.

Weitere Informationen finden Sie unter [Gruppe löschen](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Größerer Bereich zum Erstellen berechneter Felder

Jetzt ist es einfacher, komplexe berechnete Felder in einem benutzerdefinierten Formular zu erstellen. Klicken Sie auf die neue Schaltfläche Maximieren , um ein großes Bearbeitungsfenster zum Erstellen Ihrer Berechnung zu öffnen. Wenn Sie fertig sind, klicken Sie auf Minimieren , um mit der Arbeit an Ihrem benutzerdefinierten Formular fortzufahren.

Weitere Informationen finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Hinzufügen benutzerdefinierter Formulare zu Gruppen

Benutzerdefinierte Formulare werden jetzt für das Gruppenobjekt unterstützt. Dies erleichtert es Gruppen in Ihrer Organisation, Informationen zu erfassen und freizugeben, die ihren spezifischen Anforderungen und Workflows entsprechen. Benutzer können für eine Gruppe Folgendes tun, genau wie für andere Workfront-Objekte:

* Benutzerdefiniertes Formular erstellen
* Benutzerdefiniertes Formular anhängen
* Benutzerdefinierte Formulardaten speichern
* Benutzerdefiniertes Formular entfernen
* Bearbeiten benutzerdefinierter Daten aus Listen und, im neuen Workfront-Erlebnis, von der Seite Gruppe

Informationen zu benutzerdefinierten Formularen finden Sie unter [Benutzerdefinierte Formulare](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Erstellen von OAuth2-Apps zur Integration von Anwendungen in Workfront

Jetzt können Sie Workfront mit anderen Anwendungen integrieren, für die Workfront keine integrierte Integration bietet. Wenn Sie eine OAuth2-App für die Anwendung erstellen, in die Sie integrieren möchten, können Sie dieser Anwendung den Zugriff auf Workfront erlauben, wobei Sie wissen, dass Ihre Daten durch das sichere OAuth2-Authentifizierungsprotokoll des Industriestandards geschützt sind.

Zuvor war die Integration mit anderen Anwendungen nur über integrierte Integrationen, Workfront Fusion oder die Workfront-API möglich.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Verbesserungen am Schnittstellentext im Unternehmensbereich

Im Bereich &quot;Unternehmen&quot;im Setup erleichtern neue Bestätigungsnachrichten und leichte Textänderungen die Verwaltung von Firmenmitgliedschaften. Beispielsweise lautet der Abschnittsname &quot;Personen&quot;im linken Bedienfeld jetzt &quot;Unternehmensmitglieder&quot;.

Informationen zur Verwaltung von Unternehmensmitgliedschaften finden Sie unter [Verwalten von Firmenmitgliedschaften](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
