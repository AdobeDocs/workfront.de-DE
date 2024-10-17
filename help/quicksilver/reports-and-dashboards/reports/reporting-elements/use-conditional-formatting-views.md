---
product-area: reporting
navigation-topic: reporting-elements
title: Bedingte Formatierung in Ansichten verwenden
description: Wenn Sie Ihre Berichte mit anderen Benutzern in Adobe Workfront teilen, sollten Sie die Ansicht der Berichte anpassen, um das Lesen bestimmter Informationen zu vereinfachen oder einfach nur zu erkennen.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '1218'
ht-degree: 3%

---

# Bedingte Formatierung in Ansichten verwenden

<!--Audited: 01/2024-->

Wenn Sie Ihre Berichte mit anderen Benutzern in Adobe Workfront teilen, sollten Sie die Ansicht der Berichte anpassen, um das Lesen bestimmter Informationen zu vereinfachen oder einfach nur zu erkennen.

Sie können den Tab Details Ihrer Berichte anpassen, indem Sie der Ansicht Ihrer Berichte spezielle oder bedingte Formatierungen hinzufügen.

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Durch bedingte Formatierung der Spalten in der Berichtansicht können Sie Regeln einrichten, die sich auf die Anzeige des Berichts auswirken. Wenn diese Bedingungen oder Regeln erfüllt sind, wird die spezielle Formatierung angewendet.

Wenn der Prozentsatz der Abschlüsse einer Aufgabe beispielsweise weniger als 20 Prozent beträgt, können Sie das Feld markieren, indem Sie die Prozentzahl fett, roten Text und eine gelbe Hintergrundfarbe anzeigen.

Mit einer bedingt formatierten Ansicht können Sie:

* Ändern Sie die Spaltenüberschrift.
* Ändern Sie den Wert einer Spalte in benutzerdefinierten Text oder ein Bild.
* Formatieren Sie die Anzeige eines Felds, indem Sie den Schrifttyp, die Farbe, die Ausrichtung oder die Hintergrundfarbe ändern.

Die Änderungen, die Sie in der Berichtansicht vornehmen, werden nur im Tab Details des Berichts wirksam. Diese Änderungen wirken sich nicht auf die Registerkarten &quot;Zusammenfassung&quot;, &quot;Matrix&quot;oder &quot;Diagramm&quot;des Berichts aus.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Neu:</p> 
   <ul><li>Standard für Berichtsansichten</li>
  <li> Mitwirkende oder höher für Listenansichten</li></ul>

<p>Aktuell:</p>
   <ul>
    <li> Berichtansichten planen </li>
    <li> Anforderung oder höher für Listenansichten </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu bearbeiten</p> <p><b>NOTIZ</b></p> <p>Wenn Sie keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht verwalten, um eine Ansicht in einem Bericht zu erstellen oder zu bearbeiten</p> <p>Berechtigungen für eine Ansicht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie der Ansicht bedingte Formatierungen hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Bedingt formatierte Ansicht erstellen

{{step1-to-reports}}

1. Klicken Sie auf den Namen eines Berichts, für den Sie eine bedingt formatierte Ansicht erstellen möchten

   Oder

   Klicken Sie auf **Neuer Bericht** und wählen Sie dann einen Objekttyp aus, um einen neuen Bericht zu erstellen.

1. (Bedingt) Wenn Sie einen vorhandenen Bericht bearbeiten, klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.

1. Klicken Sie auf der Registerkarte **Spalten (Ansicht)** auf , um eine vorhandene Spalte auszuwählen, oder klicken Sie auf **Spalte hinzufügen** , um eine Spalte zu erstellen.
1. Wählen Sie im Feld **In dieser Spalte anzeigen** oben links im ReportBuilder das Feld aus, das in der neuen Spalte angezeigt werden soll.
1. Klicken Sie auf **Erweiterte Optionen**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefiniertes Spalten-Label</strong></td> 
      <td> <p>Geben Sie einen Namen für die Spalte an.</p> <p>Wenn Sie eine vorhandene Spalte bearbeiten, ändert sich bei Angabe eines Namens hier der Name der vorhandenen Spalte.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Feldformat</strong></td> 
      <td>Wählen Sie das Format aus, in dem der Wert in der Spalte angezeigt wird. Je nach Spaltenfeld können Sie auf diese Weise festlegen, wie Daten, Zahlen oder Währungen angezeigt werden. Diese Option wird nicht in allen Spalten angezeigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diese Spalte im Dashboard anzeigen</strong></td> 
      <td>Wählen Sie dieses Feld aus, wenn die Spalte angezeigt werden soll, wenn der Bericht in einem Dashboard platziert wird. Die Spalte wird immer angezeigt, wenn Sie sich den Bericht außerhalb eines Dashboards ansehen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Dieser Spalte eine Regel hinzufügen**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Legen Sie im Abschnitt **When the:** eine Bedingungsanweisung für die Spalte fest.

   Beispiel: &quot;Wenn der Task Percent Complete gleich (Groß-/Kleinschreibung beachten) 50 ist.&quot;
1. Geben Sie im Abschnitt **Feld wie folgt anzeigen:** an, wie dieses Feld aussieht, wenn die oben definierte Bedingung erfüllt ist.

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Textfarbe</strong></td> 
      <td> <p>Wählen Sie mithilfe der Farbauswahl die Farbe aus, in der der Text angezeigt wird.</p> <p><b>NOTIZ</b></p> <p> Wenn das Feld einen Hyperlink enthält, werden die Textfarbenselektionen nicht auf dieses Feld angewendet.</p> </td> 
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
      <td>Wählen Sie mithilfe der Farbauswahl die Hintergrundfarbe für den Text aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Symbol "Anzeigen"</strong></td> 
      <td>Wählen Sie eines von 16 Symbolen aus, wenn Sie anstelle des tatsächlichen Werts für diese Spalte ein Symbol anzeigen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text anzeigen</strong></td> 
      <td> <p>Wählen Sie diese Option aus, um anstelle des tatsächlichen Werts eine benutzerdefinierte Bezeichnung für diese Spalte anzuzeigen. Geben Sie den anzuzeigenden Text anstelle des Werts im Feld an.</p> <p><b>WICHTIG</b></p> <p>Wenn Sie <strong>Text anzeigen</strong> auswählen, wird die Möglichkeit zur Inline-Bearbeitung des Texts in dieser Spalte deaktiviert.<br>Außerdem können Sie den Wert einer Vorgängerspalte nicht ändern, da sie integrierte Logik enthält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Auf die gesamte Zeile anwenden</strong></td> 
      <td>Wählen Sie diese Option, um die Einstellungen auf die gesamte Zeile anzuwenden, anstatt nur die ausgewählte Spalte mit Einstellungen zu versehen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Regel hinzufügen**.\
   Sie können der gleichen Spalte zusätzliche Regeln hinzufügen oder Regeln zu anderen Spalten hinzufügen.

   Regeln werden in der Reihenfolge angewendet, in der sie erstellt wurden. Sie werden kombiniert, überschreiben sich jedoch nicht, obwohl eine Spaltenregel Vorrang vor einer Zeilenregel für dieselbe Zelle hat.

   **BEISPIEL 1**

   Sie können zunächst eine Regel erstellen, die besagt, dass die Textfarbe violett und fett ist, wenn sich ein Projekt im Status des Builds befindet. Dann erstellen Sie eine zweite Regel, die besagt, dass die Textfarbe rot und kursiv und die Hintergrundfarbe grün ist, wenn der Name einer Aufgabe nicht leer ist. In diesem Beispiel geschieht Folgendes:

   * Aufgaben, deren Projektstatus &quot;Erstellen&quot;ist, werden in violettem und fett gedrucktem Text angezeigt. Wenn der Aufgabenname nicht leer ist, haben Aufgaben auch einen grünen Hintergrund.
   * Aufgaben, deren Projektstatus etwas Anderes als &quot;Erstellen&quot;ist (und der Aufgabenname nicht leer ist), werden in rotem und kursiv gedrucktem Text mit grünem Hintergrund angezeigt.

   **BEISPIEL 2**

   Erstellen Sie eine Regel in der Spalte &quot;Geplantes Abschlussdatum des Projekts&quot;, die sich auf die gesamte Zeile auswirkt. Dadurch wird der Hintergrund grau dargestellt, wenn das Projekt abgebrochen wird (z. B. wenn der Projektstatus tot ist). Erstellen Sie dann eine Spaltenregel, die den Hintergrund rot darstellt, wenn das geplante Abschlussdatum des Projekts kleiner als heute ist (d. h. das Projekt ist spät). Wenn in diesem Beispiel ein abgebrochenes Projekt ein spätes Abschlussdatum hat, wird diese Zelle rot angezeigt, auch wenn die anderen Zellen in der Zeile grau sind. So korrigieren Sie diese Formatierung:

   * Bearbeiten Sie die Formatierung für das geplante Abschlussdatum und löschen Sie die Spaltenregel für den roten Hintergrund bei verspäteten Projekten.
   * Fügen Sie eine Spaltenregel mit derselben Formatierung wie die Zeilenregel hinzu (grauer Hintergrund, wenn der Projektstatus = Dead).
   * Fügen Sie die Spaltenregel für den roten Hintergrund bei verspäteten Projekten erneut hinzu.
   * Wenn Sie die Regeln und die Ansicht speichern, wird der rote Hintergrund nicht auf ein abgebrochenes Projekt angewendet.

1. Klicken Sie auf **Speichern**.
1. Klicken Sie auf **Speichern + schließen**.\
   Im Bericht sehen Benutzer Änderungen am Format, wenn die angegebenen Bedingungen erfüllt sind.
