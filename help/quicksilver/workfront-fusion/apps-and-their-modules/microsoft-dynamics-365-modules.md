---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Microsoft Dynamics 365-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-dynamics-365-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Dynamics 365] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

>[!NOTE]
>
>Der [!DNL Microsoft Dynamics 365]-Connector unterstützt keine [!DNL Dynamics Finance and Operations].
>
>Informationen zu den Microsoft Dynamics 365 Finance and Operations-Modulen finden Sie unter [[!DNL Microsoft Dynamics 365 Finance and Operations modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/dynamics-finance-operations-modules.md).

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Um [!DNL Microsoft Dynamics] 365 verwenden zu können, müssen Sie über ein [!DNL Microsoft Dynamics 365] verfügen.

## Verbinden von Microsoft Dynamics 365 mit Workfront Fusion

Sie können direkt aus einem [!DNL Microsoft Dynamics 365]-Modul heraus eine Verbindung zu Ihrem [!DNL Microsoft Dynamics 365]-Konto herstellen.

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Einverständnisbildschirm für Berechtigungen alle Berechtigungen angezeigt, die zuvor der Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn ein Benutzer beispielsweise über die über den Excel-Connector gewährten Berechtigungen zum Lesen von Tabellen verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Einverständnisbildschirm für Berechtigungen sowohl die bereits erteilte Berechtigung zum Lesen von Tabellen als auch die neu erforderliche Berechtigung zum Schreiben von E-Mails an.

1. Klicken Sie in einem [!DNL Microsoft Dynamics 365] Modul **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung].
1. Geben Sie einen Namen für die Verbindung ein.
1. Geben **[!UICONTROL im Feld]** die Adresse Ihres [!DNL Dynamics 365] Kontos ohne `https://` ein.
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

>[!NOTE]
>
>Verwenden Sie beim Registrieren von [!DNL Workfront Fusion] in Ihrem [!DNL Microsoft Azure]-Portal den folgenden Umleitungs-URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] Module und ihre Felder

Beim Konfigurieren [!DNL Microsoft Dynamics 365] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Microsoft Dynamics 365] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Datensätze beobachten (geplant)]](#watch-records-scheduled)
* [[!UICONTROL Datensätze ansehen (Echtzeit)]](#watch-records-real-time)
* [[!UICONTROL Datensatz erstellen]](#create-record)
* [[!UICONTROL Erstellen eines API-Aufrufs]](#make-an-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-record)
* [[!UICONTROL Datensätze lesen]](#read-records)
* [[!UICONTROL Eintrag aktualisieren]](#update-record)
* [[!UICONTROL Datensätze suchen]](#search-records)

### [!UICONTROL Datensätze beobachten (geplant)]

Dieses Modul für geplante Trigger führt ein Szenario aus, wenn ein Datensatz in dem angegebenen Objekt nach der letzten geplanten Ausführung in [!DNL Dynamics 365] erstellt oder aktualisiert wird.

Die Ausgabe des Moduls gibt an, ob der von ihm gefundene Datensatz neu oder aktualisiert ist (wenn er im Zeitraum hinzugefügt und aktualisiert wurde, wird er als neu markiert). Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dies geschieht in einem regelmäßig geplanten Intervall, das Sie angeben.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL include]</td> 
   <td>Wählen Sie aus, ob das Modul <strong>[!UICONTROL Only New Records]</strong>, <strong>[!UICONTROL Updated Records only]</strong> oder <strong>[!UICONTROL New Records and all changes]</strong> überwachen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Datensatztyp [!UICONTROL Microsoft Dynamics 365] aus, den das Szenario überwachen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max. Einträge]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze ansehen (Echtzeit)]

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
     <li value="1"> <p>Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> rechts neben dem Feld Webhook</p> </li> 
     <li value="2"> <p>Geben Sie in das Namensfeld <strong>[!UICONTROL Webhook]</strong> einen beschreibenden Namen für den Webhook ein.</p> </li> 
     <li value="3"> <p>Wählen Sie im Feld <strong>[!UICONTROL Connection]</strong> die Verbindung, die Sie verwenden möchten, ausgewählt aus</p> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </li> 
     <li value="4"> <p>Klicken Sie auf <strong>[!UICONTROL Speichern]</strong>, um Ihren Webhook zu speichern und zum Modul zurückzukehren.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt eine Entität, z. B. einen Termin oder eine Aufgabe.

Sie geben Informationen zu der Entität an, die Sie erstellen möchten.

Das Modul gibt die ID der neuen Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul erstellen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder zum Zuordnen auswählen]</td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte einbeziehen möchten. Die verfügbaren Felder hängen vom Entitätstyp ab.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Eigenschaftsfelder]</td> 
   <td> Dies sind die von Ihnen ausgewählten Felder. Geben Sie den Wert ein, den der Datensatz für eine bestimmte Eigenschaft haben soll. </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Microsoft Dynamics 365]-API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen [!DNL Microsoft Dynamics 365] nicht durchgeführt werden kann.

Das -Modul gibt Informationen über den Status-Code, die Kopfzeilen und den Hauptteil zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Weitere Informationen finden Sie in der [!DNL Microsoft] Dokumentation zur Verwendung des [!DNL Dynamics 365 Customer Engagement Web API].

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>&lt;Instance URL>/api/data/v9.1/</code> ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Für weitere Informationen in</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] Fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht eine Entität.

Geben Sie die ID der Entität an.

Das Modul gibt die ID der Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td> <p>Wählen Sie den Typ der Entität aus, die das Modul löschen soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Microsoft Dynamics 365]-ID des Datensatzes ein, den Sie löschen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze lesen]

Dieses Aktionsmodul liest Daten aus einer einzelnen Entität in [!DNL Microsoft Dynamics 365].

Geben Sie die ID der Entität an.

Das Modul gibt die ID der Entität und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Entitätstyp aus, den das Modul lesen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Microsoft Dynamics 365]-ID des Datensatzes ein, den das Modul lesen soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Eintrag aktualisieren]

Dieses Aktionsmodul aktualisiert eine Entität.

Geben Sie die ID der Entität an.

Das Modul gibt die ID des aktualisierten Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Typ der Entität aus, die das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder zum Zuordnen auswählen]</td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte einbeziehen möchten. Die verfügbaren Felder hängen vom Entitätstyp ab.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Eigenschaftsfelder]</td> 
   <td>Dies sind die von Ihnen ausgewählten Felder. Geben Sie den Wert ein, den der Datensatz für eine bestimmte Eigenschaft haben soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Microsoft Dynamics] 365-ID des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze suchen]

Dieses Suchmodul sucht in einem -Objekt nach Datensätzen, [!DNL Microsoft Dynamics 365] mit der angegebenen Suchanfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Microsoft Dynamics 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Microsoft Dynamics 365] mit [!DNL Workfront Fusion]</a> in diesem Artikel. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entitätstyp]</td> 
   <td>Wählen Sie den Typ der Entität aus, die das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Wählen Sie den Filter aus, den Sie für diese Suche verwenden möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standardfilter]</strong> </p> <p>Richten Sie den Filter ein, indem Sie ein Feld und einen Operator auswählen und den Wert eingeben oder zuordnen, nach dem Sie suchen möchten. Sie können AND- oder OR-Regeln für Ihren Filter verwenden.</p> </li> 
     <li> <p><strong>[!UICONTROL Abfragefunktionen]</strong> </p> <p>Geben Sie die Abfrage-Funktion der [!DNL Dynamics 365]-Web-API ein, die Sie für die Suche verwenden möchten. </p> <p>Weitere Informationen zu Abfragefunktionen finden Sie unter <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web-API-Abfragefunktionsreferenz</a> in der [!DNL Microsoft].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL sort]</td> 
   <td> <p>Geben Sie die Reihenfolge an, in der Elemente zurückgegeben werden. Sie können mehrere Sortierungen hinzufügen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL-Feld]</strong> </p> <p>Geben Sie das Feld an, nach dem Sie die Ergebnisse sortieren möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Geben Sie die Sortierrichtung an (aufsteigend oder absteigend).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max. Einträge]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>
