---
title: HubSpot CRM-Module
description: Mit den [!DNL Adobe Workfront Fusion] HubSpot CRM-Modulen können Sie Ereignisse, Datensätze, Kontakte, Interaktionen, Dateien und Formularübermittlungen überwachen oder Datensätze, Kontakte, Interaktionen, Ereignisse oder Dateien in Ihrem [!DNL HubSpot CRM] -Konto erstellen, abrufen, aktualisieren und löschen.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM] Module

Mit den Modulen [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] können Sie Ereignisse, Datensätze, Kontakte, Interaktionen, Dateien und Formularübermittlungen überwachen oder Datensätze, Kontakte, Interaktionen, Ereignisse oder Dateien in Ihrem [!DNL HubSpot CRM]-Konto erstellen, abrufen, aktualisieren und löschen.

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

Um [!DNL HubSpot CRM] -Module zu verwenden, müssen Sie über ein [!DNL HubSpot CRM] -Konto verfügen.

## [!DNL Adobe Workfront Fusion] mit [!DNL HubSpot CRM] verbinden

Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung zu  [!DNL Adobe Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Wählen Sie beim Konfigurieren einer Verbindung den Verbindungstyp **HubSpot CRM** aus. Der HubSpot CRM-Typ (nicht mehr unterstützt) unterstützt vorhandene Verbindungen. Wir empfehlen jedoch nicht, ihn zum Erstellen neuer Verbindungen zu verwenden.

## [!DNL HubSpot CRM] Module und ihre Felder

Wenn Sie [!DNL Hubspot CRM] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Hubspot CRM] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM-Objekte](#crm-objects)
* [Aufzeichnungen (Geschäfte, Kontakte und Unternehmen)](#records-deals-contacts-and-companies)
* [Kontakte](#contacts)
* [Angebote](#deals)
* [Firmen](#companies)
* [Dateien](#files)
* [Tickets](#tickets)
* [API-Aufruf durchführen](#make-an-api-call)

### CRM-Objekte

#### [!UICONTROL Suche nach CRM-Objekten]

Dieses Suchmodul sucht anhand von benutzerdefinierten Eigenschaften oder Abfragen nach CRM-Objekten. Um nach Produkten oder Zeileneinträgen zu suchen, verwenden Sie eine spezielle Verbindung mit einem erforderlichen benutzerdefinierten Bereich.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul in einem Ausführungszyklus zurückgibt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekttyp zur Suche]</td> 
   <td>Wählen Sie den Typ des Hubspot-CRM-Objekts aus, nach dem Sie suchen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die in der Ausgabe des Moduls angezeigt werden sollen. Die verfügbaren Felder hängen vom ausgewählten Objekt ab.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter nach] </td> 
   <td> <p>Auswählen, wie Sie die Suche filtern möchten</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Abfrage]</strong> </p> <p>Abfrage eingeben oder zuordnen</p> </li> 
     <li> <p><strong>[!UICONTROL Eigenschaften]</strong> </p> <p>Geben Sie die Gruppen oder Filter für Ihre Suche ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach</td> 
   <td> <p>Klicken Sie auf , um die Ergebnisse zu sortieren. Wenn Sie die Ergebnisse sortieren möchten, werden die folgenden Felder angezeigt. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Eigenschaftsname]</strong> </p> <p>Wählen Sie die Eigenschaft aus, nach der die Ergebnisse sortiert werden sollen</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Wählen Sie aus, ob die Ergebnisse in auf- oder absteigender Richtung sortiert werden sollen.</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### Aufzeichnungen (Geschäfte, Kontakte und Unternehmen)

* [[!UICONTROL Erstellen eines Datensatzes (veraltet)]](#create-a-record-legacy)
* [[!UICONTROL Datensatz abrufen]](#get-a-record)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL Einen Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Abrufen einer Datensatzeigenschaft]](#get-a-record-property)
* [[!UICONTROL Aufzeichnungen ansehen]](#watch-records)

#### [!UICONTROL Erstellen eines Datensatzes (veraltet)]

Dieses Aktionsmodul erzeugt Kontakte, Unternehmen oder Geschäfte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den zu erstellenden Datensatztyp aus</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaften]</td> 
   <td>Füllen Sie alle Eigenschaften aus, die Sie für den Datensatz festlegen möchten. Die verfügbaren Felder hängen vom zu erstellenden Datensatztyp ab.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz abrufen]

Dieses Aktionsmodul ruft Details zu einem Kontakt, einem Unternehmen oder einem Geschäft ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus.</p> 
    <ul> 
     <li>[!UICONTROL Kontakt]</li> 
     <li>[!UICONTROL Company] </li> 
     <li>[!UICONTROL Deal]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchtyp]</td> 
   <td>Wenn Sie einen Kontakt erhalten, wählen Sie aus, ob Sie ihn anhand der Kennung oder der E-Mail-Adresse identifizieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Kontakts, Unternehmens oder Geschäfts ein, den Sie abrufen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Geben Sie die E-Mail-Adresse des Kontakts ein, dessen Details Sie abrufen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen Kontakt, ein Unternehmen oder einen Deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchtyp]</td> 
   <td> <p>Wenn Sie einen Kontakt erhalten, wählen Sie aus, wie Sie den Datensatz identifizieren möchten:</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL Email]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Kontakts, Unternehmens oder der Transaktion ein, den/die Sie aktualisieren möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Geben Sie die E-Mail-Adresse des Kontakts ein, dessen Details Sie aktualisieren möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaften]</td> 
   <td>Füllen Sie alle Eigenschaften aus, die Sie für den Datensatz festlegen möchten. Die verfügbaren Felder hängen vom zu erstellenden Datensatztyp ab.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Datensatz löschen]

Dieses Aktionsmodul löscht einen Kontakt, ein Unternehmen oder eine Transaktion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Kontakts, Unternehmens oder der Transaktion ein, den/die Sie löschen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen einer Datensatzeigenschaft]

Dieses Aktionsmodul ruft Metadaten für eine bestimmte Datensatzeigenschaft anhand seines (internen) Namens ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes mit der Eigenschaft aus, für die Sie Metadaten abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaftsname]</td> 
   <td>Wählen Sie die Eigenschaft aus, für die Sie Metadaten abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Option ID]</td> 
   <td> <p> Einige Eigenschaften verfügen über eine Reihe verfügbarer Optionen, die ein Benutzer als Eigenschaftswert auswählen kann. Geben Sie die ID der Option ein, die den Eigenschaftswert darstellt, den Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aufzeichnungen ansehen]

Dieses Trigger-Modul startet ein Szenario, in dem ein Kontakt, ein Unternehmen oder eine Transaktion innerhalb der letzten 30 Tage geändert oder erstellt wurde. Die Ausgabe ist auf 10.000 Datensätze beschränkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes mit der Eigenschaft aus, die Sie sehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suche]</td> 
   <td>Wählen Sie aus, ob Sie sich kürzlich geänderte oder kürzlich erstellte Datensätze ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kontakte

* [[!UICONTROL Einen Kontakt erstellen/aktualisieren (veraltet)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Erstellen/Aktualisieren einer Kontaktgruppe]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Kontakte zu einer Liste hinzufügen]](#add-contacts-to-a-list)
* [[!UICONTROL Einen Kontakt aus einer Liste entfernen]](#remove-a-contact-from-a-list)
* [[!UICONTROL Kontakte zusammenführen]](#merge-contacts)
* [[!UICONTROL Suche nach Kontakten]](#search-for-contacts)
* [[!UICONTROL Listenkontakte]](#list-contacts)
* [[!UICONTROL Listenkontakte eines Unternehmens]](#list-contacts-of-a-company)

#### [!UICONTROL Einen Kontakt erstellen/aktualisieren (veraltet)]

Erstellt einen Kontakt, wenn er noch nicht in einem Portal vorhanden ist, oder aktualisiert ihn mit den neuesten Eigenschaftswerten, falls er in einem Portal vorhanden ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaften]</td> 
   <td>Füllen Sie alle Eigenschaften aus, die Sie für den Kontakt festlegen oder aktualisieren möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen/Aktualisieren einer Kontaktgruppe]

Erstellt eine Gruppe von Kontakten oder aktualisiert diese, falls sie bereits existieren. Die beste Leistung ist, wenn die Batch-Größe auf 100 Kontakte oder weniger beschränkt ist. Änderungen, die über diesen Endpunkt vorgenommen werden, werden asynchron verarbeitet, sodass es mehrere Minuten dauern kann, bis Änderungen auf Kontaktdatensätze angewendet werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Batch von Kontakten zur Erstellung/Aktualisierung] </td> 
   <td> <p>Fügen Sie den Kontaktstapel hinzu.</p> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong> , um einen neuen Kontakt hinzuzufügen. Geben Sie im sich öffnenden Fenster die folgenden Informationen ein oder ordnen Sie sie zu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Suchtyp]</strong> </p> <p>Wählen Sie aus, wie Sie den Kontakt identifizieren möchten:</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>Geben Sie die Kennung des Kontakts ein, den Sie erstellen oder aktualisieren möchten. </p> </li> 
       <li> <p>[!UICONTROL Email]</p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein, den Sie erstellen oder aktualisieren möchten. </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Eigenschaften]</strong> </p> <p>Füllen Sie alle Eigenschaften aus, die Sie für den Kontakt einrichten oder aktualisieren möchten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kontakte zu einer Liste hinzufügen]

Dieses Modul fügt Kontaktdatensätze, die bereits im System erstellt wurden, einer Kontaktliste hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID] </td> 
   <td>Wählen Sie die Kennung der Liste aus, der Sie den Kontakt hinzufügen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IDs/E-Mails] </td> 
   <td> <p>Wählen Sie aus, wie Sie die Kontakte identifizieren möchten, die Sie der Liste hinzufügen möchten:</p> 
    <ul> 
     <li> <p>[!UICONTROL IDs]</p> <p>Fügen Sie die Kennungen der Kontakte hinzu, die Sie der Liste hinzufügen möchten.</p> </li> 
     <li> <p>[!UICONTROL E-Mails]</p> <p>Fügen Sie die E-Mail-Adressen der Kontakte hinzu, die Sie der Liste hinzufügen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kontakt aus einer Liste entfernen]

Entfernt einen Kontakt aus einer Kontaktliste.

>[!NOTE]
>
>Sie können Kontakte nicht manuell aus einer dynamischen Liste entfernen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID] </td> 
   <td>Wählen Sie die Kennung der Liste aus, aus der Sie den Kontakt entfernen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kontakt-ID] </td> 
   <td>Geben Sie die Kennung des Kontakts ein, den Sie aus der Liste entfernen möchten. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kontakte zusammenführen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>Geben Sie die Kennung eines der Kontakte ein, die Sie zusammenführen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>Geben Sie die Kennung des anderen Kontakts ein, den Sie zusammenführen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suche nach Kontakten]

Ruft eine Liste von Kontakten mithilfe der Suchabfrage ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfrage]</td> 
   <td>Geben Sie die Suchabfrage ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Geben Sie die maximale Anzahl von Kontakten ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben soll. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listenkontakte]

Gibt alle Kontakte zurück, die im Portal erstellt wurden. Die Ausgabe ist auf 5000 Kontakte beschränkt. Um vorherige oder nächste Kontakte aufzulisten, können Sie den Parameter [!UICONTROL advanced] verwenden, um die Liste zu versetzen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Kontakten [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die in der Ausgabe des Moduls angezeigt werden sollen. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Listenkontakte eines Unternehmens]

Ruft eine Liste der Kontakte im Unternehmen ab. Die Ausgabe ist auf 5000 Kontakte beschränkt. Um vorherige oder nächste Kontakte aufzulisten, können Sie den Parameter [!UICONTROL advanced] verwenden, um die Liste zu versetzen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Unternehmens ein, dessen Kontakte Sie auflisten möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Kontakten [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Beobachten von Kontakten, die zu einer Liste hinzugefügt wurden]

Dieses Trigger-Modul startet ein Szenario, wenn ein neuer Kontakt zu einer Liste hinzugefügt wird. Dies ist nur für Benutzer mit einem gebührenpflichtigen Marketingkonto verfügbar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID]</td> 
   <td>Geben Sie die Kennung der Liste ein oder ordnen Sie sie zu, die die gewünschten Kontakte enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Angebote

* [[!UICONTROL List Deal/Ticket Pipelines]](#list-dealticket-pipelines)
* [[!UICONTROL Abrufen der CRM-Pipeline eines Deals]](#get-a-deals-crm-pipeline)

#### [!UICONTROL List Deal/Ticket Pipelines]

Gibt alle Deal- und Ticket-Pipelines für ein bestimmtes Portal zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekttyp] </td> 
   <td>Wählen Sie aus, ob Sie Angebote oder Tickets auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen der CRM-Pipeline eines Deals]

Gibt eine bestimmte Deal-Pipeline zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pipeline-ID] </td> 
   <td>Geben Sie die Kennung der Pipeline ein oder ordnen Sie sie zu, für die Sie Details abrufen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Staging-ID] </td> 
   <td>Geben Sie die ID der Phase ein oder ordnen Sie sie zu, für die Sie Details abrufen möchten. </td> 
  </tr> 
 </tbody> 
</table>

### Firmen

#### [!UICONTROL Suche nach Unternehmen nach Domäne]

Ruft eine Liste von Unternehmen ab, die auf einer exakten Übereinstimmung mit der Domain-Eigenschaft basieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Domain] </td> 
   <td>Geben Sie die Domäne der Unternehmen ein, nach denen Sie suchen möchten, z. B. <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Unternehmen [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die in der Ausgabe des Moduls angezeigt werden sollen. </td> 
  </tr> 
 </tbody> 
</table>

### Dateien

* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Ordner löschen]](#delete-a-folder)
* [[!UICONTROL Verschieben einer Datei]](#move-a-file)

#### [!UICONTROL Erstellen eines Ordners]

Dieses Modul erstellt einen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordnername] </td> 
   <td>Geben Sie einen Namen für den neuen Ordner ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID] </td> 
   <td>Wählen Sie die Kennung des übergeordneten Ordners für den Ordner aus, den Sie erstellen. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner löschen]

Markiert einen Ordner als gelöscht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, den Sie löschen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei]

Verschiebt eine Datei in einen anderen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID] </td> 
   <td>Geben Sie die Kennung der Datei ein, die Sie verschieben möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td>Wählen Sie die Kennung des Ordners aus, in den Sie die Datei verschieben möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für die verschobene Datei ein.</td> 
  </tr> 
 </tbody> 
</table>

### Tickets

#### [!UICONTROL Ticket löschen]

Löscht ein vorhandenes Ticket anhand seiner Kennung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Tickets ein, das Sie löschen möchten. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API-Aufruf durchführen]

Ermöglicht die Ausführung eines benutzerdefinierten API-Aufrufs.

>[!NOTE]
>
>Die folgenden Endpunkte wurden am 31. August 2023 in der HubSpot-API nicht mehr unterstützt und können nicht mehr in Fusion-Modulen verwendet werden.
>
>* Inhaltsereignisse auflisten
>* Social-Ereignisse auflisten
>* Kalenderaufgabenereignisse auflisten
>* Alle Kalenderereignisse auflisten
>* Kalenderaufgabe erstellen
>* Kalenderaufgabe nach ID abrufen
>* Kalenderaufgabe aktualisieren
>* Löschen einer Kalenderaufgabe

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu https://api.hubapi.com/ ein. Beispiel: /contact/v1/lists/all/contact/all</p> <p>Die Liste der verfügbaren Endpunkte finden Sie in der <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API-Dokumentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die zu verwendende HTTP-Methode aus:</p> <p>[!UICONTROL GET]</p> <p>, um Informationen für einen Eintrag abzurufen.</p> <p>[!UICONTROL POST]</p> <p>, um einen neuen Eintrag zu erstellen.</p> <p>[!UICONTROL PUT]</p> <p>, um einen vorhandenen Eintrag zu aktualisieren/zu ersetzen.</p> <p>[!UICONTROL PATCH]</p> <p>, um eine partielle Eintragsaktualisierung vorzunehmen.</p> <p>[!UICONTROL DELETE]</p> <p>, um einen Eintrag zu löschen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p> Geben Sie die gewünschten Anforderungsheader ein. Sie müssen keine Autorisierungs-Header hinzufügen. Das haben wir bereits für Sie getan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu. Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt alle Kontakte in Ihrem [!DNL HubSpot] -Konto zurück:
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**Methode**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>Übereinstimmungen der Suche finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL Hauptteil] > [!UICONTROL Kontakte].
>
>In unserem Beispiel wurden drei Kontakte zurückgegeben:
>
>![](assets/hubspot-api-output.png)

## Neue Anwendung erstellen

1. Melden Sie sich bei Ihrem [!DNL HubSpot] -Entwicklerkonto an.
1. Wählen Sie die Option **[!UICONTROL App erstellen]** aus.
1. Geben Sie den App-Namen ein und [!UICONTROL Speichern] Sie das Dialogfeld.
1. Wählen Sie die Bereiche aus, die Sie für Ihren Webhook benötigen.

   Fügen Sie beispielsweise Kontaktbereiche hinzu, um das Modul auszulösen, wenn ein neuer Kontakt erstellt oder gelöscht wird.

   Der [!UICONTROL Kontaktbereich] ist alles, was Sie benötigen, um Webhooks für Kontakte, Angebote und Unternehmensereignisse zu erhalten.

   >[!IMPORTANT]
   >
   >Füllen Sie nicht das Feld [!UICONTROL Umleitungs-URL] aus.
