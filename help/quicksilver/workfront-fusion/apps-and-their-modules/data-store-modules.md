---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Datenspeichermodule
description: Ein [!DNL Adobe Workfront Fusion] -Datenspeicher, ähnlich wie eine Datenbank oder eine einfache Tabelle, können Daten aus Szenarien speichern, sodass Daten zwischen einzelnen Szenarien oder Szenario-Läufen übertragen werden können. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# [!UICONTROL Datenspeicher] Module

Ein [!DNL Adobe Workfront Fusion] -Datenspeicher, ähnlich wie eine Datenbank oder eine einfache Tabelle, können Daten aus Szenarien speichern, sodass Daten zwischen einzelnen Szenarien oder Szenario-Läufen übertragen werden können. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.

Mit den Datenspeichermodulen können Sie Datensätze in Ihren [!DNL Adobe Workfront Fusion] Datenspeicher.

Informationen zur Erstellung, Bearbeitung und Fehlerbehebung von Datenspeichern finden Sie unter [Datenspeicher in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!UICONTROL Datenspeicher] -Modulen erstellen, müssen Sie zunächst einen Datenspeicher erstellen.

Informationen zum Erstellen von Datenspeichern finden Sie unter [Datenspeicher in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Datenspeicher] Module und ihre Felder

Wenn Sie Datenspeichermodule konfigurieren, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Datenspeicherfelder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Alle [!UICONTROL Datenspeicher] -Module sind Aktionstypmodule.

* [Hinzufügen/Ersetzen von Datensätzen](#addreplace-a-record)
* [Datensatz aktualisieren](#update-a-record)
* [Datensatz abrufen](#get-a-record)
* [Überprüfen des Vorhandenseins eines Datensatzes](#check-the-existence-of-a-record)
* [Datensatz löschen](#delete-a-record)
* [Alle Datensätze löschen](#delete-all-records)
* [Suchdatensätze](#search-records)
* [Count Records](#count-records)

### [!UICONTROL Hinzufügen/Ersetzen von Datensätzen]

Dieses Aktionsmodul fügt einen Datensatz hinzu oder ersetzt ihn.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

>[!NOTE]
>
>Das Modul gibt einen Fehler aus, wenn Sie versuchen, den Datensatz hinzuzufügen, der sich bereits im Datenspeicher unter demselben Namen befindet, und die [!UICONTROL Vorhandenen Datensatz überschreiben] deaktiviert ist.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus oder fügen Sie ihn hinzu, in dem Sie einen Datensatz erstellen möchten. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul hinzufügen oder ersetzen soll. Der Schlüssel kann später zum Abrufen des Datensatzes verwendet werden. Wenn Sie dieses Feld leer lassen, wird automatisch ein Schlüssel generiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorhandenen Datensatz überschreiben] </td> 
   <td> <p>Aktivieren Sie diese Option, um den Datensatz zu überschreiben. Der Datensatz, den Sie überschreiben möchten, muss im obigen Feld Schlüssel angegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatz] </td> 
   <td> <p>Geben Sie die gewünschten Werte in die Datensatzfelder ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen Datensatz.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus oder fügen Sie ihn hinzu, in dem Sie einen Datensatz erstellen möchten. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul aktualisieren soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fehlenden Datensatz einfügen] </td> 
   <td> <p>Aktivieren Sie diese Option, um einen neuen Datensatz zu erstellen, wenn der Datensatz mit dem angegebenen Schlüssel nicht bereits existiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatz]</td> 
   <td> <p> Geben Sie die gewünschten Werte in die Felder des Datensatzes ein, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz abrufen]

Dieses Aktionsmodul ruft einen Datensatz ab.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus, aus dem Sie einen Datensatz abrufen möchten</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul abrufen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Überprüfen des Vorhandenseins eines Datensatzes]

Dieses Aktionsmodul gibt an, ob ein bestimmter Datensatz vorhanden ist.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, den Sie auf die Existenz des Datensatzes überprüfen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul auf Existenz überprüfen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen Datensatz.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, den Sie auf die Existenz des Datensatzes überprüfen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul löschen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Alle Datensätze löschen]

Dieses Aktionsmodul löscht alle Datensätze aus einem bestimmten Datenspeicher.

Sie geben den Datenspeicher an.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, aus dem Sie alle Datensätze löschen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suchdatensätze]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt im Datenspeicher, die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den zu suchenden Datenspeicher aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Legen Sie den Filter für die Suche fest.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sortierung]</p> </td> 
   <td> <p style="font-weight: normal;">Füllen Sie für jedes Feld, nach dem Sie sortieren möchten, die folgenden Felder aus:</p> <p style="font-weight: bold;">[!UICONTROL Schlüssel]</p> <p>Wählen Sie den Spaltennamen aus, nach dem die Ergebnisse sortiert werden sollen.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Wählen Sie aus, ob die Ergebnisse in auf- oder absteigender Reihenfolge sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Maximale Anzahl von Suchergebnissen festlegen [!DNL Workfront Fusion] gibt während eines Ausführungszyklus zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p> Wenn diese Option aktiviert ist, wird die Route, zu der dieses Modul gehört, weiter verarbeitet, auch wenn dieses Modul keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Count Records]

Dieses Aktionsmodul nummeriert die Datensätze in einem Datenspeicher.

Sie geben den Datenspeicher an.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, der die zu zählenden Datensätze enthält.</p> </td> 
  </tr> 
 </tbody> 
</table>
