---
title: Feldübersicht
description: Sie können in Adobe Workfront Planning neue Felder hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jiru3zJiLp4ucCSjSRkDC-9OFRYvFVtqKz6-uPFNHOc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 481
ht-degree: 4%

---

# Feldübersicht

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

Sie können in Adobe Workfront Planning neue Felder hinzufügen, die den Lebenszyklus Ihres Unternehmens widerspiegeln. Felder sind Attribute von Datensatztypen.


## Überlegungen zu Adobe Workfront-Planungsfeldern

* Felder können nur über die Tabellenansicht einer Datensatztypseite erstellt werden. Felder werden in der Tabellenansicht als Spalten angezeigt. Alle mit einem Datensatztyp verknüpften Felder werden auch auf der Datensatzseite angezeigt.

  Informationen zum Verwalten von Tabellenspalten (oder Datensatzfeldern) finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

  Informationen zum Verwalten von Feldern finden Sie auch in den folgenden Artikeln:

   * [Bearbeiten von Einstellungen für Felder](/help/quicksilver/planning/fields/edit-fields.md)
   * [Felder löschen](/help/quicksilver/planning/fields/delete-fields.md)

* Die mit einem Datensatztyp verknüpften Felder können mit allen Datensätzen dieses Typs verknüpft werden. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Mit einem Datensatztyp verknüpfte Felder können nicht zu einem anderen Datensatztyp hinzugefügt werden. <!-- this will change when they open the Field library tab when creating a field-->

* Sie können Felder auf folgende Weise manuell oder automatisch erstellen:

   * Manuell:

      * Beim Hinzufügen von Spalten in der Tabellenansicht einer Datensatztypseite. Die Spalten der Tabelle sind die Felder, die mit dem Datensatztyp verknüpft sind. Es handelt sich um dieselben Felder, die auf der Datensatzseite angezeigt werden.

        Felder können nicht auf der Datensatzseite erstellt werden.

      * Beim Verbinden von Datensatztypen. Sie können verknüpfte Datensatzfelder erstellen, wenn Sie eine neue Verbindung zwischen zwei Datensatztypen oder einem Datensatztyp und einem Objekttyp aus anderen Anwendungen hinzufügen.

        Weitere Informationen zum Verbinden von Datensatztypen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

      * Beim Importieren vorhandener Felder aus Workfront.

        Weitere Informationen finden Sie unter [Felder aus Adobe Workfront ](/help/quicksilver/planning/fields/import-fields-from-workfront.md).


   * Automatisch:

      * Beim Erstellen eines Datensatztyps:

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

      * Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Beim Importieren von Datensatztypen mithilfe einer Excel- oder CSV-Datei.

        Weitere Informationen finden Sie unter [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

* Auf Workfront Planning-Felder kann von Workfront aus nicht zugegriffen werden.

* Auf Workfront-Felder kann von Workfront Planning nur zugegriffen werden, wenn Sie Datensatztypen mit Workfront-Objekttypen verbinden und verknüpfte Felder oder Suchfelder aus Workfront-Objekten hinzufügen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

* Sie können die Einstellungen für die Felder, die Sie oder ein anderer Benutzer erstellt haben, anzeigen und aktualisieren, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich und den Datensatztyp verfügen, zu dem das Feld gehört.

* Sie können bis zu 500 Felder für einen Datensatztyp haben.

* Feldnamen können bis zu 250 Zeichen lang sein.

* Beim Löschen eines Datensatztyps oder Arbeitsbereichs werden auch alle mit ihnen verknüpften Felder sowie die Werte der Felder gelöscht und können nicht wiederhergestellt werden. <!-- this might change with a possible recycle bin solution?!-->
* Wenn Sie Felder löschen, die Teil eines Formelausdrucks sind, ändert sich das Formelfeld.
* Wenn Sie einen Formelausdruck ändern und dieses Formelfeld in anderen Formelfeldern referenziert wird, sind auch die zusätzlichen Formeln betroffen.
