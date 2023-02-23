---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Angeschlossene Karten auf Pinnwänden verwenden
description: Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in Workfront verbunden ist.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 2a71ffd9180f2fe783675ae005165e1fd078178a
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 0%

---

# Angeschlossene Karten auf Pinnwänden verwenden

{{highlighted-preview}}

Sie können Ihrer Pinnwand eine Karte hinzufügen, die mit bestehenden Aufgaben und Problemen in [!DNL Workfront].

Wenn eine der folgenden Details für die Karte an einem Ort aktualisiert wird, wird sie automatisch an einem anderen Speicherort aktualisiert:

* [!UICONTROL Name]
* [!UICONTROL Beschreibung]
* [!UICONTROL Zugewiesene]
* [!UICONTROL Status]
* [!UICONTROL Geplantes Abschlussdatum]
* [!UICONTROL Schätzung] / [!UICONTROL Story Points]

>[!NOTE]
>Eine einzelne verbundene Aufgabe oder ein Problem kann nur einmal pro Pinnwand hinzugefügt werden. Dieselbe Aufgabe oder dasselbe Problem kann mit mehreren Pinnwänden verbunden sein.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td>
   <td><p>[!UICONTROL Ansicht] oder höherer Zugriff auf Aufgaben und Probleme</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Objektberechtigungen</strong></td>
   <td><p>[!UICONTROL Ansicht] oder höhere Berechtigungen für Workfront-Aufgaben oder -Probleme</p></td>
  </tr>
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Hinzufügen einer verbundenen Karte

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Pinnwände]**.
1. Greifen Sie auf eine Pinnwand zu. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken **[!UICONTROL Karte hinzufügen] > [!UICONTROL Verbundene Karte]**.
1. Wählen Sie ein Projekt aus und wählen Sie dann eine Aufgabe oder ein Problem, die bzw. das als Karte auf der Pinnwand hinzugefügt werden soll.

   Sie können mehrere Objekte auswählen, die alle als separate Karten hinzugefügt werden.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben. Wenn ein Element abgeblendet ist, wurde es bereits zur Pinnwand hinzugefügt.
   >* Beim Filtern nach **[!UICONTROL Eigene Projekte]** oder **[!UICONTROL Projekte, an denen ich arbeite]**, werden Projekte, die dem Status &quot;Abgeschlossen&quot;, &quot;Abgelaufen&quot;oder &quot;Abgelehnt&quot;entsprechen, nicht einbezogen. Sie können mit der **[!UICONTROL Alle]** Filter.


1. Klicken **[!UICONTROL Hinzufügen]**.

   ![Suche nach Aufgabe oder Problem, um eine Verbindung herzustellen](assets/boards-tasksissues-350x94.png)

   Die Karte wird unten in der Spalte ganz links hinzugefügt. Der verbundene [!DNL Workfront] -Objekt und dessen Bevollmächtigte werden auf der Karte angezeigt.

   >[!NOTE]
   >
   >Wenn ein Bevollmächtigter [!DNL Workfront] Aufgabe oder Problem ist kein Mitglied der Pinnwand, sie werden nicht der Karte zugewiesen.

   ![Verbundene Karte](assets/boards-connected-card-first-added.png)

1. Klicken ![Aufgabe oder Problem öffnen](assets/boards-launch-icon.png) , um [!DNL Workfront] Aufgabe oder Problem in einer neuen Browser-Registerkarte.
1. Um die Kartendetails zu bearbeiten, klicken Sie auf die Karte (nicht im Kartennamen).

   Oder

   Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Bearbeiten]**.

1. Im **[!UICONTROL Kartendetails]** die folgenden Informationen hinzufügen oder aktualisieren:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td> <p>Durch Ändern des Namens wird auch der Name auf der verbundenen Seite geändert [!DNL Workfront] -Objekt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td> 
      <td> <p>Durch Ändern der Beschreibung wird auch die Beschreibung auf der verbundenen Seite geändert [!DNL Workfront] -Objekt.</p> </td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Zuweisung]</strong></td>
      <td><p>Um der Karte weitere Personen oder ein Team zuzuweisen, geben Sie im Suchfeld einen Namen ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können sowohl Einzelanwender als auch Teams hinzufügen. Nur eine Teamzuweisung ist auf einer verbundenen Karte erlaubt.</p>
      <p>Bevollmächtigte müssen Mitglieder in der Pinnwand sein, oder sie werden nicht in der Auswahlliste angezeigt. Wenn ein Team Mitglied im Board ist, können die einzelnen Teammitglieder der Karte zugewiesen werden.</p>
      <p>Alle von Ihnen ausgewählten Bevollmächtigten werden ebenfalls der Aufgabe oder dem Problem in [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Spalte]</strong></td>
      <td><p>Wählen Sie die Spalte für die Karte aus.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Wählen Sie einen Status für die Karte aus. Die Standardwerte sind [!UICONTROL New], [!UICONTROL In Bearbeitung] und [!UICONTROL Complete], jedoch alle benutzerdefinierten Status, die für das Element unter [!DNL Workfront] sind auch verfügbar.</p>
      <p>Wenn Sie Spaltenrichtlinien zum Aktualisieren von Feldwerten aktiviert haben, wird die Karte beim Ändern des Status auf der Karte automatisch in die entsprechende Spalte verschoben. Weitere Informationen finden Sie unter "Definieren von Spalteneinstellungen und -richtlinien"im Artikel <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Pinnwandspalten verwalten</a>.</p>
      <p>Wenn Sie auf <strong>[!UICONTROL Mark Complete]</strong> oben auf der Karte, ändert sich der Status automatisch in Abgeschlossen .</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplanter Abschluss]</strong></td>
      <td><p>Durch Ändern dieses Datums wird auch das geplante Abschlussdatum am verbundenen Datum geändert [!DNL Workfront] -Objekt.</p></td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td><p>Die Anzahl der Stunden, in denen die Karte ausgefüllt werden soll.</p><p>Wenn Sie die frühe Funktion verwenden, können Sie sich für [!DNL Workfront] [!UICONTROL Pinnwände], wobei die Schätzung geändert wird, ändert sich auch der Story-Punktwert auf der verbundenen Seite [!DNL Workfront] -Objekt.</p><p>Wenn Sie sich nicht für frühe Funktionen entscheiden, ist dieses Feld nur ein manueller Eintrag und der Wert darf nicht größer als 99 sein.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Suchen Sie nach Tags für die Karte und wählen Sie sie aus.</p>
      <p>Informationen zum Erstellen neuer Tags finden Sie unter <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Tags hinzufügen</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklisten-Elemente]</strong> </td> 
      <td> <p>Klicken <strong>[!UICONTROL Checklisten-Element hinzufügen]</strong>. Geben Sie dann den Titel des Elements ein und drücken Sie die Eingabetaste. Ein weiteres Element wird automatisch hinzugefügt. Fahren Sie mit der Eingabe von Titeln fort, um weitere Elemente hinzuzufügen.</p> <p>Der Zähler oben in der Checkliste zeigt die Anzahl der abgeschlossenen Elemente und die Gesamtzahl der Elemente an.</p> <p>Weitere Informationen zu Checklisten-Elementen finden Sie unter <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Verwalten von Checklisten-Elementen auf Karten</a>.</p></td>
     </tr>
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.
Das verbundene Objekt, die zugewiesenen Personen, die Tags, das Fälligkeitsdatum, der Zähler der Checkliste, die geschätzten Stunden und der Status werden auf der Karte angezeigt.

   ![Karte zur Pinnwand hinzugefügt](assets/boards-connected-card-details-110922.png)

## Trennen Sie die verbundene Karte.

Sie können eine verbundene Karte vom Workfront-Objekt trennen und die Karte bleibt auf der Pinnwand als Ad-hoc-Karte, die Sie bearbeiten können.

So trennen Sie die Verbindung auf Pinnwandebene:

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der verbundenen Karte und wählen Sie **[!UICONTROL Trennen]**.
1. Klicken **[!UICONTROL Trennen]** in der Bestätigungsnachricht angezeigt.

So trennen Sie die Verbindung auf Kartenebene:

1. Rufen Sie die Pinnwand auf und öffnen Sie die verbundene Karte.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) im Bereich &quot;Verbindung&quot;der Kartendetails und wählen Sie **[!UICONTROL Trennen]**.
1. Klicken **[!UICONTROL Trennen]** in der Bestätigungsnachricht angezeigt.

## Eine Ad-hoc-Karte in eine verbundene Karte konvertieren

Nachdem Sie eine Ad-hoc-Karte erstellt haben, können Sie sie in eine verbundene Karte konvertieren. Weitere Informationen zu Ad-hoc-Karten finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Rufen Sie die Pinnwand auf und öffnen Sie die Ad-hoc-Karte.
1. Überprüfen Sie den Namen und die Beschreibung auf der Karte. Sie werden der Aufgabe oder dem Problem hinzugefügt, die bzw. das Sie in [!DNL Workfront].
1. Im [!UICONTROL Verbindung] Bereich der Kartendetails, klicken Sie auf **[!UICONTROL Verbindung mit Workfront herstellen]**.
1. Im [!UICONTROL Karte verbinden] auswählen, ob Sie eine Aufgabe oder ein Problem erstellen.
1. Suchen Sie nach einem Projekt, dem die Aufgabe oder das Problem hinzugefügt werden soll, und wählen Sie es aus.

   >[!NOTE]
   >
   >* In den Suchergebnissen sind nur Objekte verfügbar, für die Sie Berechtigungen haben.
   >* Beim Filtern nach **[!UICONTROL Eigene Projekte]** oder **[!UICONTROL Projekte, an denen ich arbeite]**, Projekte, die einer [!UICONTROL Fertig], [!UICONTROL Inaktiv]oder [!UICONTROL Zurückgewiesen] -Status nicht enthalten sind. Sie können mit der **[!UICONTROL Alle]** Filter.


1. Klicken **[!UICONTROL Verbinden]**.

   ![Ad-hoc-Karte mit Workfront verbinden](assets/boards-connect-ad-hoc-card.png)

   Der Projektname wird im Bereich Verbindung in den Kartendetails angezeigt.

1. Klicken **[!UICONTROL Schließen]** , um zur Pinnwand zurückzukehren.

<div class="preview">

## Login-Stunden auf einer verbundenen Karte

>[!NOTE]
>
>Diese Funktion ist nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar.

Sie müssen über die richtigen Berechtigungen verfügen, um Stunden für die verbundene Aufgabe oder das Problem zu protokollieren.

Die Zeitprotokollierungsfelder werden nicht standardmäßig auf verbundenen Karten angezeigt. Sie müssen [!UICONTROL **Stunden**] im [!UICONTROL Konfigurieren] Gebiet unter [!UICONTROL Karten]. Weitere Informationen finden Sie unter [Anpassen der angezeigten Felder auf einer Karte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Geben Sie die Anzahl der Stunden für die Aufgabe oder das Problem ein.
1. Wählen Sie eine [!UICONTROL Stündentyp] aus dem Dropdown-Menü, wenn es sich von der Standardeinstellung unterscheidet.
1. Klicken [!UICONTROL **Protokollzeit**].

   ![Login-Stunden auf der Karte](assets/log-hours-on-card.png)

   Die auf der Karte protokollierte Zeit wird auch bei der verbundenen Aufgabe oder dem Problem gespeichert.

Die Protokollierungszeit auf der Karte entspricht der Protokollierungszeit für eine Aufgabe oder ein Problem. Weitere Informationen finden Sie unter &quot;Zeitpunkt der Anmeldung für ein Projekt, eine Aufgabe oder ein Problem&quot;im Artikel [Protokollzeit](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

</div>
