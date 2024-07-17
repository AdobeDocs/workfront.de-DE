---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Datenspeichermodule
description: Ein [!DNL Adobe Workfront Fusion] Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Ausführungen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# [!UICONTROL Datenspeicher] -Module

Ein [!DNL Adobe Workfront Fusion] -Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Ausführungen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.

Mit den Datenspeichermodulen können Sie Einträge in Ihrem [!DNL Adobe Workfront Fusion] -Datenspeicher hinzufügen, ersetzen, aktualisieren, abrufen, löschen, suchen oder zählen.

Informationen zum Erstellen, Bearbeiten und Fehlerbehebung von Datenspeichern finden Sie unter [Datenspeicher in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Eine Videoeinführung zu Datenspeichern in Workfront Fusion finden Sie unter:

* [Datenspeicher](https://video.tv.adobe.com/v/3427029/){target=_blank}

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

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um die Module [!UICONTROL Datenspeicher] zu verwenden, müssen Sie zunächst einen Datenspeicher erstellen.

Informationen zum Erstellen von Datenspeichern finden Sie unter [Datenspeicher in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Datenspeicher] -Module und ihre Felder

Wenn Sie Datenspeichermodule konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Datenspeicherfelder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Alle [!UICONTROL Datenspeicher] -Module sind Aktionstyp-Module.

* [Hinzufügen/Ersetzen von Datensätzen](#addreplace-a-record)
* [Datensatz aktualisieren](#update-a-record)
* [Datensatz abrufen](#get-a-record)
* [Überprüfen des Vorhandenseins eines Datensatzes](#check-the-existence-of-a-record)
* [Datensatz löschen](#delete-a-record)
* [Alle Datensätze löschen](#delete-all-records)
* [Suchdatensätze](#search-records)
* [Count Records](#count-records)

### [!UICONTROL Datensatz hinzufügen/ersetzen]

Dieses Aktionsmodul fügt einen Datensatz hinzu oder ersetzt ihn.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

>[!NOTE]
>
>Das Modul löst einen Fehler aus, wenn Sie versuchen, den Datensatz hinzuzufügen, der sich bereits im Datenspeicher unter demselben Namen befindet, und die Option [!UICONTROL Vorhandenen Datensatz überschreiben] deaktiviert ist.

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

### [!UICONTROL Prüfen des Vorhandenseins eines Datensatzes]

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

### [!UICONTROL Einen Datensatz löschen]

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
   <td> <p> Legen Sie die maximale Anzahl von Suchergebnissen fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p> Wenn diese Option aktiviert ist, wird die Route, zu der dieses Modul gehört, weiter verarbeitet, auch wenn dieses Modul keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze zählen]

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
