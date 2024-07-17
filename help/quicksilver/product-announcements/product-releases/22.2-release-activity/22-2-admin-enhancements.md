---
title: 22.2 Verbesserungen für Administratoren
description: 22.2 Verbesserungen für Administratoren
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# 22.2 Verbesserungen für Administratoren

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 22.2 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022. Eine Liste aller in Version 22.2 verfügbaren Änderungen finden Sie unter [22.2 Versionsübersicht](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Benutzerdefiniertes Formular für die Verwendung mit mehreren Objekttypen konfigurieren

Jetzt können Sie ein neues oder vorhandenes benutzerdefiniertes Formular so konfigurieren, dass es mit mehreren Objekttypen verwendet werden kann, wodurch das Formular weitaus nützlicher wird. Benutzer können das Formular an Objekte aller Typen anhängen und ausfüllen, für die Sie es konfigurieren.

Zuvor konnten Sie ein benutzerdefiniertes Formular so konfigurieren, dass es nur mit einem Objekttyp funktioniert.

Diese Funktion funktioniert mit allen benutzerdefinierten Formularen, die zuvor in Ihrem Workfront-System erstellt wurden. Wenn Sie beispielsweise bereits über ein benutzerdefiniertes Formular verfügen, das für den Objekttyp &quot;Aufgabe&quot;erstellt wurde, können Sie jetzt das Formular so konfigurieren, dass es auch mit anderen Objekttypen wie Projekt und Problem funktioniert.

Weitere Informationen finden Sie im Abschnitt [Erstellen eines benutzerdefinierten Formulars beginnen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) im Artikel [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* Zum Zeitpunkt der ersten Vorschau dieser Funktion haben wir die Möglichkeit, ein benutzerdefiniertes Formular mit mehreren Objekten zu kopieren, vorübergehend deaktiviert. Diese Fähigkeit wurde am 24. März aktiviert. Informationen zum Kopieren eines benutzerdefinierten Formulars finden Sie unter [Kopieren eines benutzerdefinierten Formulars, um ein neues zu erstellen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* In einem berechneten benutzerdefinierten Feld sind einige Felder, auf die Sie verweisen, möglicherweise nicht mit Objekttypen kompatibel, die für das Formular konfiguriert sind. Unsere Lösung ist eine Platzhalterkarte, mit der die Berechnung je nach dem Objekt, an das das Formular angehängt ist, unterschiedliche Werte ausgeben kann. Am 24. März haben wir die Platzhalter hinzugefügt. Informationen zur Verwendung finden Sie im Abschnitt [Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) im Artikel [Berechnete Daten zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* Für Abschnittsumbrüche in benutzerdefinierten Formularen haben wir eine Reihe allgemeiner Anzeigeberechtigungen und Bearbeitungsberechtigungen erstellt, die für alle Objekttypen gelten, die Sie für ein Formular konfigurieren können. In einem Szenario haben wir festgestellt, dass eine dieser Berechtigungen, &quot;Eingeschränkte Bearbeitung&quot;, Fehler in einem Formular verursachen kann. Dieses Problem wurde am 24. März behoben. Weitere Informationen zu Abschnittspausen finden Sie unter [Einen Abschnittsumbruch zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>

## Der Blueprints-Katalog steht allen Benutzern zur Verfügung und Administratoren können Anfragen zulassen

Alle Adobe Workfront-Benutzer können jetzt den Katalog der verfügbaren Blueprints durchsuchen. Weitere Informationen finden Sie unter [Katalog mit Blueprints durchsuchen und Installation von Blueprints anfordern](../../../administration-and-setup/blueprints/browse-catalog.md).

Darüber hinaus kann der Systemadministrator den Zugriff für Benutzer aktivieren, um die Installation von Blueprints anzufordern. Durch Zuweisen einer Anforderungswarteschlange zum Speichern der Anforderungen können Benutzer Anforderungen aus dem Blueprints-Katalog stellen. Weitere Informationen finden Sie unter [Zugriff auf Blueprints konfigurieren](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Hinzufügen eines Bildes zu einem benutzerdefinierten Formular

In einem benutzerdefinierten Formular, das Sie erstellen oder bearbeiten, können Sie jetzt ein Bild hinzufügen und eine informative oder lehrreiche QuickInfo einfügen, die Benutzer lesen können, wenn sie den Mauszeiger darüber bewegen.

Dies kann beispielsweise hilfreich sein, um das Branding für ein neues Produkt anzuzeigen oder visuelle Informationen bereitzustellen, die Personen beim Ausfüllen des Formulars benötigen.

Zuvor waren benutzerdefinierte Formulare vollständig textbasiert.

>[!NOTE]
>
>In den neuen Adobe Workfront-Erlebnisbereichen, die noch nicht modernisiert wurden, wie z. B. dem Feld, das angezeigt wird, wenn Sie Elemente per Massenbearbeitung bearbeiten, werden keine benutzerdefinierten Formularbilder angezeigt. Sie werden angezeigt, wenn wir diese Bereiche weiter aktualisieren.

Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Neue standardmäßige Zugriffsstufenkonfigurationen

Um die Anforderungen der meisten Administratoren, die neue Zugriffsebenen erstellen, besser zu erfüllen, haben wir die Standardkonfiguration für die unten aufgeführten Optionen zur Anpassung Ihrer Einstellungen geändert. Diese werden angezeigt, wenn Sie auf das Zahnradsymbol ![](assets/gear-icon-in-access-levels.png) auf einer Schaltfläche &quot;Bearbeiten&quot;klicken.

Alle diese Änderungen deaktivieren eine Option, die zuvor standardmäßig aktiviert war. Wenn dies nicht den Anforderungen Ihrer Organisation entspricht, können Sie sie bei der Einrichtung einer neuen Zugriffsebene oder zu einem späteren Zeitpunkt aktivieren.

>[!IMPORTANT]
>
>Diese Änderung der Standardkonfiguration wirkt sich nur auf die von Ihnen erstellten Zugriffsebenen und nicht auf die zuvor erstellten Zugriffsebenen aus.

* In einer neuen Zugriffsstufe mit einem Plan-Lizenztyp:

   * Freigabe Systemweit ist nun für Projekte, Aufgaben, Probleme, Portfolios, Programme, Berichte, Filter, Dokumente und Vorlagen deaktiviert.
   * Integrierte Berichte anzeigen und Berichte öffentlich freigeben sind auch für Berichte deaktiviert.
   * Dokumente veröffentlichen ist auch für Dokumente deaktiviert.

* In einer neuen Zugriffsebene mit einem Lizenz-Typ &quot;Arbeit&quot;:

   * Freigabe Systemweit ist nun für Filter und Dokumente deaktiviert.
   * Dokumente veröffentlichen ist auch für Dokumente deaktiviert.

* In einer neuen Zugriffsebene mit einem Lizenztyp vom Typ Anforderung oder Überprüfung :

   * Freigabe Systemweit ist jetzt für Filter deaktiviert.

## Gruppe deaktivieren

Wenn sich Ihre internen Organisationen ändern, müssen Sie möglicherweise bestimmte Gruppen in Workfront nicht mehr verwenden und neue Gruppen erstellen. Um dies zu unterstützen, haben wir die Möglichkeit hinzugefügt, eine Gruppe zu deaktivieren, ohne ihre historischen Daten zu verlieren. Für reguläre Benutzer, die sie nicht sehen müssen, werden inaktive Gruppen aus den Typvorab-Feldern der Gruppe gelöscht.

Sie können weiterhin Optionen, Voreinstellungen und Objektverknüpfungen für von Ihnen verwaltete inaktive Gruppen finden und konfigurieren. Die Deaktivierung einer Gruppe ändert nichts an den Objekten, mit denen die Gruppe verbunden ist.

Zuvor war es nicht möglich, eine Gruppe zu deaktivieren.

Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Verbesserungen am Installationsverlauf von Blueprints

Wenn Sie einen Blueprint installieren, werden in einer Meldung jetzt die spezifischen Objekte (z. B. Rollen, Teams oder Gruppen) angezeigt, die erfolgreich mit dem Blueprint installiert wurden, sowie alle Objekte, die nicht installiert werden konnten. Sie können die Liste der installierten Objekte auch auf der Seite &quot;Blueprint-Details&quot;anzeigen, indem Sie in der Tabelle &quot;Installationsverlauf&quot;neben einer bestimmten Installation auf Details anzeigen klicken.

Weitere Informationen finden Sie unter [Blueprint installieren](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Bei der Installation eines reinen Vorschau-Blueprints in der Produktion wird jetzt ein Warnhinweis angezeigt

Bestimmte Blueprints können nur zu Testzwecken in der Vorschau-Umgebung installiert werden.

Wenn Sie auf reine Vorschau-Inhalte in Ihrer Produktionsumgebung, Sandbox 1 oder Sandbox 2 zugreifen, ist die Schaltfläche &quot;Installieren&quot;nicht aktiv und es wird möglicherweise eine Warnmeldung angezeigt.

Weitere Informationen finden Sie unter [Blueprint installieren](../../../administration-and-setup/blueprints/blueprints-install.md).
