---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard
description: Ein KPI-Bericht, der einen einzelnen aggregierten KPI hervorgehoben darstellt, kann zu einem Arbeitsflächen-Dashboard hinzugefügt werden.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Weitere Informationen finden Sie unter [Beta-Informationen zu Canvas-Dashboards](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

Sie können einen KPI-Bericht erstellen und zu einem Arbeitsflächen-Dashboard hinzufügen, das Ihre wichtigsten Leistungsindikatordaten visuell als eine Zahl darstellt, mit der Sie dann sehen können, wie Ihre Projekte und Teams funktionieren.

![Beispiel für KPI-Bericht](assets/kpi-example-main.png)

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan</p></td> 
   <td> 
<p>Beliebig </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td> 
<p>Aktuell: Plan </p> 
<p>Neu: Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p>
  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie einen KPI-Bericht erstellen können.

## Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard

Es stehen viele Konfigurationsoptionen zum Erstellen eines KPI-Berichts zur Verfügung. In diesem Abschnitt führen wir Sie durch den allgemeinen Prozess der Erstellung eines solchen.

{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken **oben rechts auf** Neues Dashboard“.

1. Geben Sie in das Feld **Dashboard erstellen** den **** Namen“ und die **Beschreibung** des Dashboards ein.

1. Klicken Sie auf **Erstellen**.

1. Wählen Sie im **Bericht hinzufügen** die Option **Bericht erstellen** aus.

1. Wählen Sie auf der linken Seite &quot;**&quot;**.

1. Klicken Sie oben rechts auf **Bericht erstellen**.

1. Gehen Sie wie folgt vor, um den Abschnitt **Details** zu konfigurieren:

   1. Einen Bericht eingeben **Name**.
   1. Einen Bericht eingeben **Beschreibung**.

      >[!NOTE]
      >
      >Die Beschreibung wird als Beschriftung unter dem KPI-Wert verwendet. Wenn Sie keine Beschreibung eingeben, wird eine Beschriftung für Sie basierend auf dem Aggregator und dem Aggregationstyp generiert, den Sie in den folgenden Schritten auswählen.

1. Gehen Sie wie folgt vor, um den Abschnitt **KPI erstellen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **KPI erstellen** ![KPI erstellen](assets/build-kpi-icon.png) .

   1. Klicken Sie **Feld auswählen** und geben Sie dann das Feld an, das Sie dem Bericht hinzufügen möchten.

   1. Wählen Sie in **Dropdown-Liste** Aggregationstyp“ aus, wie die Daten aggregiert werden, um die KPI-Ausgabe zu erzeugen. Die Optionen in diesem Feld variieren je nach dem Typ des Felds, das im vorherigen Schritt ausgewählt wurde.

1. Gehen Sie wie folgt vor, um den Abschnitt **Filter** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Filter** ![Filter](assets/filter-icon.png).

   1. Wählen Sie **Filter bearbeiten** aus.

   1. Klicken Sie **Bedingung hinzufügen** und geben Sie dann das Feld an, nach dem Sie filtern möchten, sowie den Modifikator, der definiert, welche Art von Bedingung das Feld erfüllen muss.

   1. (Optional) Klicken Sie auf **Filtergruppe hinzufügen**, um einen weiteren Satz von Filterkriterien hinzuzufügen. Der Standardoperator zwischen den Sätzen ist UND. Klicken Sie auf den Operator, um ihn in ODER zu ändern.

1. Gehen Sie wie folgt vor, um den Abschnitt **Spalteneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Drilldown-**![Spalten-Symbol](assets/drilldown-column.png). Die Felder aus dem Diagramm werden automatisch als Spalten im Vorschauabschnitt auf der rechten Seite angezeigt.

   1. (Optional) Um eine der vorhandenen Spaltenkonfigurationen zu aktualisieren, wählen Sie die Spalte, die Sie aktualisieren möchten, im Abschnitt **Aktuelle Spalten** aus und aktualisieren Sie dann die gewünschten Informationen (z. B. Beschriftung, verknüpfter Status und Formatierungsregeln).

   1. Klicken Sie **Spalte hinzufügen** und wählen Sie dann das Feld aus, das als Spalte in der Tabelle angezeigt werden soll. Wiederholen Sie diesen Vorgang für jede Spalte, die Sie hinzufügen möchten.

1. Gehen Sie wie folgt vor, um den Abschnitt **Drilldown-Gruppeneinstellungen** zu konfigurieren:

   1. Klicken Sie im linken Bedienfeld auf das Symbol **Gruppeneinstellungen** ![Drilldown-Gruppe](assets/drilldown-group-icon.png) .

   1. Klicken Sie auf **Gruppierung hinzufügen** und wählen Sie dann das Feld aus, das Sie als Gruppierung erstellen möchten.

1. Klicken Sie **Speichern**, um den Bericht zu erstellen und zum Dashboard hinzuzufügen.


