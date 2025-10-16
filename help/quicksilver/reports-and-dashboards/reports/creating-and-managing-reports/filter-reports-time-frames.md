---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Berichte nach Zeitrahmen filtern
description: Sie können einen Bericht nach dem Zeitraum eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitraum filtern, in dem die Stunden eingegeben wurden.
author: Courtney
feature: Reports and Dashboards
exl-id: 7dea484c-d38e-4786-85d0-f4c106cfa46f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 5%

---

# Berichte nach Zeitrahmen filtern

<!-- Audited: 4/2025 -->

Sie können einen Bericht nach dem Zeitraum eines Datums filtern, das in einem Objekt vorhanden ist. Sie können beispielsweise einen Stundenbericht nach einem bestimmten Zeitraum filtern, in dem die Stunden eingegeben wurden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Der Bericht muss erstellt werden, bevor Sie die Ergebnisse filtern können.

Weitere Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Filtern eines Berichts nach dem Zeitrahmen eines Datums {#filter-a-report-by-the-timeframe-of-a-date}

{{step1-to-reports}}

1. Klicken Sie oben links auf **Neuer Bericht** und wählen Sie dann den Berichtstyp aus, den Sie erstellen möchten.

1. Wählen Sie auf der **Neuer Bericht** die Registerkarte **Filter** aus.

1. Klicken Sie **Filterregel hinzufügen** und dann **Feld auswählen**.

1. Wählen **im Dialogfeld „Feld**&quot; die Option **Stunde** und dann **Eingabedatum**.
   ![Stundenbericht nach Zeitrahmen filtern](assets/qs-filtering-hour-report-by-timeframe-350x357.png)

1. Wählen Sie in der angezeigten Dropdown-Liste eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gleich</td> 
      <td>Nachdem Sie diesen Modifikator ausgewählt haben, geben Sie das Datum an, an dem die Stunden eingegeben wurden.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Ungleich</td> 
      <td>Nachdem Sie diesen Modifikator ausgewählt haben, geben Sie das Datum an, an dem die Stunden eingegeben wurden, um dieses Datum aus Ihrem Bericht auszuschließen. Der Bericht zeigt die in allen Datumsangaben protokollierten Stunden an. Erwarten Sie für das angegebene Datum.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Less Than</td> 
      <td>Nachdem Sie diesen Modifikator ausgewählt haben, geben Sie ein Datum an, vor dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die vor dem angegebenen Datum eingegeben wurden, ohne das angegebene Datum einzubeziehen.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Kleiner gleich</td> 
      <td>Nachdem Sie diesen Modifikator ausgewählt haben, geben Sie ein Datum an, vor dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die vor dem angegebenen Datum eingegeben wurden, einschließlich des angegebenen Datums.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Greater Than</td> 
      <td>Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, ohne das angegebene Datum einzubeziehen.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Größer gleich</td> 
      <td> Geben Sie nach Auswahl dieses Modifikators ein Datum an, nach dem die Stunden eingegeben wurden. Der Bericht zeigt Stunden an, die nach dem angegebenen Datum eingegeben wurden, einschließlich des angegebenen Datums. </td> 
     </tr>

   <tr> 
      <td role="rowheader">Zwischen</td> 
      <td>Nachdem Sie diesen Modifikator ausgewählt haben, geben Sie einen Datumsbereich an, in dem die Stunden eingegeben wurden. Der Bericht zeigt die Stunden an, die zwischen den angegebenen Daten eingegeben wurden.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Null</td> 
      <td>Wählen Sie diesen Modifikator, um nur Stunden anzuzeigen, in denen das Eingabedatum fehlt.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Nicht null</td> 
      <td>Wählen Sie diesen Modifikator, um nur Stunden anzuzeigen, für die das Eingabedatum einen Wert aufweist.</td> 
     </tr>

   </tbody> 
   </table>

1. Klicken Sie auf **Speichern + schließen**.

## Integrierte Zeitrahmen-Modifikatoren {#built-in-timeframe-modifiers}

Adobe Workfront verfügt über integrierte Zeitrahmen-Modifikatoren, die Sie ohne Definition eines bestimmten Datums verwenden können. Diese Modifikatoren stehen für jedes Datumsfeld in einem Filter oder eine Eingabeaufforderung in jedem Bericht zur Verfügung.

Wenn Sie beispielsweise einen Stundenbericht erstellen und Stunden anzeigen möchten, die in einem bestimmten Zeitrahmen eingegeben wurden, können Sie aus den folgenden integrierten Zeitrahmen-Filteroptionen wählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Heute</td> 
   <td>Zeigt Stunden an, in denen das Eingabedatum heute ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diese Woche</td> 
   <td>Zeigt Stunden an, in denen das Eingabedatum ein Datum in der aktuellen Woche ist, in der die Woche an einem Sonntag beginnt und an einem Samstag endet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächste Woche</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum in der Woche ist, die auf die aktuelle Woche folgt, wobei die Woche an einem Sonntag beginnt und an einem Samstag endet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letzte Woche</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum in der Woche vor der aktuellen Woche ist, wobei die Woche an einem Sonntag beginnt und an einem Samstag endet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Diesen Monat</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum im aktuellen Monat ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächsten Monat</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum im Monat nach dem aktuellen Monat ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letzter Monat</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum des Monats ist, der dem aktuellen Monat vorausgeht</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dieses Quartal</td> 
   <td> <p>Zeigt Stunden an, bei denen das Eingabedatum ein Datum im aktuellen Quartal ist, wobei Quartale wie folgt definiert sind:</p> 
    <ul> 
     <li>Erstes Quartal: 1. Januar - 30. März</li> 
     <li>Zweites Quartal: 1. April - 30. Juni</li> 
     <li>Drittes Quartal: 1. Juli - 30. September</li> 
     <li>Viertes Quartal: 1. Oktober - 31. Dezember</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nächstes Quartal</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum in dem Quartal ist, das auf das aktuelle Quartal folgt, in dem oben Quartale definiert sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letztes Quartal</td> 
   <td> <p>Zeigt Stunden an, bei denen das Eingabedatum ein Datum in dem Quartal ist, das dem aktuellen Quartal vorausgeht, in dem oben Quartale definiert sind.</p> <p>Hinweis: Wenn Ihr Workfront-Administrator benutzerdefinierte Quartale für Ihr System aktiviert und definiert hat, werden die integrierten Filter für Quartale durch Ihre benutzerdefinierten Quartalsinformationen ersetzt. Weitere Informationen zur Aktivierung benutzerdefinierter Quartale finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Benutzerdefinierte Quartale aktivieren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dieses Jahr</td> 
   <td>Zeigt Stunden an, in denen das Eingabedatum ein Datum im aktuellen Jahr ist, in dem das aktuelle Jahr am 1. Januar beginnt und am 31. Dezember endet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vergangenes Jahr</td> 
   <td>Zeigt Stunden an, bei denen das Eingabedatum ein Datum im letzten Jahr ist, wobei das vergangene Jahr 12 Monate vor dem aktuellen Datum beginnt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Letztes Jahr</td> 
   <td> <p>Zeigt Stunden an, bei denen das Eingabedatum ein Datum im letzten Jahr ist, wobei das letzte Jahr am 1. Januar beginnt und am 31. Dezember des Jahres endet, das dem aktuellen Jahr vorausgeht.</p> <p>Hinweis: Es gibt keinen integrierten Zeitraum für das Geschäftsjahr. Sie können einen Bericht erstellen und die Informationen mithilfe eines benutzerdefinierten Modifikators für den Datumsbereich des Geschäftsjahres filtern, wie er in Ihrer Organisation definiert ist. Wenn Sie einen Zeitrahmen für ein Geschäftsjahr vor Ort auswählen möchten, sollten Sie eine Eingabeaufforderung anstelle eines Filters verwenden. </p> </td> 
  </tr> 
 </tbody> 
</table>
