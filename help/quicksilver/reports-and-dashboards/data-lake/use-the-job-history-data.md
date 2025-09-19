---
product-area: reports and dashboards
navigation-topic: data-connect
title: Verwenden der Auftragsverlaufsansicht in Data Connect
description: Mit Data Connect können Workfront-Admins auf detaillierte Datensätze jedes Datenaktualisierungsauftrags in der Ansicht Vorgangsverlauf zugreifen.
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 05cf34fe6659c50da76d2478c6e79352346dc9a5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Verwenden der Auftragsverlaufsansicht in Data Connect

In der Ansicht Vorgangsverlauf können Workfront-Admins auf detaillierte Datensätze jedes Datenaktualisierungsauftrags zugreifen. Diese Datensätze liefern wertvolle insight für die Aufträge, mit denen Ihre Daten auf dem neuesten Stand gehalten werden, und helfen Ihnen, optimale Zeitrahmen für die Ausführung von Prozessen und die Aktualisierung Ihrer Geschäftsvisualisierungen festzulegen.

![Vorgangsverlauf anzeigen](assets/job-history-overview.png)

Die Spalten der Vorgangsverlauf-Ansicht enthalten die folgenden Informationen:

* **OBJECT_NAME**: Zeigt den Namen des Objekts an, das mit dem Auftrag verknüpft ist.
* **SCHEDULED_TIME**: Zeigt die Startzeit des Auftrags an.
* **COMPLETED_TIME**: Zeigt die Abschlusszeit des Auftrags an.
* **LATEST_FLAG**: Gibt an, ob der Vorgang Teil der letzten Aktualisierung war.
* **STATE**: Zeigt den Status des Vorgangs an. Weitere Informationen finden Sie im folgenden Abschnitt in diesem Artikel: [Verfügbare Auftragsstatus](#available-job-statuses).
* **LAST_UPDATED**: Der zuletzt aktualisierte Zeitstempel des Auftrags.

>[!NOTE]
>
>Die Ansicht Vorgangsverlauf enthält Details zu den vorherigen 72 Stunden geplanter Aufträge.


## Verfügbare Auftragsstatus

Jedem Datenverbindungs-Auftrag wird ein Status zugewiesen, der angibt, ob er erfolgreich, übersprungen oder fehlgeschlagen ist.

<table>
    <tr>
        <td><b>Auftragsstatus</b></td>
        <td><b>Definition</b></td>
    </tr>
    <tr>
        <td>Erfolgreich</td>
        <td>Der Auftrag hat jede verfügbare Aktualisierung erfolgreich verarbeitet, und alle Aktualisierungen für diesen Datensatztyp werden jetzt im Data Lake angezeigt.</td>
    </tr>
    <tr>
        <td>Übersprungen</td>
        <td>Der Auftrag wurde übersprungen, da sich keine Aktualisierungen in der Warteschlange befanden, die für den Datensatztyp verarbeitet werden sollten.</td>
    </tr>
    <tr>
        <td>Fehlgeschlagen</td>
        <td>Der Vorgang konnte nicht ausgeführt werden. In diesen Fällen wurden wahrscheinlich keine Daten aus der Warteschlange in den Data Lake übertragen. Datensätze, die in der Warteschlange verbleiben, werden im nächsten geplanten Auftrag für diesen Datensatztyp verarbeitet. </td>
    </tr>
   </table>


## Überlegungen zur Auftragsausführung und zum Protokollverhalten

Snowflake verwendet ein Tool zur Optimierung der Auftragsplanung , das beeinflussen kann, wie die Auftragsausführung verarbeitet und in der Ansicht „Auftragsverlauf“ protokolliert wird. Dieses Protokollierungsverhalten kann davon abhängen, ob Daten verarbeitet werden müssen oder nicht.

Wenn beispielsweise für ein bestimmtes Objekt keine neuen Zeilen verarbeitet werden sollen, kann eines der folgenden Ergebnisse auftreten:

* **Auftrag wird ausgeführt und als übersprungen markiert**: Snowflake erkennt, dass keine zu verarbeitenden Zeilen vorhanden sind, führt den Auftrag aus und zeichnet ihn mit dem Status „Übersprungen“ in der Tabelle auf.

* **Vorgang wird nicht ausgeführt**: Snowflake stellt fest, dass keine zu verarbeitenden Zeilen vorhanden sind, führt den Vorgang nicht aus und zeichnet ihn mit dem Status „Übersprungen“ in der Tabelle auf.

  >[!NOTE]
  >
  >Im zweiten Szenario, in dem der Auftrag nicht ausgeführt wird, kann der neueste Datensatz für dieses Objekt einen Zeitstempel widerspiegeln, der nicht dem erwarteten Zeitplan entspricht.

Mit anderen Worten: Ein Auftrag kann auch dann als ausgeführt betrachtet werden, wenn keine Zeilen verarbeitet wurden, und abhängig vom Verhalten des Auftragsplaners für diesen bestimmten Auftrag kann er protokolliert werden oder nicht.