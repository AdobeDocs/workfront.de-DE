---
title: Workfront Planning - Terminologieübersicht
description: Obwohl Adobe Workfront Planning ein Workfront-Produkt ist, enthält es proprietäre Konzepte und Terminologie. Machen Sie sich mit diesen Konzepten vertraut, bevor Sie Workfront-Planung für Ihre Organisation einrichten.
author: Alina
feature: Workfront Planning
role: User, Admin
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 59%

---

# Workfront Planning - Terminologieübersicht


<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Workfront Planning. Workfront Planning ist entweder ein eigenständiges Produkt oder eine zusätzlich erworbene Funktion von Adobe Workfront.
>
>
>Dieser Artikel enthält allgemeine Informationen zu Workfront Planning, wenn Kunden auch ein Workfront- oder Workflow-Paket erwerben.
>
>Eine vollständige Liste der Artikel mit Dokumentationen zu Workfront Planning finden Sie unter [Allgemeine Informationen und Artikelindex für Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Informationen zu Workfront Planning als eigenständiges Produkt finden Sie unter [Erste Schritte mit Adobe Workfront Planning als eigenständiges Produkt](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

Obwohl Workfront-Planung ein Teil von Workfront ist, verfügt es über proprietäre Konzepte und eigene Terminologie. Machen Sie sich mit diesen Konzepten vertraut, bevor Sie Workfront-Planung für Ihre Organisation einrichten.

Das Framework für Workfront-Planung ist vollständig anpassbar. Sie können alle Eintragstypen, ihre Attribute und alle diesen zugeordneten Felder für die genauen Anforderungen Ihrer Organisation erstellen.

Es gibt Einschränkungen im Hinblick auf die Anzahl der Workfront-Planung-Objekte, die Sie erstellen können. Weitere Informationen finden Sie unter [Überblick über Objektbeschränkungen für Adobe Workfront-Planung](/help/quicksilver/planning/general/limitations-overview.md).

Im Folgenden finden Sie die wichtigsten Objekte und Konzepte von Workfront-Planung:

* [Arbeitsbereiche](#workspaces)
* [Eintragstypen](#record-types)
* [Einträge](#records)
* [Arbeitsbereichsvorlagen](#workspace-templates)
* [Felder](#fields)
* [Verbundene Datensatztypen, Datensätze und Felder](#connected-record-types-records-and-fields)
* [Suchfelder](#lookup-fields)
* [Hierarchien](#hierarchies)
* [Ansichten](#views)
* [Automatisierungen](#automations)
* [Antragsformulare](#request-forms)

## Arbeitsbereiche

Arbeitsbereiche stellen den Rahmen einer Organisationseinheit dar. Es handelt sich um Sammlungen von Datensatztypen, die den Betriebslebenszyklus einer bestimmten Organisation definieren.

![Marketing-Arbeitsbereich mit Taxonomien für Eintragstypen – Startseite](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

## Eintragstypen

Datensatztypen sind die Objekttypen in Workfront Planning.

Eintragstypen befüllen Arbeitsbereiche.

Anders als bei Workfront, wo die Objekttypen vordefiniert sind, können Sie in Workfront-Planung Ihre eigenen Objekttypen erstellen.

In Workfront sind beispielsweise die Objekttypen „Programm“, „Portfolio“, „Projekt“, „Aufgabe“ oder „Problem“ bereits erstellt.

In Workfront-Planung können Sie beliebige Eintragstypen erstellen, die den Workflows Ihrer Organisation entsprechen. Später können Sie definieren, wie die Eintragstypen miteinander in Beziehung stehen oder Abhängigkeiten bilden.

Weitere Informationen finden Sie unter [Überblick über Eintragstypen](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Einträge

Ein Datensatz ist eine Instanz eines Datensatztyps.

![In der Liste der Kampagneneintragstypen hervorgehobene Einträge](assets/records-highlighted-in-campaign-record-type-list.png)

Nachdem Sie einem Arbeitsbereich einen Eintragstyp hinzugefügt haben, können Sie damit beginnen, Einträge dieses Typs auf der Seite des Eintragstyps hinzuzufügen.

Beispiel: „Kampagne“ kann ein Eintragstyp sein und „Sommerkampagne für EMEA“ ist ein Eintrag des Eintragstyps „Kampagne“.

Weitere Informationen finden Sie unter [Erstellen von Einträgen](/help/quicksilver/planning/records/create-records.md).

## Arbeitsbereichsvorlagen

Sie können einen Arbeitsbereich mithilfe vordefinierter Vorlagen erstellen. Sie können die vordefinierten Eintragstypen und Felder in einer Vorlage verwenden oder eigene hinzufügen.

![Arbeitsbereichsseite mit Vorlagen und Miniaturansichten](assets/workspaces-page-with-templates-thumbnails.png)

Adobe Workfront-Planung enthält die folgenden Vorlagen:

* Operations Initiative Studio
* Kommunikationsstudio
* Basis: Marketing-Management
* Erweitert: Marketing-Management
* Enterprise: Marketing-Management
* Vertriebs-Management
* Produkt-Management

Systemadministratoren können auch sechs Arbeitsbereiche installieren, wenn sie die Best-Practice-Vorlage für mehrere Arbeitsbereiche verwenden. Die Multi-Space-Vorlage enthält die folgenden Vorlagen, die 6 separate, aber miteinander verbundene Arbeitsbereiche gleichzeitig generieren:

* &#x200B;1. Globale Klassifizierungen und Taxonomien
* 2.Fréscopa Global Marketing
* 3.Fréscopa Social Marketing
* 4.Fréscopa Medien und PR
* 5.Fréscopa Global Events
* 6.Fréscopa Führende Unternehmensführung

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Liste der Arbeitsbereichsvorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).
* [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

## Felder

Felder sind Attribute, die Sie Datensatztypen hinzufügen können. Felder enthalten Informationen über den Datensatztyp.

![Dropdown-Liste der Eintragsfelder](assets/drop-down-list-of-record-fields.png)

Überlegungen zu Eintragsfeldern:

* Die Felder, die Sie für einen Eintragstyp hinzufügen, werden automatisch mit allen Einträgen dieses Typs verknüpft und können verwendet werden, um Daten zu diesen Einträgen zu erfassen.

* Felder werden als Spalten in der Tabellenansicht angezeigt, die auf eine Eintragstypseite angewendet wird. Sie werden auch auf der Seite des Eintrags angezeigt.

* Felder sind für einen Eintragstyp eindeutig und werden nicht von einem Eintragstyp zu einem anderen übertragen.

* Felder können vollständig angepasst werden und sind nur in Workfront-Planung verfügbar. Sie können über Workfront nicht auf Felder in Workfront-Planung zugreifen.

Weitere Informationen finden Sie unter [Erstellen von Feldern](/help/quicksilver/planning/fields/create-fields.md).

Standardmäßig ist ein neuer Eintragstyp mit den folgenden vordefinierten Feldern verknüpft:

* Name
* Beschreibung
* Startdatum
* Enddatum
* Status

Sie können benutzerdefinierte Felder der folgenden Typen erstellen:

* Einzeiliger Text
* Absatz
* Mehrfachauswahl
* Einzelauswahl
* Datum
* Zahl
* Prozentsatz
* Währung
* Kontrollkästchen
* Formel
* Personen
* Erstellt von
* Erstellungsdatum
* Zuletzt geändert von
* Zuletzt geändert am
* Genehmigt von
* Genehmigungsdatum
* Eintrags-ID

<!--update the screen shot above-->

## Verbundene Datensatztypen, Datensätze und Felder

Sie können in Workfront Planning eine Verbindung zwischen den folgenden Entitäten erstellen:

* Zwei Eintragstypen in Workfront-Planung.
* Einem Eintragstyp und einem Workfront-Projekt, -Programm, -Portfolio, -Unternehmen oder -Gruppenobjekttyp.
* Einem Eintragstyp und einem Adobe Experience Manager-Asset oder -Ordner.

  Sie müssen über eine Adobe Experience Manager-Lizenz verfügen, um Eintragstypen mit Experience Manager-Objekten verbinden zu können.

  ![Registerkarte „Neue Verbindung“ mit Workfront AEM-Optionen](assets/new-connection-tab-with-workfront-aem-options.png)

* Einem Eintragstyp und einer Adobe GenStudio for Performance Marketing-Marke.

  Sie müssen über eine Adobe GenStudio for Performance Marketing-Lizenz verfügen, um Eintragstypen mit GenStudio-Marken verbinden zu können.

  ![Registerkarte „Neue Verbindung“ mit der Option &quot;Adobe GenStudio – Marke“](assets/new-connection-tab-with-genstudio-option.png)

Nachdem Sie eine Verbindung zwischen den Datensatztypen bzw. den Datensatz- und Objekttypen hergestellt haben, können Sie einzelne Datensätze oder Objekte dieser Typen miteinander verbinden. Die Verbindung zwischen den Einträgen wird als verbundenes Eintragsfeld oder als Verbindung angezeigt.

Das Verbinden von Eintragstypen ist hilfreich, wenn sich mehrere Typen von Arbeitsobjekten gegenseitig beeinflussen. Sie können beispielsweise mit Kampagnen arbeiten, wobei jede Kampagne mehreren Marken gerecht werden kann. Um diese Beziehung anzugeben, können Sie Kampagnen mit Marken verbinden. Darüber hinaus kann es sein, dass die Arbeit für jede Kampagne in mehreren Projekten in Workfront geplant wird. Um dies anzuzeigen, können Sie die Kampagnen mit den entsprechenden Projekten verbinden. Durch das Verbinden von Eintragstypen und das anschließende Verbinden einzelner Einträge wird diese Beziehung in Workfront-Planung erreicht.

## Suchfelder

Nachdem Sie die Verbindung zwischen zwei Datensatztypen hergestellt und einzelne Datensätze miteinander verbunden haben, können Sie die Felder der verbundenen Datensätze aus dem Datensatz referenzieren, von dem aus Sie eine Verbindung herstellen.

Wenn Sie beispielsweise einen Kampagneneintragstyp mit einem Workfront-Projektobjekttyp verbinden, können Sie das Feld „Budget“ der verbundenen Projekte in den Kampagneneinträgen anzeigen.

![Feld „Suchfelder hinzufügen“](assets/add-lookup-fields-modal.png)

>[!TIP]
>
>* Die folgenden Feldtypen können nicht als Suchfelder aus den verbundenen Eintrags- oder Objekttypen hinzugefügt werden:
>
>   * Erstellt von
>   * Zuletzt geändert von
>   * Workfront-Felder mit automatischer Textvervollständigung (einschließlich Feldern wie „Projektbesitzer“ oder „Projektsponsor“)
>

Informationen zum Verbinden von Eintragstypen, Einträgen und zum Erstellen verknüpfter Felder finden Sie in den folgenden Artikeln:

* [Verbinden von Eintragstypen](/help/quicksilver/planning/architecture/connect-record-types.md)
* [Verbinden von Einträgen](/help/quicksilver/planning/records/connect-records.md)

<!--
not yet:* Fields are reusable across Record Types.
-->

## Hierarchien

Nachdem Datensatztypen in einem Arbeitsbereich verbunden sind, können Sie Hierarchien erstellen, die diese Verbindungen organisieren. Hierarchien organisieren Datensatz- und Objekttypen in hierarchisch untergeordneten Beziehungen und können bis zu vier Objekttypen enthalten.

![Hierarchien im Bereich Workspace-Einstellungen](assets/hierarchies-in-workspace-settings-area.png)

Wenn noch keine Verbindung zwischen zwei Datensatztypen besteht, kann sie beim Einrichten der Hierarchie erstellt werden. Nach der Definition richtet die Hierarchie einen strukturierten Pfad über verwandte Datensatztypen hinweg im Arbeitsbereich ein.

Hierarchien generieren Breadcrumbs für die jeweiligen Datensätze, die in ihren Kopfzeilen angezeigt werden. Auf diese Weise wissen die Benutzer in jeder Phase ihres Workflows, wo sie sich in der Hierarchie befinden.

Allgemeine Informationen zu Hierarchien und Breadcrumbs finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Ansichten

Datensätze werden auf der jeweiligen Seite mit dem Datensatztyp in verschiedenen Ansichten angezeigt.

![Dropdown-Liste mit Ansichtstypen in der Eintragstypliste](assets/view-types-drop-down-from-record-type-list.png)

Ansichten enthalten personalisierte Einstellungen eines bestimmten Ansichtstyps, z. B. die Liste der Felder (Spalten), eine Liste mit Einträgen (Zeilen), ihre Reihenfolge (Sortierung), einen angewendeten oder anwendbaren Filter und eine Gruppierung.

Im Folgenden finden Sie Ansichtstypen, die Sie auf die Eintragstypseite anwenden können:

* **Tabellenansicht** Zeigt Einträge und ihre Felder, einschließlich verbundener Felder und Suchfelder, in einem Tabellenformat an. Die Zeilen der Tabelle sind die einzelnen Einträge und die Spalten sind die Eintragsfelder. Die Tabellenansicht ist die Standardansicht.

  ![Beispiel für eine Tabellenansicht](assets/table-view-example.png)

* **Timeline-Ansicht**: Zeigt Einträge an, die mindestens zwei Datumsfelder in einer chronologischen Timeline aufweisen. In der Timeline-Ansicht können maximal 5 miteinander verbundene Eintragstypen und ihre Einträge angezeigt werden.

  ![Angewendete Gruppierung in der Timeline-Ansicht](assets/grouping-applied-in-timeline-view.png)

* **Kalenderansicht**: Zeigt Einträge mit mindestens zwei Datumsfeldern in einem Kalenderformat an.
  ![Beispiel für eine Kalenderansicht](assets/calendar-view-example.png)

<!--
add List view here when it's possible to display Planning RTs in it??
-->

Zusätzliche Ansicht:

* **Listenansicht**: Sie können Objekte in einer Listenansicht in den folgenden Bereichen von Workfront Planning anzeigen:

  * Projekte mit verbundenen Seiten.
  * Formularliste anfordern

  ![Seite „Verbundene Projekte“ in einer Listenansicht](assets/list-view-projects-connected-page.png)

Weitere Informationen finden Sie unter [Verwalten von Eintragsansichten](/help/quicksilver/planning/views/manage-record-views.md).

## Automatisierungen

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Datensätze in Workfront Planning erstellen, wenn sie aus einem Planungsdatensatz ausgelöst werden. Die erstellten Datensätze werden automatisch mit den Datensätzen verbunden, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite „Datensatztyp“ in Workfront Planning konfigurieren und aktivieren.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront Planning-Kampagne benötigt und eine Marke erstellt, die mit der Kampagne verknüpft werden soll.

Informationen zum Erstellen von Objekten mithilfe einer bestehenden Automatisierung finden Sie unter [Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Antragsformulare

Sie können ein Anfrageformular erstellen und es mit einem Datensatztyp in Adobe Workfront Planning verknüpfen. Sie können das Formular dann für andere freigeben und diese können Anfragen zum Erstellen von Datensätzen dieses Typs senden.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).