---
product-area: reporting
navigation-topic: reporting-elements
title: Erstellen oder Bearbeiten von Ansichten in Adobe Workfront
description: Sie können den Informationstyp, den Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können mehrere Arten von Ansichten in Adobe Workfront verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 1%

---

# Erstellen oder Bearbeiten von Ansichten in Adobe Workfront

<!-- Audited: 11/2024 -->

Sie können den Informationstyp, den Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können mehrere Arten von Ansichten in Adobe Workfront verwenden.

In diesem Artikel wird beschrieben, wie Sie Standardansichten für Listen und Berichte erstellen und bearbeiten und wie Sie Agile-Ansichten erstellen. Weitere Informationen finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkende oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anforderung oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu erstellen</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen*</strong></td> 
   <td> <p>Berechtigungen für einen Bericht verwalten, um eine Ansicht in einem Bericht zu erstellen oder zu bearbeiten</p> <p>Berechtigungen für eine Ansicht verwalten</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen oder Anpassen einer Ansicht

Der Prozess zum Erstellen oder Anpassen einer Ansicht hängt davon ab, ob Sie eine Standardansicht oder eine agile Ansicht erstellen oder anpassen.

* [Erstellen oder Anpassen einer Standardansicht](#create-or-customize-a-standard-view)
* [Erstellen oder Anpassen einer Agile-Ansicht](#create-or-customize-an-agile-view)

### Standardansicht erstellen oder anpassen {#create-or-customize-a-standard-view}

Sie können eine neue Standardansicht erstellen oder eine vorhandene Standardansicht anpassen, die Sie zuvor erstellt haben.

1. Klicken Sie in einer Liste, in der Sie eine Ansicht erstellen oder anpassen möchten, auf das Dropdownmenü **Ansicht** .

1. Klicken Sie auf die Schaltfläche **+ Neue Ansicht** , um eine neue Ansicht zu erstellen.
Oder
Klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png) , das beim Bewegen der Maus über die rechte Seite einer vorhandenen Ansicht angezeigt wird, die Sie bearbeiten möchten.
Das Dialogfeld **Ansicht anpassen** wird angezeigt.

1. Führen Sie im Abschnitt **Spaltenvorschau** einen der folgenden Schritte aus:

   * Ändern Sie den Wert einer Spalte, indem Sie auf den Spaltentitel klicken und dann ein neues Feld auswählen.
   * Fügen Sie eine Spalte hinzu, indem Sie auf **Spalte hinzufügen** klicken, mit der Eingabe des Namens der Spalte beginnen, die Sie hinzufügen möchten, und klicken Sie dann auf die Spalte, wenn sie in der Dropdown-Liste angezeigt wird.
   * Passen Sie die Anzeigereihenfolge der Spalten an, indem Sie den Spaltentitel an eine neue Position ziehen.

      * (Optional) Klicken Sie im Bereich **Spalteneinstellungen** auf die Dropdownliste **Diese Spalte durch** zusammenfassen und wählen Sie dann eine der verfügbaren Optionen für die Zusammenfassung der Informationen aus. Bei Auswahl dieser Option werden die Informationen in der Spalte in den Berichtsgruppen aggregiert.\
        Für Datumsfelder können Sie die Werte anhand der folgenden Optionen zusammenfassen:

         * Maximum
         * Minimum

        Bei Zahlungs- und Währungsfeldern können Sie die Werte anhand der folgenden Optionen zusammenfassen:

         * Anzahl
         * Summe
         * Durchschnitt
         * Maximum
         * Minimum

        >[!NOTE]
        >
        >Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in Gruppierungen aggregieren:
        >   
        >   * Alle Zahlungs- und Währungsfelder außer &quot;Tatsächliche Stunden&quot;(z. B. geplante/tatsächliche Arbeitskosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante/tatsächliche Kosten, Geplante Stunden) aggregieren nur die Werte für die untergeordneten Aufgaben und eigenständigen Aufgaben. Sie aggregieren nicht die Werte für die übergeordneten Aufgaben oder die übergeordneten Elemente der übergeordneten Aufgaben.
        >   * Die tatsächlichen Stunden aggregieren die Werte für die Hauptaufgaben und Einzelaufgaben; sie aggregieren nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben.
        >   * Benutzerdefinierte Datenfelder für Zahlungs- und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern und eigenständige Aufgaben.
        >   
        >

        Weitere Informationen zur Verwendung von Gruppierungen in einem Bericht finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Optional) Klicken Sie auf **Erweiterte Optionen** , um die folgenden Informationen für die Spalte anzugeben:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Benutzerdefiniertes Spalten-Label</strong></td> 
           <td><p>Geben Sie eine benutzerdefinierte Bezeichnung für die Spalte an. Diese Bezeichnung ersetzt die Standardbeschriftung.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Feldformat</strong></td> 
           <td>Wählen Sie das Format aus, in dem die Werte für die Felder der Spalte angezeigt werden sollen.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Diese Spalte im Dashboard anzeigen</strong></td> 
           <td><p>Aktivieren Sie diese Option, um diese Spalte im Dashboard anzuzeigen, wenn der Bericht zusammen mit einem anderen Bericht nebeneinander angezeigt wird. Wenn diese Option deaktiviert ist, wird diese Spalte nicht angezeigt, wenn der Bericht in einem Dashboard angezeigt wird, in dem Berichte nebeneinander angezeigt werden.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Spaltenregeln</strong></td> 
           <td><p>Klicken Sie auf <strong>+ Regel für diese Spalte hinzufügen</strong> , um eine Regel für die Spalte zu definieren. Nachdem Sie eine Regel hinzugefügt haben, können Sie Feld- und Textstile definieren, anhand derer Felder angezeigt werden, die dieser Regel entsprechen. Klicken Sie auf <strong>Regel hinzufügen</strong> , nachdem Sie die Definition der Regel abgeschlossen haben.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Weitere Informationen zur bedingten Formatierung von Ansichten in Berichten finden Sie im Artikel [Bedingte Formatierung im Textmodus verwenden](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Bedingt) Wenn Sie auf **Erweiterte Optionen** geklickt haben, klicken Sie auf **Fertig**.

1. Klicken Sie auf **Ansicht speichern** , um eine neue Ansicht zu erstellen oder die aktuelle Ansicht durch Ihre Änderungen zu ersetzen.\
   Oder\
   Klicken Sie auf **Als neue Ansicht speichern** , um Ihre Änderungen als neue Ansicht zu speichern.

   >[!TIP]
   >
   >Die Option **Als neue Ansicht speichern** ist die einzige Option, die beim Anpassen einer integrierten Workfront-Ansicht verfügbar ist.

   Ihr Zugriff bestimmt, wie die Ansicht gespeichert wird. Wenn Sie die Ansicht ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version zu speichern. Beachten Sie, dass sich Änderungen an der Ansicht auf Benutzer auswirken, für die die Ansicht freigegeben wurde.

### Erstellen oder Anpassen einer Agile-Ansicht {#create-or-customize-an-agile-view}

Sie können eine Agile-Ansicht erstellen oder eine vorhandene Agile-Ansicht anpassen, die Sie zuvor erstellt haben.

>[!IMPORTANT]
>
>Agile Ansichten sind nur verfügbar, wenn Sie ein Projekt anzeigen.

Weitere Informationen zu Agile-Ansichten finden Sie im Artikel [Projekt verwalten in der Agile-Ansicht](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Dieses Verfahren gilt nur für die veraltete Agile-Ansicht, nicht für die Pinnwandansicht eines Projekts.

So erstellen oder passen Sie eine Agile-Ansicht an:

1. Rufen Sie die Liste der Aufgaben eines Projekts auf.
1. Klicken Sie auf das Symbol **Pinnwand** ![Pinnwandsymbol](assets/board-icon-for-agile-view.png) und dann in der Pinnwandansicht auf **Legacy-Glied verwenden** .

1. (Bedingt) So passen Sie eine vorhandene Agile-Ansicht an:

   1. Klicken Sie auf das Dropdownmenü **Ansicht** und wählen Sie dann die anzupassende Agile-Ansicht aus.\
      Sie können die standardmäßige Agile-Ansicht nicht anpassen.

   1. Klicken Sie erneut auf das Dropdownmenü **Ansicht** und dann auf **Ansicht anpassen**.\
      ![](assets/view-agile-customize.png)

1. (Bedingt) Um eine neue Agile-Ansicht zu erstellen, klicken Sie auf **Neue Ansicht**.\
   Das Dialogfeld **Agile-Ansicht anpassen** wird angezeigt.

1. Geben Sie im Dialogfeld **Agile-Ansicht anpassen** einen Namen für die Agile-Ansicht an.\
   Es wird empfohlen, das Wort &quot;Agile&quot;in Ihren Ansichtsnamen einzufügen, damit Benutzer wissen, dass es sich um eine Agile-Ansicht handelt.\
   Dieser Name wird beim Auswählen einer Ansicht im Dropdown-Menü **Ansicht** angezeigt.

1. Definieren Sie die Statusspalten, die in der agilen Ansicht auf der Zeichenfläche angezeigt werden sollen. Dies sind die Aufgabenstatus, die vom Workfront-Administrator definiert werden, wie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) beschrieben.

   Auf der Agile-Story-Pinnwand stehen nur Systemstatus zur Verfügung. Wenn ein Status nur für eine einzelne Gruppe verfügbar ist, der Sie angehören, ist der Status nicht auf der Übersichtskarte verfügbar. Außerdem sind Aufgaben, die sich in einem Status befinden, der nur für eine benutzerdefinierte Gruppe verfügbar ist, nicht sichtbar, wenn das Projekt in einer Agile-Ansicht angezeigt wird.

   Benutzer können Geschichten aus diesen Statusspalten auf der Agile-Story-Pinnwand verschieben.\
   Beim Definieren von Statusspalten haben Sie folgende Möglichkeiten:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Statusspalten neu anordnen:</strong> </td> 
      <td> Ziehen Sie eine Statusspalte an die gewünschte Position.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statusspalten entfernen:</strong> </td> 
      <td>Klicken Sie auf das Symbol (x) in der Spalte, die Sie entfernen möchten.<br>Sie können den Status "Neu"nur entfernen, wenn der Ansicht ein benutzerdefinierter Status hinzugefügt wurde und dieser benutzerdefinierte Status mit "Neu"übereinstimmt.<br>Informationen zum Erstellen eines benutzerdefinierten Status finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statusspalten hinzufügen:</strong> </td> 
      <td> <p>Klicken Sie auf das Symbol <strong>Plus</strong> und wählen Sie dann den Status aus, den Sie hinzufügen möchten.<br>Es werden alle Standardsystemstatus sowie alle benutzerdefinierten Status angezeigt, die für Sie freigegeben wurden.<br>Sie können bis zu 10 Status für die Anzeige konfigurieren.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. Wählen Sie im Bereich **Kartenfarbe mit** verknüpfen eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Geschichte:</strong> </td> 
      <td>Alle Unteraufgaben stimmen mit der Farbe der übergeordneten Aufgabe überein, sodass die Farben aller Geschichten in jeder Swimlane identisch sind.<br>Farben werden Aufgaben zufällig zugewiesen, wenn sie erstellt werden, wenn die Aufgabe keine Unteraufgaben hat oder keine übergeordnete Aufgabe hat.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Freiform:</strong> </td> 
      <td> Alle Karten werden standardmäßig als blau angezeigt, bis ein Benutzer die Farbe manuell ändert, wie im Artikel <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Meldungen auf der Trommelplatine farblich kategorisieren</a> beschrieben. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität:</strong> </td> 
      <td> <p> Farben sind mit der Priorität der Geschichte wie folgt verknüpft:</p> 
       <ul> 
        <li>Hoch = rot</li> 
        <li>Medium = Gelb</li> 
        <li>Niedrig = Grün<br>Wenn Ihr Workfront-Administrator benutzerdefinierte Prioritäten für Ihr Workfront-System konfiguriert hat, ist die höchste Priorität Rot, die zweithöchste ist Gelb und die übrigen sind grün.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aufgabenbesitzer:</strong> </td> 
      <td> Alle Geschichten mit dem gleichen Hauptverantwortlichen haben dieselbe Farbe.<br>Der primäre Verantwortliche ist der Benutzer, der der Aufgabe zuerst zugewiesen wurde. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie im Bereich **Zusätzliche Felder** auf **Feld hinzufügen** und wählen Sie dann das Feld aus, das Sie den Storykarten hinzufügen möchten. (Dies sind dieselben Felder, die Sie beim Erstellen einer Ansicht oder beim Erstellen von Spalten für einen Bericht hinzufügen können.)\
   Wiederholen Sie diesen Vorgang, um bis zu drei weitere Felder zu den Storykarten hinzuzufügen.\
   Wenn Sie Felder zu Storykarten hinzufügen, sind die Felder schreibgeschützt und werden nur angezeigt, wenn das Feld ausgefüllt ist.

   Standardmäßig werden die folgenden Datentypen auf der Storykarte angezeigt:

   * Name der Meldung mit einem Link direkt zur Aufgabe
   * Der Projektname mit einem Link direkt zum Projekt\
     Dieser Link wird nur bei Verwendung der agilen Ansicht in einer Iteration angezeigt. Er wird nicht angezeigt, wenn eine Agile-Ansicht in einem Projekt verwendet wird.
   * Aufgabenbeschreibung
   * Aktuelle Zusage
   * Anzeigen und Bearbeiten der prozentualen Vollständigkeit entweder durch Anpassung der prozentualen Vollständigkeit selbst oder durch Anpassung der Anzahl der vollständigen Punkte oder Stunden
   * Zugewiesene Benutzer

   Sie können zusätzliche Daten (einschließlich benutzerdefinierter Daten) auf Storykarten anzeigen. Sie können aus verschiedenen Gründen zusätzliche Felder auf Storykarten anzeigen lassen. Beispielsweise können Sie die Kunden-ID anzeigen, wenn Sie für mehrere Kunden innerhalb des Projekts an Storys arbeiten oder das Startdatum der Aufgabe anzeigen möchten.

1. Klicken Sie auf **Speichern**.\
   Ihr Zugriff bestimmt, wie die Ansicht gespeichert wird. Wenn Sie die Ansicht ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version zu speichern. Beachten Sie, dass sich Änderungen an der Ansicht auf Benutzer auswirken, für die die Ansicht freigegeben wurde.

1. (Optional) Klicken Sie auf das Symbol **Liste** , um zur Liste der Aufgaben zurückzukehren.
