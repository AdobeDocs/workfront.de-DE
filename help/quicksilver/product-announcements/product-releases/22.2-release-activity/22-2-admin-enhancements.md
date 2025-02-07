---
title: 22.2 Administrator-Verbesserungen
description: 22.2 Administrator-Verbesserungen
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# 22.2 Administrator-Verbesserungen

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit Version 22.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022. Eine Liste aller Änderungen, die mit Version 22.2 verfügbar sind, finden Sie unter Übersicht über Version [22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Konfigurieren eines benutzerdefinierten Formulars für die Arbeit mit mehreren Objekttypen

Jetzt können Sie ein neues oder vorhandenes benutzerdefiniertes Formular so konfigurieren, dass es mit mehreren Objekttypen funktioniert, wodurch das Formular viel nützlicher wird. Benutzer können das Formular an Objekte aller Typen anhängen und ausfüllen, für die Sie es konfigurieren.

Zuvor konnten Sie ein benutzerdefiniertes Formular so konfigurieren, dass es nur mit einem Objekttyp funktioniert.

Diese Funktion funktioniert mit allen benutzerdefinierten Formularen , die zuvor in Ihrem Workfront-System erstellt wurden. Wenn Sie beispielsweise bereits über ein benutzerdefiniertes Formular verfügen, das für den Aufgabenobjekttyp erstellt wurde, können Sie das Formular jetzt so konfigurieren, dass es auch mit anderen Objekttypen wie Projekt und Problem funktioniert.

>[!NOTE]
>
>* Zum Zeitpunkt unserer ersten Vorschau-Version dieser Funktion haben wir die Möglichkeit vorübergehend deaktiviert, ein benutzerdefiniertes Formular mit mehreren Objekten zu kopieren. Diese Funktion wurde am 24. März aktiviert.
>* In einem berechneten benutzerdefinierten Feld sind einige Felder, auf die Sie verweisen, möglicherweise nicht mit den Objekttypen kompatibel, die für das Formular konfiguriert sind. Unsere Lösung ist ein Platzhalter, mit dem die Berechnung verschiedene Werte ausgeben kann, je nach dem Objekt, an das das Formular angehängt ist. Wir haben den Joker am 24. März hinzugefügt.
>* Für Abschnittsumbrüche in benutzerdefinierten Formularen haben wir einen Satz allgemeiner Anzeige- und Bearbeitungsberechtigungen erstellt, die für alle Objekttypen funktionieren, die Sie für ein Formular konfigurieren können. In einem Szenario haben wir festgestellt, dass eine dieser Berechtigungen, „Eingeschränkte Bearbeitung“, Fehler in einem Formular verursachen kann. Dieses Problem wurde am 24. März behoben.
>

## Der Blueprint-Katalog ist für alle Benutzer verfügbar und Administratoren können Anfragen zulassen.

Alle Adobe Workfront-Benutzer können jetzt den Katalog der verfügbaren Blueprints durchsuchen. Weitere Informationen finden Sie unter [Durchsuchen des Blueprint-Katalogs und Anfordern der Installation von Blueprints](../../../administration-and-setup/blueprints/browse-catalog.md).

Darüber hinaus kann der Systemadministrator den Zugriff für Benutzer aktivieren, um die Installation von Blueprints anzufordern. Wenn Sie eine Anfrage-Warteschlange zum Speichern der Anfragen zuweisen, können Benutzer Anfragen aus dem Blueprint-Katalog stellen. Weitere Informationen finden Sie unter [Zugriff auf Blueprints konfigurieren](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Hinzufügen eines Bildes zu einem benutzerdefinierten Formular

In einem benutzerdefinierten Formular, das Sie erstellen oder bearbeiten, können Sie jetzt ein Bild hinzufügen und eine informative oder lehrreiche QuickInfo einfügen, die Benutzende lesen können, wenn sie den Mauszeiger darüber bewegen.

Dies könnte beispielsweise hilfreich sein, um das Branding für ein neues Produkt anzuzeigen oder visuelle Informationen bereitzustellen, die beim Ausfüllen des Formulars benötigt werden.

Zuvor waren benutzerdefinierte Formulare vollständig textbasiert.

>[!NOTE]
>
>In den neuen Adobe Workfront-Erlebnisbereichen, die noch nicht modernisiert wurden, z. B. das Feld, das angezeigt wird, wenn Sie Elemente stapelweise bearbeiten, werden benutzerdefinierte Formularbilder nicht angezeigt. Sie werden angezeigt, während wir diese Bereiche weiter aktualisieren.


## Neue standardmäßige Zugriffsebenen-Konfigurationen

Um den Anforderungen der meisten Administratoren, die neue Zugriffsebenen erstellen, besser gerecht zu werden, haben wir die Standardkonfiguration für die unten aufgeführten Optionen „Optimieren Sie Ihre Einstellungen“ geändert. Diese werden angezeigt, wenn Sie auf das Zahnradsymbol ![Zahnradsymbol Zugriffsebenen](assets/gear-icon-in-access-levels.png) auf einer Bearbeitungsschaltfläche klicken.

Alle diese Änderungen deaktivieren eine Option, die zuvor standardmäßig aktiviert war. Wenn dies nicht den Anforderungen Ihres Unternehmens entspricht, können Sie diese beim Einrichten einer neuen Zugriffsebene oder zu einem späteren Zeitpunkt aktivieren.

>[!IMPORTANT]
>
>Diese Standardkonfigurationsänderung betrifft nur Zugriffsebenen, die Sie ab jetzt erstellen, nicht die zuvor erstellten.

* In einer neuen Zugriffsebene mit dem Lizenztyp „Plan“:

   * Die systemweite Freigabe ist jetzt für Projekte, Aufgaben, Probleme, Portfolios, Programme, Berichte, Filter, Dokumente und Vorlagen deaktiviert.
   * Die Option „Integrierte Berichte anzeigen“ und „Berichte öffentlich freigeben“ sind auch für Berichte deaktiviert.
   * Dokumente öffentlich freigeben ist auch für Dokumente deaktiviert.

* In einer neuen Zugriffsebene mit dem Lizenztyp Arbeit :

   * Die systemweite Freigabe ist jetzt für Filter und Dokumente deaktiviert.
   * Dokumente öffentlich freigeben ist auch für Dokumente deaktiviert.

* In einer neuen Zugriffsebene mit dem Lizenztyp Anfrage oder Überprüfung :

   * Die systemweite Freigabe ist jetzt für Filter deaktiviert.

## Deaktivieren von Gruppen

Wenn sich Ihre internen Organisationen ändern, müssen Sie möglicherweise bestimmte Gruppen in Workfront nicht mehr verwenden und neue erstellen. Um Ihnen dabei zu helfen, haben wir die Möglichkeit hinzugefügt, eine Gruppe zu deaktivieren, ohne ihre historischen Daten zu verlieren. Für reguläre Benutzer, die sie nicht sehen müssen, werden inaktive Gruppen aus Feldern mit Eingabepuffer für Gruppen entfernt.

Sie können weiterhin Optionen, Voreinstellungen und Objektverknüpfungen für inaktive Gruppen suchen und konfigurieren, die Sie verwalten. Und das Deaktivieren einer Gruppe ändert nichts an den Objekten, mit denen die Gruppe verbunden ist.

Zuvor war es nicht möglich, eine Gruppe zu deaktivieren.

Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Verbesserungen des Blueprint-Installationsverlaufs

Wenn Sie eine Blueprint installieren, werden in einer Meldung jetzt die spezifischen Objekte (z. B. Rollen, Teams oder Gruppen) angezeigt, die mit der Blueprint erfolgreich installiert wurden, sowie alle Objekte, die nicht installiert werden konnten. Sie können die Liste der installierten Objekte auch auf der Seite Blueprint-Details anzeigen, indem Sie neben einer bestimmten Installation in der Tabelle Installationsverlauf auf Details anzeigen klicken.

Weitere Informationen finden Sie unter [Blueprint installieren](../../../administration-and-setup/blueprints/blueprints-install.md).

![Blueprints-Installationsverlauf](assets/blueprints-installation-history-350x95.png)

## Bei der Installation einer Blueprint, die nur die Vorschau enthält, wird jetzt eine Warnung angezeigt

Bestimmte Blueprints können nur zu Testzwecken in der Vorschau-Umgebung installiert werden.

Wenn Sie in Ihrer Produktionsumgebung, Sandbox 1 oder Sandbox 2 auf Nur-Vorschau-Inhalt zugreifen, ist die Schaltfläche Installieren nicht aktiv und möglicherweise wird eine Warnmeldung angezeigt.

Weitere Informationen finden Sie unter [Blueprint installieren](../../../administration-and-setup/blueprints/blueprints-install.md).
