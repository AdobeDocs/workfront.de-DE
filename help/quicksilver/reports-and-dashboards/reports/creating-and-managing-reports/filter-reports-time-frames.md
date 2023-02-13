---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Berichte nach Zeitrahmen filtern
description: Sie können einen Bericht nach dem Zeitrahmen eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitrahmen filtern, in dem die Stunden eingegeben wurden.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 4%

---

# Berichte nach Zeitrahmen filtern

Sie können einen Bericht nach dem Zeitrahmen eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitrahmen filtern, in dem die Stunden eingegeben wurden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Der Bericht muss erstellt werden, bevor die Ergebnisse gefiltert werden.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Bericht nach Zeitrahmen eines Datums filtern {#filter-a-report-by-the-time-frame-of-a-date}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)Klicken Sie auf **Berichterstellung**.

1. Klicken **Neuer Bericht** und wählen Sie den gewünschten Berichtstyp aus.\
   Wählen Sie beispielsweise **Stundenbericht**.

1. Wählen Sie die **Filter** Registerkarte.
1. Klicken **Filterregel hinzufügen**, wählen Sie **Stündlicher Eingangsdatum**.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Wählen Sie im folgenden Dropdown-Menü eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gleich</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators das Datum an, an dem die Stunden eingegeben wurden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ungleich</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators das Datum an, an dem die Stunden eingegeben wurden, um dieses Datum aus Ihrem Bericht auszuschließen. Der Bericht zeigt Stunden, die in allen Daten angemeldet sind, erwartet für das von Ihnen angegebene Datum.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Null</td> 
      <td>Wählen Sie diesen Modifikator aus, um nur Stunden anzuzeigen, in denen das Einstiegsdatum fehlt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nicht Null</td> 
      <td>Wählen Sie diesen Modifikator aus, um nur Stunden anzuzeigen, in denen das Entrypdatum einen Wert aufweist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zwischen</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators einen Datumsbereich an, in dem die Stunden eingegeben wurden. Der Bericht zeigt die Stunden an, die zwischen den angegebenen Daten eingegeben wurden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleiner als</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators ein Datum an, vor dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die vor dem angegebenen Datum eingegeben wurden, ohne das angegebene Datum einzuschließen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kleiner gleich</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators ein Datum an, vor dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die vor dem angegebenen Datum eingegeben wurden, einschließlich des angegebenen Datums.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">größer als</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, ohne das angegebene Datum einzuschließen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größer gleich</td> 
      <td> <p>Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, einschließlich des angegebenen Datums.</p> <p>Wählen Sie einen der integrierten Zeitrahmen-Modifikatoren aus, wie unter <a href="#built-in-time-frame-modifiers" class="MCXref xref">Integrierte Zeitrahmen-Modifikatoren</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Diese Modifikatoren stehen für jedes Datumsfeld in einem Filter oder für eine Eingabeaufforderung in einem beliebigen Bericht zur Verfügung.
1. Klicken **Speichern und schließen**.

## Integrierte Zeitrahmen-Modifikatoren {#built-in-time-frame-modifiers}

Adobe Workfront verfügt über integrierte Zeitrahmen-Modifikatoren, die Sie verwenden können, ohne ein bestimmtes Datum zu definieren. 

Diese Modifikatoren stehen für jedes Datumsfeld in einem Filter oder für eine Eingabeaufforderung in einem beliebigen Bericht zur Verfügung. 

Weitere Informationen zum Filtern eines Berichts nach einem Zeitrahmen, der mit einem Datum verknüpft ist, finden Sie unter  [Bericht nach Zeitrahmen eines Datums filtern](#filter-a-report-by-the-time-frame-of-a-date).

Wenn Sie beispielsweise einen Stundenbericht erstellen und in einem bestimmten Zeitrahmen eingegebene Stunden anzeigen möchten, können Sie aus den folgenden integrierten Filter für Zeitrahmen wählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Heute</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum heute liegt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diese Woche</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum in der aktuellen Woche ist, in dem die Woche an einem Sonntag beginnt und an einem Samstag endet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächste Woche</td> 
   <td>Zeigt Stunden an, in denen das Datum der Einsendung ein Datum in der Woche ist, die auf die aktuelle Woche folgt, wobei die Woche an einem Sonntag beginnt und an einem Samstag endet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letzte Woche</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum in der Woche vor der aktuellen Woche ist, in dem die Woche an einem Sonntag beginnt und an einem Samstag endet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diesen Monat</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im aktuellen Monat ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächsten Monat</td> 
   <td>Zeigt Stunden an, in denen das Datum der Einsendung ein Datum im Monat ist, der auf den aktuellen Monat folgt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letzter Monat</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im Monat vor dem aktuellen Monat ist</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dieses Quartal</td> 
   <td> <p>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im aktuellen Quartal ist, wobei Quartale wie folgt definiert sind:</p> 
    <ul> 
     <li>Erstes Quartal: 1. Januar - 30. März</li> 
     <li>Zweites Quartal: 1. April - 30. Juni</li> 
     <li>Drittes Quartal: 1. Juli - 30. September</li> 
     <li>Viertes Quartal: 1. Oktober - 31. Dezember</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächstes Quartal</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im Quartal ist, das auf das aktuelle Quartal folgt, wobei Quartale oben definiert sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letztes Quartal</td> 
   <td> <p>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im Quartal vor dem aktuellen Quartal ist, wobei Quartale oben definiert sind.</p> <p>Hinweis: Wenn Ihr Workfront-Administrator benutzerdefinierte Quartale für Ihr System aktiviert und definiert hat, werden die integrierten Filter für Quartale durch Ihre benutzerdefinierten Quartalsinformationen ersetzt. Weitere Informationen zur Aktivierung benutzerdefinierter Quartale finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Benutzerdefinierte Quartale für Projekte aktivieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dieses Jahr</td> 
   <td>Zeigt Stunden an, in denen das Entrypdatum ein Datum im aktuellen Jahr ist, in dem das aktuelle Jahr am 1. Januar beginnt und am 31. Dezember endet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vergangenes Jahr</td> 
   <td>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im letzten Jahr ist, in dem das vergangene Jahr 12 Monate vor dem aktuellen Datum beginnt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letztes Jahr</td> 
   <td> <p>Zeigt Stunden an, in denen das Datum der Einsendung ein Datum im letzten Jahr ist, in dem das letzte Jahr am 1. Januar beginnt und am 31. Dezember des Jahres endet, das dem aktuellen Jahr vorausgeht.</p> <p>Hinweis: Es gibt keinen integrierten Zeitraum für das Geschäftsjahr. Sie können einen Bericht erstellen und die Informationen anhand eines benutzerdefinierten Modifikators für den Datumsbereich des Geschäftsjahres nach Datum filtern, wie in Ihrer Organisation definiert. Wenn Sie einen Zeitraum für ein Geschäftsjahr vor Ort auswählen möchten, sollten Sie anstelle eines Filters eine Eingabeaufforderung verwenden. </p> </td> 
  </tr> 
 </tbody> 
</table>
