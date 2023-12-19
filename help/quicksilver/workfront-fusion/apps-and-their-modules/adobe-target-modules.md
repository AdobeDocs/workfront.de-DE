---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] -Module ermöglichen es Ihnen, Datensätze eines bestimmten Typs zu erstellen, zu lesen, zu aktualisieren oder zu löschen, alle Datensätze eines bestimmten Typs aufzulisten, Datensätze anhand von von Kriterien zu suchen oder einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Target] API.
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: c0be0a1f21d5db3a480485a39e019a129d248574
workflow-type: tm+mt
source-wordcount: '2665'
ht-degree: 0%

---

# [!DNL Adobe Target] Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Target], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her. [!DNL Adobe Target] -Module ermöglichen es Ihnen, Datensätze eines bestimmten Typs aufzulisten, zu erstellen, zu lesen, zu aktualisieren oder zu löschen, Suchdatensätze auf der Grundlage der von Ihnen angegebenen Kriterien zu erstellen, zu aktualisieren oder einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Target] API.


Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
    </tr>
  </tbody>
</table>


Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Bevor Sie die [!DNL Adobe Target] müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über eine aktive [!DNL Adobe Target] -Konto.

## Erstellen Sie eine Verbindung zu [!DNL Adobe Target]

So erstellen Sie eine Verbindung für [!DNL Adobe Target] -Module:

1. Klicks **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

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
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client-ID. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Client Secret. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Organisations-ID. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
        <td>Geben Sie Ihre [!DNL Adobe] Kennung des technischen Kontos. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Mandant]</td>
        <td>
          <p> Um Ihren Mandanten zu finden, melden Sie sich bei [!DNL Adobe Experience Cloud], öffnen [!DNL Target]und klicken Sie auf [!DNL Target] Karte. Verwenden Sie den Wert der Mandanten-ID, wie in der URL-Subdomäne angegeben.</p>
          <p>Wenn beispielsweise Ihre URL bei [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> lautet dann Ihre Mandantenkennung "mycompany".</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>Eingabe <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
        <td>
          <p>Geben Sie den privaten Schlüssel ein, der beim Erstellen Ihrer Anmeldedaten im [!DNL Adobe Developer Console]. </p>
          <p>So extrahieren Sie Ihren privaten Schlüssel oder Ihr Zertifikat:</p>
          <ol>
            <li value="1">
              <p>Klicks <b>[!UICONTROL Extract]</b>.</p>
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
              <p>Klicks <b>[!UICONTROL Save]</b> , um die Datei zu extrahieren und zur Verbindungseinrichtung zurückzukehren.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Target] Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Target] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Target] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)

* [Suchvorgänge](#searches)


### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)

* [[!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]](#make-a-custom-api-call)

* [[!UICONTROL Datensatz löschen]](#delete-a-record)

* [[!UICONTROL Datensatz lesen]](#read-a-record)

* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)


#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt eine AB- oder XT-Aktivität, ein Angebot oder eine Zielgruppe.

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Record Type]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p>
      <ul>
        <li>
          <p>[!UICONTROL AB Activity]</p>
          <p>Weiter zu <a href="#ab-activity-fields" class="MCXref xref" >AB-Aktivitätsfelder</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT-Aktivität]</p>
          <p>Weiter zu <a href="#xt-activity-fields" class="MCXref xref" >XT-Aktivitätsfelder</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Angebot]</p>
          <p>Weiter zu <a href="#offer-fields" class="MCXref xref" >Angebotsfelder</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL Audience]</p>
          <p>Weiter zu <a href="#audience-fields" class="MCXref xref" >Zielgruppenfelder</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB-Aktivitätsfelder

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
        <p>Klicken Sie für jede Option, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie folgende Felder aus:</p>
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
        <p>Klicken Sie für jede Mbox, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie folgende Felder aus:</p>
        <ul>
          <li>
            <p>[!UICONTROL Zielgruppen-IDs]</p>
            <p>Klicken Sie für jede Zielgruppe, die Sie zur Mbox hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die Zielgruppen-ID aus.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
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
            <p>Klicken Sie für jede Zielgruppe, die das Erlebnis anzeigen soll, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die Zielgruppen-ID ein.

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
      <td>Datum und Uhrzeit des Aktivitätsbeginns im Format eingeben oder zuordnen <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Endet am]</td>
      <td>Datum und Uhrzeit des Endes der Aktivität im Format eingeben oder zuordnen <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
      <td>Klicken Sie für jede Eigenschaft, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die Kennung der Eigenschaft aus oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Berichterstellungszielgruppen]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Klicken Sie für jede Reporting-Zielgruppe, die Sie zur Aktivität hinzufügen möchten, auf [!UICONTROL Element hinzufügen] und geben Sie die folgenden Informationen ein:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
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
        <p>Klicken Sie für jede Option, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie folgende Felder aus:</p>
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
        <p>Klicken Sie für jede Mbox, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie folgende Felder aus:</p>
        <ul>
          <li>
            <p>[!UICONTROL Zielgruppen-IDs]</p>
            <p>Klicken Sie für jede Zielgruppe, die Sie zur Mbox hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die Zielgruppen-ID aus.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Location local ID]</b>
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
            <p>Klicken Sie für jede Zielgruppe, die das Erlebnis anzeigen soll, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die Zielgruppen-ID ein.

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
      <td>Datum und Uhrzeit des Aktivitätsbeginns im Format eingeben oder zuordnen <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Endet am]</td>
      <td>Datum und Uhrzeit des Endes der Aktivität im Format eingeben oder zuordnen <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
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
      <td>Klicken Sie für jede Eigenschaft, die Sie der Aktivität hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie die Kennung der Eigenschaft aus oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Berichterstellungszielgruppen]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Klicken Sie für jede Reporting-Zielgruppe, die Sie zur Aktivität hinzufügen möchten, auf [!UICONTROL Element hinzufügen] und geben Sie die folgenden Informationen ein:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Reporting Audience local ID]</b>
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
  </tbody>
</table>

##### Zielgruppenfelder

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Geben Sie einen Namen für diese Zielgruppe ein oder ordnen Sie ihn zu. Der Name darf maximal 250 Zeichen lang sein.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content]</td>
      <td>
        <p>Geben Sie eine Beschreibung dieser Audience ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Target-Regel]</td>
      <td>
        <p>Aktivieren Sie den Umschalter, um Regeln zu erstellen UND, d. h. alle Regeln müssen angewendet werden.</p>
        <p>Klicken Sie für jede Regel, die Sie auf die Zielgruppe anwenden möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die JSON-Datei der Regel ein, die Sie anwenden möchten. </p>
        <div class="example"><span class="autonumber"><span><b>Beispiel: </b></span></span>
          <p>Beispiele:</p>
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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>Geben Sie die Kennung des Arbeitsbereichs ein, der mit der Zielgruppe verknüpft ist, oder ordnen Sie sie zu. Wenn Sie das Feld leer lassen, wird das Angebot mit dem Standardarbeitsbereich des Kontos verknüpft. Diese Funktion gilt nur für [!DNL Target Premium] Konten.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Target] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] Basis-URL]</td>
      <td>Geben Sie Ihre [!DNL Target] Basis-URL.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu ein {baseURL}/</p>
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
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
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
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
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
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

Dieses Aktionsmodul aktualisiert eine Aktivität, ein Angebot oder eine Zielgruppe.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record Type]</td>
      <td>
        <p>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB Activity]</b>
            </p>
            <p>Siehe Feldbeschreibungen in <a href="#ab-activity-fields" class="MCXref xref" >AB-Aktivitätsfelder</a> under <a href="#create-a-record" class="MCXref xref" >Datensatz erstellen</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT-Aktivität]</b>
            </p>
            <p>Siehe Feldbeschreibungen in <a href="#xt-activity-fields" class="MCXref xref" >XT-Aktivitätsfelder</a> under <a href="#create-a-record" class="MCXref xref" >Datensatz erstellen</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Sonstige Aktivität]</b>
            </p>
            <p>Wählen Sie das Feld aus, für das Sie einen Wert aktualisieren möchten, und geben Sie dann den neuen Wert für das Feld ein.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Angebot]</b>
            </p>
            <p>Siehe Feldbeschreibungen in <a href="#offer-fields" class="MCXref xref" >Angebotsfelder</a> under <a href="#create-a-record" class="MCXref xref" >Datensatz erstellen</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>Siehe Feldbeschreibungen in <a href="#audience-fields" class="MCXref xref" >Zielgruppenfelder</a> under <a href="#create-a-record" class="MCXref xref" >Datensatz erstellen</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
      <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td>
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
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record Type]</td>
      <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">Sortieren nach</td>
      <td>Klicken Sie für jedes Feld, nach dem Sie sortieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie das Feld aus und ob die zurückgegebenen Ergebnisse aufsteigend oder absteigend sein sollen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL startet am]</td>
      <td>
        <p>Geben Sie das früheste Datum ein, für das Sie Datensätze abrufen möchten. </p>
        <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL endet am]</td>
      <td>
        <p>Geben Sie das Datum ein, für das Sie Datensätze abrufen möchten. </p>
        <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
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
    <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Target], siehe <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Target]</a> in diesem Artikel.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td>
  </tr>
  <tr>
    <td role="rowheader">Sortieren nach</td>
    <td>Klicken Sie für jedes Feld, nach dem Sie sortieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie das Feld aus und ob die zurückgegebenen Ergebnisse aufsteigend oder absteigend sein sollen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Suchkriterien]</td>
    <td>Wählen Sie für jede Regel, die Sie einrichten möchten, das Feld, den Operator und den Wert aus. Klicks <b>[!UICONTROL Add AND rule]</b> , um zusätzliche Regeln zu erstellen.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Offset]</td>
    <td>
      <p>Geben Sie die Nummer der ersten Antwort ein, die das Modul zurückgeben soll. Die erste zurückgegebene Antwort hat den Versatz <code>0</code>. Verwenden Sie dieses Feld in Kombination mit dem Feld [!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen] , um die Antworten zu paginieren.</p>
      <p>Um beispielsweise die dritte Antwortseite anzuzeigen, wenn jede Seite zehn Antworten enthält, setzen Sie [!UICONTROL Offset] auf 20 und [!UICONTROL Maximale Anzahl der zurückgegebenen] Ergebnisse auf 10.</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll. Verwenden Sie dieses Feld in Kombination mit dem Feld [!UICONTROL Offset] , um die Antworten zu paginieren.</p>
      <p>Um beispielsweise die dritte Antwortseite anzuzeigen, wenn jede Seite zehn Antworten enthält, setzen Sie [!UICONTROL Offset] auf 20 und [!UICONTROL Maximale Anzahl der zurückgegebenen] Ergebnisse auf 10.</p>
    </td>
  </tr>
</tbody>
</table>
