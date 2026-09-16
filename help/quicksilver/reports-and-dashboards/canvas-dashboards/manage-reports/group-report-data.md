---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Gruppieren von Berichtsdaten in einem Arbeitsflächen-Dashboard
description: Berichtsergebnisse in Gruppen organisieren Die Gruppierung funktioniert je nach Berichtstyp unterschiedlich.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%
---
# Gruppieren von Berichtsdaten in einem Arbeitsflächen-Dashboard

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Arbeitsflächen-Dashboards befolgen.<br>
>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kontaktieren des Kunden-Supports](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

Durch die Gruppierung werden die Berichtsergebnisse so organisiert, dass verwandte Datensätze zusammen angezeigt werden. Die Funktionsweise der Gruppierung hängt vom Berichtstyp ab. Daher enthält dieser Artikel für jede Gruppierung einen separaten Abschnitt.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebig </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td> 
<p>Standard</p> 
<p>Abo</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td><p>Berechtigungen für das Dashboard verwalten</p>
  </td> 
  </tr>
</tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Voraussetzungen

Sie müssen über einen Bericht in einem Dashboard verfügen oder einen erstellen, bevor Sie dessen Daten gruppieren können. Weitere Informationen finden Sie unter [Erstellen eines Arbeitsflächen-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Gruppieren von Zeilen in einem Tabellenbericht

In einem Tabellenbericht werden die Zeilen des Berichts durch Gruppierung organisiert.

1. Klicken Sie **Dialogfeld** Konfigurieren“ auf das Symbol **Gruppeneinstellungen** im linken Bereich.

1. Klicken Sie **Gruppierung hinzufügen** und wählen Sie dann das Feld aus, nach dem Sie gruppieren möchten. Die Gruppierung wird in der Vorschau rechts angezeigt.

1. (Optional) Wiederholen, um weitere Gruppierungen hinzuzufügen.

## Konfigurieren von Drilldown-Gruppierungen in Diagramm- und KPI-Berichten

In Diagramm- und KPI-Berichten wird die Hauptvisualisierung nicht gruppiert. Stattdessen können Sie konfigurieren, wie die Drilldown-Tabelle gruppiert wird, wenn ein Viewer einen Drilldown in einen Wert durchführt.

1. Klicken Sie **Dialogfeld** Konfigurieren“ auf das Symbol **Drilldown-Gruppeneinstellungen** im linken Bedienfeld.

1. Klicken Sie **Gruppierung hinzufügen** und wählen Sie dann das Feld aus, nach dem Sie die Drilldown-Tabelle gruppieren möchten.

## Konfigurieren von Segmenten in Pivot-Tabellenberichten

Pivot-Tabellenberichte verwenden keine Gruppierungen. Stattdessen können Sie bis zu zwei Segmente definieren, bei denen es sich um die Kategorien handelt, nach denen die Metriken des Pivot gruppiert und summiert werden.

1. Klicken Sie **Dialogfeld** Konfigurieren“ auf das Symbol **Segmente** im linken Bereich.

1. Klicken Sie **Segment hinzufügen** und wählen Sie dann das gewünschte Feld aus. Das Segment wird in der Vorschau als Spalte angezeigt.

1. (Optional) Wiederholen Sie diesen Vorgang, um ein zweites Segment hinzuzufügen. Sie können maximal zwei Segmente hinzufügen.

## Gruppierte Daten in einem Dashboard anzeigen

Report Viewer können gruppierte Daten erweitern, reduzieren und sortieren. Weitere Informationen finden Sie unter [Anzeigen von Berichten mit gruppierten Daten](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) in [Verwenden von Arbeitsflächen-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
