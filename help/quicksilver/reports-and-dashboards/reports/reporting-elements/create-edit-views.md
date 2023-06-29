---
product-area: reporting
navigation-topic: reporting-elements
title: Erstellen oder Bearbeiten von Ansichten in Adobe Workfront
description: Sie können den Informationstyp, den Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können mehrere Arten von Ansichten in Adobe Workfront verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 11e239bd47a007adbec1770dafc7f7a5d97eb57e
workflow-type: tm+mt
source-wordcount: '1787'
ht-degree: 1%

---

# Erstellen oder Bearbeiten von Ansichten in Adobe Workfront

{{highlighted-preview}}

Sie können den Informationstyp, den Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können mehrere Arten von Ansichten in Adobe Workfront verwenden.

In diesem Artikel wird beschrieben, wie Sie Standardansichten für Listen und Berichte erstellen und bearbeiten und wie Sie Agile-Ansichten erstellen. Weitere Informationen finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu erstellen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht verwalten, um eine Ansicht in einem Bericht zu erstellen oder zu bearbeiten</p> <p>Berechtigungen für eine Ansicht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen oder Anpassen einer Ansicht

Der Prozess zum Erstellen oder Anpassen einer Ansicht hängt davon ab, ob Sie eine Standardansicht oder eine agile Ansicht erstellen oder anpassen.

* [Standardansicht erstellen oder anpassen](#create-or-customize-a-standard-view)
* [Erstellen oder Anpassen einer Agile-Ansicht](#create-or-customize-an-agile-view)

### Standardansicht erstellen oder anpassen {#create-or-customize-a-standard-view}

Sie können eine neue Standardansicht erstellen oder eine bereits erstellte Standardansicht anpassen.

1. Klicken Sie auf **Ansicht** Dropdown-Menü in jeder Liste, in der Sie eine Ansicht erstellen oder anpassen möchten.
1. (Optional) Um eine vorhandene Ansicht anzupassen, wählen Sie die Standardansicht aus, die Sie anpassen möchten.\
   Standardansichten sind in Workfront für jeden Listentyp verfügbar, z. B. für einen Bericht, eine Projektliste oder eine Aufgabenliste.
1. Klicken Sie auf **Ansicht** Dropdown-Menü, und klicken Sie auf **Ansicht anpassen** oder **Neue Ansicht**.\
   Die **Ansicht anpassen** angezeigt.

1. Im **Spaltenvorschau** führen Sie einen der folgenden Schritte aus:

   * Ändern Sie den Wert einer Spalte, indem Sie auf den Spaltentitel klicken und dann ein neues Feld auswählen.
   * Fügen Sie eine Spalte hinzu, indem Sie auf **Spalte hinzufügen**, geben Sie den Namen der Spalte ein, die Sie hinzufügen möchten, und klicken Sie dann auf sie, wenn sie in der Dropdown-Liste angezeigt wird.
   * Passen Sie die Anzeigereihenfolge der Spalten an, indem Sie den Spaltentitel an eine neue Position ziehen.

      * (Optional) Im **Spalteneinstellungen** Bereich, klicken Sie auf **Zusammenfassen dieser Spalte nach** eine der verfügbaren Optionen für die Zusammenfassung der Informationen auswählen. Bei Auswahl dieser Option werden die Informationen in der Spalte in den Berichtsgruppen aggregiert.\
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
        >   * Die tatsächlichen Stunden aggregieren die Werte für die Hauptaufgaben und die Einzelaufgaben. sie aggregieren nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben.
        >   * Benutzerdefinierte Datenfelder für Zahlenwerte und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern und eigenständige Aufgaben.
        >   
        >

        Weitere Informationen zur Verwendung von Gruppierungen in einem Bericht finden Sie im Artikel [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Optional) Klicken Sie auf **Erweiterte Optionen** um die folgenden Informationen für die Spalte anzugeben:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Benutzerdefinierte Spaltenbeschriftung</strong></td> 
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
           <td><p>Klicken <strong>Eine Regel für diese Spalte hinzufügen</strong> , um eine Regel für die Spalte zu definieren. Nachdem Sie eine Regel hinzugefügt haben, können Sie Feld- und Textstile definieren, anhand derer Felder angezeigt werden, die dieser Regel entsprechen. Klicken <strong>Regel hinzufügen</strong> nach der Definition der Regel.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Weitere Informationen zur bedingten Formatierung von Ansichten in Berichten finden Sie im Artikel [Bedingte Formatierung im Textmodus verwenden](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Bedingt) Wenn Sie auf **Erweiterte Optionen** klicken **Fertig**.

1. Klicken **Ansicht speichern** , um eine neue Ansicht zu erstellen oder die aktuelle Ansicht durch Ihre Änderungen zu ersetzen.\
   Oder\
   Klicken **Als neue Ansicht speichern** , um Ihre Änderungen als neue Ansicht zu speichern.

   >[!TIP]
   >
   >Die **Als neue Ansicht speichern** ist die einzige verfügbare Option, wenn Sie eine integrierte Workfront-Ansicht anpassen.

   Ihr Zugriff bestimmt, wie die Ansicht gespeichert wird. Wenn Sie die Ansicht ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version zu speichern. Beachten Sie, dass sich Änderungen an der Ansicht auf Benutzer auswirken, für die die Ansicht freigegeben wurde.

### Erstellen oder Anpassen einer Agile-Ansicht {#create-or-customize-an-agile-view}

Sie können eine neue Agile-Ansicht erstellen oder eine vorhandene Agile-Ansicht anpassen, die Sie zuvor erstellt haben.

>[!IMPORTANT]
>
>Agile Ansichten sind nur verfügbar, wenn Sie ein Projekt anzeigen.

Weitere Informationen zu Agile-Ansichten finden Sie im Artikel [Projekt in der Agile-Ansicht verwalten](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
><span class="preview">Dieses Verfahren gilt nur für die veraltete Agile-Ansicht, nicht für die Pinnwandansicht eines Projekts.</span>

So erstellen oder passen Sie eine Agile-Ansicht an:

1. Rufen Sie die Liste der Aufgaben eines Projekts auf.
1. Klicken Sie auf **Agile Storyboard** icon ![Symbol &quot;Agile Storyboard&quot;](assets/agile-storyboard-nwe.png).

   <span class="preview">Oder</span>

   <span class="preview">Klicken Sie auf **Board** icon ![Pinnwandsymbol](assets/board-icon-for-agile-view.png)und klicken Sie anschließend auf **Verwenden des veralteten agile** in der Pinnwandansicht.</span>

1. (Bedingt) So passen Sie eine vorhandene Agile-Ansicht an:

   1. Klicken Sie auf **Ansicht** und wählen Sie dann die anzupassende Agile-Ansicht aus.\
      Sie können die standardmäßige Agile-Ansicht nicht anpassen.

   1. Klicken Sie auf **Ansicht** erneut auf das Dropdown-Menü klicken und **Ansicht anpassen**.\
      ![](assets/view-agile-customize.png)

1. (Bedingt) Um eine neue Agile-Ansicht zu erstellen, klicken Sie auf **Neue Ansicht**.\
   Die **Anpassen der Agile-Ansicht** angezeigt.

1. Im **Anpassen der Agile-Ansicht** Geben Sie einen Namen für die Agile-Ansicht an.\
   Es wird empfohlen, das Wort &quot;Agile&quot;in Ihren Ansichtsnamen einzufügen, damit Benutzer wissen, dass es sich um eine Agile-Ansicht handelt.\
   Dieser Name wird im **Ansicht** Dropdown-Menü bei der Auswahl einer Ansicht.

1. Definieren Sie die Statusspalten, die in der agilen Ansicht auf der Zeichenfläche angezeigt werden sollen. Dies sind die Aufgabenstatus, die vom Workfront-Administrator definiert werden, wie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Auf der Agile-Story-Pinnwand stehen nur Systemstatus zur Verfügung. Wenn ein Status nur für eine einzelne Gruppe verfügbar ist, der Sie angehören, ist der Status nicht auf der Übersichtskarte verfügbar. Außerdem sind Aufgaben, die sich in einem Status befinden, der nur für eine benutzerdefinierte Gruppe verfügbar ist, nicht sichtbar, wenn das Projekt in einer Agile-Ansicht angezeigt wird.

   Benutzer können Geschichten aus diesen Statusspalten auf der Agile-Story-Pinnwand verschieben.\
   Beim Definieren von Statusspalten haben Sie folgende Möglichkeiten:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Die Statusspalten neu anordnen:</strong> </td> 
      <td> Ziehen Sie eine Statusspalte in die Reihenfolge, in der sie angezeigt werden soll.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statusspalten entfernen:</strong> </td> 
      <td>Klicken Sie auf das Symbol (x) in der Spalte, die Sie entfernen möchten.<br>Sie können den Status "Neu"nur entfernen, wenn der Ansicht ein benutzerdefinierter Status hinzugefügt wurde und dieser benutzerdefinierte Status mit "Neu"übereinstimmt.<br>Informationen zum Erstellen eines benutzerdefinierten Status finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statusspalten hinzufügen:</strong> </td> 
      <td> <p>Klicken Sie auf <strong>Plus</strong> und wählen Sie dann den Status aus, den Sie hinzufügen möchten.<br>Es werden alle Standardsystemstatus sowie alle benutzerdefinierten Status angezeigt, die für Sie freigegeben wurden.<br>Sie können bis zu 10 Status für die Anzeige konfigurieren.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. Im **Kartenfarbe zuordnen zu** -Bereich aus den folgenden Optionen auswählen:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Alle Unteraufgaben stimmen mit der Farbe der übergeordneten Aufgabe überein, sodass die Farben aller Geschichten in jeder Swimlane identisch sind.<br>Farben werden Aufgaben zufällig zugewiesen, wenn sie erstellt werden, wenn die Aufgabe keine Unteraufgaben hat oder keine übergeordnete Aufgabe hat.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Freiform:</strong> </td> 
      <td> Alle Karten werden standardmäßig als blau angezeigt, bis ein Benutzer die Farbe manuell ändert, wie im Artikel beschrieben <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Kategorisieren von Meldungen nach Farbe auf der Scrum-Pinnwand</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität:</strong> </td> 
      <td> <p> Farben sind mit der Priorität der Geschichte wie folgt verknüpft:</p> 
       <ul> 
        <li>Hoch = Rot</li> 
        <li>Mittel = Gelb</li> 
        <li>Niedrig = Grün<br>Wenn Ihr Workfront-Administrator benutzerdefinierte Prioritäten für Ihr Workfront-System konfiguriert hat, ist die höchste Priorität rot, die zweithöchste gelb und die übrigen grün.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aufgabenbesitzer:</strong> </td> 
      <td> Alle Geschichten mit dem gleichen Hauptverantwortlichen haben dieselbe Farbe.<br>Der primäre Verantwortliche ist der Benutzer, der der Aufgabe zuerst zugewiesen wurde. </td> 
     </tr> 
    </tbody> 
   </table>

1. Im **Agile** im Abschnitt **Zusätzliche Felder** Bereich, klicken Sie **Feld hinzufügen** und wählen Sie dann das Feld aus, das Sie den Storykarten hinzufügen möchten. (Dies sind dieselben Felder, die Sie beim Erstellen einer Ansicht oder beim Erstellen von Spalten für einen Bericht hinzufügen können.)\
   Wiederholen Sie diesen Vorgang, um bis zu drei weitere Felder zu den Storykarten hinzuzufügen.\
   Wenn Sie Felder zu Storykarten hinzufügen, sind die Felder schreibgeschützt und werden nur angezeigt, wenn das Feld ausgefüllt ist.

   Standardmäßig werden die folgenden Datentypen auf der Storykarte angezeigt:

   * Name der Meldung mit einem Link direkt zur Aufgabe
   * Der Projektname mit einem Link direkt zum Projekt\
     Dieser Link wird nur bei Verwendung der agilen Ansicht bei einer Iteration angezeigt. sie wird bei Verwendung einer Agile-Ansicht in einem Projekt nicht angezeigt.
   * Aufgabenbeschreibung
   * Aktuelle Zusage
   * Anzeigen und Bearbeiten der prozentualen Vollständigkeit entweder durch Anpassung der prozentualen Vollständigkeit selbst oder durch Anpassung der Anzahl der vollständigen Punkte oder Stunden
   * Zugewiesene Benutzer

   Sie können zusätzliche Daten (einschließlich benutzerdefinierter Daten) auf Storykarten anzeigen. Sie können aus verschiedenen Gründen zusätzliche Felder auf Storykarten anzeigen lassen. Beispielsweise können Sie die Kunden-ID anzeigen, wenn Sie für mehrere Kunden innerhalb des Projekts an Storys arbeiten oder das Startdatum der Aufgabe anzeigen möchten.

1. Klicken Sie auf **Speichern**.\
   Ihr Zugriff bestimmt, wie die Ansicht gespeichert wird. Wenn Sie die Ansicht ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version zu speichern. Beachten Sie, dass sich Änderungen an der Ansicht auf Benutzer auswirken, für die die Ansicht freigegeben wurde.

1. (Optional) Klicken Sie auf die **Listenansicht** icon ![](assets/list-view-in-agile-view-for-tasks.png) , um zur Aufgabenliste zurückzukehren.
