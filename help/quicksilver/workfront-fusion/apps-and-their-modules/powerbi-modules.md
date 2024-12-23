---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Power BI-Module
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2493'
ht-degree: 0%

---

# [!DNL Power BI] Module

[!DNL Power BI] ist eine Anwendung, mit der Sie Daten für Ihre Stakeholder visualisieren und darstellen können. Es kann Daten aus einer Vielzahl von Quellen aufnehmen.

>[!NOTE]
>
>[!DNL Workfront Fusion] ist keine Datenquelle. [!DNL Workfront Fusion] kann zwar Datenquellen erstellen und verwenden, speichert aber Ihre Daten nicht.


## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
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

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Microsoft Power BI API-Informationen

Der Microsoft Power BI-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://api.powerbi.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.0.2</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Power BI] Module und ihre Felder

Wenn Sie [!DNL Power BI] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Felder angezeigt werden. Ein fett gedruckter Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zwischen Modulen in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Dashboards](#dashboards)
* [Berichte](#reports)
* [Datensatz](#dataset)
* [Apps](#apps)
* [Sonstige](#other)

### Dashboards

* [Dashboard erstellen](#create-a-dashboard)
* [Abrufen eines Dashboards](#get-a-dashboard)
* [Dashboard-Kachel abrufen](#get-a-dashboard-tile)
* [Dashboard-Kacheln auflisten](#list-dashboard-tiles)
* [Dashboards auflisten](#list-dashboards)

#### [!UICONTROL Erstellen eines Dashboards]

Dieses Aktionsmodul erstellt ein neues Dashboard.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Geben Sie einen Namen für das Dashboard ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der das neue Dashboard gehört.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Dashboard abrufen]

Dieses Aktionsmodul ruft Metadaten eines angegebenen Dashboards ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard-ID eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um das Dashboard auszuwählen, für das Sie Metadaten abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard-ID]</td>
      <td>
        <p>Geben Sie die ID des Dashboards ein, für das Sie Metadaten abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die ID der Gruppe aus oder ordnen Sie sie zu, deren Inhaber die Dashboards ist, für die Sie Metadaten abrufen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Dashboard-Kachel abrufen]

Dieses Aktionsmodul ruft Metadaten einer angegebenen Dashboard-Kachel ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard-ID eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um die Dashboard-Details auszuwählen, die Sie abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Dashboard-ID]</td>
      <td>
        <p>Geben Sie die ID des Dashboards ein oder ordnen Sie sie zu, für das Sie Details abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Kachel-ID]</td>
      <td>Geben Sie die ID der Kachel [!DNL Power BI] ein oder ordnen Sie sie zu, für die Sie Details abrufen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der die abzurufende Kachel gehört.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Dashboard-Kacheln auflisten]

Dieses Suchmodul ruft eine Liste von Dashboard-Kacheln ab.

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard-ID eingeben]</td>
    <td>
      <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um das Dashboard auszuwählen, dessen Kacheln Sie auflisten möchten.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Dashboard-ID]</td>
    <td>
      <p>Geben Sie die ID des Dashboards ein, das die aufzulistenden Kacheln enthält, oder ordnen Sie sie zu.</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
    <td>Wählen Sie die ID der Gruppe aus oder ordnen Sie sie zu, der die Dashboards gehören, die die aufzulistenden Kacheln enthalten.</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL Limit]  </td>
    <td>
      <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL Listen-Dashboards]

Dieses Suchmodul ruft eine Liste von Dashboards ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>
        <p>Wählen Sie die ID der Gruppe aus oder ordnen Sie sie zu, der die Dashboards gehören, die Sie auflisten möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

### Berichte

* [Bericht kopieren](#copy-a-report)
* [Einen Bericht löschen](#delete-a-report)
* [Bericht abrufen](#get-a-report)
* [Berichte auflisten](#list-reports)

#### [!UICONTROL Einen Bericht kopieren]

Dieses Aktionsmodul kopiert einen vorhandenen Bericht.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichtkennung eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Bericht auszuwählen, den Sie kopieren möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Berichts ein, den Sie kopieren möchten, oder ordnen Sie ihn zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der der Bericht gehört, den Sie kopieren möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Neuer kopierter Berichtsname]</td>
      <td>Geben Sie einen Namen für den neuen Bericht ein oder ordnen Sie ihn zu.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Einen Bericht löschen]

Dieses Aktionsmodul löscht einen Bericht.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichtkennung eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Bericht auszuwählen, den Sie löschen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Berichts ein, den Sie löschen möchten, oder ordnen Sie ihn zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der der Bericht gehört, den Sie löschen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Einen Bericht abrufen]

Dieses Aktionsmodul ruft Metadaten eines angegebenen Berichts ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichtkennung eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Bericht auszuwählen, für den Sie Metadaten abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>Geben Sie die ID des Berichts ein oder ordnen Sie sie zu, für den Sie Metadaten abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der der Bericht gehört, für den Sie Metadaten abrufen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listenberichte]

Dieses Suchmodul ruft eine Liste von Berichten ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>
        <p>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der die Berichte gehören, die Sie auflisten möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>


### Datensatz

* [Hinzufügen/Löschen von Zeilen in einer Datensatztabelle](#add-or-delete-rows-in-a-dataset-table)
* [Datensatz erstellen](#create-a-dataset)
* [Datensatz löschen](#delete-a-dataset)
* [Datensatz abrufen](#get-a-dataset)
* [Datensätze auflisten](#list-datasets)
* [Datensatz aktualisieren](#refresh-a-dataset)

#### [!UICONTROL Hinzufügen oder Löschen von Zeilen in einer Datensatztabelle]

Dieses Aktionsmodul fügt Zeilen einer angegebenen Push-Datensatztabelle hinzu oder löscht sie.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabelle eingeben]</td>
      <td>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Datensatz auszuwählen, der die anzupassende Tabelle enthält.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
      <td>Geben Sie die ID des Datensatzes ein oder ordnen Sie sie zu, der die Zeilen enthält, die Sie hinzufügen oder löschen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabellenname]  </td>
      <td>
        <p>Geben Sie den Namen der Tabelle ein oder ordnen Sie ihn zu, die die Zeilen enthält, die Sie hinzufügen oder löschen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Geben Sie die Kennung der Gruppe ein oder ordnen Sie sie zu, der der Datensatz gehört.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Aktion auswählen]</td>
      <td>
        <p>Wählen Sie die Aktion aus oder ordnen Sie sie zu.</p>
        <ul>
          <li>
            <p>[!UICONTROL Zeilen hinzufügen]</p>
          </li>
          <li>
            <p>[!UICONTROL Alle Zeilen löschen]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Zeilen]</td>
      <td>
        <p>Fügen Sie die Zeilenfelder hinzu.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Schlüssel]</b>
            </p>
            <p>Geben Sie den Schlüsselnamen ein oder ordnen Sie ihn zu.</p>
          </li>
          <li>
            <p><b>[!UICONTROL Feldtyp]</b>
            </p>
            <p>Wählen Sie den Feldtyp aus oder ordnen Sie ihn zu:</p>
            <ul>
              <li>
                <p>Boolesch</p>
              </li>
              <li>
                <p>Datum</p>
              </li>
              <li>
                <p>Text</p>
              </li>
              <li>
                <p>Zahl</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL Wert]</p>
            <p>Geben Sie den Schlüsselwert ein oder ordnen Sie ihn zu.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>Geben Sie einen Namen für den Datensatz ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der der neue Datensatz gehört.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Standardmodus]</td>
      <td>
        <p>Wählen Sie den Standardmodus für den Datensatz aus oder ordnen Sie ihn zu:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>: Ein Datensatz mit einer Live-Verbindung zu [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL As on Prem]</b>: Ein Datensatz mit einer Live-Verbindung zum [!DNL On-premise Analysis]-Dienst</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>: Ein Datensatz, der einen programmgesteuerten Zugriff zum Übertragen von Daten in ermöglicht. [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>: Ein Datensatz, der Daten-Streaming unterstützt und programmgesteuerten Zugriff zum Senden von Daten in ermöglicht [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>: Ein Datensatz, der Daten-Streaming unterstützt</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabellen]</td>
      <td>Fügen Sie dem Datensatz Tabellen hinzu. Informationen zu Feldern finden Sie unter <a href="#Table" class="MCXref_0">Tabellenfelder</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>Hinzufügen der Datenquellen. Informationen zu Feldern finden Sie unter <a href="#Data" class="MCXref_0">Datenquellenfelder</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>Wählen Sie die absichtliche Richtlinie für den Datensatz aus oder ordnen Sie sie zu:</p>
        <ul>
          <li>
            <p>[!UICONTROL None]</p>
          </li>
          <li>
            <p>[!UICONTROL Basic FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### Tabellenfelder

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>  Geben Sie einen Namen für die Tabelle ein oder ordnen Sie ihn zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Spalten]</td>
      <td>
        <p>Fügen Sie die Spalten hinzu:</p>
        <ul>
          <li>
            <p><b>[!UICONTROL Name]</b>
            </p>
            <p>Geben Sie einen Spaltennamen ein (zuordnen).</p>
          </li>
          <li>
            <p><b>[!UICONTROL Datentyp]</b>
            </p>
            <p>Wählen Sie den Datentyp aus oder ordnen Sie ihn zu:</p>
            <ul>
              <li>
                <p>[!UICONTROL String]</p>
              </li>
              <li>
                <p>[!UICONTROL Integer]</p>
              </li>
              <li>
                <p>[!UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[!UICONTROL Date Time]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL Formatzeichenfolge]</b>
            </p>
            <p>Geben Sie die Formatzeichenfolge ein (map).</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Zeilen]</td>
      <td>Zeilendetails eingeben oder zuordnen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maßnahmen]</td>
      <td>Fügen Sie die Kennzahl für die Tabellen hinzu.</td>
    </tr>
  </tbody>
</table>

##### Datenquellen-Felder

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Datenbank]  </td>
      <td>
        <p>Geben Sie die Datenbank ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Server]  </td>
      <td>
        <p>Geben Sie den Namen des Servers ein, den Sie verwenden möchten, oder ordnen Sie ihn zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>Geben Sie die URL ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datenquellen-ID]</td>
      <td>
        <p>  Geben Sie die Kennung der Datenquelle ein oder ordnen Sie sie zu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datenquellentyp]  </td>
      <td>
        <p>Wählen Sie den Datenquellentyp aus oder ordnen Sie ihn zu. Beispiel: SQL.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gateway ID]  </td>
      <td>Geben Sie die Kennung des Gateways ein, das Sie verwenden möchten, oder ordnen Sie sie zu.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen Datensatz.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichtkennung eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Datensatz auszuwählen, den Sie löschen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu, den Sie löschen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die ID der Gruppe aus oder ordnen Sie sie zu, der der Datensatz gehört, den Sie löschen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz abrufen]

Dieses Aktionsmodul ruft Metadaten eines angegebenen Datensatzes ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Berichtkennung eingeben]</td>
      <td>
        <p>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Bericht auszuwählen, für den Sie Metadaten abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>Geben Sie die ID des Datensatzes ein oder ordnen Sie sie zu, für den Sie Metadaten abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die ID der Gruppe aus oder ordnen Sie sie zu, der der Datensatz gehört, für den Sie Metadaten abrufen möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensätze auflisten]

Dieses Suchmodul ruft eine Liste von Datensätzen ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Wählen Sie die Kennung der Gruppe aus oder ordnen Sie sie zu, der der Bericht gehört, für den Sie Metadaten abrufen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie [Aktion] für das Modul während jedes Szenario-Ausführungszyklus zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen angegebenen Datensatz.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz eingeben]</td>
      <td>Wählen Sie die Option aus oder ordnen Sie sie zu, um den Datensatz auszuwählen, den Sie aktualisieren möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
      <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu, den Sie aktualisieren möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Tabellenname]  </td>
      <td>
        <p>Geben Sie den Namen der Tabelle ein oder ordnen Sie ihn zu, die die Zeilen enthält, die Sie hinzufügen oder löschen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Gruppen-ID]  </td>
      <td>Geben Sie die Kennung der Gruppe ein oder ordnen Sie sie zu, der der Datensatz gehört.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Benachrichtigungsoption]  </td>
      <td>
        <p>Wählen Sie die zu benachrichtigende Option aus oder ordnen Sie sie zu:</p>
        <ul>
          <li>
            <p>[!UICONTROL Mail bei Abschluss]</p>
          </li>
          <li>
            <p>[!UICONTROL Mail bei Fehler]</p>
          </li>
          <li>
            <p>Keine Benachrichtigung!</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Apps

* [App abrufen](#get-an-app)
* [Abrufen des Dashboards einer App](#get-an-apps-dashboard)
* [App-Bericht abrufen](#get-an-apps-report)
* [Dashboards der App auflisten](#list-apps-dashboards)
* [Berichte der App auflisten](#list-apps-reports)
* [Listen-Apps](#list-apps)
* [Apps ansehen](#watch-apps)

#### [!UICONTROL App abrufen]

Dieses Aktionsmodul ruft Metadaten einer angegebenen App ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Wählen Sie die ID der App aus, die Sie abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Dashboard einer App abrufen]

Dieses Aktionsmodul ruft Metadaten des Dashboards einer bestimmten App ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Wählen Sie die ID der App aus oder ordnen Sie sie zu, die das Dashboard enthält, das Sie abrufen möchten.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>  Wählen Sie die ID des Dashboards aus, das Sie abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Abrufen des Berichts einer App]

Dieses Aktionsmodul ruft Metadaten aus dem Bericht einer bestimmten App ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]  </td>
      <td>
        <p>Wählen Sie die ID der App aus oder ordnen Sie sie zu, die den abzurufenden Bericht enthält.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bericht-ID]</td>
      <td>
        <p>  Wählen Sie die Kennung des Berichts aus, den Sie abrufen möchten, oder ordnen Sie sie zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listen-Apps]

Dieses Suchmodul ruft eine Liste aller installierten Apps ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Dashboards der App auflisten]

Dieses Suchmodul ruft eine Liste von Dashboards aus einer bestimmten App ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Wählen Sie die ID der App aus oder ordnen Sie sie zu, aus der Sie Dashboards auflisten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Berichte der App auflisten]

Dieses Suchmodul ruft eine Liste aller Berichte aus der angegebenen App ab.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL App ID]</td>
      <td>Wählen Sie die ID der App aus oder ordnen Sie sie zu, aus der Sie Berichte auflisten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Apps ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine App aktualisiert wird.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p>
      </td>
    </tr>
  </tbody>
</table>

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Dieses Aktionsmodul führt einen API-Aufruf an die [!DNL Power BI] -API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Power BI]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://api.powerbi.com</code> ein. Beispiel: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
      <td>
        <p>Wählen Sie die [!UICONTROL HTTP]-Anforderungsmethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter [!UICONTROL HTTP]-Anforderungsmethoden.</p>
      </td>
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
