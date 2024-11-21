---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Split.io-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Split.io] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1819'
ht-degree: 0%

---

# [!DNL Split.io] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Split.io] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Split.io] -Module zu verwenden, müssen Sie über ein [!DNL Split.io] -Konto verfügen.

## API-Informationen für Split.io

Der Connector Split.io verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.split.io/internal/api</td>
   </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v2 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.34.1</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Split.io] mit [!DNL Workfront Fusion] verbinden {#connect-split-io-to-workfront-fusion}

Sie können eine Verbindung zu Ihrem [!DNL Split.io]-Konto direkt aus einem [!DNL Split.io]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL Split.io]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Geben Sie einen Namen für die Verbindung ein.
1. Geben Sie Ihren [!DNL Split.io] API-Schlüssel ein.

   Weitere Informationen zu [!DNL Split.io] API-Schlüsseln finden Sie unter [API-Schlüssel](https://help.split.io/hc/en-us/articles/360019916211-API-keys) in der Dokumentation zu [!DNL Split.io].

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Split.io] Module und ihre Felder

Wenn Sie [!DNL split.io] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL split.io] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Aktionen

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Aufspaltung abrufen]](#get-split)
* [[!UICONTROL Aufspaltungsdefinition in Umgebung abrufen]](#get-split-definition-in-environment)
* [[!UICONTROL Aufspaltung erstellen]](#create-split)
* [[!UICONTROL Aufspaltung löschen]](#delete-split)
* [[!UICONTROL Erstellen einer Aufspaltungsdefinition in der Umgebung]](#create-split-definition-in-environment)
* [[!UICONTROL Trenndefinition aus Umgebung entfernen]](#remove-split-definition-from-environment)
* [[!UICONTROL Teilweise Aktualisierung der Aufspaltungsdefinition in der Umgebung]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Tags zuordnen]](#associate-tags)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL split.io] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL split.io] -Modulen nicht ausgeführt werden kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://api.split.io/internal/api/v2/</code> ein.</td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Aufspaltung enthält, die Sie abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Geben Sie den Namen der Aufspaltung ein oder ordnen Sie sie zu.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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

#### [!UICONTROL Erstellen einer Aufspaltungsdefinition in der Umgebung]

Dieses Aktionsmodul konfiguriert eine Aufspaltungsdefinition für eine bestimmte Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Geben Sie den Namen der Aufspaltung ein, für die Sie eine Definition erstellen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentare]</td> 
   <td>Geben Sie Kommentare ein oder ordnen Sie sie der Aufspaltungsdefinition zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Regeln]</td> 
   <td> <p>Klicken Sie für jede Targeting-Regel, die Sie zur Definition hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die Regel ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen zu Targeting-Regeln finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> in der Dokumentation zu [!DNL Split.io] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standardregel]</td> 
   <td> <p>Geben Sie die Regel ein oder ordnen Sie sie zu, die die Aufspaltung für den Traffic verwenden soll, der die Spezifikationen für die anderen Regeln nicht erfüllt.</p> <p>Weitere Informationen zu Targeting-Regeln finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> in der Dokumentation zu [!DNL Split.io] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standardbehandlung]</td> 
   <td> <p>Geben Sie die Behandlung ein oder ordnen Sie sie zu, die verwendet werden soll, wenn die Aufteilung beendet wird oder der Kunde nicht in der Traffic-Zuordnung enthalten ist.</p> <p>Weitere Informationen zu Behandlungen finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> in der [!DNL Split.io] -Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Behandlungen]</td> 
   <td> <p>Klicken Sie für jede Behandlung, die Sie der Definition hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die Behandlung ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen zu Behandlungen finden Sie unter <a href="https://docs.split.io/reference#create-split-definition-in-environment">Erstellen einer Aufspaltungsdefinition in einer Umgebung</a> in der [!DNL Split.io] -Dokumentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trenndefinition aus Umgebung entfernen]

Dieses Aktionsmodul deinstalliert die Konfiguration einer Aufspaltungsdefinition für eine bestimmte Umgebung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Klicken Sie für jedes Attribut der Aufspaltung, die Sie aktualisieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die gewünschten Änderungen ein oder ordnen Sie sie zu.</p> <p>Weitere Informationen finden Sie unter <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Teilweise Aktualisierung der Aufspaltungsdefinition in der Umgebung</a> in der Dokumentation zu [!DNL Split.io].</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
* [[!UICONTROL Umgebungen abrufen]](#get-environments)
* [[!UICONTROL Aufspaltungen abrufen]](#get-splits)
* [[!UICONTROL Aufspaltungsdefinitionen in einer Umgebung ]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Traffic-Typen abrufen]](#get-traffic-types)

#### [!UICONTROL Arbeitsbereiche abrufen]

Dieses Suchmodul ruft die Arbeitsbereiche für eine Organisation ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Arbeitsbereichen ein oder ordnen Sie sie zu, die das Modul während der einzelnen Szenario-Ausführungszyklen abrufen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Umgebungen abrufen]

Dieses Suchmodul ruft eine Liste von Umgebungen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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

#### [!UICONTROL Aufspaltungsdefinitionen in einer Umgebung ]

Dieses Suchmodul ruft eine Liste von Aufspaltungsdefinitionen in einer bestimmten Umgebung ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Split.io]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Split.io] mit [!UICONTROL Workfront Fusion] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die Traffic-Typen enthält, die Sie auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>
