---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Azure DevOps-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Azure DevOps] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 0%

---

# [!DNL Azure DevOps] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Azure DevOps] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Um [!DNL Azure DevOps] -Module verwenden zu können, müssen Sie über ein DevOps-Konto vom Typ [!DNL Azure] verfügen.

## [!DNL Azure DevOps] mit [!DNL Workfront Fusion] verbinden {#connect-azure-devops-to-workfront-fusion}

1. Fügen Sie Ihrem Szenario ein [!DNL Azure DevOps] -Modul hinzu.
1. Klicken Sie neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie im Feld [!UICONTROL Verbindungstyp] die Option **[!DNL Azure DevOps]** aus.

   >[!IMPORTANT]
   >
   >Der Verbindungstyp [!UICONTROL [!DNL Azure DevOps] (Alle Bereiche anfordern)] wird in naher Zukunft nicht mehr unterstützt. Daher empfehlen wir die Verwendung dieser Funktion nicht.

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Verbindungsname]</td>
            <td>Geben Sie einen Namen für die Verbindung ein, die Sie erstellen.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organisation]</td>
            <td>Geben Sie den Namen der Organisation ein, unter der Sie Ihre [!DNL Azure DevOps] -Anwendung erstellt haben.</td>
        </tr>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung einzurichten und mit der Erstellung Ihres Szenarios fortzufahren.

## [!UICONTROL Azure DevOps] -Module und ihre Felder

Wenn Sie [!DNL Azure DevOps] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Azure DevOps] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Auf Arbeitselemente achten]

Dieses Instant Trigger-Modul führt ein Szenario aus, wenn ein Datensatz in [!UICONTROL Azure DevOps] hinzugefügt, aktualisiert oder gelöscht wird.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie einen Webhook für das Modul aus oder fügen Sie ihn hinzu.</p> <p>Weitere Informationen zu Webhooks in Trigger-Modulen finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Informationen zum Erstellen eines Webhooks finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [Benutzerspezifischer API-Aufruf](#custom-api-call)
* [Datensatz lesen](#read-record)
* [Datensatz erstellen](#create-a-record)
* [Arbeitselement aktualisieren](#update-a-work-item)
* [[!UICONTROL Hochladen eines Anhangs]](#upload-an-attachment)
* [Anlage herunterladen](#download-an-attachment)
* [Verknüpfen von Arbeitselementen]([!UICONTROL #link-work-items])

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Azure DevOps] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Azure DevOps] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Basis-URL]</td> 
   <td> <p>Auswählen oder Zuordnen der Basis-URL, mit der Sie eine Verbindung zu Ihrem [!DNL Azure DevOps]-Konto herstellen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Relative URL von [!UICONTROL]</td> 
   <td> <p>Geben Sie die relative URL ein, mit der Sie eine Verbindung für diesen API-Aufruf herstellen möchten.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API-Version]</td> 
   <td>Wählen Sie die Version der [!DNL Azure DevOps]-API aus oder ordnen Sie sie zu, mit der Sie für diesen API-Aufruf eine Verbindung herstellen möchten. Wenn keine Version ausgewählt ist, stellt [!DNL Workfront Fusion] eine Verbindung zur [!DNL Azure DevOps] API-Version 5.1 her.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> </td> 
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

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen Datensatz in [!DNL Azure DevOps].

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Auswählen, ob Sie ein Projekt oder ein Arbeitselement lesen möchten</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Projekt]</strong>: Wählen Sie das Projekt aus, das Sie lesen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Arbeitselement]</strong>: Wählen Sie das Projekt aus, das das Arbeitselement enthält, das Sie lesen möchten, und wählen Sie dann den Arbeitselementtyp aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen. Die verfügbaren Felder hängen vom Arbeitselement-Typ ab.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie lesen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt ein neues Projekt oder Arbeitselement.

Das Modul gibt die Objekt-ID für das neu erstellte Arbeitselement oder die URL und den Status-Code eines neu erstellten Projekts aus.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie aus, ob Sie ein Arbeitselement oder ein Projekt erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Projekt]</strong> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>: Geben Sie einen Namen für das neue Projekt ein oder ordnen Sie ihn zu.</p> </li> 
       <li> <p><strong>[!UICONTROL Beschreibung]</strong>: Geben Sie eine Beschreibung für das neue Projekt ein oder ordnen Sie sie zu. </p> </li> 
       <li> <p><strong>[!UICONTROL Sichtbarkeit]</strong>: Wählen Sie aus, ob Ihr Projekt öffentlich oder privat sein soll. Benutzer müssen bei Ihrer Organisation angemeldet sein und Zugriff auf das Projekt erhalten haben, damit sie mit einem privaten Projekt interagieren können. Öffentliche Projekte sind für Benutzer sichtbar, die nicht bei Ihrer Organisation angemeldet sind.</p> </li> 
       <li> <p><strong>[!UICONTROL Versionskontrolle]</strong>: Wählen Sie aus, ob das Projekt [!DNL Git] oder [!UICONTROL Team Foundation Version Control (TFCV)] für die Versionskontrolle verwenden soll.</p> </li> 
       <li> <p><strong>[!UICONTROL Arbeitselementprozess]</strong>: Wählen Sie den Arbeitsprozess aus, den Sie für das Projekt verwenden möchten. Die Optionen sind [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)] und [!UICONTROL Agile].</p> <p>Weitere Informationen zu [!DNL Azure DevOps] -Prozessen finden Sie unter <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Einen Prozess auswählen</a> in der Dokumentation zu [!DNL Azure DevOps] .</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Arbeitselement]</strong> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Projekt]</strong>: Wählen Sie das Projekt aus, in dem Sie das Arbeitselement erstellen möchten.</p> </li> 
       <li> <p><strong>[!UICONTROL Arbeitselementtyp]</strong>: Wählen Sie den Typ des zu erstellenden Arbeitselements aus.</p> </li> 
       <li> <p><strong>[!UICONTROL Andere Felder]</strong>: Geben Sie in diesen Feldern den Wert ein, den das Arbeitselement für eine bestimmte Eigenschaft aufweisen soll. Die verfügbaren Felder hängen vom Arbeitselement-Typ ab.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Arbeitselement aktualisieren]

Dieses Aktionsmodul aktualisiert ein vorhandenes Arbeitselement mit seiner ID.

Das Modul gibt die ID des aktualisierten Arbeitselements zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt]</td> 
   <td>Wählen Sie das Projekt aus, das das zu aktualisierende Arbeitselement enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitselement Typ]</td> 
   <td> <p>Wählen Sie den Typ des Arbeitselements aus, das Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Andere Felder]</td> 
   <td>Geben Sie in jedem dieser Felder den Wert ein, den das Arbeitselement für eine bestimmte Eigenschaft aufweisen soll. Die verfügbaren Felder hängen vom Arbeitselement-Typ ab.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitselement-ID]</td> 
   <td>Geben Sie die ID des Arbeitselements ein, das Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hochladen eines Anhangs]

Dieses Aktionsmodul lädt eine Datei hoch und hängt sie an ein Arbeitselement an.

Das Modul gibt die Anlagen-ID und eine Download-URL für den Anhang zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt] </td> 
   <td> <p>Wählen Sie das Projekt aus, in das Sie einen Anhang hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitselement-ID]</td> 
   <td> <p>Geben Sie die Kennung des Arbeitselements ein oder ordnen Sie sie zu, in das Sie einen Anhang hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar]</td> 
   <td>Geben Sie den Text eines Kommentars ein, den Sie zum hochgeladenen Anhang hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei] </td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder geben Sie den Namen und den Inhalt der Quelldatei ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Herunterladen eines Anhangs]

Dieses Aktionsmodul lädt einen Anhang herunter.

Das Modul gibt den Dateiinhalt des Anhangs zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anlage-URL]</td> 
   <td> <p>Geben Sie die URL des Anhangs ein, den Sie herunterladen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verknüpfen von Arbeitselementen]

Dieses Aktionsmodul verknüpft zwei Arbeitselemente und definiert die Beziehung zwischen ihnen.

Das Modul gibt die ID des Hauptarbeitselements und aller zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitselement-ID]</td> 
   <td>Geben Sie die ID des Hauptelement ein, mit dem Sie ein anderes Arbeitselement verknüpfen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>Geben Sie die ID des Arbeitselements ein, das Sie mit dem Hauptarbeitselement verknüpfen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Definieren Sie die Beziehung zwischen den Arbeitselementen, die Sie verknüpfen möchten.</p> <p>Weitere Informationen finden Sie unter <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Link Type Reference</a> in der [!UICONTROL Azure DevOps]-Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar]</td> 
   <td>Geben Sie den Text eines Kommentars ein oder ordnen Sie ihn zu. Dies ist nützlich, um die Begründung oder Absicht des Links zu erläutern.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Arbeitselemente auflisten]

Dieses Aktionsmodul ruft alle Arbeitselemente eines bestimmten Typs in einem [!DNL Azure DevOps] -Projekt ab.

Das Modul gibt die ID des Hauptarbeitselements und aller zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Azure DevOps]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Azure DevOps] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt]</td> 
   <td>Wählen Sie das Projekt aus, aus dem Sie Arbeitselemente abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Arbeitselement Typ]</td> 
   <td> <p>Wählen Sie den Typ des Arbeitselements aus, das Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Eigenschaften aus, die in der Ausgabe des Moduls angezeigt werden sollen. Die verfügbaren Felder hängen vom Typ des Arbeitselements ab, das Sie abrufen möchten. Sie müssen mindestens eine Eigenschaft auswählen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Arbeitselementen ein, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>
