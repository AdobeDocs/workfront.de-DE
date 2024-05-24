---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Angeschlossene Karten auf Pinnwänden verwenden
description: Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in Workfront verbunden ist.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 6371f6d19bfbad31c4564f9726f52e3ce394e516
workflow-type: tm+mt
source-wordcount: '1507'
ht-degree: 0%

---

# Angeschlossene Karten auf Pinnwänden verwenden

<!-- Audited: 2/2024 -->

Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in [!DNL Workfront].

Wenn eine der folgenden Details für die Karte an einem Ort aktualisiert wird, wird sie automatisch an einem anderen Speicherort aktualisiert:

* [!UICONTROL Name]
* [!UICONTROL Beschreibung]
* [!UICONTROL Zuweisung]
* [!UICONTROL Status]
* [!UICONTROL Geplantes Abschlussdatum]
* [!UICONTROL Schätzung] / [!UICONTROL Story Points]
* [!UICONTROL Unteraufgaben]
* [!UICONTROL Dokumente]

>[!NOTE]
>
>Eine einzelne verbundene Aufgabe oder ein Problem kann nur einmal pro Board hinzugefügt werden. Dieselbe Aufgabe oder dasselbe Problem kann mit mehreren Pinnwänden verbunden sein.

## Zugriffsanforderungen

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
   <p><strong>Hinweis:</strong> Benutzer mit Ansichtsberechtigungen für eine Aufgabe oder ein Problem können keine Aktionen auf Karten durchführen, die mit der Aufgabe verbunden sind, einschließlich der Verschiebung der Karte in eine andere Spalte auf der Pinnwand. Benutzer anzeigen können die Karte nur öffnen, um ihre Eigenschaften anzuzeigen, und die verbundene Aufgabe oder das Problem öffnen. Um zusätzlichen Zugriff anzufordern, öffnen Sie die Aufgabe oder das Problem und fordern Sie dort den Zugriff an.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Hinzufügen einer verbundenen Karte

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Pinnwände]**.
1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicks **[!UICONTROL Karte hinzufügen] > [!UICONTROL Verbundene Karte]**.
1. Wählen Sie ein Projekt aus und wählen Sie dann eine Aufgabe oder ein Problem, die bzw. das als Karte auf der Pinnwand hinzugefügt werden soll.

   Sie können mehrere Objekte auswählen, die alle als separate Karten hinzugefügt werden.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben. Wenn ein Element abgeblendet ist, wurde es bereits zur Pinnwand hinzugefügt.
   >* Beim Filtern nach **[!UICONTROL Eigene Projekte]** oder **[!UICONTROL Projekte, an denen ich arbeite]**, werden Projekte, die dem Status &quot;Abgeschlossen&quot;, &quot;Abgelaufen&quot;oder &quot;Abgelehnt&quot;entsprechen, nicht einbezogen. Sie können mit der **[!UICONTROL Alle]** Filter.

1. Klicks **[!UICONTROL Hinzufügen]**.

   ![Suche nach Aufgabe oder Problem, um eine Verbindung herzustellen](assets/boards-tasksissues-350x94.png)

   Die Karte wird unten in der Spalte ganz links hinzugefügt. Der verbundene [!DNL Workfront] -Objekt und dessen Bevollmächtigte werden auf der Karte angezeigt.

   ![Verbundene Karte](assets/boards-connected-card-first-added.png)

1. Klicks ![Aufgabe oder Problem öffnen](assets/boards-launch-icon.png) , um die [!DNL Workfront] Aufgabe oder Problem in einer neuen Browser-Registerkarte.
1. Um die Kartendetails zu bearbeiten, klicken Sie auf die Karte (nicht im Kartennamen).

   Oder

   Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Bearbeiten]**.

1. Im **[!UICONTROL Kartendetails]** die folgenden Informationen hinzufügen oder aktualisieren:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Durch Ändern des Namens wird auch der Name der verbundenen [!DNL Workfront] -Objekt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td> 
      <td>Durch Ändern der Beschreibung wird auch die Beschreibung auf der verbundenen Seite geändert [!DNL Workfront] -Objekt. Sie können der Beschreibung URLs hinzufügen. Diese werden beim Speichern der Karte zu klickbaren Links.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Spalte]</strong></td>
      <td>Wählen Sie die Spalte für die Karte aus.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Wählen Sie einen Status für die Karte aus. Die Standardwerte sind [!UICONTROL New], [!UICONTROL In Bearbeitung] und [!UICONTROL Complete], jedoch alle benutzerdefinierten Status, die für das Element unter [!DNL Workfront] sind auch verfügbar.</p>
      <p>Wenn Sie Spaltenrichtlinien zum Aktualisieren von Feldwerten aktiviert haben, wird die Karte beim Ändern des Status auf der Karte automatisch in die entsprechende Spalte verschoben. Weitere Informationen finden Sie unter "Spalteneinstellungen und Richtlinien definieren"im Artikel <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Pinnwandspalten verwalten</a>.</p>
      <p>Wenn Sie auf <strong>[!UICONTROL Mark Complete]</strong> oben auf der Karte, ändert sich der Status automatisch in Abgeschlossen .</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplanter Abschluss]</strong></td>
      <td>Durch Ändern dieses Datums wird auch das geplante Abschlussdatum am verbundenen Datum geändert [!DNL Workfront] -Objekt.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td><p>Die Anzahl der Stunden, in denen die Karte ausgefüllt werden soll.</p><p>Wenn Sie die Schätzung ändern, ändert sich auch der Story-Punkt-Wert auf dem verbundenen [!DNL Workfront] -Objekt.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Zuweisung]</strong></td>
      <td><p>Um der Karte weitere Personen oder ein Team zuzuweisen, klicken Sie auf <strong>[!UICONTROL Zuweisung hinzufügen]</strong> und beginnen Sie, einen Namen in das Suchfeld einzugeben. Wählen Sie sie dann aus, wenn sie in der Ergebnisliste angezeigt wird. Sie können sowohl Einzelanwender als auch Teams hinzufügen. Nur eine Teamzuweisung ist auf einer verbundenen Karte erlaubt.</p>
      <p>Alle von Ihnen ausgewählten Bevollmächtigten werden ebenfalls der Aufgabe oder dem Problem in [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Suchen Sie nach Tags für die Karte und wählen Sie sie aus.</p>
      <p>Informationen zum Erstellen neuer Tags finden Sie unter <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Tags hinzufügen</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Benutzerdefinierte Felder]</strong></td>
      <td><p>Alle von Ihnen hinzugefügten benutzerdefinierten Felder werden in diesem Bereich angezeigt.</p>
      <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen der angezeigten Felder auf einer Karte</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Unteraufgabe]</strong></td>
      <td><p>Alle vorhandenen Unteraufgaben für die Aufgabe werden in diesem Abschnitt angezeigt. Klicks <strong>[!UICONTROL Unteraufgabe hinzufügen]</strong> , um eine neue Unteraufgabe hinzuzufügen.</p>
      <p>Der Zähler oben im Abschnitt zeigt die Anzahl der abgeschlossenen Unteraufgaben und die Gesamtzahl der Unteraufgaben an.</p>
      <p>Weitere Informationen zu Unteraufgaben finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Verwalten von Unteraufgaben auf Pinnwänden</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checkliste]</strong></td>
      <td><p>Klicks <strong>[!UICONTROL Checklisten-Element hinzufügen]</strong>. Geben Sie dann den Titel des Elements ein und drücken Sie die Eingabetaste. Ein weiteres Element wird automatisch hinzugefügt. Fahren Sie mit der Eingabe von Titeln fort, um weitere Elemente hinzuzufügen.</p>
      <p>Der Zähler oben in der Checkliste zeigt die Anzahl der abgeschlossenen Elemente und die Gesamtzahl der Elemente an.</p> <p>Weitere Informationen zu Checklisten-Elementen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Verwalten von Checklisten-Elementen auf Karten</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Dokumente]</strong></td>
      <td>Bewegen Sie bei einem vorhandenen Dokument den Mauszeiger über die Dokumentminiaturansicht und klicken Sie auf <strong>Vorschau</strong> , um die Datei im Browser anzuzeigen, oder <strong>Herunterladen</strong> , um die Datei auf Ihren Computer herunterzuladen. Ein neues Dokument finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Hinzufügen von Dokumenten zu Karten</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Siehe "Loggen Sie Stunden auf einer verbundenen Karte ein" unten.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Kommentare]</strong></td>
      <td><p>Klicken Sie in der <strong>[!UICONTROL Neuer Kommentar]</strong> und geben Sie Ihren Kommentar ein. Formatieren Sie den Text mithilfe der Formatierungs-Tools und klicken Sie auf die <strong>Anlage hinzufügen</strong> icon <img src="assets/attachment-icon.png" alt="Anlagensymbol"> , um eine Datei an den Kommentar anzuhängen. Verwenden Sie das Suchfeld unten im Kommentarbereich, um eine Person oder ein Team mit Tags zu versehen. Der Benutzer muss kein Mitglied auf der Pinnwand sein. Benutzer mit Tags auf verbundenen Karten erhalten E-Mail-Benachrichtigungen.</p><p>Klicks <strong>[!UICONTROL Submit]</strong> , um den Kommentar zur Karte hinzuzufügen.</p>
      <p><strong>NOTE:</strong> Der Kommentarbereich auf Karten verwendet das neue Adobe Workfront-Kommentarerlebnis. Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Update der Arbeit</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Systemaktivität]</strong></td> 
      <td><p>Wenn Sie <strong>Systemaktivität</strong> als Kartenabschnitt aktiviert wurde, wird die Aktivität in diesem Bereich angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassen der angezeigten Felder auf einer Karte</a> und <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Vom System getrackte Aktualisierungen</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Verwenden Sie das linke Navigationsfenster, um zwischen den Bereichen der Felder in den Kartendetails zu wechseln.

1. Klicks **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.
Das verbundene Objekt, die zugewiesenen Personen, die Tags, das Fälligkeitsdatum, der Zähler der Checkliste, die geschätzten Stunden und der Status werden auf der Karte angezeigt.

   ![Karte zur Pinnwand hinzugefügt](assets/boards-connected-card-details-110922.png)

## Trennen Sie die verbundene Karte.

Sie können eine verbundene Karte vom Workfront-Objekt trennen und die Karte bleibt auf der Pinnwand als Ad-hoc-Karte, die Sie bearbeiten können.

So trennen Sie die Verbindung auf Pinnwandebene:

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der verbundenen Karte und wählen Sie **[!UICONTROL Trennen]**.
1. Klicks **[!UICONTROL Trennen]** in der Bestätigungsnachricht angezeigt.

So trennen Sie die Verbindung auf Kartenebene:

1. Rufen Sie die Pinnwand auf und öffnen Sie die verbundene Karte.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) im Bereich &quot;Verbindung&quot;der Kartendetails und wählen Sie **[!UICONTROL Trennen]**.
1. Klicks **[!UICONTROL Trennen]** in der Bestätigungsnachricht angezeigt.

## Eine Ad-hoc-Karte in eine verbundene Karte konvertieren

Nachdem Sie eine Ad-hoc-Karte erstellt haben, können Sie sie in eine verbundene Karte konvertieren. Weitere Informationen zu Ad-hoc-Karten finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Rufen Sie die Pinnwand auf und öffnen Sie die Ad-hoc-Karte.
1. Überprüfen Sie den Namen und die Beschreibung auf der Karte. Sie werden der Aufgabe oder dem Problem hinzugefügt, die/das Sie in erstellen [!DNL Workfront].
1. Im [!UICONTROL Verbindung] Bereich der Kartendetails, klicken Sie auf **[!UICONTROL Verbindung mit Workfront herstellen]**.
1. Im [!UICONTROL Karte verbinden] auswählen, ob Sie eine Aufgabe oder ein Problem erstellen.
1. Suchen Sie nach einem Projekt, dem die Aufgabe oder das Problem hinzugefügt werden soll, und wählen Sie es aus.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben.
   >* Beim Filtern nach **[!UICONTROL Eigene Projekte]** oder **[!UICONTROL Projekte, an denen ich arbeite]**, Projekte, die einer [!UICONTROL Fertig], [!UICONTROL Inaktiv]oder [!UICONTROL Abgelehnt] -Status nicht enthalten sind. Sie können mit der **[!UICONTROL Alle]** Filter.

1. Klicks **[!UICONTROL Verbinden]**.

   ![Ad-hoc-Karte mit Workfront verbinden](assets/boards-connect-ad-hoc-card.png)

   Der Projektname wird im Bereich Verbindung in den Kartendetails angezeigt.

1. Klicks **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.

## Login-Stunden auf einer verbundenen Karte

Sie müssen über die richtigen Berechtigungen verfügen, um Stunden für die verbundene Aufgabe oder das Problem zu protokollieren.

Die Zeitprotokollierungsfelder werden nicht standardmäßig auf verbundenen Karten angezeigt. Sie müssen [!UICONTROL **Stunden**] im [!UICONTROL Konfigurieren] Gebiet unter [!UICONTROL Karten]. Weitere Informationen finden Sie unter [Anpassen der angezeigten Felder auf einer Karte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Geben Sie die Anzahl der Stunden für die Aufgabe oder das Problem ein.
1. Wählen Sie eine [!UICONTROL Stündentyp] aus dem Dropdown-Menü, wenn es sich von der Standardeinstellung unterscheidet.
1. Klicks [!UICONTROL **Protokollzeit**].

   ![Login hours on card](assets/log-hours-on-card.png)

   Die auf der Karte protokollierte Zeit wird auch bei der verbundenen Aufgabe oder dem Problem gespeichert.

Die Protokollierungszeit auf der Karte entspricht der Protokollierungszeit für eine Aufgabe oder ein Problem. Weitere Informationen finden Sie unter &quot;Zeitpunkt der Anmeldung für ein Projekt, eine Aufgabe oder ein Problem&quot;im Artikel [Protokollzeit](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

