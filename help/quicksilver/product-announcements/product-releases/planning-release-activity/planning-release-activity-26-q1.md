---
content-type: release-notes
title: Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2026
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im ersten Quartal 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: af1a54ea-1717-45fa-bb94-55774eb28f28
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '2017'
ht-degree: 0%

---

# Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2026

In diesem Artikel werden die Funktionen beschrieben, die in der Version vom ersten Quartal 2026 für Workfront Planning veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Globale Datensatztypen können über den sekundären Arbeitsbereich freigegeben werden

>[!NOTE]
>
>Vorschau: 15. Januar 2026
>Produktions-Schnellveröffentlichung: 15. Januar 2026
>Produktion für alle: 15. Januar 2026
>[!BADGE Aus dem Zeitplan]{type=Neutral}

Sie können jetzt globale Datensatztypen freigeben, die Sie einem sekundären Arbeitsbereich aus diesem Arbeitsbereich hinzugefügt haben. Benutzer erhalten dieselben Berechtigungen für alle Datensätze im sekundären Arbeitsbereich, den Sie freigeben.

>[!NOTE]
>
>Benutzer können im primären Arbeitsbereich oder in jedem anderen sekundären Arbeitsbereich, in dem der Datensatztyp hinzugefügt wurde, unterschiedliche Berechtigungen für denselben globalen Datensatztyp haben. Berechtigungen für Workspace und Datensatztypen werden auf die Datensätze übertragen.

Vor dieser Änderung konnten Sie den globalen Datensatztyp nur über den ursprünglichen, primären Arbeitsbereich freigeben.

Weitere Informationen finden Sie [Übersicht über Workspace-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


## Datensätze, die einem globalen Datensatztyp in einem sekundären Arbeitsbereich hinzugefügt wurden, sind von anderen sekundären Arbeitsbereichen nicht sichtbar

>[!NOTE]
>
>Vorschau: 15. Januar 2026
>Produktions-Schnellveröffentlichung: 15. Januar 2026
>Produktion für alle: 15. Januar 2026
>[!BADGE Aus dem Zeitplan]{type=Neutral}

Datensätze, die einem globalen Datensatztyp in einem sekundären Arbeitsbereich hinzugefügt wurden, sind nur in diesem Arbeitsbereich oder im ursprünglichen primären Arbeitsbereich des Datensatztyps sichtbar. Vor diesem Update waren Datensätze, die zu einem sekundären Arbeitsbereich hinzugefügt wurden, auch von anderen sekundären Arbeitsbereichen sichtbar, für die Sie möglicherweise über die Berechtigung zum Anzeigen verfügten.

Weitere Informationen finden Sie [Übersicht über Workspace-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Erstellen von Hierarchien von Datensatztypen in Arbeitsbereichen

>[!NOTE]
>
>Vorschau: 23. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

Sie können jetzt flexible, aber strukturierte Hierarchien zwischen Datensatz- oder Objekttypen definieren.

Hierarchien sind Verbindungen zwischen Datensatztypen. Es können bis zu 4 Datensatz- und Objekttypen in einer Hierarchie verbunden sein, und es können bis zu 5 Hierarchien in einem Arbeitsbereich vorhanden sein. Der erste Datensatztyp in der Hierarchie ist das erste übergeordnete Element.

Sie können Hierarchien verwenden, um die Arbeit zu organisieren und zu visualisieren, wie die Strategie in die Ausführung fließt.

Beachten Sie beim Erstellen von Hierarchien Folgendes:

* Sie können nur Planning-Datensatztypen aus einem Arbeitsbereich und Workfront-Projekten in einer Hierarchie verbinden.
* Ein Datensatztyp oder Projekt kann nur ein übergeordnetes Element im selben Arbeitsbereich haben.
* Ein Datensatztyp kann in mehreren Hierarchien das übergeordnete Element sein.
* Verbindbare Datensatztypen können nicht in Hierarchien in anderen Arbeitsbereichen als ihren eigenen verwendet werden.
* Globale Datensatztypen können in Hierarchien nur in den Arbeitsbereichen verwendet werden, in denen sie erstellt wurden oder denen sie hinzugefügt wurden.

Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Neue einheitliche Breadcrumbs zu den Datensatzseiten hinzugefügt

>[!NOTE]
>
>Vorschau: 23. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

Wenn Sie Hierarchien zwischen Datensatztypen erstellen, generieren diese Breadcrumbs für Datensätze, die zu diesen Datensatztypen gehören.

Breadcrumbs für Datensätze spiegeln ihre Position in der Hierarchie wider. Nachdem Sie Hierarchien erstellt haben, können Sie den Breadcrumb eines Datensatzes oben auf der Seite sehen. Er gibt an, welche anderen übergeordneten oder untergeordneten Objekte mit ihm verbunden sind. Hierarchien sind in Workfront und Planning konsistent.

Sie können beispielsweise die Planungshierarchie eines Projekts anzeigen, wenn es mit den Planungs-Datensatztypen im Planungs-Breadcrumb verbunden ist, und die Workfront-Hierarchie, wenn es mit Workfront-Objekttypen wie Portfolios oder Programmen in Workfront verbunden ist.

Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Verbesserungen bei verbundenen Datensätzen und Seiten

>[!NOTE]
>
>Vorschau: 19. Dezember 2025
>Produktionsgeschwindigkeit: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

Um Ihnen bei der Arbeit mit verbundenen Datensatzseiten mehr Flexibilität zu bieten, haben wir die Funktionalität der Ansichten in diesem Bereich von Workfront Planning erweitert. Im Folgenden finden Sie Verbesserungen bei den verbundenen Datensatzseiten eines Datensatzes:

* Sie können der Seite „Verbundene Datensätze“ eines Datensatzes jetzt eine Timeline und eine Kalenderansicht hinzufügen.
* Sie können jetzt alle Ansichten einer verbundenen Datensatzseite freigeben. Die auf diesen Seiten freigegebenen Ansichten sind systemweit für alle Benutzenden sichtbar, für die Sie sie in einem anderen Bereich von Workfront Planning freigeben. Alle in anderen Bereichen von Planning freigegebenen Ansichten sind auch auf der Seite „Verbundene Datensätze“ für dieselben Benutzer sichtbar, für die sie freigegeben wurden.
* Wir haben eine Einschränkung hinzugefügt, die besagt, dass pro Datensatz oder Objekttyp nur eine verbundene Datensatzseite zulässig ist. Vor dieser Verbesserung konnten Sie mehrere Seiten für denselben Datensatz oder Objekttyp hinzufügen. Jetzt können Sie mehrere Ansichten für denselben Datensatztyp auf einer verbundenen Datensatzseite verwenden.
* Wir haben einen **Neue Zeile**-Link am unteren Rand einer Tabellenansicht und eine Schaltfläche **Datensätze verbinden** im oberen rechten Bereich der Seite „Verbundene Datensätze“ hinzugefügt. Vor dieser Verbesserung waren der Link **Neue Zeile** und die Schaltfläche **Datensätze verbinden** nur auf einer projektverbundenen Seite vorhanden.

Weitere Informationen finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Freigeben von Ansichten auf der Seite „Verbundene Projekte“

>[!NOTE]
>
>Vorschau: 18. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026\
>Produktion für alle: 15. Januar 2026

Um die Anzeige der benötigten Informationen zu vereinfachen, haben wir die Möglichkeit hinzugefügt, Ansichten auf der Seite „Verbundene Projektdatensätze“ freizugeben. Jetzt können Sie Ansichten mit anderen Benutzern, Teams oder Gruppen teilen.

Weitere Informationen finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Platzhalter für aktuelle Benutzer jetzt in den Filtern für die Projektansicht verfügbar

>[!NOTE]
>
>Vorschau: 18. Dezember 2025
>Produktions-Schnellveröffentlichung: 14. Januar 2026\
>Produktion für alle: 15. Januar 2026

Um das Filtern nach Projektverbindungen zu vereinfachen, die für Sie gelten, haben wir einen Platzhalter für aktuelle Benutzer erstellt. Jetzt können Sie beim Filtern „Ich (angemeldeter Benutzer)“ auswählen. Der Filter gilt dann für den Benutzer, der die Anfrageliste anzeigt.

Dies kann praktisch sein, wenn ein Filter zu einer Ansicht hinzugefügt wird, die von mehreren Benutzern verwendet wird. Jeder Benutzer sieht die Filterergebnisse, die für ihn gelten.

Der Platzhalter ist in Feldern verfügbar, in denen der Wert ein Benutzer ist.

Weitere Informationen zum Konfigurieren von Projektverbindungsansichten, einschließlich Filtern, finden Sie unter [Hinzufügen einer Seite mit verbundenen Datensätzen zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).


## Verbesserungen an der Workspace-Hauptseite

>[!IMPORTANT]
>
>Diese wurde zwischen dem 20. Januar und dem 17. Februar 2026 vorübergehend aus der Vorschau- und Produktionsumgebung entfernt.

>[!NOTE]
>
>Vorschau: 18. Dezember 2025
>Produktionsgeschwindigkeit: 14. Januar 2026
>Produktion für alle: 15. Januar 2026

An der Hauptseite für Arbeitsbereiche in Workfront Planning wurden folgende Verbesserungen vorgenommen:

* Ein schnelleres, dynamischeres Scrollen. Dies wird besonders deutlich, wenn Ihr Unternehmen über eine große Anzahl von Arbeitsbereichen verfügt, und gilt für Systemadministratoren.

* Wir haben ein Suchfeld hinzugefügt, mit dem Sie jetzt nach einem bestimmten Arbeitsbereich anhand des Namens suchen können.

* Die Registerkarte **Andere Arbeitsbereiche** wurde in &quot;**Arbeitsbereiche“** und enthält alle Arbeitsbereiche, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen, einschließlich der von Ihnen erstellten.

Weitere Informationen finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/planning/architecture/edit-workspaces.md).


## Hinzufügen des Felds Markenverbindung zu Produkten und Rollen im GenStudio Workspace

>[!NOTE]
>
>Vorschau: 11. Dezember 2025
>Produktions-Schnellveröffentlichung: 11. Dezember 2025
>Produktion für alle: 11. Dezember 2025
>[!BADGE Aus dem Zeitplan]{type=Neutral}

Das Feld Verbindung zur Marke GenStudio for Performance Marketing wird jetzt standardmäßig zu den Datensatztypen „Produkte“ und „Personas“ im Arbeitsbereich &quot;GenStudio&quot; von Workfront Planning hinzugefügt.

Ihr Unternehmen muss sowohl über Workfront Planning als auch über Adobe GenStudio for Performance Marketing verfügen.

Vor dieser Verbesserung konnten Sie das Feld Markenverbindung nur manuell zu einem beliebigen Datensatztyp hinzufügen, einschließlich Produkten und Rollen. Sie können den Datensatztyp Brand GenStudio weiterhin manuell mit anderen Datensatztypen in Workfront Planning verbinden.

Weitere Informationen finden Sie [Erste Schritte mit der Adobe Workfront Planning and Adobe GenStudio for Performance Marketing-Integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Entfernen von GenStudio for Performance Marketing-Benutzerberechtigungen aus Planning einschränken

>[!NOTE]
>
>Vorschau: 11. Dezember 2025
>Produktions-Schnellveröffentlichung: 11. Dezember 2025
>Produktion für alle: 11. Dezember 2025
>[!BADGE Aus dem Zeitplan]{type=Neutral}

Wir haben einen Schutzmechanismus hinzugefügt, der verhindert, dass Berechtigungen von GenStudio for Performance Marketing-Benutzenden aus Workfront Planning-Objekten entfernt werden. Mit dieser Verbesserung können Sie GenStudio-Benutzende nicht mehr aus dem GenStudio-Arbeitsbereich in Planning entfernen. Ebenso können Sie keine geerbten Berechtigungen für Datensatztypen im GenStudio-Arbeitsbereich deaktivieren, wenn diese Berechtigungen GenStudio-Benutzende enthalten. Wenn Sie diese Benutzenden vor dieser Verbesserung aus GenStudio Workspace in Planning entfernt haben, verlieren sie auch die Berechtigungen für Datensatztypen in GenStudio.

Ihr Unternehmen muss sowohl über Workfront Planning als auch über Adobe GenStudio for Performance Marketing verfügen.

Weitere Informationen finden Sie [Erste Schritte mit Adobe Workfront Planning und Adobe GenStudio for Performance Marketing Integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Öffentliche Freigabe von Ansichten für einen globalen Datensatztyp in einem sekundären Arbeitsbereich entfernt


>[!NOTE]
>
>Vorschau: 3. Dezember 2025
>Produktions-Schnellveröffentlichung: 4. Dezember 2025
>Produktion für alle: 15. Januar 2026


Wir haben die Registerkarte Öffentliche Freigabe bei der Freigabe einer Ansicht für einen globalen Datensatz in einem sekundären Arbeitsbereich entfernt. Sie können eine Ansicht nicht öffentlich über einen globalen Datensatztyp freigeben, der über einen vorhandenen globalen Datensatztyp zu einem anderen Arbeitsbereich hinzugefügt wurde. Sie können eine Ansicht des globalen Datensatztyps öffentlich über den ursprünglichen Arbeitsbereich freigeben.

Weitere Informationen finden Sie unter [Freigeben von Ansichten](/help/quicksilver/planning/access/share-views.md).


## Verbinden von GenStudio for Performance Marketing Brands mit Workfront Planning-Datensatztypen

>[!NOTE]
>
>Vorschau: 13. November 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 13. November 2025

Sie können jetzt Datensatztypen für Workfront Planning mit Marken aus Adobe GenStudio for Performance Marketing verbinden. Ihr Unternehmen muss sowohl über Workfront Planning als auch über Adobe GenStudio for Performance Marketing verfügen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).


## Neues Suchfeld für Felder in den Symbolen für Filter, Felder und Zeilenfarben in Planning-Ansichten

>[!NOTE]
>
>Vorschau: 6. November 2025
>Produktions-Schnellveröffentlichung: 11. Dezember 2025
>Produktion für alle: 15. Januar 2026

Sie können jetzt beim Erstellen eines Ansichtselements in einer Datensatztypansicht nach einem bestimmten Feld suchen. Wir haben Suchfelder hinzugefügt, wenn Sie einen Filter, eine Sortierung, eine Gruppierung oder Ihre Felder- oder Zeilenfarben konfigurieren. Vor dieser Verbesserung konnten Sie einfach durch die Liste der verfügbaren Felder scrollen.

Diese Verbesserung ist in allen Ansichten vom Typ Datensatz verfügbar.

Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).


## Globale Datensatztypen und die Möglichkeit, sie als vorhandene Datensatztypen zu anderen Arbeitsbereichen hinzuzufügen

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Bei der Implementierung von Workfront Planning für ein Unternehmen mit mehreren Teams mit gemeinsamen Workflows müssen Sie möglicherweise eine zusammenhängende Struktur und Metadaten für wichtige Datensatztypen (wie Kampagnen oder Ergebnisse) definieren, die den Arbeitsbereichen jedes Teams hinzugefügt werden können, um ihre Arbeit zu erfassen und zu verwalten.

Außerdem benötigen Sie möglicherweise die Arbeit jedes Teams, um eine zentrale Ebene zu erreichen.

In einem solchen Workflow können Sie sicherstellen, dass Teams ihre Arbeit konsistent erfassen, während Sie die Team-übergreifende Sichtbarkeit erschließen, ohne dass alle Personen in der Organisation zu jedem Arbeitsbereich hinzugefügt werden müssen. Sie können dazu globale Datensatztypen verwenden.

Sie können jetzt einen Datensatztyp als „global“ festlegen und ihn über mehrere Arbeitsbereiche hinweg verwenden. Benutzer können dieselbe Feldstruktur und dieselben Verbindungen verwenden, die bereits in einem zentralen Arbeitsbereich konfiguriert sind.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Arbeitsbereichsübergreifende Übersicht über den Datensatztyp](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Konfigurieren von arbeitsbereichsübergreifenden Datensatztyp-Funktionen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Neues Limit für Verbindungsfelder für einen Datensatztyp

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Wir haben für jeden Datensatztyp ein Limit von 30 Verbindungsfeldern eingeführt.

HINWEIS: Wenn Ihr Unternehmen derzeit mehr als 30 Verbindungsfelder für einen Datensatztyp hat, können Sie die zusätzlichen Felder beibehalten, die das Limit von 30 überschreiten. Sie können jedoch nicht mehr Verbindungsfelder zu diesen Datensatztypen hinzufügen, die das Limit überschreiten. In Zukunft wird die neue Beschränkung von 30 Verbindungsfeldern erzwungen.

Weitere Informationen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Festlegen benutzerfreundlicher Werte für Feldoptionen vom Typ Auswahl

>[!NOTE]
>
>Vorschau: 16. Oktober 2025
>Produktions-Schnellveröffentlichung: 13. November 2025
>Produktion für alle: 15. Januar 2026

Beim Hinzufügen von Feldoptionen zu einem Ein- oder Mehrfachauswahlfeld weist Workfront jeder Auswahl jetzt benutzerfreundliche Werte zu. Vor dieser Verbesserung generierte Workfront eine alphanumerische ID, die in API-Aufrufen und anderen Integrationen schwer zu verstehen und zu verwenden war.

Beachten Sie bei dieser Verbesserung Folgendes:

* Die neuen Werte werden den neuen Feldoptionen hinzugefügt. Vorhandene Feldoptionen behalten ihre alphanumerischen IDs bei.

* Auswahlwerte sind für ein Feld eindeutig, können jedoch zwischen verschiedenen Feldern wiederholt werden.

* Beim Umbenennen einer Auswahl wird ihr ursprünglicher Wert nicht aktualisiert.

* Bei Auswahl mit mehreren Wörtern werden die Auswahlwerte in Kleinbuchstaben angezeigt und bei Auswahl mit mehreren Wörtern durch Unterstriche getrennt. Wenn Sie eine bereits als anderer Auswahlname für dasselbe Feld verwendete Beschriftung verwenden, fügt Workfront eine sequenzielle Zahl zum Wert hinzu.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
