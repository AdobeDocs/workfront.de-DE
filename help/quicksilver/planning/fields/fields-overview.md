---
title: Feldübersicht
description: Sie können neue Felder in der Adobe Workfront-Planung hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 8d5006532e93dc687beb79e817b725f18b0c65d3
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 2%

---


# Feldübersicht

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


{{planning-important-intro}}

Sie können neue Felder in der Adobe Workfront-Planung hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.


## Überlegungen zu Adobe Workfront-Planungsfeldern

* Sie können Felder nur aus der Tabellenansicht einer Seite vom Typ Datensatz erstellen. Felder werden in der Tabellenansicht als Spalten angezeigt. Alle Felder, die mit einem Datensatztyp verknüpft sind, werden ebenfalls auf der Datensatzseite angezeigt.

  Informationen zum Verwalten von Tabellenspalten (oder Datensatzfeldern) finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

  Weitere Informationen zum Verwalten von Feldern finden Sie in den folgenden Artikeln:

   * [Feldeinstellungen bearbeiten](/help/quicksilver/planning/fields/edit-fields.md)
   * [Felder löschen](/help/quicksilver/planning/fields/delete-fields.md)

* Die mit einem Datensatztyp verknüpften Felder können allen Datensätzen dieses Typs zugeordnet werden. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Felder, die einem Datensatztyp zugeordnet sind, können keinem anderen Datensatztyp hinzugefügt werden. <!-- this will change when they open the Field library tab when creating a field-->

* Sie können Felder manuell oder automatisch wie folgt erstellen:

   * Manuell:

      * Durch Hinzufügen von Spalten in der Tabellenansicht einer Seite vom Typ Datensatz. Die Spalten der Tabelle sind die Felder, die dem Datensatztyp zugeordnet sind. Es handelt sich um dieselben Felder, die auf der Seite eines Datensatzes angezeigt werden.

        Auf der Datensatzseite können keine Felder erstellt werden.

      * Durch Verbinden von Datensatztypen. Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Datensatztypen oder einen Datensatztyp und einen Objekttyp aus anderen Anwendungen hinzufügen.

        Weitere Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

      * <span class="preview">Durch Importieren vorhandener Felder aus Workfront. </span>
        <span class="preview">Weitere Informationen finden Sie unter [Importieren von Feldern aus Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md).</span>

      * <span class="preview">Durch Importieren von Datensatztypen mit einer Excel- oder CSV-Datei. </span>

        <span class="preview">Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).</span>

   * Automatisch:

     Die folgenden Standardfelder werden standardmäßig für jeden neuen Datensatztyp erstellt:

      * Name
      * Beschreibung
      * Startdatum
      * Enddatum
      * Status. Die Standardwerte für den Datensatzstatus sind:
         * Entwicklung
         * Geplant
         * Aktiv
         * Abgeschlossen
         * Zurückgestellt

        Sie können weitere Werte hinzufügen oder die vorhandenen umbenennen.

     Workfront Planning erstellt Felder für Datensatztypen, wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

* Auf Workfront-Planungsfelder kann nicht über Workfront zugegriffen werden.

* Auf Workfront-Felder kann über die Workfront-Planung nur zugegriffen werden, wenn Sie Datensatztypen mit Workfront-Objekttypen verbinden und verknüpfte oder Suchfelder aus Workfront-Objekten hinzufügen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

* Sie können die Einstellungen für die Felder, die Sie oder ein anderer Benutzer erstellt haben, anzeigen und aktualisieren, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, zu dem das Feld gehört.

* Sie können bis zu 500 Felder für einen Datensatztyp haben.

* Feldnamen können bis zu 250 Zeichen enthalten.

* Beim Löschen eines Datensatztyps oder Arbeitsbereichs werden auch alle mit ihm verknüpften Felder und die Feldwerte gelöscht und können nicht wiederhergestellt werden. <!-- this might change with a possible recycle bin solution?!-->
