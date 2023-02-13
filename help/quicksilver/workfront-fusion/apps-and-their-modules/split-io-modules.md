---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Split.io-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Split.io], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Split.io], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Split.io] -Module, müssen Sie über eine [!DNL Split.io] -Konto.

## Verbinden [!DNL Split.io] nach [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Sie können eine Verbindung zu Ihrem [!DNL Split.io] direkt in einer [!DNL Split.io] -Modul.

1. In jeder [!DNL Split.io] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Geben Sie einen Namen für die Verbindung ein.
1. Geben Sie Ihre [!DNL Split.io] API-Schlüssel.

   Weitere Informationen finden Sie unter [!DNL Split.io] API-Schlüssel, siehe [API-Schlüssel](https://help.split.io/hc/en-us/articles/360019916211-API-keys) im [!DNL Split.io] Dokumentation.

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Split.io] Module und ihre Felder

Bei der Konfiguration [!DNL split.io] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL split.io] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Aktionen

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Aufspaltung abrufen]](#get-split)
* [[!UICONTROL Aufspaltungsdefinition in Umgebung abrufen]](#get-split-definition-in-environment)
* [[!UICONTROL Aufspaltung erstellen]](#create-split)
* [[!UICONTROL Aufspaltung löschen]](#delete-split)
* [[!UICONTROL Geteilte Definition in Umgebung erstellen]](#create-split-definition-in-environment)
* [[!UICONTROL Geteilte Definition aus Umgebung entfernen]](#remove-split-definition-from-environment)
* [[!UICONTROL Teilweise Aktualisierung der Aufspaltungsdefinition in der Umgebung]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Tags zuordnen]](#associate-tags)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL split.io] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL split.io] Module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu ein <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, mit denen das Modul während der verschiedenen Ausführungszyklen eines Szenarios arbeiten soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltung abrufen]

Dieses Aktionsmodul ruft die Aufspaltung ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Aufspaltung enthält, die Sie abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein, die Sie abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltungsdefinition in Umgebung abrufen]

Dieses Aktionsmodul ruft eine bestimmte Aufspaltungsdefinition aus der angegebenen Umgebung ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Aufspaltungsdefinition enthält, die Sie abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umgebungsname oder ID]</td> 
   <td>Wählen Sie die Umgebung aus, die die Aufspaltungsdefinition enthält, die Sie abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein oder ordnen Sie sie zu, für die Sie die Aufspaltungsdefinition abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltung erstellen]

Dieses Aktionsmodul erstellt eine neue Aufspaltung in Ihrer Organisation, wenn ein Traffic-Typ angegeben wird.

>[!NOTE]
>
>Die API konfiguriert die Aufspaltung in keiner Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in dem Sie die Aufteilung erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traffic Type ID or Name]</td> 
   <td>Wählen Sie den Traffic-Typ aus oder ordnen Sie ihn zu, den Sie zum Erstellen der Aufspaltung verwenden möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie einen Namen für die zu erstellende Aufspaltung ein oder ordnen Sie einen Namen zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aufspaltung Beschreibung]</td> 
   <td>Geben Sie eine [!UICONTROL Aufspaltung] Beschreibung für die zu erstellende Aufspaltung ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltung löschen]

Dieses Aktionsmodul löscht eine Aufspaltung aus Ihrer Organisation. Dadurch wird die Konfiguration der Aufspaltungsdefinition automatisch für alle Umgebungen aufgehoben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in dem Sie die Aufspaltung löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Geteilte Definition in Umgebung erstellen]

Dieses Aktionsmodul konfiguriert eine Aufspaltungsdefinition für eine bestimmte Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in dem Sie eine Aufspaltungsdefinition erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umgebungsname oder ID]</td> 
   <td>Wählen Sie die Umgebung aus oder ordnen Sie sie zu, in der Sie eine Aufspaltungsdefinition erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein oder ordnen Sie sie zu, für die Sie eine Definition erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentare]</td> 
   <td>Geben Sie Kommentare ein oder ordnen Sie sie der Aufspaltungsdefinition zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regeln]</td> 
   <td> <p>Klicken Sie für jede Targeting-Regel, die Sie zur Definition hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b>, geben Sie die Regel ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen zu Targeting-Regeln finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> im [!DNL Split.io] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standardregel]</td> 
   <td> <p>Geben Sie die Regel ein oder ordnen Sie sie zu, die die Aufspaltung für den Traffic verwenden soll, der die Spezifikationen für die anderen Regeln nicht erfüllt.</p> <p>Weitere Informationen zu Targeting-Regeln finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> im [!DNL Split.io] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standardbehandlung]</td> 
   <td> <p>Geben Sie die Behandlung ein oder ordnen Sie sie zu, die verwendet werden soll, wenn die Aufteilung beendet wird oder der Kunde nicht in der Traffic-Zuordnung enthalten ist.</p> <p>Weitere Informationen zu Behandlungen finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> im [!DNL Split.io] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Behandlungen]</td> 
   <td> <p>Klicken Sie für jede Behandlung, die Sie der Definition hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b>, geben Sie die Behandlung ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen zu Behandlungen finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> im [!DNL Split.io] Dokumentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Geteilte Definition aus Umgebung entfernen]

Dieses Aktionsmodul deinstalliert die Konfiguration einer Aufspaltungsdefinition für eine bestimmte Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in dem Sie eine Aufspaltungsdefinition entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umgebungsname oder ID]</td> 
   <td>Wählen Sie die Umgebung aus oder ordnen Sie sie zu, in der Sie eine Aufspaltungsdefinition entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein oder ordnen Sie sie zu, für die Sie eine Definition entfernen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentare]</td> 
   <td>Geben Sie Kommentare ein oder ordnen Sie sie der Aufspaltungsdefinition zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Teilweise Aktualisierung der Aufspaltungsdefinition in der Umgebung]

Dieses Aktionsmodul aktualisiert eine Aufspaltungsdefinition für eine bestimmte Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in dem Sie eine Aufspaltungsdefinition aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umgebungsname oder ID]</td> 
   <td>Wählen Sie die Umgebung aus oder ordnen Sie sie zu, in der Sie eine Aufspaltungsdefinition aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein oder ordnen Sie sie zu, für die Sie eine Definition aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhalt aktualisieren]</td> 
   <td> <p>Klicken Sie für jedes Attribut der Aufspaltung, die Sie aktualisieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die gewünschten Änderungen ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen finden Sie unter <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Teilweise Aktualisierung der Aufspaltungsdefinition in der Umgebung</a> im [!DNL Split.io] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentare]</td> 
   <td>Geben Sie Kommentare ein oder ordnen Sie sie der Aufspaltungsdefinition zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tags zuordnen]

Dieses Aktionsmodul fügt dem angegebenen Objekt Tags hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, in den Sie ein Tag einfügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objektname]</td> 
   <td>Geben Sie den Namen des Objekts ein, dem Sie Tags hinzufügen möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekttyp]</td> 
   <td> <p>Geben Sie den Objekttyp ein oder ordnen Sie ihn zu, dem Sie Tags hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>Klicken Sie für jedes Tag, das Sie hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie das Tag ein oder ordnen Sie es zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Arbeitsbereiche abrufen]](#get-workspaces)
* [[!UICONTROL Abrufen von Umgebungen]](#get-environments)
* [[!UICONTROL Aufspaltungen abrufen]](#get-splits)
* [[!UICONTROL Aufspaltungsdefinitionen in einer Umgebung auflisten]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Traffic-Typen abrufen]](#get-traffic-types)

#### [!UICONTROL Arbeitsbereiche abrufen]

Dieses Suchmodul ruft die Arbeitsbereiche für eine Organisation ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Arbeitsbereichen ein oder ordnen Sie sie zu, die das Modul während der einzelnen Szenario-Ausführungszyklen abrufen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen von Umgebungen]

Dieses Suchmodul ruft eine Liste von Umgebungen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Umgebungen enthält, die Sie auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltungen abrufen]

Dieses Suchmodul ruft eine Liste von Aufspaltungen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Auflistungen enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Aufspaltungen ein oder ordnen Sie sie zu, die das Modul während der einzelnen Szenario-Ausführungszyklen abrufen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufspaltungsdefinitionen in einer Umgebung auflisten]

Dieses Suchmodul ruft eine Liste von Aufspaltungsdefinitionen in einer bestimmten Umgebung ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die aufzulistenden Aufspaltungsdefinitionen enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umgebungsname oder ID]</td> 
   <td>Wählen Sie die Umgebung aus, die die aufzulistenden Aufspaltungsdefinitionen enthält, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Aufspaltungsdefinitionen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus abrufen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Traffic-Typen abrufen]

Dieses Suchmodul ruft eine Liste von Traffic-Typen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Split.io] Konto [!DNL Workfront Fusion], siehe <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Split.io] nach [!UICONTROL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Traffic-Typen enthält, die Sie auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>
