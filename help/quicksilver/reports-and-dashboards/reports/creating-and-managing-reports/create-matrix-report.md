---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Erstellen eines Matrix-Berichts
description: Matrix-Berichte stellen zusammenfassende Informationen in einem aggregierten Tabellenformat dar, was die Anzeige vereinfachen würde, als wenn sie in einer Liste wie in einem herkömmlichen Bericht angezeigt würden.
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Erstellen eines Matrix-Berichts

Matrix-Berichte stellen zusammenfassende Informationen in einem aggregierten Tabellenformat dar, was die Anzeige vereinfachen würde, als wenn sie in einer Liste wie in einem herkömmlichen Bericht angezeigt würden.

## Verwendung eines Matrix-Berichts

Sie können für jeden Bericht, der 2 oder mehr Gruppierungen enthält, einen Matrix-Bericht erstellen. Ein herkömmlicher Bericht kann bis zu 3 Gruppierungen enthalten, ein Matrix-Bericht kann bis zu 4 Gruppierungen enthalten.

Sie möchten beispielsweise einen Bericht &quot;Stunde&quot;erstellen, in dem die während eines Zeitraums von 3 Monaten protokollierten Stunden angezeigt werden. Der Bericht soll danach organisiert werden, wer die Stunden eingegeben hat, sowie nach Monat und Woche.

![](assets/report-matrix-overview-350x123.png)

## Anzeige von Daten in einem Matrix-Bericht

Die Informationen im Matrix-Bericht werden immer als numerische Werte angezeigt. In den meisten Fällen eignen sich Spalten, die einen numerischen Wert enthalten, am besten für die Anzeige in einem Matrix-Bericht (z. B. protokollierte Stunden und tatsächliche Kosten).

Andere Spalten (z. B. Status) können jedoch weiterhin im Matrix-Bericht angezeigt werden, wie in der folgenden Grafik dargestellt:\
![](assets/report-matrix-status-350x73.png)

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

## Einrichten eines Matrix-Berichts

1. Erstellen Sie einen herkömmlichen Bericht, der numerische Daten aus der Berichtsausgabe enthält.\
   Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicken Sie im Bericht, den Sie in Schritt 1 erstellt haben, auf **Berichtaktionen**, wählen Sie **Bearbeiten**.

1. (Bedingt) Wenn Sie bereits eine Ansicht erstellt haben und sie auf diesen Bericht anwenden möchten, klicken Sie auf **Anwenden einer vorhandenen Ansicht** und wählen Sie dann die Ansicht aus der Dropdownliste aus.
1. (Bedingt) Wenn Sie eine neue Ansicht für den Bericht erstellen möchten, führen Sie die folgenden Schritte aus:

   1. Klicken Sie auf **Spalten (Ansicht)** und wählen Sie dann eine Spalte aus, die im Matrix-Bericht zusammengefasst werden soll.
   1. Im **Spalteneinstellungen** Bereich, klicken Sie auf **Zusammenfassen dieser Spalte nach** eine der verfügbaren Optionen für die Zusammenfassung der Informationen auswählen.

      >[!IMPORTANT]
      >
      >Wenn diese Option nicht ausgewählt ist, werden die Informationen aus der Spalte nicht korrekt im Matrix-Bericht angezeigt.

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. Wiederholen Sie diesen Vorgang für jede Spalte auf der Registerkarte Spalten (Ansicht) und klicken Sie auf **Fertig**.

1. Klicken Sie auf **Gruppierungen** Registerkarte.
1. (Bedingt) Wenn Sie bereits eine Gruppierung erstellt haben und diese auf diesen Bericht anwenden möchten, klicken Sie auf **Vorhandene Gruppierung anwenden** und wählen Sie dann aus der Dropdown-Liste die Gruppierung aus.
1. (Bedingt) Wenn Sie eine neue Matrixgruppierung für den Bericht erstellen möchten, führen Sie die folgenden Schritte aus:

   1. Auswählen **Zur Matrix-Gruppierung wechseln** in der rechten oberen Ecke der Builder-Oberfläche.
   1. Im **Zeilengruppierungen** -Abschnitt die Gruppierung der Zeilen angeben, die die horizontalen Gruppierungen der Tabelle ergibt.
   1. (Optional) Um eine zusätzliche Zeilengruppierung hinzuzufügen, klicken Sie auf **Sekundäre Zeilengruppierung hinzufügen**.
   1. Im **Spaltengruppierungen** die Spaltengruppierung, die die vertikalen Gruppierungen der Tabelle bestimmt.
   1. (Optional) Um eine zusätzliche Spaltengruppierung hinzuzufügen, klicken Sie auf **Sekundäre Spaltengruppierung hinzufügen**.
   1. (Bedingt) Wenn Sie eine Gruppierung nach Datum hinzufügen, geben Sie auch an, ob die Ergebnisse nach Tag, Woche, Monat, Quartal oder Jahr gruppiert werden.\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. (Bedingt) Wenn Sie die Gruppierung nach Datum und die Anzeige der Ergebnisse nach Quartal ausgewählt haben, geben Sie beispielsweise an, ob Sie Quartale ohne Daten anzeigen möchten, indem Sie die Option **Anzeigen von Quartalen ohne Ergebnisse** aktivieren.\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >Die **Anzeigen von Quartalen ohne Ergebnisse** -Feld ist nur für Matrixgruppierungen verfügbar, nicht aber für Standardgruppierungen.\
      >Nur die Quartale ohne Daten, die sich zwischen zwei Quartalen mit gültigen Daten befinden, zeigen den Nullwert für die Datenwerte im Matrix-Tab an. Die Quartale ohne Daten, die sich am Anfang und am Ende des von Ihrem Filter ausgewählten Zeitrahmens befinden, werden in der Matrixgruppierung überhaupt nicht angezeigt. Die Quartale ohne Ergebnis werden im Tab Details des Berichts nicht in einer Gruppierung angezeigt.

1. (Optional und bedingt) Klicken Sie auf **Matrix-Einstellungen** und wählen Sie dann aus den folgenden Optionen aus:\
   **Anzahl der Datensätze anzeigen:** Aktivieren Sie diese Option, um eine Zeile mit der Gesamtzahl der Einträge für das angegebene Feld anzuzeigen.\
   **Wertspalte anzeigen:** Wählen Sie diese Option aus, um die folgenden Informationen in der Matrix anzuzeigen:

   * Anzahl der Datensätze
   * Die Spalte Wert

      >[!NOTE]
      >
      >Diese Spalte enthält Informationen, die beschreiben, was die Daten in den einzelnen Zeilen darstellen.\
      >Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in Gruppierungen aggregieren:
      >
      >   
      >   
      >   * Alle Zahlungs- und Währungsfelder außer &quot;Tatsächliche Stunden&quot;(z. B. geplante/tatsächliche Arbeitskosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante Stunden) aggregieren nur die Werte für die untergeordneten Aufgaben und eigenständigen Aufgaben. Sie aggregieren nicht die Werte für die übergeordneten Aufgaben oder die übergeordneten Elemente der übergeordneten Aufgaben.
      >   * Die tatsächlichen Stunden aggregieren die Werte für die Hauptaufgaben und die Einzelaufgaben. sie aggregieren nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben.
      >   * Benutzerdefinierte Datenfelder für Zahlenwerte und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern und eigenständige Aufgaben. Wenn Sie den Matrix-Bericht erstellt haben, um geplante Stunden oder tatsächliche Stunden im **Wert** Beachten Sie, dass Stunden- oder Kosteninformationen für übergeordnete Objekte (z. B. übergeordnete Aufgaben) nicht im Matrix-Bericht angezeigt werden. Um Stunden für übergeordnete Objekte anzuzeigen, müssen Sie die **Details** Registerkarte.

   **Bedingte Regeln:** Richten Sie alle Formatierungsregeln für aggregierte Werte ein.\
   Nachdem Sie eine Regel hinzugefügt haben, können Sie Feld- und Textstile definieren, anhand derer Felder angezeigt werden, die dieser Regel entsprechen. Klicken **Regel hinzufügen** nach der Definition der Regel **Fertig** , um die Regel zu speichern.

1. Klicken Sie auf **Filter** um festzulegen, welche Informationen im Bericht angezeigt werden.
1. (Bedingt) Wenn Sie bereits einen Filter erstellt haben und ihn auf diesen Bericht anwenden möchten, klicken Sie auf **Vorhandenen Filter anwenden** und wählen Sie dann aus der Dropdown-Liste den Filter aus.
1. (Bedingt) Wenn Sie einen neuen Filter für diesen Bericht erstellen möchten, finden Sie weitere Informationen unter [Filter- und Bedingungs-Modifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   für Informationen zu den verschiedenen Kennungen, die Sie beim Erstellen von Filtern verwenden können.

1. Klicken **Speichern+Schließen** , um den Matrix-Bericht zu speichern und anzuzeigen.
