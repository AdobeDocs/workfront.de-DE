---
product-area: reporting
navigation-topic: reporting-elements
title: Bedingte Formatierung in Ansichten verwenden
description: Wenn Sie Ihre Berichte mit anderen Benutzern in Adobe Workfront teilen, sollten Sie die Ansicht der Berichte anpassen, um das Lesen bestimmter Informationen zu vereinfachen oder einfach nur zu erkennen.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# Bedingte Formatierung in Ansichten verwenden

Wenn Sie Ihre Berichte mit anderen Benutzern in Adobe Workfront teilen, sollten Sie die Ansicht der Berichte anpassen, um das Lesen bestimmter Informationen zu vereinfachen oder einfach nur zu erkennen.

Sie können den Tab Details Ihrer Berichte anpassen, indem Sie der Ansicht Ihrer Berichte spezielle oder bedingte Formatierungen hinzufügen.

Sie müssen über Verwaltungsberechtigungen für den Bericht verfügen, um ihn bearbeiten und der Ansicht spezielle Formatierungen hinzufügen zu können.

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Durch bedingte Formatierung der Spalten in der Berichtansicht können Sie Regeln einrichten, die sich auf die Anzeige des Berichts auswirken. Wenn diese Bedingungen oder Regeln erfüllt sind, wird die spezielle Formatierung angewendet.

Wenn der Prozentsatz der Abschlüsse einer Aufgabe beispielsweise weniger als 20 Prozent beträgt, können Sie das Feld markieren, indem Sie die Prozentzahl fett, roten Text und eine gelbe Hintergrundfarbe anzeigen.

Mit einer bedingt formatierten Ansicht können Sie:

* Ändern Sie die Spaltenüberschrift.
* Ändern Sie den Wert einer Spalte in benutzerdefinierten Text oder ein Bild.
* Formatieren Sie die Anzeige eines Felds, indem Sie den Schrifttyp, die Farbe, die Ausrichtung oder die Hintergrundfarbe ändern.

Die Änderungen, die Sie in der Berichtansicht vornehmen, werden nur im Tab Details des Berichts wirksam. Diese Änderungen wirken sich nicht auf die Registerkarten Zusammenfassung, Matrix oder Diagramm des Berichts aus.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anforderung oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht verwalten, um eine Ansicht in einem Bericht zu erstellen oder zu bearbeiten</p> <p>Berechtigungen für eine Ansicht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie ihm bedingte Formatierungen hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Bedingt formatierte Ansicht erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Klicken Sie auf den Namen eines Berichts, für den Sie eine bedingt formatierte Ansicht erstellen möchten.

   Oder

   Klicken **Berichtaktionen** Klicken Sie auf **Bearbeiten**.

1. (Bedingt) Wenn Sie einen Bericht bearbeitet haben, wählen Sie eine vorhandene Spalte aus oder erstellen Sie eine neue Spalte.
1. Klicken **Erweiterte Optionen**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefinierte Spaltenbeschriftung</strong></td> 
      <td> <p>Geben Sie einen Namen für die Spalte an.</p> <p>Wenn Sie eine vorhandene Spalte bearbeiten, ändert sich bei Angabe eines Namens hier der Name der vorhandenen Spalte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Feldformat</strong></td> 
      <td>Wählen Sie das Format aus, in dem der Wert in der Spalte angezeigt wird. Je nach Spaltenfeld können Sie auf diese Weise festlegen, wie Daten, Zahlen oder Währungen angezeigt werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diese Spalte im Dashboard anzeigen</strong></td> 
      <td>Wählen Sie dieses Feld aus, wenn die Spalte angezeigt werden soll, wenn der Bericht in einem Dashboard platziert wird. Die Spalte wird immer angezeigt, wenn Sie sich den Bericht außerhalb eines Dashboards ansehen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Eine Regel für diese Spalte hinzufügen**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Im **Wenn das** -Abschnitt, legen Sie eine Bedingungsanweisung für die Spalte fest. Beispiel: wenn der Task Percent Complete gleich (Groß-/Kleinschreibung beachten) 50 ist.
1. Im **Zeigen Sie das Feld wie folgt an:** -Abschnitt geben Sie an, wie dieses Feld aussieht, wenn die oben definierte Bedingung erfüllt ist.

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Textfarbe</strong></td> 
      <td> <p>Wählen Sie die Farbe aus, in der der Text angezeigt wird. Es sind 8 Farben verfügbar.</p> <p>Hinweis: Wenn das Feld einen Hyperlink enthält, werden die Textfarbenselektionen nicht auf dieses Feld angewendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textformat</strong></td> 
      <td>Wählen Sie aus, ob Text fett oder kursiv angezeigt werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textausrichtung</strong></td> 
      <td>Wählen Sie aus, ob der Text in der Spalte rechts, zentriert oder links ausgerichtet werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Hintergrund</strong></td> 
      <td>Wählen Sie die Hintergrundfarbe für den Text aus. Es sind 8 Farben verfügbar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Symbol "Anzeigen"</strong></td> 
      <td>Wählen Sie eines von 16 Symbolen aus, wenn Sie anstelle des tatsächlichen Werts für diese Spalte ein Symbol anzeigen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text anzeigen</strong></td> 
      <td> <p>Wählen Sie diese Option aus, um anstelle des tatsächlichen Werts eine benutzerdefinierte Bezeichnung für diese Spalte anzuzeigen. Geben Sie den anzuzeigenden Text anstelle des Werts im Feld an.</p> <p>Wichtig: Auswählen <strong>Text anzeigen</strong> Deaktiviert die Inline-Bearbeitung des Textes in dieser Spalte.<br>Außerdem können Sie den Wert einer Vorgängerspalte nicht ändern, da sie integrierte Logik enthält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Auf die gesamte Zeile anwenden</strong></td> 
      <td>Wählen Sie diese Option, um die Einstellungen auf die gesamte Zeile anzuwenden, anstatt nur die ausgewählte Spalte mit Einstellungen zu versehen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Regel hinzufügen**.\
   Sie können der gleichen Spalte zusätzliche Regeln hinzufügen oder Regeln zu anderen Spalten hinzufügen.

   Regeln werden in der Reihenfolge angewendet, in der sie erstellt wurden. Sie werden kombiniert, überschreiben einander jedoch nicht, obwohl eine Spaltenregel Vorrang vor einer Zeilenregel für dieselbe Zelle hat.

   Beispiel 1: Sie können zunächst eine Regel erstellen, die angibt, wann der Projektstatus &quot;Erstellen&quot;lautet, die Textfarbe violett und fett ist. Anschließend erstellen Sie eine zweite Regel, die angibt, ob der Aufgabenname nicht leer ist, die Textfarbe rot und kursiv ist und die Hintergrundfarbe grün ist. In diesem Beispiel geschieht Folgendes:

   * Aufgaben, deren Projektstatus &quot;Erstellen&quot;ist, werden in violettem und fett gedrucktem Text angezeigt. Wenn der Aufgabenname nicht leer ist, haben Aufgaben auch einen grünen Hintergrund.
   * Aufgaben, deren Projektstatus etwas Anderes als &quot;Erstellen&quot;ist (und der Aufgabenname nicht leer ist), werden in rotem und kursiv gedrucktem Text mit grünem Hintergrund angezeigt.

   Beispiel 2: Erstellen Sie eine Regel für das geplante Abschlussdatum des Projekts, die sich auf die gesamte Zeile auswirkt, und drehen Sie den Hintergrund grau, wenn das Projekt abgebrochen wird (Status = &quot;Dead&quot;). Erstellen Sie dann eine Spaltenregel, die den Hintergrund rot darstellt, wenn das geplante Abschlussdatum des Projekts kleiner als heute ist (d. h. das Projekt ist spät). Wenn in diesem Beispiel ein abgebrochenes Projekt ein spätes Abschlussdatum hat, wird diese Zelle rot angezeigt, auch wenn die anderen Zellen in der Zeile grau sind. So korrigieren Sie diese Formatierung:

   * Bearbeiten Sie die Formatierung für das geplante Abschlussdatum und löschen Sie die Spaltenregel für den roten Hintergrund bei verspäteten Projekten.
   * Fügen Sie eine Spaltenregel mit derselben Formatierung wie die Zeilenregel hinzu (grauer Hintergrund, wenn der Projektstatus = &quot;Dead&quot;).
   * Fügen Sie die Spaltenregel für den roten Hintergrund bei verspäteten Projekten erneut hinzu.
   * Wenn Sie die Regeln und die Ansicht speichern, wird der rote Hintergrund nicht auf ein abgebrochenes Projekt angewendet.


1. Klicken **Fertig**.
1. Klicken **Speichern und schließen**.\
   Im Bericht sehen Benutzer Änderungen am Format, wenn die angegebenen Bedingungen erfüllt sind.
