---
product-area: reports and dashboards
navigation-topic: data-connect
title: Verwenden der Ansicht „Datenaktualisierungen überwachen“ in Data Connect
description: Mit Data Connect können Workfront-Admins auf detaillierte Aufzeichnungen der letzten Aktualisierungen zugreifen, die am Data Lake-Datum während der letzten Aktualisierung vorgenommen wurden.
author: Courtney
feature: Reports and Dashboards
exl-id: 230d1a30-2af9-4d2c-9ec1-34c3d4c080d4
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 6%

---

# Verwenden der Ansicht „Datenaktualisierungen überwachen“ in Data Connect

Die Ansicht Datenaktualisierungen überwachen zeigt die letzten Aktualisierungen an, die am Data-Lake-Datum während der letzten Aktualisierung vorgenommen wurden. Die Daten dieser Ansicht werden nach jedem erfolgreichen Abschluss eines Datenladevorgangs aktualisiert.

Aufgrund des hohen Datenvolumens und der Komplexität der Aggregationen zeigt die Ansicht Aktualisierung der Überwachungsdaten nur die Objektansichten an, die in den letzten 2 Wochen aktualisiert wurden. Wenn ein bestimmter Datensatztyp in dieser Ansicht fehlt, liegt das wahrscheinlich an einer mangelnden Aktivität innerhalb dieses Zeitraums.

>[!NOTE]
>
>Diese Ansicht zeigt eine detaillierte Sammlung der von der Anwendung bereitgestellten Daten und Aktualisierungsaktivitäten an, im Gegensatz zu einer täglichen Verlaufs- oder Ereignisansicht, die den Verlauf der Aktualisierungsaktivitäten anzeigt. Um Details zu historischen Aktualisierungsaktivitäten abzurufen, können Sie den <code>DL_LOAD_TIMESTAMP verwenden</code> Datumsobjekt

## Ansichtsspalten bei Datenaktualisierungen überwachen

Die Ansichtsspalten Aktualisierung der Überwachungsdaten enthalten die folgenden Informationen:

<table>
    <tr>
        <td><b>Spaltenname</b></td>
        <td><b>Typ</b></td>
        <td><b>Beschreibung</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>varchar
        </td>
        <td> 
      Der Objekttyp, der mit den Workfront-Datensätzen verknüpft ist, die an den Data Lake gesendet werden. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Datum</td>
        <td>
   Das Datum der letzten erfolgreichen Datenaktualisierung für den Objekttyp, das in der Spalte OBJ_TYPE angezeigt wird. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>timestamp_NTZ</td>
        <td>
 Datum und Uhrzeit der letzten Datenaktualisierung für den Objekttyp, die in der Spalte OBJ_TYPE angezeigt wird.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>timestamp_NTZ </td>
        <td>
       Datum und Uhrzeit der zweitletzten Datenaktualisierung für den Objekttyp, die in der Spalte OBJ_TYPE angezeigt wird. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Zahl</td>
        <td>
     Die Zeit in Minuten, die seit der letzten Datenaktualisierung für den Objekttyp verstrichen ist. </td>
    </tr>
            <tr>
        <td>ERSTELLT </td>
        <td>Zahl </td>
        <td>Eine Anzahl der CREATE-Datensatz-Ereignisse, die zwischen der vorherigen und der letzten Datenaktualisierung für den Objekttyp erfasst wurden.  </td>
    </tr>
                <tr>
        <td>AKTUALISIERT</td>
        <td>Zahl </td>
        <td>Anzahl der zwischen der vorherigen und der letzten Datenaktualisierung erfassten UPDATE-Datensatz-Ereignisse für den Objekttyp.</td>
    </tr>
                <tr>
        <td>GELÖSCHT</td>
        <td>Zahl </td>
        <td>Anzahl der DELETE-Datensatzereignisse, die zwischen der vorherigen und der letzten Datenaktualisierung für den Objekttyp erfasst wurden. </td>
    </tr>
                <tr>
        <td>INSGESAMT</td>
        <td>Zahl </td>
        <td>Anzahl der Ereignisse insgesamt zwischen der vorherigen und der letzten Datenaktualisierung für den Objekttyp. 
        <br> 
        <br><b>Hinweis</b>: Dies ist nicht dasselbe wie die Gesamtzahl der Datensätze, die von CREATE-, UPDATE- oder DELETE-Ereignissen betroffen sind, da derselbe Datensatz innerhalb des Intervalls zwischen Aktualisierungen mehrmals erstellt und aktualisiert werden konnte.  </td>
    </tr>
   </table>
