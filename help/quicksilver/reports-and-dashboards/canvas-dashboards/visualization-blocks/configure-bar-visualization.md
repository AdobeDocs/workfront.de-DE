---
title: Konfigurieren einer Balkenvisualisierung auf der Reporting-Arbeitsfläche
description: Konfigurieren einer Balkenvisualisierung auf der Reporting-Arbeitsfläche
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 2%

---

# Konfigurieren einer Balkenvisualisierung auf der Reporting-Arbeitsfläche

Eine Balkenvisualisierung kann Ihnen dabei helfen, schnell eine Geschichte über Ihre Daten zu erzählen, indem wichtige Informationen mithilfe von horizontalen Balken hervorgehoben werden.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich für die Betaversion der Reporting-Arbeitsfläche registrieren. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Betaversion: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Konfigurieren einer Balkenvisualisierung

>[!NOTE]
>
>Alle Ihre Änderungen werden automatisch gespeichert, wenn Sie die Blöcke in Ihrem Bericht erstellen und bearbeiten.

1. Fügen Sie zunächst einen Visualisierungsblock mit dem Visualisierungstyp **Leiste** zu einem Bericht hinzu, wie unter [Hinzufügen oder Bearbeiten eines Visualisierungsblocks auf der Reporting-Arbeitsfläche](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md) beschrieben.

1. Klicken Sie auf das Symbol Visualisierung bearbeiten ![Bearbeiten](assets/edit-icon.png) in der oberen rechten Ecke der Visualisierung und führen Sie dann einen der folgenden Schritte aus.

   1. Auf der Registerkarte **Einstellungen**:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visualisierungstyp</td>
         <td><p>Wechseln Sie zu einem anderen Visualisierungstyp. In diesem Fall können sich die nachfolgenden Optionen im Menü ändern.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Vertikale Achse</td>
         <td><p>Wählen Sie die Daten aus, die entlang der vertikalen linken Kante oder der Y-Achse der Balkenvisualisierung dargestellt werden sollen. Die Visualisierung vergleicht die Elemente auf dieser Achse entsprechend jedem Element auf der horizontalen Achse.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Horizontale Achse</td>
         <td><p>Wählen Sie im linken Dropdown-Menü die Daten aus, die Sie entlang der horizontalen Achse oder der X-Achse darstellen möchten. Die Elemente auf dieser Achse werden als Vergleichsbalken basierend auf ihren Werten angezeigt.</p><p>Wählen Sie im rechten Dropdown-Menü aus, wie die Visualisierung die Werte entlang der horizontalen Achse berechnen und anzeigen soll:</p>
          <ul>
           <li><p><b>count</b>: Die Anzahl der Werte</p></li>
           <li><p><b>Summe</b>: Die Summe aller Werte </p></li>
           <li><p><b>Durchschnitt</b>: Der Durchschnitt aller Werte</p></li>
           <li><p><b>Minimum</b>: Nur der niedrigste Wert</p></li>
           <li><p><b>Maximum</b>: Nur der höchste Wert</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ Wert hinzufügen</td>
         <td>Fügen Sie ein weiteres Feld hinzu, das Sie entlang der horizontalen Achse verfolgen möchten.</td>
        </tr>
       </tbody>
      </table>

   1. Auf der Registerkarte **Daten**:

      | Datenquelle (Dropdown-Menü) | Ändern Sie die Datenquelle für die Visualisierung in eine andere Tabelle auf der Arbeitsfläche des Berichts. |
      |---|---|
      | Daten-Source anzeigen | Aktivieren Sie diese Option, um die Quelltabelle für die Visualisierung auf der Berichtsfläche anzuzeigen, oder deaktivieren Sie die Option, um sie auszublenden. |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. Klicken Sie auf eine beliebige Stelle außerhalb des Menüs Visualisierungseinstellungen, um es zu schließen.
