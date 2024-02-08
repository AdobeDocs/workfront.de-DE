---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Journey Optimizer], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 50078aec71a4173a67c386ae5a8a4b5ba6cf3ade
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Module

<!--
Becky: pull from main, add to TOCs, then push to merge.
-->

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Adobe Journey Optimizer], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her. [!DNL Adobe Journey Optimizer] -Module ermöglichen es Ihnen, Datensätze zu erstellen, zu lesen, zu aktualisieren, zu löschen oder einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Journey Optimizer] API.


Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table>
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
  </tbody>
</table>


Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Bevor Sie die [!DNL Adobe Journey Optimizer] müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über eine aktive [!DNL Adobe Journey Optimizer] -Konto.

## Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]

So erstellen Sie eine Verbindung für [!DNL Adobe Journey Optimizer] -Module:

1. In jeder [!DNL Adobe Journey Optimizer] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

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
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client Secret]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Technische Konto-ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Organisations-ID]</td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID]. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] im Abschnitt [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Meta-Bereiche]</td>
          <td>
            Geben Sie die für die Verbindung erforderlichen Metadatenbereiche ein.
          </td>
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

## [!DNL Adobe Journey Optimizer] Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Journey Optimizer] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Journey Optimizer] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]](#make-a-custom-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt eine Platzierung, Entscheidungsregel, ein Tag, ein personalisiertes Angebot, eine Sammlung oder ein Fallback-Angebot.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Wählen Sie den zu erstellenden Datensatztyp aus
        <ul>
        <li><b>[!UICONTROL Platzierung]</b>: Fahren Sie mit <a href="#placement-fields" >[!UICONTROL Platzierungsfelder]</a>.</li>
        <li><b>[!UICONTROL Entscheidungsregel]</b>: Fahren Sie mit <a href="#decision-rule-fields" >Felder für [!UICONTROL Entscheidungsregel]</a>.</li>
        <li><b>[!UICONTROL Entscheidung]</b>: Fahren Sie mit <a href="#decision-fields" >[!UICONTROL Entscheidungsfelder</a>.</li>
        <li><b>[!UICONTROL Tag]</b>: Fahren Sie mit <a href="#tag-fields" >Felder des [!UICONTROL Tags]</a>.</li>
        <li><b>[!UICONTROL Sammlung]</b>: Fahren Sie mit <a href="#collection-fields" >[!UICONTROL Kollektionsfelder]</a>.</li>
        <li><b>[!UICONTROL Fallback-Angebot]</b>: Fahren Sie mit <a href="#fallback-offer-fields" >[!UICONTROL Fallback-Angebot]-Felder</a>.</li>
        <li><b>[!UICONTROL Personalisiertes Angebot]</b>: Fahren Sie mit <a href="#personalized-offer-fields" >Felder für personalisierte Angebote</a>.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Platzierung] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für die Platzierung ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Beschreibung]
      </td>
      <td>Geben Sie eine Beschreibung für die Platzierung ein oder ordnen Sie sie zu.
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL Entscheidungsregel] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für die Beschreibungsregel ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Beschreibung]
      </td>
      <td>Geben Sie eine Beschreibung für die Entscheidungsregel ein oder ordnen Sie sie zu.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Bedingung]
      </td>
      <td>Geben Sie die Bedingung der Entscheidungsregel ein oder ordnen Sie sie zu.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Entscheidung] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für die Beschreibungsregel ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Wählen Sie den Status für die Entscheidung aus.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Startdatum]</td>
      <td><p>Geben Sie das Startdatum für die Entscheidung ein oder ordnen Sie es zu.</p><p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Enddatum]</td>
      <td><p>Geben Sie das Enddatum für die Entscheidung ein oder ordnen Sie es zu.</p><p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Praktika]</td>
      <td>Auswählen der Platzierungen, die dieser Entscheidung hinzugefügt werden sollen
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Sammlung]</td>
      <td>Wählen Sie die Angebotskollektion aus, die die Angebote enthält, die bei dieser Entscheidung berücksichtigt werden sollen.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Fallback-Angebot]</td>
      <td>Wählen Sie das Fallback-Angebot aus, das Kunden unterbreitet wird, die nicht mit den Regeln für diese Entscheidung übereinstimmen.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Tag] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für das Tag ein oder ordnen Sie ihn zu.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Sammlung] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für die Sammlung ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Filtertyp]
      </td>
      <td>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Elemente]
      </td>
      <td>Wählen Sie die Tags aus, die in die Sammlung aufgenommen werden sollen.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Fallback-Angebot] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für das Fallback-Angebot ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Status]
      </td>
      <td> Wählen Sie den Status des Fallback-Angebots aus.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Platzierung]
      </td>
      <td>Geben Sie die Platzierung für das Fallback-Angebot ein oder ordnen Sie es zu.
      </td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL Personalisiertes Angebot] fields

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
     <td>Geben Sie einen Namen für die Beschreibungsregel ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Status]</td>
      <td>Wählen Sie den Status für die Entscheidung aus.
      </td>
    </tr>
    <tr>
      <td role="rowheader">Platzierung</td>
      <td>Wählen Sie die Platzierung für das personalisierte Angebot aus.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Startdatum]</td>
      <td><p>Geben Sie das Startdatum für das personalisierte Angebot ein oder ordnen Sie es zu.</p><p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Enddatum]</td>
      <td><p>Geben Sie das Enddatum für das personalisierte Angebot ein oder ordnen Sie es zu.</p><p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typenkonvertierung in [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Entscheidungsregeln]</td>
      <td>Wählen Sie die Entscheidungsregeln aus, die diesem personalisierten Angebot hinzugefügt werden sollen.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Priority]</td>
      <td>Wählen Sie die Priorität dieses Angebots aus. Die Priorität wirkt sich darauf aus, ob dieses Angebot statt eines anderen Angebots unterbreitet wird.
      </td>
    </tr>
   <tr>
      <td role="rowheader">[!UICONTROL Begrenzung]</td>
      <td>Geben Sie ein oder ordnen Sie die Anzahl der Vorschläge für dieses Angebot zu.
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen einzelnen Datensatz in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Wählen Sie den zu löschenden Datensatztyp aus
        <ul>
        <li>[!UICONTROL Platzierung]</li>
        <li>[!UICONTROL Entscheidungsregel]</li>
        <li>[!UICONTROL Entscheidung]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Sammlung]</li>
        <li>[!UICONTROL Fallback-Angebot]</li>
        <li>[!UICONTROL Personalisiertes Angebot]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Platzierung]/[!UICONTROL Entscheidungsregel]/[!UICONTROL Entscheidung]/[!UICONTROL Tag]/[!UICONTROL Kollektion]/[!UICONTROL Fallback-Angebot]/[!UICONTROL Personalisiertes Angebot]
      </td>
      <td>
        Wählen Sie den Datensatz aus, den Sie löschen möchten.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Journey Optimizer] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu ein {baseURL} beginnt mit<code>/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion fügt Autorisierungs-Header und x-api-Schlüssel-Header automatisch hinzu.</p>
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
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Ergebnissen an, die das Modul in einem Ausführungszyklus zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen einzelnen Datensatz in [!DNL Adobe Journey Optimizer].

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Wählen Sie den zu löschenden Datensatztyp aus
        <ul>
        <li>[!UICONTROL Platzierung]</li>
        <li>[!UICONTROL Entscheidungsregel]</li>
        <li>[!UICONTROL Entscheidung]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Sammlung]</li>
        <li>[!UICONTROL Fallback-Angebot]</li>
        <li>[!UICONTROL Personalisiertes Angebot]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Platzierung]/[!UICONTROL Entscheidungsregel]/[!UICONTROL Entscheidung]/[!UICONTROL Tag]/[!UICONTROL Kollektion]/[!UICONTROL Fallback-Angebot]/[!UICONTROL Personalisiertes Angebot]
      </td>
      <td>
        Wählen Sie den Datensatz aus, den Sie löschen möchten.
      </td>
    </tr>

</tbody>
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul erstellt eine Platzierung, eine Entscheidung, eine Entscheidungsregel, ein Tag, ein personalisiertes Angebot, eine Sammlung oder ein Fallback-Angebot.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Record Type]
      </td>
      <td>
        Wählen Sie den zu aktualisierenden Datensatztyp aus
        <ul>
        <li>[!UICONTROL Platzierung]</li>
        <li>[!UICONTROL Entscheidungsregel]</li>
        <li>[!UICONTROL Entscheidung]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Sammlung]</li>
        <li>[!UICONTROL Fallback-Angebot]</li>
        <li>[!UICONTROL Personalisiertes Angebot]</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Platzierung]/[!UICONTROL Entscheidungsregel]/[!UICONTROL Entscheidung]/[!UICONTROL Tag]/[!UICONTROL Kollektion]/[!UICONTROL Fallback-Angebot]/[!UICONTROL Personalisiertes Angebot]
      </td>
      <td>
        Wählen Sie den zu aktualisierenden Datensatz aus.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        [!UICONTROL Felder]
      </td>
      <td>Für jedes Feld, das Sie aktualisieren möchten:
      <ol>
      <li>Klicks <b>[!UICONTROL Hinzufügen]</b>.</li>
      <li>Wählen Sie aus, ob Sie Werte hinzufügen, ersetzen oder entfernen möchten.</li>
      <li>Geben Sie das Feld ein, das Sie aktualisieren möchten.</li>
      <li>Geben Sie den neuen Wert für das Feld ein.</li>
      </td>
    </tr>

</tbody>
</table>


### Suchvorgänge

#### [!UICONTROL Auflisten von Datensätzen]

Dieses Suchmodul listet Datensätze des ausgewählten Typs auf und gibt Ergebnisse basierend auf von Ihnen festgelegten Kriterien zurück.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
     <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer], siehe <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Journey Optimizer]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record Type]</p>
      </td>
      <td>
        <p>Wählen Sie den Typ des Datensatzes aus, den Sie auflisten möchten.</p>
        <ul>
        <li>[!UICONTROL Platzierung]</li>
        <li>[!UICONTROL Entscheidungsregel]</li>
        <li>[!UICONTROL Entscheidung]</li>
        <li>[!UICONTROL Tag]</li>
        <li>[!UICONTROL Sammlung]</li>
        <li>[!UICONTROL Fallback-Angebot]</li>
        <li>[!UICONTROL Personalisiertes Angebot]</li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Query operator]</p>
      </td>
      <td>
        <p>Wählen Sie einen Operator aus, der auf die Parameter in der Abfrage angewendet werden soll</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Felder]</td>
      <td><p>Wenn Sie die Suche auf bestimmte Felder beschränken möchten, geben Sie die Felder ein. Klicken Sie für jedes Feld, auf das Sie die Suche beschränken möchten, auf [!UICONTROL Element hinzufügen] und geben Sie den Namen des Felds ein.</p><p>Pfadausdrücke haben die Form von durch Punkte getrennten Pfaden, z. B. <code>_instance.xdm:name</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reihenfolge nach] </td>
      <td>Geben Sie die Eigenschaft ein oder ordnen Sie sie zu, nach der Sie die Ergebnisse sortieren möchten.
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Auftragsrichtung]</td>
   <td>Wählen Sie aus, ob die Ergebnisse in auf- oder absteigender Richtung sortiert werden sollen.
    </td>
     </tr>
  </tbody>
</table>
