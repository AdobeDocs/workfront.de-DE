---
title: HubSpot CRM-Module
description: Mit den [!DNL Adobe Workfront Fusion] HubSpot CRM-Modulen können Sie Ereignisse, Datensätze, Kontakte, Interaktionen, Dateien und Formularübermittlungen überwachen oder Datensätze, Kontakte, Interaktionen, Ereignisse oder Dateien in Ihrem [!DNL HubSpot CRM] -Konto erstellen, abrufen, aktualisieren und löschen.
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: d550ba76a5a6c1d241d1dc73e63e49ef4c22a40d
workflow-type: tm+mt
source-wordcount: '6394'
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
* [Interaktionen](#engagements)
* [Ereignisse und Benachrichtigungen](#events-and-notifications)
* [Dateien](#files)
* [Aufgaben](#tasks)
* [Benutzende](#users)
* [Tickets](#tickets)
* [Formulare](#forms)
* [Social Media (Broadcast)](#social-media-broadcast)
* [Blog-Beiträge](#blog-posts)
  <!--* [Workflows]-->
* [Abonnements](#subscriptions)
  <!--* [Associations](#associations)-->
* [Sonstige](#other)

+++**CRM-Objekte**

### CRM-Objekte

* [Suche nach CRM-Objekten](#search-for-crm-objects)
* [CRM-Objekte überwachen](#watch-crm-objects)

#### [!UICONTROL Suche nach CRM-Objekten]

Dieses Suchmodul sucht anhand von benutzerdefinierten Eigenschaften oder Abfragen nach CRM-Objekten. Um nach Produkten oder Zeileneinträgen zu suchen, verwenden Sie eine spezielle Verbindung mit einem erforderlichen benutzerdefinierten Bereich.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
  </tr> 
   <tr> 
    <td role="rowheader">Versatz starten</td> 
    <td>Geben Sie die ID des ersten Elements ein, für das Sie Details abrufen möchten, oder ordnen Sie sie zu. Dieses Modul gibt nur bis zu 5000 Ergebnisse gleichzeitig zurück. Wenn Sie einen Startversatz festlegen, können Sie andere Elemente als die ersten 5000 abrufen. Wenn der Startversatz 5000 ist, gibt das Modul die Elemente 5000-9999 zurück.</td> 
   </tr>
 </tbody> 
</table>

#### CRM-Objekte überwachen

Dieses Trigger-Modul startet ein Szenario, wenn ein CRM-Objekt erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul in einem Ausführungszyklus zurückgibt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL zu suchender Objekttyp]</td> 
   <td> <p>Wählen Sie den Objekttyp aus, nach dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die Sie in die Ausgabe für dieses Modul aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erstellt/aktualisiert]</td> 
   <td>Wählen Sie aus, ob Sie erstellte (neue) oder aktualisierte (geänderte) Objekte ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter nach]</td> 
   <td>Sie können einen Filter hinzufügen, um sicherzustellen, dass das Szenario nur startet, wenn bestimmte Bedingungen erfüllt sind.<ul><li><b>Abfrage</b><p>Geben Sie die Abfrage ein, nach der Sie filtern möchten.</li><li><b>Eigenschaften</b><p>Klicken Sie für jede Eigenschaft, die Sie zum Filtern der Ergebnisse verwenden möchten, auf "<b>Element hinzufügen</b>"und geben Sie den Eigenschaftsnamen, den Operator und den Eigenschaftswert ein.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Aufzeichnungen (Geschäfte, Kontakte und Unternehmen)**

### Aufzeichnungen (Geschäfte, Kontakte und Unternehmen)

* [Datensatz erstellen](#create-a-record)
* [[!UICONTROL Erstellen eines Datensatzes (veraltet)]](#create-a-record-legacy)
* [[!UICONTROL Einen Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Datensatz abrufen]](#get-a-record)
* [[!UICONTROL Abrufen einer Datensatzeigenschaft]](#get-a-record-property)
* [Listen-Datensätze](#list-records)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL Aufzeichnungen ansehen]](#watch-records)

#### Datensatz erstellen

Dieses Aktionsmodul erstellt einen Kontakt, ein Unternehmen oder einen Deal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaftsgruppen]</td> 
   <td>Wählen Sie für jede Eigenschaft, die Sie beim Erstellen des Datensatzes hinzufügen möchten, die Gruppe aus, in der sich die Eigenschaft befindet. Die Eigenschaftsgruppe wird geöffnet und Sie können dann den Wert für die Eigenschaften ausfüllen. Die verfügbaren Eigenschaftsgruppen und Eigenschaften hängen vom Typ des Datensatzes ab, den Sie erstellen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Datensatzes (veraltet)]

Dieses Aktionsmodul erzeugt Kontakte, Unternehmen oder Geschäfte.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Datensatz abrufen]

Dieses Aktionsmodul ruft Details zu einem Kontakt, einem Unternehmen oder einem Geschäft ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Abrufen einer Datensatzeigenschaft]

Dieses Aktionsmodul ruft Metadaten für eine bestimmte Datensatzeigenschaft anhand seines (internen) Namens ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### Listen-Datensätze

Dieses Suchmodul gibt eine Liste von Kontakten, Unternehmen oder Angeboten zurück. Die Produktion ist auf 5000 Kontakte, 12.500 Unternehmen oder 12.500 Geschäfte beschränkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie zurückgeben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output Properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die Sie in die Ausgabe für dieses Modul aufnehmen möchten.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Aufzeichnungen ansehen]

Dieses Trigger-Modul startet ein Szenario, in dem ein Kontakt, ein Unternehmen oder eine Transaktion innerhalb der letzten 30 Tage geändert oder erstellt wurde. Die Ausgabe ist auf 10.000 Datensätze beschränkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

+++

+++**Contacts**

### Kontakte

* [[!UICONTROL Kontakte zu einer Liste hinzufügen]](#add-contacts-to-a-list)
* [Erstellen/Aktualisieren eines Kontakts](#createupdate-a-contact)
* [[!UICONTROL Einen Kontakt erstellen/aktualisieren (veraltet)]](#createupdate-a-contact-legacy)
* [[!UICONTROL Erstellen/Aktualisieren einer Kontaktgruppe]](#createupdate-a-group-of-contacts)
* [[!UICONTROL Listenkontakte]](#list-contacts)
* [[!UICONTROL Listenkontakte eines Unternehmens]](#list-contacts-of-a-company)
* [[!UICONTROL Kontakte zusammenführen]](#merge-contacts)
* [[!UICONTROL Einen Kontakt aus einer Liste entfernen]](#remove-a-contact-from-a-list)
* [[!UICONTROL Suche nach Kontakten]](#search-for-contacts)
* [Zu einer Liste hinzugefügte Überwachungskontakte](#watch-contacts-added-to-a-list)

#### [!UICONTROL Kontakte zu einer Liste hinzufügen]

Dieses Modul fügt Kontaktdatensätze, die bereits im System erstellt wurden, einer Kontaktliste hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### Erstellen/Aktualisieren eines Kontakts

Dieses Aktionsmodul erstellt einen Kontakt, wenn er nicht in einem Portal vorhanden ist. Wenn der Kontakt im Portal vorhanden ist, aktualisiert dieses Modul ihn mit den bereitgestellten Werten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eigenschaftsgruppen]</td> 
   <td>Wählen Sie für jede Eigenschaft, die Sie beim Erstellen des Kontakts hinzufügen möchten, die Gruppe aus, in der sich die Eigenschaft befindet. Die Eigenschaftsgruppe wird geöffnet und Sie können dann die Werte für die Eigenschaften ausfüllen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kontakt erstellen/aktualisieren (veraltet)]

Erstellt einen Kontakt, wenn er noch nicht in einem Portal vorhanden ist, oder aktualisiert ihn mit den neuesten Eigenschaftswerten, falls er in einem Portal vorhanden ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Listenkontakte]

Gibt alle Kontakte zurück, die im Portal erstellt wurden. Die Ausgabe ist auf 5000 Kontakte beschränkt. Um vorherige oder nächste Kontakte aufzulisten, können Sie den Parameter [!UICONTROL advanced] verwenden, um die Liste zu versetzen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Kontakten [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output properties]</td> 
   <td>Wählen Sie die Eigenschaften aus, die in der Ausgabe des Moduls angezeigt werden sollen. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">Kontakt-ID [Startversatz] </td> 
    <td>Geben Sie die ID des Benutzers ein oder ordnen Sie sie zu, der die Liste starten soll. Wenn Sie beispielsweise die Kontakt-ID als Kennung des 101. Kontakts festlegen, kann das Modul die Kontakte 101-5100 anstatt 1-5000 auflisten. </td> 
   </tr>
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Unternehmens ein, dessen Kontakte Sie auflisten möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Kontakten [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> 
   <tr> 
    <td role="rowheader">Kontakt-ID [Startversatz] </td> 
    <td>Geben Sie die ID des Benutzers ein oder ordnen Sie sie zu, der die Liste starten soll. Wenn Sie beispielsweise die Kontakt-ID als Kennung des 101. Kontakts festlegen, kann das Modul die Kontakte 101-5100 anstatt 1-5000 auflisten. </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL Kontakte zusammenführen]

Dieses Aktionsmodul führt Kontakte zusammen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Suche nach Kontakten]

Ruft eine Liste von Kontakten mithilfe der Suchabfrage ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL Beobachten von Kontakten, die zu einer Liste hinzugefügt wurden]

Dieses Trigger-Modul startet ein Szenario, wenn ein neuer Kontakt zu einer Liste hinzugefügt wird. Dies ist nur für Benutzer mit einem gebührenpflichtigen Marketingkonto verfügbar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

+++

+++**Angebote**

### Angebote

* [[!UICONTROL Abrufen der CRM-Pipeline eines Deals]](#get-a-deals-crm-pipeline)
* [[!UICONTROL List Deal/Ticket Pipelines]](#list-dealticket-pipelines)

#### [!UICONTROL Abrufen der CRM-Pipeline eines Deals]

Gibt eine bestimmte Deal-Pipeline zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### [!UICONTROL List Deal/Ticket Pipelines]

Gibt alle Deal- und Ticket-Pipelines für ein bestimmtes Portal zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekttyp] </td> 
   <td>Wählen Sie aus, ob Sie Angebote oder Tickets auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Unternehmen**

### Firmen

#### [!UICONTROL Suche nach Unternehmen nach Domäne]

Ruft eine Liste von Unternehmen ab, die auf einer exakten Übereinstimmung mit der Domain-Eigenschaft basieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

+++

+++**Interaktionen**

### Interaktionen

* [Interaktion mit einem CRM-Objekt verknüpfen](#associate-an-engagement-with-a-crm-object)
* [Interaktion erstellen](#create-an-engagement)
* [Interaktion löschen](#delete-an-engagement)
* [Überwachungsinteraktionen](#watch-engagements)

#### Interaktion mit einem CRM-Objekt verknüpfen

Dieses Aktionsmodul verknüpft eine Interaktion mit einem Kontakt, einem Unternehmen oder einem Geschäft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td>Wählen Sie den Typ des CRM-Datensatzes aus, mit dem Sie eine Interaktion verbinden möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Interaktions-ID]</td> 
  <td>Geben Sie die Kennung der Interaktion ein, die Sie mit dem Objekt verknüpfen möchten, oder ordnen Sie sie zu.</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatz-ID]</td> 
  <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie sie zu.</td> 
   </tr> 
 </tbody> 
</table>

#### Interaktion erstellen

Dieses Aktionsmodul erstellt eine Interaktion (z. B. eine Notiz, eine Aufgabe oder eine Aktivität) mit einem CRM-Objekt in HubSpot. Interaktionen sind Interaktionen mit Kontakten, die im CRM protokolliert werden sollen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ist aktiv?]</td> 
   <td>Aktivieren Sie diese Option, wenn die neue Interaktion bei ihrer Erstellung aktiv sein soll. Eine Interaktion muss aktiv sein, damit sie in der Timeline angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
  <td>Wählen Sie den Interaktionstyp aus, den Sie erstellen möchten.
  <ul>
  <li><b>E-Mail</b><p></p>Fahren Sie mit <a href="#email-metadata" class="MCXref xref" >E-Mail-Metadaten</a> fort.</p></li>
  <li><b>Aufruf</b><p>Fahren Sie mit <a href="#call-metadata" class="MCXref xref" >Aufrufen von Metadaten</a> fort.</p></li>
  <li><b>Besprechung</b><p>Fahren Sie mit "<a href="#meeting-fields" class="MCXref xref" >Meeting fields</a>"fort.</p></li>
  <li><b>Aufgabe</b><p>Fahren Sie mit <a href="#task-fields" class="MCXref xref" >Aufgabenfeldern</a> fort.</p></li>
  <li><b>Notiz</b><p>Geben Sie im Feld Hauptteil den Text der Notiz ein.</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Zeitstempel</td> 
   <td>Geben Sie einen Zeitstempel für die Interaktion ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Inhaber-ID</td> 
   <td>Geben Sie die Eigentümerkennung der Person ein, der die Interaktion zugewiesen wird, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>Geben Sie eine ID für die Interaktion ein oder ordnen Sie sie zu, die über Objekttypen hinweg verwendet werden kann.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Portal-ID</td> 
   <td>Geben Sie die Kennung des Portals ein oder ordnen Sie sie zu. Dies ist nützlich, wenn Ihr Unternehmen über mehrere Portale verfügt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assoziierte Kontakte</td> 
   <td>Klicken Sie für jeden Kontakt, mit dem Sie diese Interaktion verbinden möchten, auf <b>Element hinzufügen</b> und geben Sie die Kontakt-ID ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assoziierte Unternehmen</td> 
   <td>Klicken Sie für jedes Unternehmen, mit dem Sie diese Interaktion verknüpfen möchten, auf <b>Element hinzufügen</b> und geben Sie die Firmen-ID ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugehörige Angebote</td> 
   <td>Klicken Sie für jede Transaktion, mit der Sie diese Interaktion verknüpfen möchten, auf <b>Element hinzufügen</b> und geben Sie die Angebots-ID ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugehörige Tickets</td> 
   <td>Klicken Sie für jedes Ticket, mit dem Sie diese Interaktion verknüpfen möchten, auf <b>Element hinzufügen</b> und geben Sie die Ticket-ID ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Anhänge</td> 
   <td>Klicken Sie für jeden Anhang, mit dem Sie diese Interaktion verknüpfen möchten, auf <b>Element hinzufügen</b> und geben Sie die Datei-ID der Datei ein, die Sie anhängen möchten.</td> 
  </tr> 
 </tbody> 
</table>

##### E-Mail-Metadaten

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Von &gt; E-Mail]</p> </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorname]</td> 
   <td>Geben Sie den Vornamen der Person ein, von der die E-Mail gesendet wird, oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachname]</td> 
  <td>Geben Sie den Nachnamen der Person ein, von der die E-Mail gesendet wird, oder ordnen Sie ihn zu.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Bis</td> 
   <td>Klicken Sie für jede E-Mail-Adresse, an die Sie die E-Mail senden möchten, auf <b>Element hinzufügen</b> und geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cc</td> 
   <td>Klicken Sie für jede E-Mail-Adresse, an die die E-Mail gesendet werden soll, auf <b>Element hinzufügen</b> und geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bcc</td> 
   <td>Klicken Sie für jede E-Mail-Adresse, an die die E-Mail gebunden werden soll, auf <b>Element hinzufügen</b> und geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Betreff</td> 
   <td>Text des E-Mail-Betreffs eingeben oder zuordnen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>Um eine E-Mail im HTML-Format zu senden, geben Sie den Text der E-Mail ein oder ordnen Sie ihn zu, einschließlich HTML-Tags.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td>Um eine reine Text-E-Mail zu senden, geben Sie den Text des Textkörpers der E-Mail ein oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>

##### Aufrufmetadaten

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL To Number]</p> </td> 
   <td> <p>Geben Sie die Telefonnummer ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Von der Nummer]</td> 
   <td>Geben Sie die Telefonnummer ein oder ordnen Sie sie zu, von der aus der Anruf erfolgt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
  <td>Wählen Sie den Status des Aufrufs aus.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td>Geben Sie die Details oder Notizen für den Aufruf ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Externe ID</td> 
   <td>Dieses Feld stellt die interne ID eines Aufrufs dar, der in HubSpot erfolgt ist. Dazu sind keine Maßnahmen erforderlich.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Dauer</td> 
   <td>Geben Sie die Länge des Aufrufs in Millisekunden ein oder ordnen Sie sie zu</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Externe Konto-ID</td> 
   <td>Dieses Feld stellt die interne Konto-ID eines Aufrufs dar, der in HubSpot erfolgt ist. Dazu sind keine Maßnahmen erforderlich.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Recording URL</td> 
   <td>Geben Sie die URL der Aufzeichnungsdatei ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

##### Konferenzfelder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Titel]</p> </td> 
   <td> <p>Geben Sie den Titel oder Betreff der Sitzung ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Text der Sitzungsbeschreibung oder der Details ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startzeit]</td> 
  <td>Geben Sie die Startzeit des Meetings als UNIX-Zeitstempel ein oder ordnen Sie sie zu.
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">Endzeit</td> 
   <td>Geben Sie die Endzeit des Meetings als UNIX-Zeitstempel ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

##### Aufgabenfelder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Betreff]</p> </td> 
   <td> <p>Geben Sie den Titel oder Betreff der Aufgabe ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Text der Aufgabenbeschreibung oder der Aufgabendetails ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status</td> 
   <td>Wählen Sie den Status der Aufgabe aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL für Objekttyp]</td> 
  <td>Geben Sie entweder <code>CONTACT</code> oder <code>COMPANY</code> ein.
  </td> 
   </tr> 
 </tbody> 
</table>

#### Interaktion löschen

Dieses Aktionsmodul löscht eine Interaktion anhand ihrer Kennung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Geben Sie die Kennung der Interaktion ein, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Überwachungsinteraktionen

Dieses Trigger-Modul startet ein Szenario, wenn eine neue Interaktion in einem Portal erstellt wird. Dieses Modul gibt nur Datensätze zurück, die in den letzten 30 Tagen oder in den 10.000 zuletzt erstellten Datensätzen erstellt wurden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Die maximale Anzahl von Unternehmen [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seit]</td> 
   <td>Geben Sie das früheste Datum ein oder ordnen Sie es zu, für das Sie Ereignisse anzeigen möchten. Verwenden Sie das Format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Ereignisse und Benachrichtigungen**

### Ereignisse und Benachrichtigungen

* [Erstellen/Aktualisieren eines Timeline-Ereignisses](#create--update-a-timeline-event)
* [Ereignistypen in der Timeline auflisten](#list-timeline-event-types)
* [Kalenderereignisse ansehen](#watch-calendar-events)
* [Überwachungsbenachrichtigungen](#watch-notifications)

#### Erstellen/Aktualisieren eines Timeline-Ereignisses

Dieses Aktionsmodul erstellt oder aktualisiert ein Timeline-Ereignis. Dieses Modul kann nur mit einer Entwicklerverbindung verwendet werden, die Ihre Benutzer-ID, Ihren HubSpot API-Schlüssel, die Client-ID und den Client Secret umfasst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anwendungs-ID]</td> 
   <td>Geben Sie die Kennung der Anwendung ein, zu der dieses Ereignis gehört, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td>Geben Sie eine ID für dieses Ereignis ein oder ordnen Sie sie zu. Ereignis-IDs werden vom System nicht generiert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignistyp-ID]</td> 
   <td>Geben Sie die ID des Ereignistyps ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Geben Sie die E-Mail-Adresse des Kontakts ein, für den Sie das Ereignis erstellen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekt-ID]</td> 
   <td>Geben Sie die Kennung des Kontakts ein oder ordnen Sie sie zu, für den Sie das Ereignis erstellen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeitstempel]</td> 
   <td>Geben Sie den Zeitstempel für dieses Ereignis ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Daten]</td> 
   <td>Klicken Sie für jedes Element mit benutzerdefinierten Daten, das Sie diesem Ereignis hinzufügen möchten, auf "<b>Element hinzufügen</b>"und geben Sie den Namen und Wert des Elements ein.</td> 
  </tr> 
 </tbody> 
</table>

#### Ereignistypen in der Timeline auflisten

Dieses Suchmodul gibt eine Liste aller Timeline-Ereignisse für eine bestimmte Anwendung zurück. Dieses Modul kann nur mit einer Entwicklerverbindung verwendet werden, die Ihre Benutzer-ID, Ihren HubSpot API-Schlüssel, die Client-ID und den Client Secret umfasst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anwendungs-ID]</td> 
   <td>Geben Sie die Kennung der Anwendung ein, zu der diese Ereignisse gehören, oder ordnen Sie sie zu. </td> 
  </tr> 
 </tbody> 
</table>

#### Kalenderereignisse ansehen

Dieses Kalendermodul startet ein Trigger, wenn einem  ein neues Ereignis hinzugefügt wird. Es umfasst bis zu 500 Aufgaben in einem Intervall zwischen dem Start- und dem Enddatum. Dieses Modul kann nur mit einer Entwicklerverbindung verwendet werden, die Ihre Benutzer-ID, Ihren HubSpot API-Schlüssel, die Client-ID und den Client Secret umfasst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignistyp]</td> 
   <td>Wählen Sie aus, ob Sie Social-Ereignisse, Inhaltsereignisse oder alle Ereignisse überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Dateien ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td>Geben Sie das Startdatum ein oder ordnen Sie es zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td>Geben Sie das Enddatum ein oder ordnen Sie es zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Überwachungsbenachrichtigungen

Dieses Trigger-Modul startet ein Szenario, wenn eine neue Benachrichtigung über Änderungen gesendet wird.  Es umfasst bis zu 500 Aufgaben in einem Intervall zwischen dem Start- und dem Enddatum. Dieses Modul kann nur mit einer Entwicklerverbindung verwendet werden, die Ihre Benutzer-ID, Ihren HubSpot API-Schlüssel, die Client-ID und den Client Secret umfasst. Sie können in HubSpot nur eine Webhook-URL pro Entwickleranwendung haben.

Um einen Webhook für dieses Modul zu erstellen, klicken Sie neben dem Webhook-Feld auf **Hinzufügen** und füllen Sie die folgenden Felder aus:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anwendungs-ID]</td> 
   <td>Geben Sie die Anwendungs-ID ein, die Sie für diesen Webhook verwenden möchten. Sie finden die ID in Ihrem HubSpot-Entwicklerportal.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonnements]</td> 
   <td> <p>Klicken Sie für jeden Benachrichtigungstyp, den Sie sehen möchten, auf <b>Element hinzufügen</b> und wählen Sie den Abonnementtyp aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Immer alte Abonnements entfernen]</td> 
   <td>Aktivieren Sie diese Option, um alte Abonnements, die an diesen Webhook angehängt sind, zu trennen oder zu löschen.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Dateien**

### Dateien

* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [Datei löschen](#delete-a-file)
* [[!UICONTROL Ordner löschen]](#delete-a-folder)
* [Listendateien](#list-files)
* [[!UICONTROL Verschieben einer Datei]](#move-a-file)
* [Datei hochladen](#upload-a-file)
* [Dateien überwachen](#watch-files)

#### [!UICONTROL Erstellen eines Ordners]

Dieses Modul erstellt einen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### Datei löschen

Dieses Aktionsmodul löscht eine Datei sowie alle zugehörigen Daten und Miniaturansichten dauerhaft aus dem Dateimanager.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Geben Sie die Kennung der Datei ein, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Listendateien

Dieses Suchmodul gibt eine Liste von Dateien zurück, die im Dateimanager gespeichert sind.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Dateien ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, der die Dateien enthält, die Sie auflisten möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Um nur Dateien mit bestimmten Zeichen im Dateinamen einzuschließen, geben Sie die Zeichen ein oder ordnen Sie sie zu, die der Dateiname enthalten soll.</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

#### Datei hochladen

Dieses Aktionsmodul lädt eine Datei in den Dateimanager hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zugriffstyp] </td> 
   <td>Wählen Sie aus, ob die Datei privat, öffentlich, aber nicht indexierbar oder öffentlich und indexierbar sein soll. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td>Wählen Sie die Kennung des Ordners aus, in den Sie die Datei hochladen möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Aktivieren Sie diese Option, um die Datei zu überschreiben, wenn sie bereits im Ordner vorhanden ist.</td> 
  </tr> 
 </tbody> 
</table>

### Überwachungsdateien

Dieses Dateimodul startet ein Trigger, wenn eine neue Datei im Dateimanager gespeichert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Dateien ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, der die Dateien enthält, die Sie sehen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Um nur Dateien mit bestimmten Zeichen im Dateinamen einzuschließen, geben Sie die Zeichen ein oder ordnen Sie sie zu, die der Dateiname enthalten soll.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Aufgaben**

### Aufgaben

* [Erstellen einer Kalenderaufgabe](#create-a-calendar-task)
* [Löschen einer Kalenderaufgabe](#create-a-calendar-task)
* [Aufgabenereignisse überwachen](#watch-task-events)

#### Erstellen einer Kalenderaufgabe

Dieses Aktionsmodul erstellt eine neue Aufgabe für einen Kalender. Die in diesem Modul verwendete Verbindung muss die Anmeldeinformationen eines Benutzers mit einem gebührenpflichtigen Marketing-Konto verwenden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für die neue Kalenderaufgabe ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für die neue Kalenderaufgabe ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Owner ID]</td> 
   <td>Geben Sie die Besitzer-ID des Benutzers ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignisdatum]</td> 
   <td>Geben Sie das Datum für diese Aufgabe ein oder ordnen Sie es zu.<p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kategorie]</td> 
   <td>Wählen Sie den Ereignistyp aus.<ul><li><b>Blogpost</b><p>Geben Sie die Inhaltsgruppen-ID ein. Dies ist die ID der Blog-Seite.</p></li><li><b>E-Mail</b><p>Geben Sie den Pfad der zu verwendenden E-Mail-Vorlage ein oder ordnen Sie ihn zu.</li><li><b>Landingpage</b><p>Geben Sie den Pfad zur Landingpage-Vorlage ein, die Sie verwenden möchten, oder ordnen Sie ihn zu.</li><li><b>Benutzerdefiniert</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td>Geben Sie an, ob das Ereignis den Status "Aufgaben"oder "Fertig"aufweist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign GUID]</td> 
   <td>Geben Sie die interne HubSpot-ID der Kampagne ein oder ordnen Sie sie zu, zu der dieses Ereignis gehört.</td> 
  </tr> 
 </tbody> 
</table>

#### Löschen einer Kalenderaufgabe

Dieses Aktionsmodul löscht eine Kalenderaufgabe. Die in diesem Modul verwendete Verbindung muss die Anmeldeinformationen eines Benutzers mit einem gebührenpflichtigen Marketing-Konto verwenden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die ID der Aufgabe ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Aufgabenereignisse überwachen

Dieses Trigger-Modul startet ein Szenario, wenn ein neues Aufgabenereignis in einem Kalender vorhanden ist. Die in diesem Modul verwendete Verbindung muss die Anmeldeinformationen eines Benutzers mit einem gebührenpflichtigen Marketing-Konto verwenden. Das Modul gibt bis zu 500 Ereignisse zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Dateien ein oder ordnen Sie sie zu, die das Modul während des Ausführungszyklus eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td>Geben Sie das früheste Datum ein oder ordnen Sie es zu, für das Sie Ereignisse anzeigen möchten. Verwenden Sie das Format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td>Geben Sie das aktuelle Datum ein oder ordnen Sie es zu, für das Sie Ereignisse anzeigen möchten. Verwenden Sie das Format <code>MM/DD/YYYY h:mm</code>.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Benutzende**

### Benutzende

* [Inhaber abrufen](#get-an-owner)
* [Inhaber auflisten](#list-owners)

#### Inhaber abrufen

Dieses Aktionsmodul gibt Details eines Eigentümers zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Owner ID]</td> 
   <td> <p>Geben Sie die ID des Eigentümers ein oder ordnen Sie sie zu, für den Sie Details zurückgeben möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Inhaber auflisten

Dieses Suchmodul gibt eine Liste aller Eigentümer in einem HubSpot-Konto zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Tickets**

### Tickets

<!--* [Create a Ticket]-->
* [Ticket löschen](#delete-a-ticket)
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

#### [!UICONTROL Ticket löschen]

Löscht ein vorhandenes Ticket anhand seiner Kennung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Tickets ein, das Sie löschen möchten. </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

&lt;!— Ticket aktualisieren Eine funktionierende Verbindung muss gefunden werden—>

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### Formulare

* [Datei über Formular hochladen](#get-a-file-uploaded-via-form)
* [Forms auflisten](#list-forms)
  <!--* [Submit Data to a Form]-->
  <!--* [Watch Submissions for a Form]-->

#### Datei über Formular hochladen

Dieses Aktionsmodul gibt eine Datei zurück, die über ein Formular hochgeladen wurde.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-URL]</td> 
   <td>Geben Sie die URL der Datei ein oder ordnen Sie sie zu. Dies finden Sie in den Formularmetadaten.</td> 
  </tr> 
 </tbody> 
</table>

#### Forms auflisten

Dieses Aktionsmodul gibt alle Formulare zurück, die in dem Konto erstellt wurden, das mit der für dieses Modul verwendeten Verbindung verknüpft ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Formularen ein oder ordnen Sie sie zu, die das Modul in einem Ausführungszyklus zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



&lt;!—##### Überwachen von Übermittlungen für ein Formular — Benötigen Sie eine funktionierende Verbindung.>—>

+++

+++**Social Media (Broadcast)**

### Social Media (Broadcast)

* [Abbrechen einer Broadcast-Nachricht](#cancel-a-broadcast-message)
* [Erstellen einer Broadcast-Nachricht](#create-a-broadcast-message)
* [Broadcast-Nachrichten ansehen](#watch-broadcast-messages)

#### Abbrechen einer Broadcast-Nachricht

Dieses Aktionsmodul bricht einen geplanten Broadcast ab, z. B. einen Tweet oder einen Facebook-Beitrag.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>Geben Sie die ID des Broadcasts ein oder ordnen Sie sie zu, den Sie abbrechen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Erstellen einer Broadcast-Nachricht

Dieses Aktionsmodul erstellt eine Nachricht und veröffentlicht sie sofort im angegebenen Social-Media-Kanal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanal-ID]</td> 
   <td>Geben Sie die Kennung des Kanals ein, den Sie für diesen Broadcast verwenden möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel]</td> 
   <td>Geben Sie einen Titel für diesen Broadcast ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td>Geben Sie den Text des Broadcasts ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Foto-URL]</td> 
   <td>Geben Sie die URL eines Fotos ein, das Sie in den Broadcast aufnehmen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Miniatur-URL]</td> 
   <td>Geben Sie die URL einer Miniaturansicht ein, die Sie für diesen Broadcast verwenden möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trigger at]</td> 
   <td>Geben Sie Datum und Uhrzeit ein oder ordnen Sie sie zu, zu der der Broadcast gesendet werden soll. Wenn dies leer gelassen wird, wird der Broadcast sofort gesendet.<p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Broadcast-Nachrichten ansehen

Dieses Trigger-Modul startet ein Szenario, wenn eine Nachricht von HubSpot an den angegebenen Social-Media-Kanal gesendet wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul in einem Ausführungszyklus zurückgibt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter nach Status]</td> 
   <td>Um das Szenario nur zu starten, wenn die Nachricht einen bestimmten Status aufweist, wählen Sie den Status aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter nach Kanal</td> 
   <td>Um das Szenario nur zu starten, wenn sich die Nachricht in einem bestimmten Kanal befindet, wählen Sie den Kanal aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Broadcast ID]</td> 
   <td>Um das Szenario nur zu starten, wenn die Nachricht an einem bestimmten Datum oder nach einem bestimmten Datum liegt, geben Sie das Datum im Format <code>MM/DD/YYYY</code> ein oder ordnen Sie es zu.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Blog-Beiträge**

### Blogbeiträge

<!--* [Create a Blog Post]-->
* [Einen Blogpost löschen](#delete-a-blog-post)
  <!--* [List Blog Posts]-->
* [Publish/Veröffentlichung eines Blog-Beitrags rückgängig machen](#publish--unpublish-a-blog-post)
  <!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### Löschen eines Blog-Beitrags

Dieses Aktionsmodul löscht einen einzelnen Blogpost.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die ID des Blogpost ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish/Veröffentlichung eines Blog-Beitrags rückgängig machen

Dieses Aktionsmodul plant bzw. hebt die Veröffentlichung eines Blogpost auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die ID des Blogpost ein oder ordnen Sie sie zu, den Sie planen oder abbrechen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td>Wählen Sie aus, ob Sie den Blogpost planen oder einen zuvor geplanten Blogpost abbrechen möchten.</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**Abonnements**

### Abonnements

* [E-Mail-Abonnement aktualisieren](#update-email-subscription)
* [Zeitleiste für Abonnements für ein Portal ansehen](#watch-subscriptions-timeline-for-a-portal)

#### E-Mail-Abonnement aktualisieren

Dieses Aktionsmodul aktualisiert ein E-Mail-Abonnement in HubSpot.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email]</td> 
   <td>Geben Sie die E-Mail-Adresse des Abonnements ein, das Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Klicken Sie für jeden Status, für den Sie das Abonnement aktualisieren möchten, auf "<b>Element hinzufügen</b>", geben Sie die Kennung des Status ein und geben Sie an, ob die E-Mail-Adresse diesen Status abonniert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal Subscription Legal Status]</td> 
   <td>Um die Rechtsgrundlage für dieses Abonnement für die DSGVO aufzuzeichnen, wählen Sie den rechtlichen Status dieses Abonnements aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portal Subscription Legal Base Erläuterung]</td> 
   <td>Um einen Hinweis zur Rechtsgrundlage für dieses Abonnement für die DSGVO hinzuzufügen, geben Sie den Text der Notiz ein oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Zeitleiste für Abonnements für ein Portal ansehen

Dieses Trigger-Modul startet ein Szenario, wenn dem Portal ein neues E-Mail-Timeline-Abonnement hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Elementen ein oder ordnen Sie sie zu, die das Modul in einem Ausführungszyklus zurückgibt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Timestamp]</td> 
   <td>Um Ergebnisse aus einem oder nach einem bestimmten Datum zurückzugeben, geben Sie das Datum im Format <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Endzeitstempel]</td> 
   <td>Um Ergebnisse aus einem oder vor einem bestimmten Datum zurückzugeben, geben Sie das Datum im Format <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**Sonstige**

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL HubSpot CRM]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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

+++

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
