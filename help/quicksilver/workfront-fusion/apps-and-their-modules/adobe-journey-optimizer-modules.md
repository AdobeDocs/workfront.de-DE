---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Adobe Journey Optimizer] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
hide: true
hidefromtoc: true
source-git-commit: 5c80b8f7c8934500679d31fc15a06fe3789a6f2b
workflow-type: tm+mt
source-wordcount: '3659'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Adobe Journey Optimizer] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. Mit den [!DNL Adobe Journey Optimizer] -Modulen können Sie Datensätze erstellen, lesen, aktualisieren, löschen oder einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Journey Optimizer] -API durchführen.


Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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

+++

## Voraussetzungen

Bevor Sie den Connector [!DNL Adobe Journey Optimizer] verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Journey Optimizer] -Konto verfügen.

## Herstellen einer Verbindung zu Adobe Journey Optimizer

Sie können eine Verbindung in einem beliebigen Adobe Journey Optimizer-Modul erstellen.

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
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen möchten.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organisations-ID]</td>
        <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Organisations-ID] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>


## [!DNL Adobe Journey Optimizer] Module und ihre Felder

Wenn Sie [!DNL Adobe Journey Optimizer] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Journey Optimizer] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Konfigurationsverwaltung](#configuration-management)
* [Package-Verwaltung](#package-management)
* [Datenverwaltung](#record-management)
* [Nachrichtenverwaltung](#message-management)
* [Statusprüfungen](#status-checks)
* [Suchvorgänge](#searches)
* [Sonstige](#other)




### Konfigurationsverwaltung

* [Erstellen einer Konfiguration](#create-a-configuration)
* [Bereitstellen einer Konfiguration](#deploy-a-configuration)
* [Konfiguration aktualisieren](#update-a-configuration)
* [Bereitstellung einer Konfiguration aufheben](#undeploy-a-configuration)
* [Überprüfen, ob die Konfiguration bereitgestellt werden kann](#check-if-configuration-can-be-deployed)
* [Konfiguration löschen](#delete-a-configuration)
* [Konfiguration abrufen](#get-a-configuration)

#### Erstellen einer Konfiguration

Dieses Aktionsmodul erstellt eine Begrenzungsendpunkt- oder Einschränkungskonfiguration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration erstellen.<ul><li><p><b>Begrenzung</b></p>Fahren Sie mit <a href="#capping-fields" class="MCXref xref" >Feldbegrenzung</a> fort.</li><li><p><b>Einschränken</b></p>Fahren Sie mit <a href="#throttling-fields" class="MCXref xref" >Einschränkungsfeldern</a> fort.</li></ul></td> 
  </tr> 
   </tbody> 
</table>

##### Felder begrenzen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie die URL des Endpunkts ein, den Sie konfigurieren möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL IMS-Organisations-ID]</td> 
   <td>Geben Sie die Adobe IMS-ID der Organisation ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methoden]</td> 
   <td>Wählen Sie die in dieser Konfiguration zu verwendenden Methoden aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service]</td> 
   <td>Wählen Sie aus, ob Sie eine Aktion oder eine Datenquelle für diese Konfiguration verwenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale HTTP-Verbindungen]</td> 
   <td>Geben Sie die maximale Anzahl gleichzeitiger Verbindungen an diesen Endpunkt an oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Aufrufe]</td> 
   <td>Geben Sie die maximale Anzahl von Aufrufen ein oder ordnen Sie sie zu, die in dem im Feld Zeitraum angegebenen Zeitraum durchgeführt werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeitraum (Millisekunden)]</td> 
   <td>Geben Sie die Anzahl der Millisekunden ein oder ordnen Sie sie dem Feld Maximale Aufrufe zu.</td> 
  </tr> 
 </tbody> 
</table>

##### Einschränkungsfelder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für diese Konfiguration ein oder ordnen Sie ihn zu.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für diese Konfiguration ein oder ordnen Sie sie zu.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL URL pattern]</td> 
   <td>Geben Sie die URL für den Endpunkt ein, den Sie drosseln möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methoden]</td> 
   <td>Wählen Sie die in dieser Konfiguration zu verwendenden Methoden aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max. Durchsatz]</td> 
   <td>Wählen Sie aus, ob Sie eine Aktion oder eine Datenquelle für diese Konfiguration verwenden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale HTTP-Verbindungen]</td> 
   <td>Geben Sie die maximale Anzahl gleichzeitiger Verbindungen an diesen Endpunkt an oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Aufrufe]</td> 
   <td>Geben Sie den maximalen Durchsatz für diesen Endpunkt ein oder ordnen Sie ihn zu. Dieser Wert muss zwischen 200 und 5000 liegen.</td> 
  </tr> 
 </tbody> 
</table>

#### Bereitstellen einer Konfiguration

Dieses Aktionsmodul stellt die angegebene Begrenzungs- oder Einschränkungskonfiguration bereit.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration bereitstellen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurations-ID]</td> 
   <td>Geben Sie die ID der Konfiguration ein, die Sie bereitstellen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Konfiguration aktualisieren

Dieses Aktionsmodul aktualisiert die angegebene Begrenzungs- oder Einschränkungskonfiguration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration aktualisieren.<ul><li><p><b>Begrenzung</b></p>Informationen zu Feldern finden Sie unter <a href="#capping-fields" class="MCXref xref" >Feldbegrenzung</a> im Abschnitt Konfiguration erstellen dieses Artikels.</li><li><p><b>Einschränken</b></p>Informationen zu Feldern finden Sie unter <a href="#throttling-fields" class="MCXref xref" >Einschränkungsfelder</a> im Abschnitt Konfiguration erstellen dieses Artikels.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### Bereitstellung einer Konfiguration aufheben

Dieses Aktionsmodul hebt die Bereitstellung einer Begrenzungs- oder Einschränkungskonfiguration auf. Der Konfigurationsstatus wird wieder in den Status vor der Bereitstellung (`created` oder `updated`) geändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie die Bereitstellung einer Begrenzungskonfiguration oder einer Einschränkungskonfiguration aufheben.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurations-ID]</td> 
   <td>Geben Sie die ID der Konfiguration ein, deren Bereitstellung Sie aufheben möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Überprüfen, ob die Konfiguration bereitgestellt werden kann

Dieses Aktionsmodul überprüft, ob eine Begrenzungs- oder Einschränkungskonfiguration bereitgestellt werden kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration überprüfen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurations-ID]</td> 
   <td>Geben Sie die ID der Konfiguration ein, die Sie überprüfen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Konfiguration löschen

Dieses Aktionsmodul löscht eine Begrenzungs-Endpunkt- oder Einschränkungskonfiguration.

Wenn die Konfiguration bereitgestellt wurde, muss die Bereitstellung aufgehoben werden, bevor sie gelöscht werden kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurations-ID]</td> 
   <td>Geben Sie die ID der Konfiguration ein, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Konfiguration abrufen

Dieses Aktionsmodul gibt die Begrenzungs- oder Einschränkungskonfiguration zurück, die durch die angegebene ID identifiziert wird. Die aktuelle Definition wird zurückgegeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration abrufen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurations-ID]</td> 
   <td>Geben Sie die ID der Konfiguration ein, die Sie abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>




### Package-Verwaltung

* [Package erstellen](#create-a-package)
* [Aktualisieren eines Pakets](#update-a-package)
* [Löschen eines Pakets](#delete-a-package)
* [Paket nachschlagen](#look-up-a-package)
* [Package importieren](#import-a-package)
* [Publish a package](#publish-a-package)
* [Importe übermitteln](#submit-an-import)



#### Package erstellen

Dieses Aktionsmodul erstellt ein Artefaktpaket mit mehreren Artefakten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für das Paket ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung des Pakets ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ablaufdatum]</td> 
   <td>Geben Sie den Zeitstempel ein oder ordnen Sie ihn zu, der das Ablaufdatum für das Paket definiert. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Pakettyp]</td> 
   <td>Wählen Sie den Pakettyp aus, den Sie erstellen möchten.<ul><li><p><b>Voll</b></p>Das Paket enthält alle Artefakte</p></li><li><p><b>Teilweise</b></p><p>Das Paket enthält nur Artefakte, die Sie hinzufügen. </p></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>Wenn Sie ein Teilpaket erstellen, klicken Sie für jedes Artefakt, das Sie hinzufügen möchten, auf <b>Artefakt hinzufügen</b> und geben Sie die ID, den Typ und den Titel des Artefakts an. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Sandbox]</td> 
   <td>Geben Sie den Namen und die Kennung der IMS-Organisation der Sandbox ein oder ordnen Sie sie zu, die die Elemente enthält, die das Paket enthalten soll.</td> 
  </tr> 
 </tbody> 
</table>

#### Aktualisieren eines Pakets

Dieses Aktionsmodul fügt Artefakte zu einem Paket hinzu oder löscht diese oder aktualisiert Paketmetadaten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion auswählen]</td> 
   <td>Wählen Sie die gewünschte Aktion aus.<ul><li><p><b>Hinzufügen von Artefakten</b></p><p>Klicken Sie für jedes Artefakt, das Sie hinzufügen möchten, auf "<b>Artefakt hinzufügen</b>", geben Sie die ID, den Typ und den Titel des Artefakts an und geben Sie das Ablaufdatum für das Paket ein oder ordnen Sie es zu. </p></li><li><p><b>Artefakt löschen</b></p><p>Klicken Sie für jedes Artefakt, das Sie löschen möchten, auf <b>Artefakt hinzufügen</b> und geben Sie die ID, den Typ und den Titel des Artefakts an. </p></li><li><p><b>Aktualisieren von Metadaten</b></p><p>Geben Sie neue Werte für den Namen, die Beschreibung oder den Namen der Quell-Sandbox oder der IMS-Organisations-ID ein.</p></li></ul></td> 
  </tr> 
 </tbody> 
</table>

#### Löschen eines Pakets

Dieses Aktionsmodul löscht ein Multiartefakt-Paket.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, das Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Paket nachschlagen

Dieses Aktionsmodul ruft Details zum angegebenen Paket ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein oder ordnen Sie es zu, für das Sie Details zurückgeben möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Package importieren

Dieses Aktionsmodul ruft die in Konflikt stehenden Objekte in der angegebenen Ziel-Sandbox ab. Konfliktobjekte stellen ähnliche Objekte dar, die bereits in der Ziel-Sandbox vorhanden sind.

Sie müssen ein Paket veröffentlichen, bevor Sie es importieren können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, das Sie importieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Target-Sandbox]</td> 
   <td>Geben Sie den Namen der Sandbox ein oder ordnen Sie ihn zu, in die Sie das Paket importieren möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Publish a package

Sie müssen ein Paket veröffentlichen, bevor Sie es importieren können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, das Sie veröffentlichen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### Importe übermitteln

Dieses Aktionsmodul sendet einen Import für ein Paket, nachdem Sie Konflikte überprüft und Ersatzteile bereitgestellt haben. Das Ergebnis wird als Payload bereitgestellt, die den Importauftrag für die Ziel-Sandbox startet, wie in der Payload angegeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, das Sie veröffentlichen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für den Importauftrag ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Eine Beschreibung des Importvorgangs eingeben oder zuordnen</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Ziel-Sandbox) Name]</td> 
   <td>Geben Sie den Namen der Sandbox ein oder ordnen Sie ihn zu, an die Sie den Import senden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Ziel-Sandbox) IMS-Organisations-ID]</td> 
   <td>Geben Sie die Adobe IMS-Organisations-ID für die Sandbox ein oder ordnen Sie sie zu, an die Sie den Import senden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source-Sandbox)-ID]</td> 
   <td>Geben Sie die Kennung der Sandbox ein oder ordnen Sie sie zu, die das Paket enthält, das Sie veröffentlichen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source-Sandbox)-Typ]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL (Source-Sandbox)-Link]</td> 
   <td>Geben Sie den Link für das Paket ein, das Sie veröffentlichen möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>


<!--

### Artifact management

* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)

#### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination sandbox]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to copy, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

#### Export Artifacts asynchronously

This action module exports artifacts from the specified sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to export, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



#### Import Artifacts asynchronously

This action module imports a snapshot containing artifacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Snapshot ID]</td> 
   <td>Enter or map the ID of the snapshot you want to import.</td> 
  </tr> 
 </tbody> 
</table>

-->

### Datenverwaltung

* [Datensatz erstellen](#create-a-record)
* [Datensatz aktualisieren](#update-a-record)
* [Datensatz löschen](#delete-a-record)
* [Patch einen Datensatz](#patch-a-record)
* [Datensatz abrufen](#get-a-record)

#### Datensatz erstellen

Dieses Aktionsmodul erstellt eine neue Inhaltsvorlage oder ein neues Inhaltsfragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Inhaltsvorlage oder ein Inhaltsfragment erstellen.<ul><li><p><b>Inhaltsvorlage</b></p>Fahren Sie mit <a href="#template-fields" class="MCXref xref" >Vorlagenfeldern</a> fort.</li><li><p><b>Inhaltsfragment</b></p>Fahren Sie mit <a href="#fragment-fields" class="MCXref xref" >Fragmentfelder</a> fort.</li></ul></td> 
  </tr> 
  </tbody> 
</table>

##### Vorlagenfelder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für diese Inhaltsvorlage ein oder ordnen Sie ihn zu.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für diese Inhaltsvorlage ein oder ordnen Sie sie zu.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td>Wählen Sie den Typ der Vorlage aus, die Sie erstellen möchten.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanäle]</td> 
   <td>Wählen Sie die in dieser Vorlage enthaltenen Kanäle aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ursprung der Inhaltsvorlage]</td> 
   <td>Wählen Sie die Quelle für diese Vorlage aus.</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadaten]</td> 
   <td>Um benutzerdefinierte Eigenschaften in die neue Vorlage einzubeziehen, wählen Sie "Metadaten hinzufügen"aus und geben Sie den Schlüssel und Wert der Metadaten ein oder ordnen Sie sie zu. Wiederholen Sie diesen Vorgang für jedes benutzerdefinierte Feld, das Sie einbeziehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email HTML]</td> 
   <td>Geben Sie die HTML der in dieser Vorlage enthaltenen E-Mail ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Um benutzerdefinierte Eigenschaften in die E-Mail einzuschließen, wählen Sie "Editor-Kontext hinzufügen"und geben Sie den Schlüssel und Wert des Kontexts ein oder ordnen Sie ihn zu. Wiederholen Sie diesen Vorgang für jedes benutzerdefinierte Feld, das Sie einbeziehen möchten.</td> 
  </tr> 
 </tbody> 
</table>

##### Fragmentfelder

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Geben Sie einen Namen für dieses Inhaltsfragment ein oder ordnen Sie ihn zu.</td> 
<tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für dieses Inhaltsfragment ein oder ordnen Sie sie zu.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td>Wählen Sie den Typ der Vorlage aus, die Sie erstellen möchten.</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanäle]</td> 
   <td>Wählen Sie die in dieser Vorlage enthaltenen Kanäle aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltsfragmentursprung]</td> 
   <td>Wählen Sie die Quelle für dieses Fragment aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadaten]</td> 
   <td>Um benutzerdefinierte Eigenschaften in die neue Vorlage einzubeziehen, wählen Sie "Metadaten hinzufügen"aus und geben Sie den Schlüssel und Wert der Metadaten ein oder ordnen Sie sie zu. Wiederholen Sie diesen Vorgang für jedes benutzerdefinierte Feld, das Sie einbeziehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td>Geben Sie den Inhalt des Fragments ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Editor context]</td> 
   <td>Um benutzerdefinierte Eigenschaften in die E-Mail einzuschließen, wählen Sie "Editor-Kontext hinzufügen"und geben Sie den Schlüssel und Wert des Kontexts ein oder ordnen Sie ihn zu. Wiederholen Sie diesen Vorgang für jedes benutzerdefinierte Feld, das Sie einbeziehen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz aktualisieren

Dieses Aktionsmodul aktualisiert eine Inhaltsvorlage oder ein Fragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Begrenzungskonfiguration oder eine Einschränkungskonfiguration aktualisieren.<ul><li><p><b>Vorlage</b></p>Informationen zu Feldern finden Sie unter <a href="#template-fields" class="MCXref xref" >Vorlagenfelder</a> im Abschnitt Datensatz erstellen dieses Artikels.</li><li><p><b>Fragment</b></p>Informationen zu Feldern finden Sie unter <a href="#fragment-fields" class="MCXref xref" >Fragmentfelder</a> im Abschnitt Datensatz erstellen dieses Artikels.</li></ul></td> 
  </tr> 
  </tbody> 
  </table>

#### Datensatz löschen

Dieses Aktionsmodul löscht eine Inhaltsvorlage oder ein Inhaltsfragment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Inhaltsvorlage oder ein Inhaltsfragment löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorlage/Fragment-ID]</td> 
   <td>Geben Sie die Kennung der Vorlage oder des Fragments ein, die/das Sie löschen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Patch einen Datensatz

Dieses Aktionsmodul aktualisiert einen Datensatz mithilfe von PATCH mit dem JSON-Zeigerformat

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Inhaltsvorlage oder ein Inhaltsfragment patchen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorlage/Fragment-ID]</td> 
   <td>Geben Sie die Kennung der Vorlage oder des Fragments ein, die bzw. das Sie patchen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload-Daten]</td> 
   <td>So fügen Sie einen Datensatz zur Payload dieses Patches hinzu: <ol><li>Klicken Sie auf <b>Datensatz hinzufügen</b>.</li><li>Wählen Sie den Vorgang aus: Hinzufügen, Entfernen oder Ersetzen.</li><li>Wählen Sie im Feld Pfad aus, ob Sie den Namen oder die Beschreibung patchen möchten.</li><li> Geben Sie im Feld Von eine Zeichenfolge ein oder ordnen Sie sie zu, die einen JSON-Zeiger-Wert enthält.</li><li>Geben Sie im Feld Wert den Wert ein, der für den Vorgang verwendet werden soll.</li></ol></td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz abrufen

Dieses Aktionsmodul gibt die Inhaltsvorlage oder das Inhaltsfragment zurück, die durch die angegebene ID identifiziert wurden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Inhaltsvorlage oder ein Inhaltsfragment abrufen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorlage/Fragment-ID]</td> 
   <td>Geben Sie die Kennung der Vorlage oder des Fragments ein, die/das Sie abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>


### Nachrichtenverwaltung

* [Trigger einer einmaligen Nachrichtenausführung](#trigger-a-unitary-message-execution)
* [Trigger einer zielgruppenbasierten Nachricht](#trigger-an-audience-based-message)
* [Status einer zielgruppenbasierten Nachricht überprüfen](#check-the-status-for-audience-based-message)



#### Trigger einer einmaligen Nachrichtenausführung

Dieses Aktionsmodul Trigger eine einmalige Nachricht an die von Ihnen angegebenen Empfänger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antrags-ID]</td> 
   <td>Geben Sie die Kennung der mit dieser Nachricht verknüpften Anforderung ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Geben Sie die Kennung der mit dieser Nachricht verknüpften Kampagne ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Empfänger]</td> 
   <td>Klicken Sie für jeden Empfänger, der diese Nachricht erhalten soll, auf "<b>Empfänger hinzufügen</b>" und geben Sie Folgendes ein:
   <ul>
   <li><p><b>Typ</b></p>Wählen Sie <code>aep</code> aus.</li>
   <li><p><b>Benutzer-ID</b></p>Geben Sie die Adobe Experience Platform-Profilkennung des Empfängers ein oder ordnen Sie sie zu.</li>
   <li><p><b>Namespace</b></p>Geben Sie den Adobe Experience Platform Profile-Namespace des Empfängers ein oder ordnen Sie ihn zu.</li>
   <li><p><b>E-Mail-Adresse</b></p></li>
   <li><p><b>Mobiltelefonnummer</b></p></li>
   <li><p><b>Vorname</b></p></li>
   <li><p><b>Nachname</b></p></li>
   <li><p><b>Produkt</b></p>Geben Sie das mit dieser Nachricht verknüpfte Produkt ein oder ordnen Sie es zu. Dies wird zum Ersetzen dynamischer Variablen im Nachrichteninhalt verwendet.</li>
   </ul></td> 
  </tr> 
 </tbody> 
</table>

#### Trigger einer zielgruppenbasierten Nachricht

Dieses Aktionsmodul Trigger die Ausführung einer zielgruppenbasierten Nachricht basierend auf der von Ihnen angegebenen Anforderung und Kampagne.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antrags-ID]</td> 
   <td>Geben Sie die Kennung der mit dieser Nachricht verknüpften Anforderung ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Geben Sie die Kennung der mit dieser Nachricht verknüpften Kampagne ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Produkt]</td> 
   <td>Geben Sie das mit dieser Nachricht verknüpfte Produkt ein oder ordnen Sie es zu. Dies wird zum Ersetzen dynamischer Variablen im Nachrichteninhalt verwendet.</td> 
  </tr> 
 </tbody> 
</table>

#### Prüfen des Status auf zielgruppenbasierte Nachrichten

Dieses Aktionsmodul überprüft den Status einer zielgruppenbasierten Batch-Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-Ausführungs-ID]</td> 
   <td>Geben Sie die Kennung der Nachrichtenausführung ein, die Sie überprüfen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Statusprüfungen

<!--* [Check service health](#check-service-health)-->
* [Überprüfen der Importabhängigkeiten](#check-the-import-dependencies)
* [Status eines Importvorgangs überprüfen](#check-the-status-of-an-import-job)

<!--

#### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

-->

#### Überprüfen der Importabhängigkeiten

Dieses Aktionsmodul überprüft die Abhängigkeiten auf Paketartefakte. Auf diese Weise können Sie überprüfen, ob Sie berechtigt sind, Paketartefakte zu importieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, für das Sie Berechtigungen überprüfen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Target-Sandbox]</td> 
   <td>Geben Sie den Namen der Sandbox ein oder ordnen Sie ihn zu, in die Sie das Paket importieren möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Status eines Importvorgangs überprüfen

Dieses Aktionsmodul prüft, ob ein Importauftrag erfolgreich oder fehlgeschlagen war.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Auftrags-ID]</td> 
   <td>Geben Sie die ID des Auftrags ein oder ordnen Sie sie zu, für den Sie Daten abrufen möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [Alle abhängigen Objekte auflisten](#list-all-dependent-objects)
* [Listenkonfigurationen](#list-configurations)
* [Listen von Export- und Importvorgängen](#list-export-and-import-jobs)
* [Auflisten von Packages](#list-packages)
* [Auflisten von Datensätzen](#list-records)

#### Alle abhängigen Objekte auflisten

Dieses Suchmodul listet alle abhängigen Objekte für Objekte im angegebenen Paket auf

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Paketobjekte]</td> 
   <td>Klicken Sie für jedes Objekt im Paket, für das Sie ein abhängiges Objekt zurückgeben möchten, auf "<b>Objekt hinzufügen</b>"und geben Sie den Namen und den Typ des Objekts ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Package-ID]</td> 
   <td>Geben Sie die Kennung des Pakets ein, für das Sie abhängige Objekte auflisten möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Target-Sandbox]</td> 
   <td>Geben Sie den Namen der Sandbox ein oder ordnen Sie ihn zu, die das Paket enthält, für das Sie abhängige Objekte auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Listenkonfigurationen

Dieses Aktionsmodul listet alle Begrenzungs- oder Einschränkungskonfigurationen auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Konfigurationstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie Begrenzungskonfigurationen oder Einschränkungskonfigurationen auflisten möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### Listen von Export- und Importvorgängen

Dieses Suchmodul listet den aktuellen Export- und Importauftrag auf. Sie können Abfrageparameter verwenden, um die Liste zu filtern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
      <td>Wählen Sie aus, ob die Ergebnisse nach Erstellungsdatum oder Änderungsdatum sortiert werden sollen.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Abfrageparameter]</td> 
   <td>Klicken Sie für jeden Abfrageparameter, nach dem Sie filtern möchten, auf "<b>Abfrageparameter hinzufügen</b>", wählen Sie dann das Feld und den Operator aus und geben Sie den Feldwert für den Filter ein.</td> 
  </tr> 
 </tbody> 
</table>



#### Auflisten von Packages

Dieses Suchmodul listet alle Pakete in Ihrer Organisation auf. Sie können Abfrageparameter verwenden, um die Liste zu filtern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
      <td>Wählen Sie aus, ob die Ergebnisse nach Erstellungsdatum oder Änderungsdatum sortiert werden sollen.</td>
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL Abfrageparameter]</td> 
   <td>Klicken Sie für jeden Abfrageparameter, nach dem Sie filtern möchten, auf "<b>Abfrageparameter hinzufügen</b>", wählen Sie dann das Feld und den Operator aus und geben Sie den Feldwert für den Filter ein.</td> 
  </tr> 
 </tbody> 
</table>

#### Auflisten von Datensätzen

Dieses Suchmodul listet alle Begrenzungs- oder Einschränkungskonfigurationen auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp auswählen]</td> 
   <td>Wählen Sie aus, ob Sie eine Inhaltsvorlage oder ein Inhaltsfragment abrufen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
   <td>Geben Sie den Parameternamen ein oder ordnen Sie ihn zu, nach dem Sie diese Liste sortieren möchten. Fügen Sie <code>-</code> oder <code>+</code> hinzu, um absteigend oder aufsteigend zu sortieren. Wenn kein Zeichen angegeben ist, wird die Liste in absteigender Reihenfolge sortiert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Dieses Feld wird für die Paginierung verwendet. Geben Sie die Kriterien für die nächste Seite in Bezug auf die Eigenschaft ein, die im Feld Reihenfolge nach angegeben ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
   <td>Geben Sie den Parameternamen ein oder ordnen Sie ihn zu, nach dem Sie diese Liste sortieren möchten. Fügen Sie <code>-</code> oder <code>+</code> hinzu, um absteigend oder aufsteigend zu sortieren. Wenn kein Zeichen angegeben ist, wird die Liste in absteigender Reihenfolge sortiert.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filtern nach Eigenschaft]</td> 
   <td>Klicken Sie für jeden Eigenschaftenfilter, den Sie hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und Wert der Eigenschaft ein. Datensätze, die den angegebenen Wert für die Eigenschaft enthalten, werden in die Liste aufgenommen.</td> 
  </tr> 
 </tbody> 
</table>


### Sonstige


#### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten API-Aufruf an die Adobe Journey Optimizer-API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Journey Optimizer]</a> .</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zur Basis-URL ein.</p>
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
        <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen, <code>x-api-key</code> und <code>x-gw-ims-org-id</code> hinzu.</p>
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







<!--

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
* [Check the import dependencies](#check-the-import-dependencies)
* [Check the status for audience-based message](#status-for-audience-based-message)
* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Create a configuration](#create-a-configuration)
* [Create a package](#create-a-package)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a package](#delete-a-package)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
* [Import a package](#import-a-package)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)
* [List all dependent objects](#list-all-dependent-objects)
* [List export and import jobs](#list-import-and-export-jobs)
* [Look up a package](#look-up-a-package)
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
* [Publish a package](#publish-a-package)
* [Submit an import](#submit-an-import)
* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)
* [Trigger an audience-based message](#trigger-an-audience-based-message)
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a package](#update-a-package)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List packages](#list-packages)
* [List records](#list-records)

-->
