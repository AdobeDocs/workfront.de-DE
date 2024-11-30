---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Berichte nach Zeitrahmen filtern
description: Sie können einen Bericht nach dem Zeitrahmen eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitrahmen filtern, in dem die Stunden eingegeben wurden.
author: Nolan
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 5%

---

# Berichte nach Zeitrahmen filtern

<!-- Audited: 11/2024 -->

Sie können einen Bericht nach dem Zeitrahmen eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitrahmen filtern, in dem die Stunden eingegeben wurden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Der Bericht muss erstellt werden, bevor die Ergebnisse gefiltert werden.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Bericht nach Zeitrahmen eines Datums filtern {#filter-a-report-by-the-time-frame-of-a-date}

1. Klicken Sie auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) und dann auf **Berichterstellung**.

1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann den gewünschten Berichtstyp aus.\
   Wählen Sie beispielsweise **Stündlicher Bericht** aus.

1. Wählen Sie die Registerkarte **Filter** aus.
1. Klicken Sie auf **Filterregel hinzufügen** und wählen Sie dann **Stündliches Einstiegsdatum** aus.\
   ![](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Wählen Sie im folgenden Dropdownmenü eine der folgenden Optionen aus:

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
      <td role="rowheader">Größer als</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, ohne das angegebene Datum einzuschließen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größer gleich</td> 
      <td> <p>Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, einschließlich des angegebenen Datums.</p> <p>Wählen Sie einen der integrierten Zeitrahmen-Modifikatoren aus, wie unter <a href="#built-in-time-frame-modifiers" class="MCXref xref">Integrierte Zeitrahmen-Modifikatoren</a> beschrieben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Diese Modifikatoren stehen für jedes Datumsfeld in einem Filter oder für eine Eingabeaufforderung in einem beliebigen Bericht zur Verfügung.
1. Klicken Sie auf **Speichern + schließen**.

## Integrierte Zeitrahmen-Modifikatoren {#built-in-time-frame-modifiers}

Adobe Workfront verfügt über integrierte Zeitrahmen-Modifikatoren, die Sie verwenden können, ohne ein bestimmtes Datum zu definieren. 

Diese Modifikatoren stehen für jedes Datumsfeld in einem Filter oder für eine Eingabeaufforderung in einem beliebigen Bericht zur Verfügung. 

Weitere Informationen zum Filtern eines Berichts nach einem Zeitrahmen, der mit einem Datum verknüpft ist, finden Sie unter  [Filtern eines Berichts nach dem Zeitrahmen eines Datums](#filter-a-report-by-the-time-frame-of-a-date).

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
   <td> <p>Zeigt Stunden an, in denen das Einstiegsdatum ein Datum im Quartal vor dem aktuellen Quartal ist, wobei Quartale oben definiert sind.</p> <p>Hinweis: Wenn Ihr Workfront-Administrator benutzerdefinierte Quartale für Ihr System aktiviert und definiert hat, werden die integrierten Filter für Quartale durch Ihre benutzerdefinierten Quartalsinformationen ersetzt. Weitere Informationen zum Aktivieren benutzerdefinierter Quartale finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Benutzerdefinierte Quartale für Projekte aktivieren</a>.</p> </td> 
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
   <td> <p>Zeigt Stunden an, in denen das Datum der Einsendung ein Datum im letzten Jahr ist, in dem das letzte Jahr am 1. Januar beginnt und am 31. Dezember des Jahres endet, das dem aktuellen Jahr vorausgeht.</p> <p>Hinweis: Für das Geschäftsjahr gibt es keinen integrierten Zeitraum. Sie können einen Bericht erstellen und die Informationen anhand eines benutzerdefinierten Modifikators für den Datumsbereich des Geschäftsjahres nach Datum filtern, wie in Ihrer Organisation definiert. Wenn Sie einen Zeitraum für ein Geschäftsjahr vor Ort auswählen möchten, sollten Sie anstelle eines Filters eine Eingabeaufforderung verwenden. </p> </td> 
  </tr> 
 </tbody> 
</table>
