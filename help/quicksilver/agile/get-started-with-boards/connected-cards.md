---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Verwenden von verbundenen Karten auf Pinnwänden
description: Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in Workfront verbunden ist.
author: Jenny
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 6e136bed16c2b20f05267ac181dcc462b1a2aed4
workflow-type: tm+mt
source-wordcount: '1533'
ht-degree: 2%

---

# Verwenden von verbundenen Karten auf Pinnwänden

<!-- Audited: 2/2024 -->

Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit vorhandenen Aufgaben und Problemen in [!DNL Workfront] verbunden ist.

Wenn eines der folgenden Details für die Karte an einer Stelle aktualisiert wird, wird es automatisch an der anderen Stelle aktualisiert:

* [!UICONTROL Name]
* [!UICONTROL Beschreibung]
* [!UICONTROL Verantwortliche]
* [!UICONTROL Status]
* [!UICONTROL Geplantes Abschlussdatum]
* [!UICONTROL Schätzung]/[!UICONTROL Story-Punkte]
* [!UICONTROL Teilaufgaben]
* [!UICONTROL Dokumente]

Um verbundene Karten mit Workfront zu synchronisieren, klicken Sie auf das Menü **[!UICONTROL Mehr]** ![[!UICONTROL Mehr]](assets/more-icon-spectrum.png) neben dem Namen der Pinnwand und wählen Sie **[!UICONTROL Verbundene Elemente synchronisieren]**. Archivierte Karten werden nicht mit Workfront-Aufgaben und -Problemen synchronisiert. Wenn Sie eine Karte wiederherstellen, wird sie erneut synchronisiert.

>[!NOTE]
>
>Eine einzelne verbundene Aufgabe oder Anfrage kann nur einmal pro Pinnwand hinzugefügt werden. Dieselbe Aufgabe bzw. dasselbe Problem kann mit mehreren Boards verbunden werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader">Konfigurationen der Zugriffsebene</td>
   <td><p>Zugriff auf Aufgaben und Probleme anzeigen oder erhöhen</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objektberechtigungen</td>
   <td><p>Berechtigung zum Anzeigen oder Erhöhen der Berechtigungen für die Aufgabe oder das Problem von Workfront</p>
</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verbundene Karte hinzufügen

{{step1-to-boards}}

1. Zugriff auf eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie **[!UICONTROL Karte hinzufügen] > [!UICONTROL Verbundene Karte]**.
1. Wählen Sie ein Projekt und dann eine Aufgabe oder ein Problem aus, die bzw. das als Karte auf der Pinnwand hinzugefügt werden soll.

   Sie können mehrere Objekte auswählen, die alle als separate Karten hinzugefügt werden.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie über Berechtigungen verfügen. Wenn ein Element abgeblendet ist, wurde es der Pinnwand bereits hinzugefügt.
   >* Wenn Sie nach **[!UICONTROL Projekte in meinem Besitz]** oder **[!UICONTROL Projekte in]** filtern, werden Projekte, die dem Status „Abgeschlossen“, „Inaktiv“ oder „Abgelehnt“ entsprechen, nicht einbezogen. Sie können mit dem Filter **[!UICONTROL Alle]** weiterhin nach diesen Projekten suchen.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![Nach Aufgabe oder Problem zum Verbinden suchen](assets/boards-tasksissues-350x94.png)

   Die Karte wird unten in der Spalte ganz links hinzugefügt. Das verbundene [!DNL Workfront] und seine Bevollmächtigten werden auf der Karte angezeigt.

   ![Verbundene Karte](assets/boards-connected-card-first-added.png)

1. Klicken Sie ![Aufgabe oder Problem öffnen](assets/boards-launch-icon.png), um die [!DNL Workfront] Aufgabe oder das Problem in einer neuen Browser-Registerkarte zu öffnen.
1. Um die Kartendetails zu bearbeiten, klicken Sie auf die Karte (nicht im Kartennamen).

   ODER

   Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Bearbeiten]**.

1. Fügen Sie im Feld **[!UICONTROL Kartendetails]** die folgenden Informationen hinzu oder aktualisieren Sie sie:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Durch Ändern des Namens wird auch der Name des verbundenen [!DNL Workfront] geändert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td> 
      <td>Durch Ändern der Beschreibung wird auch die Beschreibung des verbundenen [!DNL Workfront] geändert. Sie können der Beschreibung URLs hinzufügen, die beim Speichern der Karte zu anklickbaren Links werden.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Wählen Sie die Spalte für die Karte.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Wählen Sie einen Status für die Karte. Die Standardwerte sind [!UICONTROL Neu], [!UICONTROL In Bearbeitung] und [!UICONTROL Abgeschlossen], aber auch alle benutzerdefinierten Status, die für das Element in [!DNL Workfront] definiert sind, sind verfügbar.</p>
      <p>Wenn Sie Spaltenrichtlinien zum Aktualisieren von Feldwerten aktiviert haben, wird die Karte beim Ändern des Status auf der Karte automatisch in die entsprechende Spalte verschoben. Weitere Informationen finden Sie unter „Definieren von Spalteneinstellungen und Richtlinien“ im Artikel <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Verwalten von </a>".</p>
      <p>Wenn Sie oben auf der Karte auf <strong>[!UICONTROL Als abgeschlossen markieren]</strong> klicken, ändert sich der Status automatisch in „Abgeschlossen“.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplanter Abschluss]</strong></td>
      <td>Wenn Sie dieses Datum ändern, wird auch das geplante Abschlussdatum für das verbundene [!DNL Workfront] geändert.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td><p>Die Anzahl der Stunden, die die Karte ausgefüllt werden soll.</p><p>Durch Ändern der Schätzung wird auch der Wert der Story-Punkte auf dem verbundenen [!DNL Workfront] geändert.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL -Zuweisungen]</strong></td>
      <td><p>Um der Karte weitere Personen oder ein Team zuzuweisen, klicken Sie auf <strong>[!UICONTROL Zuweisung hinzufügen]</strong> und geben Sie einen Namen in das Suchfeld ein. Wählen Sie ihn dann aus, wenn er in der Ergebnisliste angezeigt wird. Sie können sowohl Einzelpersonen als auch Teams hinzufügen. Auf einer verbundenen Karte ist nur ein Team-Arbeitsauftrag zulässig.</p>
      <p>Alle ausgewählten Bevollmächtigten werden auch der Aufgabe oder dem Problem in [!DNL Workfront] zugewiesen.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Suchen Sie nach Tags für die Karte und wählen Sie diese aus.</p>
      <p>Informationen zum Erstellen neuer Tags finden Sie unter <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Tags hinzufügen</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Felder]</strong></td>
      <td><p>Alle benutzerdefinierten Felder, die Sie hinzufügen, werden in diesem Bereich angezeigt.</p>
      <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen der auf einer Karte angezeigten Felder</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Teilaufgabe]</strong></td>
      <td><p>Alle vorhandenen Teilaufgaben für die Aufgabe werden in diesem Abschnitt angezeigt. Klicken Sie auf <strong>[!UICONTROL Unteraufgabe hinzufügen]</strong>, um eine neue Unteraufgabe hinzuzufügen.</p>
      <p>Der Zähler oben im Abschnitt zeigt die Anzahl der abgeschlossenen Teilaufgaben und die Gesamtzahl der Teilaufgaben an.</p>
      <p>Weitere Informationen zu Teilaufgaben finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Teilaufgaben auf Pinnwänden verwalten</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checkliste]</strong></td>
      <td><p>Klicken Sie auf <strong>[!UICONTROL Checklisten-Element hinzufügen]</strong>. Geben Sie dann den Titel des Elements ein und drücken Sie die Eingabetaste. Ein weiteres Element wird automatisch hinzugefügt. Fahren Sie mit der Eingabe von Titeln fort, um weitere Elemente hinzuzufügen.</p>
      <p>Der Zähler oben in der Checkliste zeigt die Anzahl der abgeschlossenen Elemente und die Gesamtzahl der Elemente an.</p> <p>Weitere Informationen zu Checklistenelementen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Verwalten von Checklistenelementen auf Karten</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Dokumente]</strong></td>
      <td>Bewegen Sie bei einem vorhandenen Dokument den Mauszeiger über die Dokumentminiaturansicht und klicken Sie auf <strong>Vorschau</strong>, um die Datei im Browser anzuzeigen, oder auf <strong>Herunterladen</strong>, um die Datei auf Ihren Computer herunterzuladen. Ein neues Dokument finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Dokumente auf Karten hinzufügen</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Stunden]</strong></td>
      <td>Siehe „Stunden auf einer verbundenen Karte protokollieren“ weiter unten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Kommentare]</strong></td>
      <td><p>Klicken Sie in das Feld <strong>[!UICONTROL Neuer Kommentar]</strong> und geben Sie Ihren Kommentar ein. Formatieren Sie den Text mit den Formatierungswerkzeugen. Um eine Person oder ein Team mit Tags zu versehen, verwenden Sie das Suchfeld unten im Kommentarbereich. Der Benutzer muss kein Mitglied des Boards sein. Getaggte Benutzende auf verbundenen Karten erhalten E-Mail-Benachrichtigungen.</p><p>Klicken Sie auf <strong>[!UICONTROL Senden]</strong>, um den Kommentar zur Karte hinzuzufügen.</p>
      <p>Weitere Informationen zum Kommentieren finden Sie unter <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Arbeit aktualisieren</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Systemaktivität]</strong></td> 
      <td><p>Wenn Sie <strong>Systemaktivität</strong> als Kartenbereich aktiviert haben, wird die Aktivität in diesem Bereich angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen, welche Felder auf einer Karte angezeigt werden</a> und <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Vom System verfolgte Aktualisierungen</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Verwenden Sie das linke Navigationsfenster, um zwischen den Abschnitten der Felder auf den Kartendetails zu wechseln.

1. Klicken Sie auf **[!UICONTROL Schließen]**, um zur Pinnwand zurückzukehren.
Das verbundene Objekt, die Bevollmächtigten, Tags, das Fälligkeitsdatum, der Checklisten-Zähler, die geschätzten Stunden und der Status werden auf der Karte angezeigt.

   ![Karte zur Pinnwand hinzugefügt](assets/boards-connected-card-details-110922.png)

## Trennen einer verbundenen Karte

Sie können eine verbundene Karte vom Workfront-Objekt trennen, und die Karte bleibt auf der Pinnwand als Ad-hoc-Karte erhalten, die Sie bearbeiten können.

>[!NOTE]
>
>Wenn Sie eine verbundene Karte auf einer dynamischen Pinnwand trennen, wird sie beim Aktualisieren der Pinnwand erneut angezeigt, da dieser Pinnwand-Typ alle Aufgaben und Probleme aus einem bestimmten Projekt abruft.
>
>Wenn Sie eine verbundene Karte von einem anderen Pinnwand-Typ trennen, der über eine Aufnahmespalte verfügt, wird die Karte in der Aufnahmespalte erneut angezeigt, wenn Sie die Pinnwand aktualisieren, falls die verbundene Aufgabe oder das verbundene Problem noch nicht als abgeschlossen markiert ist.
>
>In beiden Fällen verfügen Sie nach einer Aktualisierung über zwei Karten für dieselbe Aufgabe oder dasselbe Problem: eine Ad-hoc-Karte und eine verbundene Karte.

So trennen Sie eine Karte auf der Platinenebene:

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das **[!UICONTROL Mehr]** Menü ![Mehr](assets/more-icon-spectrum.png) auf der verbundenen Karte und wählen Sie **[!UICONTROL Trennen]**.
1. Klicken Sie **[!UICONTROL der Bestätigungsmeldung]** Verbindung trennen“.

So trennen Sie eine Karte auf Kartenebene:

1. Rufen Sie die Pinnwand auf und öffnen Sie die verbundene Karte.
1. Klicken Sie auf das **[!UICONTROL Mehr]** Menü ![Mehr](assets/more-icon-spectrum.png) im Bereich „Verbindung“ der Kartendetails und wählen Sie **[!UICONTROL Trennen]**.
1. Klicken Sie **[!UICONTROL der Bestätigungsmeldung]** Verbindung trennen“.

## Konvertieren einer Ad-hoc-Karte in eine verbundene Karte

Nachdem Sie eine Ad-hoc-Karte erstellt haben, können Sie sie in eine verbundene Karte konvertieren. Weitere Informationen zu Ad-hoc-Karten finden [&#x200B; unter „Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Rufen Sie die Pinnwand auf und öffnen Sie die Ad-hoc-Karte.
1. Überprüfen Sie den Namen und die Beschreibung auf der Karte. Sie werden zu der Aufgabe oder dem Problem hinzugefügt, die bzw. das Sie in [!DNL Workfront] erstellen.
1. Klicken [!UICONTROL &#x200B; im Bereich &quot;]&quot; der Kartendetails auf **[!UICONTROL Mit Workfront verbinden]**.
1. Wählen Sie im Fenster [!UICONTROL Karte verbinden] aus, ob Sie eine Aufgabe oder ein Problem erstellen möchten.
1. Suchen Sie nach einem Projekt und wählen Sie es aus, dem die Aufgabe oder das Problem hinzugefügt werden soll.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie über Berechtigungen verfügen.
   >* Wenn Sie nach **[!UICONTROL Projekte in meinem Besitz]** oder **[!UICONTROL Projekte in]** filtern, werden Projekte, die dem Status [!UICONTROL Abgeschlossen], [!UICONTROL Eingestellt] oder [!UICONTROL Abgelehnt] entsprechen, nicht einbezogen. Sie können mit dem Filter **[!UICONTROL Alle]** weiterhin nach diesen Projekten suchen.

1. Klicken Sie auf **[!UICONTROL Verbinden]**.

   ![Ad-hoc-Karte mit Workfront verbinden](assets/boards-connect-ad-hoc-card.png)

   Der Projektname wird im Bereich Verbindung auf der Kartendetails angezeigt.

1. Klicken Sie auf **[!UICONTROL Schließen]**, um zur Pinnwand zurückzukehren.

## Stunden auf einer verbundenen Karte protokollieren

Sie müssen über die richtigen Berechtigungen verfügen, um Stunden für die verbundene Aufgabe oder das verbundene Problem zu protokollieren.

Die Zeitprotokollierungsfelder werden nicht standardmäßig auf verbundenen Karten angezeigt. Sie müssen [!UICONTROL **Stunden**] im Bereich [!UICONTROL Konfigurieren] unter &quot;[!UICONTROL &quot; &#x200B;]. Weitere Informationen finden Sie unter [Anpassen der auf einer Karte angezeigten Felder](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Geben Sie die Anzahl der Stunden für die Aufgabe oder das Problem ein.
1. Wählen Sie einen [!UICONTROL Stundentyp] aus dem Dropdown-Menü aus, wenn er sich von der Standardeinstellung unterscheidet.
1. Klicken Sie [!UICONTROL **Zeit protokollieren**].

   ![Stunden auf Karte protokollieren](assets/log-hours-on-card.png)

   Die auf der Karte protokollierte Zeit wird auch für die damit verbundene Aufgabe oder das damit verbundene Problem gespeichert.

Die Protokollierungszeit auf der Karte entspricht der Protokollierungszeit für eine Aufgabe oder ein Problem. Weitere Informationen finden Sie unter „Zeit für ein Projekt, eine Aufgabe oder ein Problem protokollieren“ im Artikel [Zeit protokollieren](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

