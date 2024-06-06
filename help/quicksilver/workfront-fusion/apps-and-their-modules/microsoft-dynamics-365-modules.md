---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Microsoft Dynamics 365 verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 46c282062ed737be860aeb4af96ac5f5efe9360d
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Microsoft Dynamics 365], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

>[!NOTE]
>
>Die [!DNL Microsoft Dynamics 365] Connector unterstützt nicht [!DNL Dynamics Finance and Operations].

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Microsoft Dynamics] 365, Sie müssen eine [!DNL Microsoft Dynamics 365] -Konto.

## Verbinden von Microsoft Dynamics 365 mit Workfront Fusion

Sie können eine Verbindung zu Ihrem [!DNL Microsoft Dynamics 365] direkt in einer [!DNL Microsoft Dynamics 365] -Modul.

1. In jeder [!DNL Microsoft Dynamics 365] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Geben Sie einen Namen für die Verbindung ein.
1. Im **[!UICONTROL Ressource]** -Feld die Adresse Ihres [!DNL Dynamics 365] Konto, ohne `https://`.
1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

>[!NOTE]
>
>Bei der Registrierung [!DNL Workfront Fusion] in [!DNL Microsoft Azure] Portal verwenden Sie den folgenden Umleitungs-URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] Module und ihre Felder

Bei der Konfiguration [!DNL Microsoft Dynamics 365] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Microsoft Dynamics 365] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Datensätze ansehen (geplant)]](#watch-records-scheduled)
* [[!UICONTROL Aufzeichnungen ansehen (in Echtzeit)]](#watch-records-real-time)
* [[!UICONTROL Datensatz erstellen]](#create-record)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-record)
* [[!UICONTROL Datensätze lesen]](#read-records)
* [[!UICONTROL Datensatz aktualisieren]](#update-record)
* [[!UICONTROL Suchdatensätze]](#search-records)

### [!UICONTROL Datensätze ansehen (geplant)]

Dieses Modul für geplante Trigger führt ein Szenario aus, wenn ein Datensatz im angegebenen Objekt nach der letzten geplanten Ausführung in [!DNL Dynamics 365].

Die Ausgabe des Moduls gibt an, ob der gefundene Datensatz neu oder aktualisiert ist (wenn er im Zeitraum hinzugefügt und aktualisiert wurde, wird er als neu markiert). Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dies geschieht in einem regelmäßig von Ihnen festgelegten Intervall.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Auswählen, ob das Modul überwacht werden soll <strong>[!UICONTROL Nur neue Datensätze]</strong>, <strong>[!UICONTROL Nur aktualisierte Datensätze]</strong>oder <strong>[!UICONTROL Neue Datensätze und alle Änderungen]</strong>.</td> 
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

### [!UICONTROL Aufzeichnungen ansehen (in Echtzeit)]

Dieses Instant Trigger-Modul führt ein Szenario aus, wenn ein von Ihnen angegebener Datensatz (Objekt) in erstellt oder aktualisiert wird. [!DNL Dynamics 365].

In diesem Modul ist ein Webhook erforderlich.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie für dieses Modul verwenden möchten. </p> <p>So fügen Sie einen neuen Webhook hinzu:</p> 
    <ol> 
     <li value="1"> <p>Klicks <strong>[!UICONTROL Hinzufügen]</strong> rechts neben dem Webhook-Feld</p> </li> 
     <li value="2"> <p>Im <strong>[!UICONTROL Webhook]</strong> name ein, geben Sie einen beschreibenden Namen für den Webhook ein.</p> </li> 
     <li value="3"> <p>Im <strong>[!UICONTROL Verbindung]</strong> auswählen, wählen Sie die gewünschte Verbindung aus.</p> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </li> 
     <li value="4"> <p>Klicks <strong>[!UICONTROL Save]</strong> , um Ihren Webhook zu speichern und zum Modul zurückzukehren.</p> </li> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
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

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Microsoft Dynamics 365] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Microsoft Dynamics 365] Module.

Das Modul gibt Informationen zum Statuscode, zu Kopfzeilen und zum Hauptteil zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Weitere Informationen finden Sie unter [!DNL Microsoft] Dokumentation zur Verwendung der [!DNL Dynamics 365 Customer Engagement Web API].

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
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
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td> <p>Wählen Sie den Entitätstyp aus, den das Modul löschen soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Eindeutige Eingabe oder Zuordnung [!DNL Microsoft Dynamics 365] Kennung des Datensatzes, den das Modul löschen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze lesen]

Dieses Aktionsmodul liest Daten von einer einzelnen Entität in [!DNL Microsoft Dynamics 365].

Sie geben die ID der Entität an.

Das Modul gibt die ID der Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
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
   <td>Eindeutige Eingabe oder Zuordnung [!DNL Microsoft Dynamics 365] Kennung des Datensatzes, den das Modul lesen soll.</td> 
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
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
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
   <td>Eindeutige Eingabe oder Zuordnung [!DNL Microsoft Dynamics] 365 ID des Datensatzes, den das Modul aktualisieren soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suchdatensätze]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Microsoft Dynamics 365] die mit der angegebenen Suchabfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden der [!DNL Microsoft Dynamics 365] -Konto [!DNL Workfront Fusion], siehe <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Microsoft Dynamics 365] nach [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
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
     <li> <p><strong>[!UICONTROL Abfragefunktionen]</strong> </p> <p>Geben Sie die [!DNL Dynamics 365] Web-API-Abfragefunktion, die Sie für die Suche verwenden möchten. </p> <p>Weitere Informationen zu Abfragefunktionen finden Sie unter <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Referenz zu Web-API-Abfragen</a> im [!DNL Microsoft] Dokumentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierung]</td> 
   <td> <p>Geben Sie die Reihenfolge an, in der Elemente zurückgegeben werden. Sie können mehrere Arten hinzufügen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Geben Sie das Feld an, nach dem die Ergebnisse sortiert werden sollen.</p> </li> 
     <li> <p><strong>[!UICONTROL Richtung]</strong> </p> <p>Geben Sie die Sortierrichtung an (aufsteigend oder absteigend).</p> </li> 
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
