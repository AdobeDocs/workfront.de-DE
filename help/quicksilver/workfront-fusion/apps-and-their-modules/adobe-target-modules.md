---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] Module verwenden, um Datensätze zu erstellen, zu lesen, zu aktualisieren oder zu löschen, alle Datensätze eines bestimmten Typs aufzulisten, Datensätze nach von Ihnen festgelegten Kriterien zu suchen oder einen benutzerdefinierten API-Aufruf an die  [!DNL Adobe Target] API durchzuführen.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2249'
ht-degree: 0%

---

# [!DNL Adobe Target] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Adobe Target] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. [!DNL Adobe Target] -Module ermöglichen es Ihnen, Datensätze eines bestimmten Typs aufzulisten, zu erstellen, zu lesen, zu aktualisieren oder zu löschen, Suchdatensätze nach von Ihnen festgelegten Kriterien aufzulisten oder einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Target] -API durchzuführen.


Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] oder höher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p>
      </td>
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
    </tr>
  </tbody>
</table>


Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Bevor Sie den Connector [!DNL Adobe Target] verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Target] -Konto verfügen.

## Adobe Target-API-Informationen

Der Adobe Target-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.7.33</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Verbindung zu [!DNL Adobe Target]

>[!IMPORTANT]
>
>Nach dem 3. Juni 2024 erstellte Verbindungen erfordern eine Adobe Target-Server-zu-Server-Verbindung.
>
>* Die bestehenden Dienstkontoverbindungen funktionieren bis Januar 2025 weiterhin. Sie müssen Ihre Dienstkontoverbindungen bis Januar 2024 durch Adobe Target-Server-zu-Server-Verbindungen ersetzen.
>* Sie müssen Entwickler sein, damit Ihr Unternehmen eine Server-zu-Server-Verbindung mit Adobe Target herstellen kann. Die Entwicklerrolle wird in der Adobe Admin Console festgelegt.

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Target] -Module:

1. Klicken Sie neben dem Feld Verbindung auf **[!UICONTROL Hinzufügen]** .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungstyp]</td>
        <td>Wählen Sie aus, ob Sie eine Dienstkontenverbindung oder eine Server-zu-Server-Verbindung von Adobe Target erstellen.<p><b>WICHTIG</b>: Verbindungen, die nach dem 3. Juni 2024 erstellt wurden, erfordern eine Adobe Target-Server-zu-Server-Verbindung. Die bestehenden Dienstkontoverbindungen funktionieren bis Januar 2025 weiterhin. Sie müssen Ihre Dienstkontoverbindungen bis Januar 2024 durch Adobe Target-Server-zu-Server-Verbindungen ersetzen.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen möchten.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihr [!DNL Adobe] Client-Geheimnis ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] ID des technischen Kontos ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Organisations-ID ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Mandant]</td>
        <td>
          <p> Um Ihren Mandanten zu finden, melden Sie sich bei [!DNL Adobe Experience Cloud] an, öffnen Sie [!DNL Target] und klicken Sie auf die Karte [!DNL Target]. Verwenden Sie den Wert der Mandanten-ID, wie in der URL-Subdomäne angegeben.</p>
          <p>Wenn Ihre URL beispielsweise bei [!DNL Adobe Target] den Wert <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> aufweist, lautet die Mandantenkennung "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td><code>ent_marketing_sdk</code> eingeben       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten in der [!DNL Adobe Developer Console] generiert wurde. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicken Sie auf <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Wählen Sie den Dateityp aus, den Sie extrahieren.</p>
            </li>
            <li value="3">
              <p>Wählen Sie die Datei aus, die den privaten Schlüssel oder das Zertifikat enthält.</p>
            </li>
            <li value="4">
              <p>Geben Sie das Kennwort für die Datei ein.</p>
            </li>
            <li value="5">
              <p>Klicken Sie auf <b>[!UICONTROL Save]</b> , um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Target] Module und ihre Felder

Wenn Sie [!DNL Adobe Target] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Target] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)

* [Suchvorgänge](#searches)


### Aktionen

* [[!UICONTROL Erstellen eines Datensatzes]](#create-a-record)

* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)

* [[!UICONTROL Datensatz löschen]](#delete-a-record)

* [[!UICONTROL Datensatz lesen]](#read-a-record)

* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)


#### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt eine AB- oder XT-Aktivität, ein Angebot oder eine Zielgruppe.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record Type]</td>
    <td>
      <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p>
      <ul>
        <li>
        <b>Eigenschaft</b><p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Properties/operation/createProperty">Erstellen einer Eigenschaft</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
        <b>Angebotsempfehlung</b><p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Offers/operation/createOffer">Neues recs-Angebot erstellen</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
          <b>[!UICONTROL Angebot JSON]</b>
          <p>Fahren Sie mit <a href="#offer-fields" class="MCXref xref" >Angebotsfeldern</a> fort.</p>
        </li>
        <li>
          <b>[!UICONTROL Angebotsinhalt]</b>
          <p>Fahren Sie mit <a href="#offer-fields" class="MCXref xref" >Angebotsfeldern</a> fort.</p>
        </li>
        <li>
        <b>Umgebung</b><p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Environments/operation/createEnvironment">Umgebung erstellen</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
          <b>[!UICONTROL Audience]</b>
          <p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Audiences/operation/createAudience_1_1">Erstellen einer Audience</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
          <b>[!UICONTROL AB Activity]</b>
          <p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">AB-Aktivität erstellen</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
          <b>[!UICONTROL XT Activity]</b>
          <p>Fahren Sie mit <a href="#xt-activity-fields" class="MCXref xref" >XT-Aktivitätsfeldern</a> fort.</p>
        </li>
        <li>
          <b>[!UICONTROL AP Activity]</b>
          <p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_2">AP-Aktivität erstellen</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
        <li>
          <b>[!UICONTROL Antwort-Token]</b>
          <p>Weitere Informationen zu Feldern finden Sie unter <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Response-tokens/operation/createResponseToken">Antwort-Token erstellen</a> in der Dokumentation zur Adobe Target-API.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

<!--

##### AB Activity fields

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this activity. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Options]</td>
      <td>
        <p>For each option that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the option across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the option. The name must be no more than 250 characters.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Offer ID]</b>
            </p>
          </li>
          <li>
            <p>Select or map the Offer associated with the option.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Mboxes]</td>
      <td>
        <p>For each Mbox that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selectors]</td>
      <td>
        <p>For each selector that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and fill in the following fields:</p>
        <ul>
          <li>
            <p>[!UICONTROL Audience IDs]</p>
            <p>For each audience that you want to add to the Mbox, click <b>[!UICONTROL Add item]</b> and select the Audience ID.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Selector]</b>
            </p>
            <p>Enter or map a string to be used to track the location across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map a name for the Location. The name must be no more than 250 characters.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Experiences]</td>
      <td>
        <p>A list of locations on the page where the content offer is served. A location contains the following:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience local ID]</b>
            </p>
            <p>Enter or map the ID of the experience</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Enter or map the name of the experience
</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>For each audience that you want to see the experience, click <b>[!UICONTROL Add item]</b> and enter the Audience ID.
</p>
          </li>
          <li>
            <p><b>[!UICONTROL Visitor Percentage]</b>
            </p>
            <p>Enter or map the percentage of visitors that is allocated to the experience</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metrics]</td>
      <td><p>For details on metrics, see <a href="https://developer.adobe.com/target/administer/admin-api/#tag/Activities/operation/createActivity_4_1">Create AB activity</a> in the Adobe Target API documentation.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Third Party ID]</td>
      <td>Enter or map an ID to identify this activity. You can choose this ID. This ID must not be the same as another activity, and can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starts at]</td>
      <td>Enter or map the date and time to start the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Ends at]</td>
      <td>Enter or map the date and time to end the activity in the format <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Enter or map the state of the activity.</p>
        <ul>
          <li>
            <p>[!UICONTROL Approved]</p>
          </li>
          <li>
            <p>[!UICONTROL Deactivated]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL Saved] </p>
          </li>
          <li>
            <p>[!UICONTROL Deleted]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Enter a number that defines the priority of the activity. Higher numbers have higher priority. This value must be between 0 and 999. The default value is 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auto-allocate traffic]</td>
      <td>
        <p>Enable this option to auto-allocate traffic. Auto-allocating sends more traffic to the more successful experience.</p>
        <p>Select or map the evaluation criteria by which to judge which experience is more successful.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Enter or map the workspace that the activity is associated with</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Property IDs] </td>
      <td>For each property that you want to add to the activity, click <b>[!UICONTROL Add item]</b> and select or map the property's ID.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reporting audiences]</td>
      <td>
        <p>For each reporting audience that you want to add to the activity, click [!UICONTROL Add item] and enter the following information:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the Reporting Audience across API requests.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Audience ID]</b>
            </p>
            <p>Enter or map the Segment to be used in reporting</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metric local ID]</b>
            </p>
            <p>Enter or map a string to be used to track the metric across API requests.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

##### XT-Aktivitätsfelder

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Geben Sie einen Namen für diese Aktivität ein oder ordnen Sie ihn zu. Der Name darf maximal 250 Zeichen lang sein.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Optionen]</td>
      <td>
        <p>Klicken Sie für jede Option, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie die folgenden Felder aus:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Option local ID]</b>
            </p>
            <p>Geben Sie eine Zeichenfolge ein oder ordnen Sie sie zu, um die Option über API-Anfragen hinweg zu verfolgen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Geben Sie einen Namen für die Option ein oder ordnen Sie ihn zu. Der Name darf maximal 250 Zeichen lang sein.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Angebots-ID]</b>
            </p>
          </li>
          <li>
            <p>Wählen Sie die der Option zugeordnete Angebot aus oder ordnen Sie sie zu.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Standorte]</td>
      <td>
        <p>Klicken Sie für jede Mbox, die Sie zur Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie die folgenden Felder aus:</p>
        <ul>
          <li>
            <p>[!UICONTROL Zielgruppen-IDs]</p>
            <p>Klicken Sie für jede Zielgruppe, die Sie zur Mbox hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die Zielgruppen-ID aus.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Ortskennung]</b>
            </p>
            <p>Geben Sie eine Zeichenfolge ein oder ordnen Sie sie zu, um den Standort über API-Anfragen hinweg zu verfolgen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Geben Sie einen Namen für den Standort ein oder ordnen Sie ihn zu. Der Name darf maximal 250 Zeichen lang sein.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Erlebnisse]</td>
      <td>
        <p>Eine Liste der Stellen auf der Seite, an denen das Inhaltsangebot bereitgestellt wird. Ein Speicherort enthält Folgendes:
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Experience Local ID]</b>
            </p>
            <p>Kennungen des Erlebnisses eingeben oder zuordnen</p>
          </li>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Erlebnisname eingeben oder zuordnen

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>Klicken Sie für jede Zielgruppe, die das Erlebnis anzeigen soll, auf "<b>[!UICONTROL Element hinzufügen]</b>"und geben Sie die Zielgruppen-ID ein.

</p>
          </li>
          <li>
            <p><b>[!UICONTROL Besucherprozentsatz]</b>
            </p>
            <p>Geben Sie den Prozentsatz der Besucher ein oder ordnen Sie ihn zu, der dem Erlebnis zugeordnet ist.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Metriken]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Drittanbieter-ID]</td>
      <td>Geben Sie eine ID ein oder ordnen Sie sie zu, um diese Aktivität zu identifizieren. Sie können diese ID auswählen. Diese ID darf nicht mit einer anderen Aktivität übereinstimmen und darf nicht mehr als 250 Zeichen umfassen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Beginnt am]</td>
      <td>Geben Sie Datum und Uhrzeit für den Start der Aktivität im Format <code>YYYY-MM-DD hh:mm:ss.z</code> ein oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Endet am]</td>
      <td>Geben Sie Datum und Uhrzeit ein oder ordnen Sie sie dem Ende der Aktivität im Format <code>YYYY-MM-DD hh:mm:ss.z</code> zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL State]</td>
      <td>
        <p>Geben Sie den Status der Aktivität ein oder ordnen Sie ihn zu.</p>
        <ul>
          <li>
            <p>[!UICONTROL Genehmigt]</p>
          </li>
          <li>
            <p>[!UICONTROL Deaktiviert]</p>
          </li>
          <li>
            <p>[!UICONTROL Paused]</p>
          </li>
          <li>
            <p>[!UICONTROL gespeichert] </p>
          </li>
          <li>
            <p>[!UICONTROL gelöscht]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Geben Sie eine Zahl ein, die die Priorität der Aktivität definiert. Höhere Zahlen haben höhere Priorität. Dieser Wert muss zwischen 0 und 999 liegen. Der Standardwert ist 5.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Automatisch zuordnender Traffic]</td>
      <td>
        <p>Aktivieren Sie diese Option, um Traffic automatisch zuzuweisen. Die automatische Zuordnung sendet mehr Traffic an das erfolgreichere Erlebnis.</p>
        <p>Wählen Sie die Bewertungskriterien aus oder ordnen Sie sie zu, anhand derer beurteilt werden soll, welches Erlebnis erfolgreicher ist.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Arbeitsbereich eingeben oder zuordnen, dem die Aktivität zugeordnet ist</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Eigenschaften-IDs] </td>
      <td>Klicken Sie für jede Eigenschaft, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die ID der Eigenschaft aus oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichterstellungszielgruppen]</td>
      <td>
        <p>Klicken Sie für jede Reporting-Zielgruppe, die Sie zur Aktivität hinzufügen möchten, auf [!UICONTROL Element hinzufügen] und geben Sie die folgenden Informationen ein:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Lokale ID der Berichterstellungszielgruppe]</b>
            </p>
            <p>Geben Sie eine Zeichenfolge ein oder ordnen Sie sie zu, um die Berichterstellungszielgruppe über API-Anfragen hinweg zu verfolgen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Zielgruppen-ID]</b>
            </p>
            <p>Eingeben oder Zuordnen des Segments für die Berichterstellung</p>
          </li>
          <li>
            <p><b>[!UICONTROL Metrik, lokale ID]</b>
            </p>
            <p>Geben Sie eine Zeichenfolge ein oder ordnen Sie sie zu, um die Metrik über API-Anfragen hinweg zu verfolgen.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Angebotsfelder

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Geben Sie einen Namen für diese Aktivität ein oder ordnen Sie ihn zu. Der Name darf maximal 250 Zeichen lang sein.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Geben Sie den Inhalt des Angebots ein oder ordnen Sie ihn dem Benutzer zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Geben Sie die Kennung des mit dem Angebot verknüpften Arbeitsbereichs ein oder ordnen Sie sie zu. Wenn Sie das Feld leer lassen, wird das Angebot mit dem Standardarbeitsbereich des Kontos verknüpft. Diese Funktion gilt nur für [!DNL Target] Premium-Konten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Geben Sie Datum und Uhrzeit der Änderung dieses Angebots ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

<!--

##### Audience fields

>[!NOTE]
>
>Audiences created through Workfront Fusion can only be edit in Fusion or through the API. They cannot be edited from within Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Enter or map a name for this audience. The name can be no more than 250 characters.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Description]</td>
      <td>
        <p>Enter or map a description of this audience.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Origin]</td>
      <td>
        <p>Select whether this audience's origin is from Target or from the cloud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target Rule]</td>
      <td>
        <p>Enable the toggle to make rules AND, that is, all rules must be applied.</p>
        <p>For each rule that you want to apply to the audience, click <b>[!UICONTROL Add item]</b> and enter the JSON of the rule you want to apply. </p>
        <div class="example"><span class="autonumber"><span><b>Example: </b></span></span>
          <p>Example 1:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p>Example 2</p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>Enter or map the ID of the workspace associated with the audience. If left blank, the offer is associated with the default workspace of the account. This functionality applies only to [!DNL Target Premium] accounts.</p>
      </td>
    </tr>
  </tbody>
</table>

-->

#### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Target] -API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Basis-URL]</td>
      <td>Geben Sie Ihre Basis-URL für [!DNL Target] ein oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu {baseURL}/ ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungs-Header und x-api-key-Header hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht eine einzelne AB-Aktivität, XT-Aktivität, Angebot oder Zielgruppe.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
    <td>Geben Sie die Kennung des Datensatzes ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul ruft Daten für eine einzelne Aktivität, ein Angebot, eine Zielgruppe, eine Eigenschaft oder einen Bericht ab.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ des Datensatzes aus, den Sie lesen möchten.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
    <td>Geben Sie die Kennung des Datensatzes ein, den Sie lesen möchten, oder ordnen Sie sie zu.</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen Datensatz in Target.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record Type]</td>
      <td>
        <p>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</p>
       </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Feldnamen]</td>
      <td>Wählen Sie die zu aktualisierenden Felder aus. Die Felder werden unten angezeigt.
          <p>Weitere Informationen zu Feldern finden Sie in der Dokumentation zur Adobe Target-API </a>.<a href="https://developer.adobe.com/target/administer/admin-api/"></p>
      </td>
    </tr>
  </tbody>
</table>

### Suchvorgänge

* [[!UICONTROL Abrufen von Datensätzen]](#get-records)

* [[!UICONTROL Suche]](#search)


#### [!UICONTROL Abrufen von Datensätzen]

Dieses Suchmodul ruft eine Liste von Datensätzen des ausgewählten Typs ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record Type]</td>
      <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">Sortieren nach</td>
      <td>Klicken Sie für jedes Feld, nach dem Sie sortieren möchten, auf "<b>[!UICONTROL Element hinzufügen]</b>"und wählen Sie das Feld aus und ob die zurückgegebenen Ergebnisse auf- oder absteigend sein sollen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL startet am]</td>
      <td>
        <p>Geben Sie das früheste Datum ein, für das Sie Datensätze abrufen möchten. </p>
        <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL endet am]</td>
      <td>
        <p>Geben Sie das Datum ein, für das Sie Datensätze abrufen möchten. </p>
        <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Suche]

Dieses Suchmodul sucht nach Aktivitäten, Angeboten oder Zielgruppen basierend auf von Ihnen festgelegten Kriterien.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Target]</a> .</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td>
  </tr>
  <tr>
    <td role="rowheader">Sortieren nach</td>
    <td>Klicken Sie für jedes Feld, nach dem Sie sortieren möchten, auf "<b>[!UICONTROL Element hinzufügen]</b>"und wählen Sie das Feld aus und ob die zurückgegebenen Ergebnisse auf- oder absteigend sein sollen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Suchkriterien]</td>
    <td>Wählen Sie für jede Regel, die Sie einrichten möchten, das Feld, den Operator und den Wert aus. Klicken Sie auf <b>[!UICONTROL Add AND rule]</b> , um zusätzliche Regeln zu erstellen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Geben Sie die Nummer der ersten Antwort ein, die das Modul zurückgeben soll. Die erste zurückgegebene Antwort hat den Versatz <code>0</code>. Verwenden Sie dieses Feld in Kombination mit dem Feld [!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen] , um die Antworten zu paginieren.</p>
      <p>Um beispielsweise die dritte Antwortseite anzuzeigen, wenn jede Seite zehn Antworten enthält, setzen Sie [!UICONTROL Offset] auf 20 und [!UICONTROL Maximale Anzahl der zurückgegebenen] Ergebnisse auf 10.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]</td>
    <td>
      <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll. Verwenden Sie dieses Feld in Kombination mit dem Feld [!UICONTROL Offset] , um die Antworten zu paginieren.</p>
      <p>Um beispielsweise die dritte Antwortseite anzuzeigen, wenn jede Seite zehn Antworten enthält, setzen Sie [!UICONTROL Offset] auf 20 und [!UICONTROL Maximale Anzahl der zurückgegebenen] Ergebnisse auf 10.</p>
    </td>
  </tr>
</tbody>
</table>
