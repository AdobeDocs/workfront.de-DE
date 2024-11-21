---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront-Boards-Module
description: Sie können den Adobe Workfront-Mainboards-Connector verwenden, um Ihre Prozesse in Workfront-Pinnwänden zu automatisieren und mit Apps und Diensten von Drittanbietern zu verbinden.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 0b4a25f7-a8f1-47f4-8929-7eff82f1dfdc
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '2647'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Forumsmodule

>[!NOTE]
>
>Der Boards Fusion-Connector befindet sich im Beta-Status. Daher ist die Unterstützung für diesen Connector begrenzt und kann sich aufgrund der künftigen Entwicklung von Foren ändern. Darüber hinaus kann es ohne Vorankündigung Änderungen an der GraphQL-API geben, die sich auf Ihren Fusion-Connector-Prozess auswirken könnten.

Adobe Workfront-Pinnwände sind flexible Tools, die die Teamzusammenarbeit ermöglichen, indem sie Zugriff auf eine freigegebene Pinnwand mit Spalten und Karten bieten.

Sie können die Adobe Workfront-Pinnwandmodule verwenden, um Datensätze zu lesen oder zu aktualisieren, einen API-Aufruf an die Workfront-Pinnwand-API durchzuführen oder ein Trigger zu erstellen, wenn eine Aktion auf einer Pinnwand stattfindet.

Allgemeine Informationen zu Workfront-Pinnwänden finden Sie unter [Überblick über Pinnwände](/help/quicksilver/agile/boards-overview.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>
  <td> <p>Alle</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>
   <td> <p>Neu: Standard</p><p>Oder</p><p>Aktuell: [!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Voraussetzungen

Sie müssen eine Pinnwand in Adobe Workfront konfiguriert haben, bevor Sie eine Verbindung herstellen können.

## API-Informationen zu Adobe Workfront Boards

Der Adobe Workfront Boards-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.23.6</td> 
  </tr>
 </tbody> 
 </table>

## Herstellen einer Verbindung zu Workfront-Pinnwänden

>[!NOTE]
>
>Sie können eine Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine separate Workfront-Pinnwand-Verbindung erstellen.

So erstellen Sie eine Workfront-Pinnwandverbindung:

1. Klicken Sie in einem beliebigen [!DNL Adobe Workfront Boards]-Modul neben dem Feld &quot;Verbindung&quot;auf **[!UICONTROL Hinzufügen]** .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Verbindungsname]</td>
          <td>
            <p>Geben Sie einen Namen für diese Verbindung ein.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Umgebung]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen möchten.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Typ]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-ID]<p>(Optional)</p></td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client-ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]<p>(Optional)</p></td>
          <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Authentifizierungs-URL]<p>(Optional)</p></td>
          <td>Geben Sie die URL ein, die Ihre Instanz von Workfront zum Authentifizieren dieser Verbindung verwendet. <p>Der Standardwert ist <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Host-Präfix]</td>
          <td>Geben Sie Ihr Host-Präfix ein.<p>Der Standardwert ist <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## Adobe Workfront-Forumsmodule und ihre Felder

Wenn Sie Workfront-Pinnwandmodule konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Workfront-Pinnwände-Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Karten](#cards)
* [Pinnwände](#boards)
* [Spalten](#columns)
* [Tags](#tags)
* [Kommentare](#comments)
* [Sonstige](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### Karten

* [Checklisten-Objekt hinzufügen](#add-checklist-item)
* [Unteraufgabe hinzufügen](#add-subtask)
* [Karte erstellen](#create-a-card)
* [Karte verschieben](#move-a-card)
* [Karte lesen](#read-a-card)
* [Karte aktualisieren](#update-a-card)

#### Checklisten-Objekt hinzufügen

Dieses Aktionsmodul fügt der angegebenen Karte ein Element der Checkliste hinzu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein oder ordnen Sie sie zu, der Sie ein Element der Checkliste hinzufügen möchten.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Checklisten-Elemente]</td> 
   <td>Klicken Sie für jedes Checklisten-Element, das Sie hinzufügen möchten, auf Element hinzufügen, geben Sie den Namen des Checklisten-Elements ein und wählen Sie aus, ob das Element fertig gestellt wurde.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Unteraufgabe hinzufügen

Dieses Aktionsmodul fügt einer Karte in Foren eine Unteraufgabe hinzu. Die Karte muss eine vernetzte Karte sein. Die Unteraufgabe wird auch der Workfront-Aufgabe hinzugefügt, die die Karte darstellt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Übergeordnete Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein oder ordnen Sie sie zu, der Sie eine Unteraufgabe hinzufügen möchten.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein, die die Karte enthält, der Sie eine Unteraufgabe hinzufügen möchten, oder ordnen Sie sie zu.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für die neue Unteraufgabe ein oder ordnen Sie ihn zu.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Karte erstellen

Dieses Aktionsmodul erstellt eine neue Karte auf einer Workfront-Pinnwand.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, der Sie eine Karte hinzufügen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spalten-ID]</td> 
   <td>Geben Sie die Kennung der Spalte ein, der Sie eine Unteraufgabe hinzufügen möchten, oder ordnen Sie sie zu.<p>Sie finden die Spaltenkennung in den Informationen, die vom Modul Pinnwand lesen zurückgegeben werden.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für die neue Karte ein oder ordnen Sie ihn zu.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Karte verschieben

Dieses Aktionsmodul verschiebt eine Karte in eine andere Spalte auf derselben Pinnwand.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein, die Sie verschieben möchten, oder ordnen Sie sie zu.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, die die Karte enthält, die Sie verschieben möchten.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ziel-Spalte-ID]</td> 
   <td>Geben Sie die Kennung der Spalte ein, in die Sie die Karte verschieben möchten, oder ordnen Sie sie zu.<p>Sie finden die Spaltenkennung in den Informationen, die vom Modul Pinnwand lesen zurückgegeben werden.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To Index]</td> 
   <td>Geben Sie die Position ein oder ordnen Sie sie der Karte in der neuen Spalte zu.<p>Die oberste Position in der Spalte in Index 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Karte lesen

Dieses Aktionsmodul ruft Informationen zu einer bestimmten Karte ab.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein, die Sie lesen möchten, oder ordnen Sie sie zu.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Karte aktualisieren

Dieses Aktionsmodul aktualisiert Informationen für eine von Ihnen angegebene Karte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein, die Sie aktualisieren möchten, oder ordnen Sie sie zu.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, die die zu aktualisierende Karte enthält.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Geben Sie einen neuen Namen für die Karte ein oder ordnen Sie ihn zu.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie eine neue Beschreibung für die Karte ein oder ordnen Sie sie zu.</p></td> 
  </tr> 
 </tbody> 
</table>

### Pinnwände

* [Pinnwand erstellen](#create-a-board)
* [Pinnwand lesen](#read-a-board)

#### Pinnwand erstellen

Dieses Aktionsmodul erstellt eine Pinnwand in Workfront. Sie können den Typ der Pinnwand angeben, die Sie erstellen möchten.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandname]</td> 
   <td>Geben Sie einen Namen für die neue Pinnwand ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ]</td> 
   <td>Wählen Sie den Typ der Pinnwand aus, die Sie erstellen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Pinnwand lesen

Dieses Aktionsmodul gibt Informationen zu einer einzelnen Pinnwand zurück, z. B. zu den Karten, Spalten, Tags und Mitgliedern der Pinnwand.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, für die Sie Informationen abrufen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
 </tbody> 
</table>

### Spalten

* [Spalte erstellen](#create-a-column)
* [Nach einer Spalte suchen](#search-for-a-column)
* [Spalte aktualisieren](#update-a-column)

#### Spalte erstellen

Dieses Aktionsmodul erstellt eine neue Spalte auf der angegebenen Pinnwand.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, der Sie eine Spalte hinzufügen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spalten-ID]</td> 
   <td>Geben Sie die Kennung der Spalte ein, die Sie aktualisieren möchten, oder ordnen Sie sie zu.<p>Sie finden die Spaltenkennung in den Informationen, die vom Modul Pinnwand lesen zurückgegeben werden.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spaltenname]</td> 
   <td>Geben Sie einen neuen Namen für die Spalte ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL WIP Limit]</td> 
   <td>Geben Sie eine neue WIP-Begrenzung für die Spalte ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Nach einer Spalte suchen

Dieses Suchmodul gibt Informationen zur Spalte mit dem angegebenen Namen zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, die die Spalte enthält, die Sie abrufen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spaltenname]</td> 
   <td>Geben Sie den Namen der Spalte ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Spalte aktualisieren

Dieses Aktionsmodul aktualisiert den Namen oder die WIP-Grenze der angegebenen Spalte.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, die die Spalte enthält, die Sie abrufen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spaltenname]</td> 
   <td>Geben Sie den Namen der Spalte ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Tags

* [Tag zu einer Karte hinzufügen](#add-card-tag)
* [Tag erstellen](#create-a-tag)

#### Tag zu einer Karte hinzufügen

Dieses Aktionsmodul fügt einer Karte ein Tag hinzu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die ID der Karte ein oder ordnen Sie sie zu, der Sie ein Tag hinzufügen möchten.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein, die die Karte enthält, der Sie ein Tag hinzufügen möchten, oder ordnen Sie sie zu.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag-ID]</td> 
   <td>Geben Sie die ID des Tags ein, das Sie hinzufügen möchten, oder ordnen Sie sie zu.<p>Sie finden die Tag-ID in den Informationen, die vom Modul Pinnwand lesen zurückgegeben werden.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Tag erstellen

Dieses Aktionsmodul erstellt ein neues Tag und weist ihm eine Farbe zu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pinnwandkennung]</td> 
   <td>Geben Sie die ID der Pinnwand ein oder ordnen Sie sie zu, für die Sie ein Tag erstellen möchten.<p>Sie können die Pinnwand-ID in der URL finden, wenn Sie die Pinnwand in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag name]</td> 
   <td>Geben Sie einen Namen für das neue Tag ein oder ordnen Sie ihn zu.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag Color]</td> 
   <td>Wählen Sie die Farbe für dieses Tag aus.</td> 
  </tr> 
 </tbody> 
</table>

### Kommentare

* [Kommentare erstellen](#create-a-comment)
* [Kommentare zu Karten lesen](#read-card-comments)

#### Kommentare erstellen

Dieses Aktionsmodul hat einen Kommentar für die angegebene Karte erstellt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein, zu der Sie einen Kommentar hinzufügen möchten, oder ordnen Sie sie zu.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kommentar]</td> 
   <td>Geben Sie den Text des Kommentars ein, den Sie hinzufügen möchten, oder ordnen Sie ihn zu.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Kommentare zu Karten lesen

Dieses Aktionsmodul ruft die Kommentare von der angegebenen Karte ab.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Karten-ID]</td> 
   <td>Geben Sie die Kennung der Karte ein, für die Sie die Kommentare abrufen möchten, oder ordnen Sie sie zu.<p>Sie können die Karten-ID in der URL finden, wenn Sie die Karte in Workfront anzeigen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Kommentaren ein, die das Modul in einem Ausführungszyklus zurückgeben soll.</p></td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

#### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Workfront-Foren-API durch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
      <td> <p>Sie können eine bestehende Workfront-Verbindung verwenden, um eine Verbindung zu Workfront-Pinnwänden herzustellen, oder Sie können eine bestimmte Workfront-Pinnwand-Verbindung verwenden. </p><p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Erstellen einer Verbindung zu Workfront-Pinnwänden</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code> ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p><p>Bei den meisten Foren-Aufrufen ist die Methode POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu. Dadurch wird der Inhaltstyp der Anforderung bestimmt.</p> <p>Beispiel:<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Bei Workfront-Pinnwänden bleibt dieser Abschnitt normalerweise leer.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form einer eingebetteten JSON-Grafik hinzu. </p> <p>Beispiel:</p><p>In diesem Beispiel wird der Spaltenname aktualisiert. Sie können die <code>boardId</code> und <code>columnId</code> als GUIDs einbeziehen, die entweder hartcodiert sind oder von einem vorherigen Modul zugeordnet wurden.<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
