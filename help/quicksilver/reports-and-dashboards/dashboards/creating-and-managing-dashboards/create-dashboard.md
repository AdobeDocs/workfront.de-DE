---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Dashboard erstellen
description: Sie können Dashboards erstellen, um schnell auf Informationen in Adobe Workfront zuzugreifen. Berichte, Kalender und externe Seiten können zu Dashboards hinzugefügt werden, die Sie für eine optimale Zusammenarbeit mit anderen freigeben können.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 39a8d670baa19aa37e29b0312e6c9a296569f44c
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 4%

---

# Dashboard erstellen

<!--Audited: 01/2025-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar.</span>


Sie können Dashboards erstellen, um schnell auf Informationen in Adobe Workfront zuzugreifen. Bis zu 25 Berichte, Kalender und externe Seiten können zu Dashboards hinzugefügt werden, die Sie für eine optimale Zusammenarbeit mit anderen freigeben können.

Weitere Informationen zu Dashboards finden Sie unter [Erste Schritte mit Dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie erhalten Verwaltungsberechtigungen für die Dashboards, die Sie erstellen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen eines der folgenden Objekte erstellen, bevor Sie sie einem Dashboard hinzufügen können:

* **Berichte**: Informationen zum Erstellen von Berichten finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Kalender**: Informationen zum Erstellen von Kalendern finden Sie unter [Übersicht über Kalenderberichte](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Sie können vorhandene externe Seiten zu einem Dashboard hinzufügen oder eine aus dem neuen Dashboard erstellen. Informationen zum Erstellen externer Seiten finden Sie unter [Externe Webseite in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Dashboard erstellen

{{step1-to-dashboards}}

1. Klicken Sie auf **Neues Dashboard**.\
   Das Dialogfeld Neues Dashboard wird angezeigt.

1. Geben Sie Folgendes an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Name</strong></td>
      <td><p>Dies ist der Name Ihres Dashboards. Es wird empfohlen, nur UTF-8-Zeichen zu verwenden, um Kompatibilitätsprobleme zu vermeiden.</p><p>Wenn Sie keinen Namen angeben, wird standardmäßig der Name des ersten Berichts auf dem Dashboard zum Namen des Dashboards.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschreibung (optional)</strong></td>
      <td>Dies ist eine Beschreibung Ihres Dashboards.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Währung</strong></td>
      <td><span class="preview">Dies ist der standardmäßige Währungstyp für das Dashboard. <br>
      <br>Benutzer können beim Filtern des Dashboards zwischen verschiedenen Währungstypen wechseln. Weitere Informationen finden Sie unter <a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md">Dashboard nach Währungstyp filtern</a>.</span></td>
     </tr>
    </tbody>
   </table>

1. Wählen Sie ein Layout aus, indem Sie auf das entsprechende Optionsfeld oben im Abschnitt **Layout auswählen/Berichte hinzufügen/Kalender hinzufügen** klicken. Dies ist das Layout, in dem die Berichte, Kalender oder externen Seiten im Dashboard angezeigt werden.

   Das einspaltige Layout ist die Standardeinstellung.

   Informationen zum Berichtslayout in Dashboards finden Sie unter [So werden Berichte in einem Dashboard angezeigt](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Beginnen Sie im Abschnitt **Verfügbare Berichte und Kalender** mit der Eingabe des Namens eines Berichts, Kalenders oder einer externen Seite in die Suchleiste und ziehen Sie den Bericht, den Kalender oder die externe Seite per Drag-and-Drop in den Layout-Bereich auf der rechten Seite.

   >[!NOTE]
   >
   >Bei der Suche nach einem Element gibt die Suche einen der 2.000 zuletzt erstellten Berichte zurück. Berichtsnamen, die Unicode-Zeichen enthalten, werden nicht in den Suchergebnissen zurückgegeben. Es empfiehlt sich, beim Benennen von Objekten in Workfront keine Unicode-Zeichen einzuschließen, indem Sie Namen eingeben, anstatt Namen aus einer anderen Quelle zu kopieren und einzufügen.

   ![Nach Berichten suchen](assets/unshimmed-dashboard-ui.png)

1. (Optional) Klicken Sie auf **Externe Seite hinzufügen**, um eine neue externe Seite zum Dashboard hinzuzufügen.

   Weitere Informationen zum Erstellen externer Seiten und zum Einbetten in Dashboards finden Sie unter [Externe Web-Seite in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Klicken Sie auf **Speichern + schließen**.

   Ein Zeitstempel wird in der oberen rechten Ecke des Dashboards angezeigt. Der Zeitstempel enthält das Datum, die Uhrzeit und die Zeitzone, in der das Dashboard zuletzt aktualisiert wurde.
