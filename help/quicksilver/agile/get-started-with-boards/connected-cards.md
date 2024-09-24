---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Verwenden von vernetzten Karten auf Pinnwänden
description: Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in Workfront verbunden ist.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 0c0c1f538cfd12e18c504fcb42ee424789d1cde8
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 0%

---

# Angeschlossene Karten auf Pinnwänden verwenden

<!-- Audited: 2/2024 -->

Sie können eine Karte auf Ihrer Pinnwand hinzufügen, die mit vorhandenen Aufgaben und Problemen in [!DNL Workfront] verbunden ist.

Wenn eine der folgenden Details für die Karte an einem Ort aktualisiert wird, wird sie automatisch an einem anderen Speicherort aktualisiert:

* [!UICONTROL Name]
* [!UICONTROL Beschreibung]
* [!UICONTROL Zuweisung]
* [!UICONTROL Status]
* [!UICONTROL Geplantes Abschlussdatum]
* [!UICONTROL Schätzung] / [!UICONTROL Meldungspunkte]
* [!UICONTROL Unteraufgaben]
* [!UICONTROL Dokumente]

Um verbundene Karten mit Workfront zu synchronisieren, klicken Sie neben dem Pinnwandnamen auf das Menü **[!UICONTROL Mehr]** ![[!UICONTROL Mehr Menü]](assets/more-icon-spectrum.png) und wählen Sie **[!UICONTROL Angeschlossene Elemente synchronisieren]**.

>[!NOTE]
>
>Eine einzelne verbundene Aufgabe oder ein Problem kann nur einmal pro Board hinzugefügt werden. Dieselbe Aufgabe oder dasselbe Problem kann mit mehreren Pinnwänden verbunden sein.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Mitarbeiter oder höher</p>
   <p>Oder</p>
   <p>Aktuell: Anforderung oder höher</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td>
   <td><p>Zugriff auf Aufgaben und Probleme anzeigen oder höher</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objektberechtigungen</td>
   <td><p>Anzeigen oder Höhere Berechtigungen für Workfront-Aufgaben oder -Probleme</p>
   <p><strong>Hinweis:</strong> Benutzer mit Anzeigeberechtigungen für eine Aufgabe oder ein Problem können keine Aktionen auf mit ihr verbundenen Karten durchführen, einschließlich der Verschiebung der Karte in eine andere Spalte auf der Pinnwand. Benutzer anzeigen können die Karte nur öffnen, um ihre Eigenschaften anzuzeigen, und die verbundene Aufgabe oder das Problem öffnen. Um zusätzlichen Zugriff anzufordern, öffnen Sie die Aufgabe oder das Problem und fordern Sie dort den Zugriff an.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer verbundenen Karte

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf **[!UICONTROL Karte hinzufügen] > [!UICONTROL Verbundene Karte]**.
1. Wählen Sie ein Projekt aus und wählen Sie dann eine Aufgabe oder ein Problem, die bzw. das als Karte auf der Pinnwand hinzugefügt werden soll.

   Sie können mehrere Objekte auswählen, die alle als separate Karten hinzugefügt werden.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben. Wenn ein Element abgeblendet ist, wurde es bereits zur Pinnwand hinzugefügt.
   >* Wenn Sie nach **[!UICONTROL Projekten filtern, deren Inhaber ich bin]** oder **[!UICONTROL Projekte, die ich bin,]** filtern, werden Projekte, die dem Status &quot;Abgeschlossen&quot;, &quot;Abgelaufen&quot;oder &quot;Abgelehnt&quot;entsprechen, nicht berücksichtigt. Mit dem Filter **[!UICONTROL Alle]** können Sie weiterhin nach diesen Projekten suchen.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![Suche nach Aufgabe oder Problem, um eine Verbindung herzustellen](assets/boards-tasksissues-350x94.png)

   Die Karte wird unten in der Spalte ganz links hinzugefügt. Das verbundene [!DNL Workfront] -Objekt und seine Bevollmächtigten werden auf der Karte angezeigt.

   ![Verbundene Karte](assets/boards-connected-card-first-added.png)

1. Klicken Sie auf ![Aufgabe oder Problem öffnen](assets/boards-launch-icon.png) , um die Aufgabe bzw. das Problem mit [!DNL Workfront] in einer neuen Registerkarte des Browsers zu öffnen.
1. Um die Kartendetails zu bearbeiten, klicken Sie auf die Karte (nicht im Kartennamen).

   Oder

   Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Bearbeiten]** aus.

1. Fügen Sie im Feld **[!UICONTROL Kartendetails]** die folgenden Informationen hinzu oder aktualisieren Sie sie:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Durch Ändern des Namens wird auch der Name des verbundenen [!DNL Workfront] -Objekts geändert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td> 
      <td>Wenn Sie die Beschreibung ändern, wird auch die Beschreibung des verbundenen [!DNL Workfront] -Objekts geändert. Sie können der Beschreibung URLs hinzufügen. Diese werden beim Speichern der Karte zu klickbaren Links.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Spalte]</strong></td>
      <td>Wählen Sie die Spalte für die Karte aus.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Wählen Sie einen Status für die Karte aus. Die Standardeinstellungen lauten [!UICONTROL New], [!UICONTROL In Bearbeitung] und [!UICONTROL Complete], aber alle benutzerdefinierten Status, die für das Element in [!DNL Workfront] definiert sind, sind ebenfalls verfügbar.</p>
      <p>Wenn Sie Spaltenrichtlinien zum Aktualisieren von Feldwerten aktiviert haben, wird die Karte beim Ändern des Status auf der Karte automatisch in die entsprechende Spalte verschoben. Weitere Informationen finden Sie unter "Spalteneinstellungen und Richtlinien definieren"im Artikel <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Pinnwandspalten verwalten</a>.</p>
      <p>Wenn Sie oben auf der Karte auf <strong>[!UICONTROL Mark Complete]</strong> klicken, ändert sich der Status automatisch in "Complete".</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplanter Abschluss]</strong></td>
      <td>Wenn Sie dieses Datum ändern, wird auch das geplante Abschlussdatum für das verbundene [!DNL Workfront] -Objekt geändert.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td><p>Die Anzahl der Stunden, in denen die Karte ausgefüllt werden soll.</p><p>Wenn Sie die Schätzung ändern, wird auch der Story-Punkt-Wert auf dem verbundenen [!DNL Workfront] -Objekt geändert.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Zuweisung]</strong></td>
      <td><p>Um der Karte weitere Personen oder ein Team zuzuweisen, klicken Sie auf <strong>[!UICONTROL Zuweisung hinzufügen]</strong> und geben Sie einen Namen in das Suchfeld ein. Wählen Sie sie dann aus, wenn sie in der Ergebnisliste angezeigt wird. Sie können sowohl Einzelanwender als auch Teams hinzufügen. Nur eine Teamzuweisung ist auf einer verbundenen Karte erlaubt.</p>
      <p>Alle von Ihnen ausgewählten Bevollmächtigten werden auch der Aufgabe oder dem Problem in [!DNL Workfront] zugewiesen.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Suchen Sie nach Tags für die Karte und wählen Sie sie aus.</p>
      <p>Informationen zum Erstellen neuer Tags finden Sie unter <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Tags hinzufügen</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Felder]</strong></td>
      <td><p>Alle von Ihnen hinzugefügten benutzerdefinierten Felder werden in diesem Bereich angezeigt.</p>
      <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen, welche Felder auf einer Karte angezeigt werden</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Unteraufgabe]</strong></td>
      <td><p>Alle vorhandenen Unteraufgaben für die Aufgabe werden in diesem Abschnitt angezeigt. Klicken Sie auf <strong>[!UICONTROL Unteraufgabe hinzufügen]</strong> , um eine neue Unteraufgabe hinzuzufügen.</p>
      <p>Der Zähler oben im Abschnitt zeigt die Anzahl der abgeschlossenen Unteraufgaben und die Gesamtzahl der Unteraufgaben an.</p>
      <p>Weitere Informationen zu Unteraufgaben finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Verwalten von Unteraufgaben auf Pinnwänden</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checkliste]</strong></td>
      <td><p>Klicken Sie auf <strong>[!UICONTROL Checklisten-Element hinzufügen]</strong>. Geben Sie dann den Titel des Elements ein und drücken Sie die Eingabetaste. Ein weiteres Element wird automatisch hinzugefügt. Fahren Sie mit der Eingabe von Titeln fort, um weitere Elemente hinzuzufügen.</p>
      <p>Der Zähler oben in der Checkliste zeigt die Anzahl der abgeschlossenen Elemente und die Gesamtzahl der Elemente an.</p> <p>Weitere Informationen zu Checklisten-Elementen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Verwalten von Checklisten-Elementen auf Karten</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Dokumente]</strong></td>
      <td>Bewegen Sie bei einem vorhandenen Dokument den Mauszeiger über die Miniaturansicht des Dokuments und klicken Sie auf <strong>Vorschau</strong> , um die Datei im Browser anzuzeigen, oder auf <strong>Herunterladen</strong> , um die Datei auf Ihren Computer herunterzuladen. Ein neues Dokument finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Dokumente auf Karten hinzufügen</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Siehe "Loggen Sie Stunden auf einer verbundenen Karte ein" unten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Kommentare]</strong></td>
      <td><p>Klicken Sie in das Feld <strong>[!UICONTROL Neuer Kommentar]</strong> und geben Sie Ihren Kommentar ein. Verwenden Sie die Formatierungs-Tools, um den Text zu formatieren. Verwenden Sie das Suchfeld unten im Kommentarbereich, um eine Person oder ein Team mit Tags zu versehen. Der Benutzer muss kein Mitglied auf der Pinnwand sein. Benutzer mit Tags auf verbundenen Karten erhalten E-Mail-Benachrichtigungen.</p><p>Klicken Sie auf <strong>[!UICONTROL Submit]</strong> , um den Kommentar zur Karte hinzuzufügen.</p>
      <p>Weitere Informationen zu Kommentaren finden Sie unter <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Arbeit aktualisieren</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Systemaktivität]</strong></td> 
      <td><p>Wenn Sie <strong>Systemaktivität</strong> als Kartenabschnitt aktiviert haben, wird die Aktivität in diesem Bereich angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen, welche Felder auf einer Karte angezeigt werden</a> und <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Vom System getrackte Updates</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Verwenden Sie das linke Navigationsfenster, um zwischen den Bereichen der Felder in den Kartendetails zu wechseln.

1. Klicken Sie auf **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.
Das verbundene Objekt, die zugewiesenen Personen, die Tags, das Fälligkeitsdatum, der Zähler der Checkliste, die geschätzten Stunden und der Status werden auf der Karte angezeigt.

   ![Karte zur Pinnwand hinzugefügt](assets/boards-connected-card-details-110922.png)

## Trennen Sie die verbundene Karte.

Sie können eine verbundene Karte vom Workfront-Objekt trennen und die Karte bleibt auf der Pinnwand als Ad-hoc-Karte, die Sie bearbeiten können.

So trennen Sie die Verbindung auf Pinnwandebene:

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) auf der verbundenen Karte und wählen Sie **[!UICONTROL Trennen]** aus.
1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Trennen]** .

So trennen Sie die Verbindung auf Kartenebene:

1. Rufen Sie die Pinnwand auf und öffnen Sie die verbundene Karte.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) im Bereich Verbindung der Kartendetails und wählen Sie **[!UICONTROL Trennen]**.
1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Trennen]** .

## Eine Ad-hoc-Karte in eine verbundene Karte konvertieren

Nachdem Sie eine Ad-hoc-Karte erstellt haben, können Sie sie in eine verbundene Karte konvertieren. Weitere Informationen zu Ad-hoc-Karten finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Rufen Sie die Pinnwand auf und öffnen Sie die Ad-hoc-Karte.
1. Überprüfen Sie den Namen und die Beschreibung auf der Karte. Sie werden der Aufgabe oder dem Problem hinzugefügt, die/das Sie in [!DNL Workfront] erstellen.
1. Klicken Sie im Bereich [!UICONTROL Verbindung] der Kartendetails auf **[!UICONTROL Verbindung mit Workfront herstellen]**.
1. Wählen Sie im Fenster [!UICONTROL Karte verbinden] aus, ob Sie eine Aufgabe oder ein Problem erstellen.
1. Suchen Sie nach einem Projekt, dem die Aufgabe oder das Problem hinzugefügt werden soll, und wählen Sie es aus.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben.
   >* Wenn Sie nach **[!UICONTROL Projekten filtern, deren Inhaber ich bin]** oder **[!UICONTROL Projekte, die ich bin,]** filtern, werden Projekte, die dem Status [!UICONTROL Abgeschlossen], [!UICONTROL Dead] oder [!UICONTROL Abgelehnt] entsprechen, nicht berücksichtigt. Mit dem Filter **[!UICONTROL Alle]** können Sie weiterhin nach diesen Projekten suchen.

1. Klicken Sie auf **[!UICONTROL Verbinden]**.

   ![Ad-hoc-Karte mit Workfront verbinden](assets/boards-connect-ad-hoc-card.png)

   Der Projektname wird im Bereich Verbindung in den Kartendetails angezeigt.

1. Klicken Sie auf **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.

## Login-Stunden auf einer verbundenen Karte

Sie müssen über die richtigen Berechtigungen verfügen, um Stunden für die verbundene Aufgabe oder das Problem zu protokollieren.

Die Zeitprotokollierungsfelder werden nicht standardmäßig auf verbundenen Karten angezeigt. Sie müssen [!UICONTROL **Stunden**] im Bereich [!UICONTROL Konfigurieren] unter [!UICONTROL Karten] aktivieren. Weitere Informationen finden Sie unter [Anpassen, welche Felder auf einer Karte angezeigt werden](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Geben Sie die Anzahl der Stunden für die Aufgabe oder das Problem ein.
1. Wählen Sie einen [!UICONTROL Stündentyp] aus dem Dropdown-Menü aus, wenn er sich von der Standardeinstellung unterscheidet.
1. Klicken Sie auf [!UICONTROL **Protokollzeit**].

   ![Log hours on card](assets/log-hours-on-card.png)

   Die auf der Karte protokollierte Zeit wird auch bei der verbundenen Aufgabe oder dem Problem gespeichert.

Die Protokollierungszeit auf der Karte entspricht der Protokollierungszeit für eine Aufgabe oder ein Problem. Weitere Informationen finden Sie unter &quot;Log time on a project, task, or issue&quot;im Artikel [Log time](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

