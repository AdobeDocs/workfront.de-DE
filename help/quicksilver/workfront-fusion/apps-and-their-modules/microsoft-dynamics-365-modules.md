---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Microsoft Dynamics 365 verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Dynamics 365] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

>[!NOTE]
>
>Der [!DNL Microsoft Dynamics 365]-Connector unterstützt [!DNL Dynamics Finance and Operations] nicht.

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

Um [!DNL Microsoft Dynamics] 365 zu verwenden, müssen Sie über ein [!DNL Microsoft Dynamics 365] -Konto verfügen.

## Verbinden von Microsoft Dynamics 365 mit Workfront Fusion

Sie können eine Verbindung zu Ihrem [!DNL Microsoft Dynamics 365]-Konto direkt aus einem [!DNL Microsoft Dynamics 365]-Modul erstellen.

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

1. Klicken Sie in einem beliebigen [!DNL Microsoft Dynamics 365]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Geben Sie einen Namen für die Verbindung ein.
1. Geben Sie im Feld **[!UICONTROL Ressource]** die Adresse Ihres [!DNL Dynamics 365]-Kontos ohne `https://` ein.
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

>[!NOTE]
>
>Verwenden Sie bei der Registrierung von [!DNL Workfront Fusion] in Ihrem [!DNL Microsoft Azure]-Portal den folgenden Umleitungs-URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] Module und ihre Felder

Wenn Sie [!DNL Microsoft Dynamics 365] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Microsoft Dynamics 365] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Aufnahmen ansehen (geplant)]](#watch-records-scheduled)
* [[!UICONTROL Aufzeichnungen ansehen (Echtzeit)]](#watch-records-real-time)
* [[!UICONTROL Datensatz erstellen]](#create-record)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-record)
* [[!UICONTROL Datensätze lesen]](#read-records)
* [[!UICONTROL Datensatz aktualisieren]](#update-record)
* [[!UICONTROL Suchdatensätze]](#search-records)

### [!UICONTROL Aufnahmen ansehen (geplant)]

Dieses Modul für geplante Trigger führt ein Szenario aus, wenn ein Datensatz im angegebenen Objekt nach der letzten geplanten Ausführung in [!DNL Dynamics 365] erstellt oder aktualisiert wird.

Die Ausgabe des Moduls gibt an, ob der gefundene Datensatz neu oder aktualisiert ist (wenn er im Zeitraum hinzugefügt und aktualisiert wurde, wird er als neu markiert). Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dies geschieht in einem regelmäßig von Ihnen festgelegten Intervall.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Wählen Sie aus, ob das Modul <strong>[!UICONTROL Only new records]</strong>, <strong>[!UICONTROL Updated records only]</strong> oder <strong>[!UICONTROL New records and all changes]</strong> überwachen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den [!UICONTROL Microsoft Dynamics 365]-Datensatztyp aus, den Sie für das Szenario sehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Aufzeichnungen ansehen (Echtzeit)]

Dieses Instant Trigger-Modul führt ein Szenario aus, wenn ein von Ihnen angegebener Datensatz (Objekt) in [!DNL Dynamics 365] erstellt oder aktualisiert wird.

In diesem Modul ist ein Webhook erforderlich.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie für dieses Modul verwenden möchten. </p> <p>So fügen Sie einen neuen Webhook hinzu:</p> 
    <ol> 
     <li value="1"> <p>Klicken Sie rechts neben dem Webhook-Feld auf <strong>[!UICONTROL Add]</strong> .</p> </li> 
     <li value="2"> <p>Geben Sie im Namensfeld <strong>[!UICONTROL Webhook]</strong> einen beschreibenden Namen für den Webhook ein.</p> </li> 
     <li value="3"> <p>Wählen Sie im Feld <strong>[!UICONTROL Connection]</strong> die gewünschte Verbindung aus.</p> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </li> 
     <li value="4"> <p>Klicken Sie auf <strong>[!UICONTROL Save]</strong> , um Ihren Webhook zu speichern und zum Modul zurückzukehren.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt eine Entität, z. B. einen Termin oder eine Aufgabe.

Sie geben Informationen über die Entität an, die Sie erstellen möchten.

Das Modul gibt die ID der neuen Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul erstellen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zu zuordnende Felder auswählen]</td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte einfügen möchten. Die verfügbaren Felder hängen vom Entitätstyp ab.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Eigenschaftenfelder]</td> 
   <td> Dies sind die von Ihnen ausgewählten Felder. Geben Sie den Wert ein, den der Datensatz für eine bestimmte Eigenschaft aufweisen soll. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Microsoft Dynamics 365] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Microsoft Dynamics 365] -Modulen nicht ausgeführt werden kann.

Das Modul gibt Informationen zum Statuscode, zu Kopfzeilen und zum Hauptteil zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Weitere Informationen finden Sie in der [!DNL Microsoft] -Dokumentation zur Verwendung des [!DNL Dynamics 365 Customer Engagement Web API].

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>&lt;Instance URL>/api/data/v9.1/</code> ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Weitere Informationen finden Sie unter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
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
 </tbody> 
</table>

### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht eine Entität.

Sie geben die ID der Entität an.

Das Modul gibt die ID der Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td> <p>Wählen Sie den Entitätstyp aus, den das Modul löschen soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Microsoft Dynamics 365]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul löschen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze lesen]

Dieses Aktionsmodul liest Daten aus einer einzelnen Entität in [!DNL Microsoft Dynamics 365].

Sie geben die ID der Entität an.

Das Modul gibt die ID der Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul lesen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Microsoft Dynamics 365]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul lesen soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert eine Entität.

Sie geben die ID der Entität an.

Das Modul gibt die ID des aktualisierten Datensatzes und aller zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zu zuordnende Felder auswählen]</td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte einfügen möchten. Die verfügbaren Felder hängen vom Entitätstyp ab.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Eigenschaftenfelder]</td> 
   <td>Dies sind die von Ihnen ausgewählten Felder. Geben Sie den Wert ein, den der Datensatz für eine bestimmte Eigenschaft aufweisen soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Microsoft Dynamics] 365 ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul aktualisieren soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suchdatensätze]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Microsoft Dynamics 365], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> . </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Wählen Sie den Filter aus, den Sie für diese Suche verwenden möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standardfilter]</strong> </p> <p>Richten Sie den Filter ein, indem Sie ein Feld und einen Operator auswählen und den Wert eingeben oder zuordnen, nach dem Sie suchen möchten. Sie können UND- oder ODER-Regeln für Ihren Filter verwenden.</p> </li> 
     <li> <p><strong>[!UICONTROL Abfragefunktionen]</strong> </p> <p>Geben Sie die Web-API-Abfragefunktion [!DNL Dynamics 365] ein, die Sie für die Suche verwenden möchten. </p> <p>Weitere Informationen zu Abfragefunktionen finden Sie unter <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referenz zur Web-API-Abfragefunktion</a> in der Dokumentation zu [!DNL Microsoft] .</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierung]</td> 
   <td> <p>Geben Sie die Reihenfolge an, in der Elemente zurückgegeben werden. Sie können mehrere Arten hinzufügen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Geben Sie das Feld an, nach dem die Ergebnisse sortiert werden sollen.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Geben Sie die Sortierrichtung an (aufsteigend oder absteigend).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>
