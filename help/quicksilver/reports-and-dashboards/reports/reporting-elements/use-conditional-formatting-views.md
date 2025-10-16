---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden der bedingten Formatierung in Ansichten
description: Wenn Sie Ihre Berichte für andere Benutzende in Adobe Workfront freigeben, sollten Sie die Ansicht der Berichte anpassen, um bestimmte Informationen leichter lesbar zu machen oder einfach nur hervorzuheben.
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 3%

---

# Verwenden der bedingten Formatierung in Ansichten

<!-- Audited: 11/2024 -->

Wenn Sie Ihre Berichte für andere Benutzende in Adobe Workfront freigeben, sollten Sie die Ansicht der Berichte anpassen, um bestimmte Informationen leichter lesbar zu machen oder einfach nur hervorzuheben.

Sie können die Registerkarte „Details“ Ihrer Berichte anpassen, indem Sie der Ansicht Ihrer Berichte eine spezielle oder bedingte Formatierung hinzufügen.

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Durch die bedingte Formatierung von Spalten in der Ansicht des Berichts können Sie Regeln einrichten, die sich auf die Anzeige des Berichts auswirken. Wenn diese Bedingungen oder Regeln erfüllt sind, wird die spezielle Formatierung angewendet.

Wenn beispielsweise der Prozentsatz der Fertigstellung einer Aufgabe weniger als 20 Prozent beträgt, können Sie das Feld durch die Anzeige der Prozentzahl in fett gedrucktem, rotem Text und einer gelben Hintergrundfarbe hervorheben.

Mit einer bedingt formatierten Ansicht haben Sie folgende Möglichkeiten:

* Ändern der Kopfzeile einer Spalte.
* Ändern Sie den Wert einer Spalte in benutzerdefinierten Text oder ein Bild.
* Formatieren Sie die Anzeige eines Felds, indem Sie den Schrifttyp, die Farbe, die Ausrichtung oder die Hintergrundfarbe ändern.

Die Änderungen, die Sie an der Berichtsansicht vornehmen, werden nur auf der Registerkarte Details des Berichts wirksam. Diese Änderungen wirken sich nicht auf die Registerkarten Zusammenfassung, Matrix oder Diagramm des Berichts aus.

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
   <td role="rowheader">Adobe Workfront-Lizenz</strong></td> 
   <td> 
    <p>Standard oder Plan für Berichtsansichten</p>
    <p>Mitwirkende oder Anfrage für Listenansichten</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu bearbeiten</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
    <td> <p>Verwalten der Berechtigungen für einen Bericht zum Erstellen oder Bearbeiten einer Ansicht in einem Bericht</p> <p>Verwalten der Berechtigungen für eine Ansicht</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Bericht erstellen, bevor Sie seiner Ansicht bedingte Formatierung hinzufügen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Erstellen einer bedingt formatierten Ansicht

{{step1-to-reports}}

1. Klicken Sie auf den Namen eines Berichts, für den Sie eine bedingt formatierte Ansicht erstellen möchten

   Oder

   Klicken Sie **Neuer Bericht** und wählen Sie dann einen Objekttyp aus, um einen neuen Bericht zu erstellen.

1. (Bedingt) Wenn Sie einen vorhandenen Bericht bearbeiten, klicken Sie auf **Berichtsaktionen** und dann auf **Bearbeiten**.

1. Klicken Sie auf der **Spalten (Ansicht** auf eine vorhandene Spalte, um sie auszuwählen, oder klicken Sie auf **Spalte hinzufügen**, um eine Spalte zu erstellen.
1. Wählen Sie **Feld „In dieser** anzeigen“ in der oberen linken Ecke von Report Builder das Feld aus, das Sie in der neuen Spalte anzeigen möchten.
1. Klicken Sie **Erweiterte Optionen**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefiniertes Spalten-Label</strong></td> 
      <td> <p>Geben Sie einen Namen für die Spalte an.</p> <p>Wenn Sie eine vorhandene Spalte bearbeiten, wird durch die Angabe eines Namens hier der vorhandene Spaltenname geändert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Feldformat</strong></td> 
      <td>Wählen Sie das Format aus, in dem der Wert in der Spalte angezeigt wird. Je nachdem, was das Spaltenfeld ist, können Sie damit festlegen, wie Daten, Zahlen oder Währungen angezeigt werden. Diese Option wird nicht in allen Spalten angezeigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Diese Spalte im Dashboard anzeigen</strong></td> 
      <td>Wählen Sie dieses Feld aus, wenn die Spalte angezeigt werden soll, wenn der Bericht auf einem Dashboard platziert wird. Die Spalte wird immer angezeigt, wenn Sie den Bericht außerhalb eines Dashboards betrachten.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Dieser Spalte eine Regel hinzufügen**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. Legen Sie im **Wenn:**-Abschnitt eine Bedingungsanweisung für die Spalte fest.

   Beispiel: „Wenn der Prozentsatz der abgeschlossenen Aufgabe 50 (von Schreibweise abhängig) entspricht.“
1. Geben Sie im Abschnitt **Feld wie folgt anzeigen** an, wie dieses Feld aussehen soll, wenn die oben definierte Bedingung erfüllt ist.

   Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Textfarbe</strong></td> 
      <td> <p>Wählen Sie mit dem Farbselektor die Farbe aus, in der der Text angezeigt werden soll.</p> <p><b>NOTIZ</b></p> <p> Wenn das Feld einen Hyperlink enthält, wird die Auswahl der Textfarbe nicht auf dieses Feld angewendet.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textformat</strong></td> 
      <td>Auswählen, ob Text fett oder kursiv angezeigt werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Textausrichtung</strong></td> 
      <td>Wählen Sie aus, ob der Text innerhalb der Spalte rechts, zentriert oder links ausgerichtet werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Hintergrund</strong></td> 
      <td>Wählen Sie mit dem Farbselektor die Hintergrundfarbe für den Text aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Symbol anzeigen</strong></td> 
      <td>Wählen Sie eines von 16 Symbolen aus, wenn Sie ein Symbol anstelle des tatsächlichen Werts für diese Spalte anzeigen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Text anzeigen</strong></td> 
      <td> <p>Wählen Sie diese Option aus, um eine benutzerdefinierte Beschriftung für diese Spalte anstelle des tatsächlichen Werts anzuzeigen. Geben Sie den Text an, der anstelle des Werts in dem entsprechenden Feld angezeigt werden soll.</p> <p><b>WICHTIG</b></p> <p>Wenn Sie <strong>Text anzeigen</strong> auswählen, können Sie den Text in dieser Spalte nicht inline bearbeiten.<br>Außerdem können Sie den Wert einer Vorgängerspalte nicht ändern, da sie eine integrierte Logik enthält.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Auf die gesamte Zeile anwenden</strong></td> 
      <td>Wählen Sie diese Option aus, um Einstellungen auf die gesamte Zeile anzuwenden, anstatt nur auf die ausgewählte Spalte Einstellungen anzuwenden.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Regel hinzufügen**.\
   Sie können derselben Spalte zusätzliche Regeln oder anderen Spalten Regeln hinzufügen.

   Regeln werden in der Reihenfolge angewendet, in der sie erstellt wurden. Sie werden kombiniert, überschreiben einander jedoch nicht, obwohl eine Spaltenregel Vorrang vor einer Zeilenregel in derselben Zelle hat.

   **BEISPIEL 1**

   Sie können zunächst eine Regel erstellen, die angibt, dass die Textfarbe violett und fett dargestellt wird, wenn sich ein Projekt im Status „Gebäude“ befindet. Anschließend erstellen Sie eine zweite Regel, die besagt, dass, wenn der Name einer Aufgabe nicht leer ist, die Textfarbe rot und kursiv ist und die Hintergrundfarbe grün ist. In diesem Beispiel geschieht Folgendes:

   * Aufgaben, deren Projektstatus „Erstellen“ ist, werden in violettem und fett gedrucktem Text angezeigt. Wenn der Aufgabenname nicht leer ist, haben Aufgaben auch einen grünen Hintergrund.
   * Aufgaben, deren Projektstatus alles andere als „Erstellen“ ist (und deren Aufgabenname nicht leer ist), werden in einem roten und kursiv gedruckten Text mit grünem Hintergrund angezeigt.

   **BEISPIEL 2**

   Erstellen Sie eine Regel in der Spalte Geplantes Abschlussdatum des Projekts, die sich auf die gesamte Zeile auswirkt, und färben Sie den Hintergrund grau, wenn das Projekt abgebrochen wird (z. B. wenn der Projektstatus Eingestellt ist). Erstellen Sie dann eine Spaltenregel, die im Hintergrund rot wird, wenn das geplante Abschlussdatum des Projekts vor heute liegt (d. h. das Projekt ist in Verzug). Wenn ein abgebrochenes Projekt in diesem Beispiel ein spätes Abschlussdatum hat, wird diese Zelle rot angezeigt, obwohl die anderen Zellen in der Zeile grau sind. So korrigieren Sie diese Formatierung:

   * Bearbeiten Sie die Formatierung für das geplante Abschlussdatum und löschen Sie bei verspäteten Projekten die Spaltenregel für den roten Hintergrund.
   * Fügen Sie eine Spaltenregel mit derselben Formatierung wie die Zeilenregel hinzu (grauer Hintergrund, wenn der Projektstatus = Eingestellt).
   * Fügen Sie bei verspäteten Projekten die Spaltenregel für den roten Hintergrund erneut hinzu.
   * Beim Speichern der Regeln und der Ansicht wird der rote Hintergrund nicht auf ein abgebrochenes Projekt angewendet.

1. Klicken Sie auf **Speichern**.
1. Klicken Sie auf **Speichern + schließen**.\
   Im Bericht sehen Benutzerinnen und Benutzer Formatänderungen, wenn die angegebenen Bedingungen erfüllt sind.
