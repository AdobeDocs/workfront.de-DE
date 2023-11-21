---
title: Feldübersicht
description: Sie können neue Felder in Adobe Maestro hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 2%

---

# Feldübersicht

<!--
title: Field overview
description: You can add new fields in Adobe Maestro that reflect your organization's lifecycle. Fields are attributes of record types. 
hidefromtoc: yes
author: Alina
feature: Work Management (***************WE NEED A NEW ONE HERE***********)
role: User, Admin
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können neue Felder in Adobe Maestro hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.


## Überlegungen zu Maestro-Feldern

* Sie können Felder nur aus der Tabellenansicht einer Seite vom Typ Datensatz erstellen. Felder werden in der Tabellenansicht als Spalten angezeigt. Alle mit einem Datensatztyp verknüpften Felder werden auch auf der Detailseite jedes Datensatzes dieses Typs angezeigt.

  Informationen zum Verwalten von Tabellenspalten (oder Datensatzfeldern) finden Sie unter [Tabellenansicht verwalten](../views/manage-the-table-view.md).

  Weitere Informationen zum Verwalten von Feldern finden Sie in den folgenden Artikeln:

   * [Felder bearbeiten](../fields/edit-fields.md)
   * [Felder löschen](../fields/delete-fields.md)

* Die mit einem Datensatztyp verknüpften Felder können allen Datensätzen dieses Typs zugeordnet werden. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Felder, die einem Datensatztyp zugeordnet sind, können keinem anderen Datensatztyp hinzugefügt werden. <!-- this will change when they open the Field library tab when creating a field-->

* Sie können Felder manuell oder automatisch wie folgt erstellen:

   * Manuell:

      * Durch Hinzufügen von Spalten in der Tabellenansicht einer Seite vom Typ Datensatz. Die Spalten der Tabelle sind die Felder, die dem Datensatztyp zugeordnet sind. Es handelt sich dabei um dieselben Felder, die auf der Detailseite eines Datensatzes angezeigt werden.

        Auf der Detailseite eines Datensatzes können keine Felder erstellt werden.

        In diesem Artikel wird beschrieben, wie Sie Felder manuell erstellen.

      * Durch Verbinden von Datensatztypen. Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Maestro-Datensatztypen oder einen Datensatztyp und einen Objekttyp aus anderen Anwendungen hinzufügen.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Weitere Informationen zum Verbinden von Maestro-Datensatztypen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

      * Durch Import von Datensatztypen mithilfe einer Excel- oder CSV-Datei. Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   * Automatisch:

      * Standardmäßig jedes Mal, wenn Sie einen Datensatztyp erstellen.

        Die folgenden Standardfelder werden standardmäßig für jeden neuen operationellen Datensatztyp erstellt:

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

        Im Folgenden finden Sie die Standardfelder, die standardmäßig für jeden neuen Taxonomiedatensatztyp erstellt werden:

         * Name <!--will more be added? If not, consider rephrasing this bullet-->

      * Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen. Maestro erstellt Felder für betriebliche Datensatztypen und Taxonomien, wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).

* Maestro-Felder können nicht über Workfront aufgerufen werden.

* Auf Workfront-Felder kann nur von Maestro aus zugegriffen werden, wenn Sie Maestro-Datensatztypen mit Workfront-Objekttypen verbinden und verknüpfte oder Suchfelder aus Workfront-Objekten hinzufügen. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

* Sie können die Einstellungen für die Felder anzeigen und aktualisieren, die Sie oder ein anderer Benutzer erstellt haben. <!--this will change with access/ permissions-->

* Sie können bis zu 500 Felder für einen Datensatztyp haben.

* Feldnamen können bis zu 250 Zeichen enthalten.

* Beim Löschen eines Datensatztyps, einer Taxonomie oder eines Arbeitsbereichs werden auch alle Felder, die mit ihnen verknüpft sind, und die Werte der Felder gelöscht und können nicht wiederhergestellt werden. <!-- this might change with a possible recycle bin solution?!-->