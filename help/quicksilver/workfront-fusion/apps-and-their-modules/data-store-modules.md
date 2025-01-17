---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Datenspeichermodule
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 0%

---

# [!UICONTROL Datenspeicher] Module

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Datenspeichermodule](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/data-store-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Ein [!DNL Adobe Workfront Fusion] Datenspeicher, ähnlich einer Datenbank oder einer einfachen Tabelle, kann Daten aus Szenarien speichern und ermöglicht so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenarioausführungen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.

Mit den Datenspeichermodulen können Sie Datensätze in Ihrem [!DNL Adobe Workfront Fusion] Datenspeicher hinzufügen, ersetzen, aktualisieren, abrufen, löschen, suchen oder zählen.

Informationen zum Erstellen, Bearbeiten und Fehlerbehebung von Datenspeichern finden Sie unter [Datenspeicher in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

Eine Videoeinführung zu Datenspeichern in Workfront Fusion finden Sie unter:

* [Datenspeicher](https://video.tv.adobe.com/v/3427029/){target=_blank}

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!UICONTROL Datenspeicher]-Module verwenden zu können, müssen Sie zunächst einen Datenspeicher erstellen.

Informationen zum Erstellen von Datenspeichern finden Sie unter [Datenspeicher in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Datenspeicher]-Module und ihre Felder

Beim Konfigurieren von Datenspeichermodulen zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere Datenspeicherfelder angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Alle [!UICONTROL Datenspeicher]-Module sind Module vom Typ Aktion .

* [Datensatz hinzufügen/ersetzen](#addreplace-a-record)
* [Aktualisieren eines Datensatzes](#update-a-record)
* [Datensatz abrufen](#get-a-record)
* [Überprüfen, ob ein Datensatz vorhanden ist](#check-the-existence-of-a-record)
* [Löschen eines Datensatzes](#delete-a-record)
* [Alle Datensätze löschen](#delete-all-records)
* [Datensätze suchen](#search-records)
* [Datensätze zählen](#count-records)

### [!UICONTROL Datensatz hinzufügen/ersetzen]

Dieses Aktionsmodul fügt einen Datensatz hinzu oder ersetzt ihn.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

>[!NOTE]
>
>Das Modul gibt einen Fehler aus, wenn Sie versuchen, den Datensatz hinzuzufügen, der sich bereits unter demselben Namen im Datenspeicher befindet, und die Option [!UICONTROL Vorhandenen Datensatz überschreiben] deaktiviert ist.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus, in dem Sie einen Datensatz erstellen möchten, oder fügen Sie ihn hinzu. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul hinzufügen oder ersetzen soll. Der Schlüssel kann später zum Abrufen des Datensatzes verwendet werden. Wenn Sie dieses Feld leer lassen, wird automatisch ein Schlüssel generiert.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Vorhandenen Datensatz überschreiben] </td> 
   <td> <p>Aktivieren Sie diese Option, um den Datensatz zu überschreiben. Der Datensatz, den Sie überschreiben möchten, muss im obigen Feld Schlüssel angegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Eintrag] </td> 
   <td> <p>Geben Sie die gewünschten Werte in die Felder des Datensatzes ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aktualisieren eines Datensatzes]

Dieses Aktionsmodul aktualisiert einen Datensatz.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus, in dem Sie einen Datensatz erstellen möchten, oder fügen Sie ihn hinzu. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul aktualisieren soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fehlenden Eintrag einfügen] </td> 
   <td> <p>Aktivieren Sie diese Option, um einen neuen Datensatz zu erstellen, wenn der Datensatz mit dem angegebenen Schlüssel noch nicht vorhanden ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Eintrag]</td> 
   <td> <p> Geben Sie die gewünschten Werte in die Felder des Datensatzes ein, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz abrufen]

Dieses Aktionsmodul ruft einen Datensatz ab.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den Datenspeicher aus, aus dem Sie einen Datensatz abrufen möchten</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, den das Modul abrufen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Überprüfen Sie, ob ein Datensatz vorhanden ist]

Dieses Aktionsmodul gibt an, ob ein bestimmter Datensatz vorhanden ist.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, den Sie auf das Vorhandensein des Datensatzes überprüfen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Schlüssel] </td> 
   <td> <p>Geben Sie den eindeutigen Schlüssel des Datensatzes ein, auf dessen Existenz das Modul prüfen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Löschen eines Datensatzes]

Dieses Aktionsmodul löscht einen Datensatz.

Sie geben den Datenspeicher und den Schlüssel des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, den Sie auf das Vorhandensein des Datensatzes überprüfen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Schlüssel] </td> 
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

### [!UICONTROL Datensätze suchen]

Dieses Suchmodul sucht in einem -Objekt im Datenspeicher nach Datensätzen, die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher]</td> 
   <td> <p> Wählen Sie den zu durchsuchenden Datenspeicher aus.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL filter]</p> </td> 
   <td> <p>Filter für die Suche festlegen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL sort]</p> </td> 
   <td> <p style="font-weight: normal;">Füllen Sie für jedes Feld, nach dem Sie sortieren möchten, die folgenden Felder aus:</p> <p style="font-weight: bold;">[!UICONTROL-Schlüssel]</p> <p>Wählen Sie den Spaltennamen aus, nach dem die Ergebnisse sortiert werden sollen.</p> <p style="font-weight: bold;">[!UICONTROL-Reihenfolge]</p> <p>Wählen Sie aus, ob die Ergebnisse in auf- oder absteigender Reihenfolge sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Suchergebnissen fest, [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p> Wenn diese Option aktiviert ist, wird die Route, zu der dieses Modul gehört, auch dann weiter verarbeitet, wenn dieses Modul keine Ergebnisse zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze zählen]

Dieses Aktionsmodul nummeriert die Datensätze in einem Datenspeicher.

Sie geben den Datenspeicher an.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Datenspeicher] </td> 
   <td> <p>Wählen Sie den Datenspeicher aus, der die Datensätze enthält, die gezählt werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>
