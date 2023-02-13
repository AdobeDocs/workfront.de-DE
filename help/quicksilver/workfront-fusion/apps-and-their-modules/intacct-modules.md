---
title: Integrationsmodule
description: Integrationsmodule
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---

# Integrationsmodule

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Intact verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um Intact-Module verwenden zu können, müssen Sie über ein Konto für die Verbindung verfügen.

## Verbindung mit Workfront Fusion herstellen

### Authorization [!DNL Workfront Fusion] , um Änderungen in Intact vorzunehmen

Vorher [!DNL Workfront Fusion] kann eine Verbindung zu [!DNL Intacct], müssen Sie sie autorisieren.

Navigieren Sie in Ihrem Konto zur **[!UICONTROL Firma]** Registerkarte.

1. Klicken **Unternehmensinformationen**.
1. Navigieren Sie zum **Sicherheit** Registerkarte.
1. Klicken [!UICONTROL Bearbeiten] in der oberen rechten Ecke
1. Wählen Sie Web-Services-Berechtigungen aus.
1. Klicken Sie auf das Pluszeichen
1. Geben Sie AzuquaMPP als sender_id ein.
1. (Optional) Geben Sie eine Beschreibung für die Verbindung ein

### Einrichten einer Verbindung in [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Sie können eine Verbindung zu Ihrem [!DNL Intacct] direkt in einer [!DNL Intacct] -Modul.

1. Klicken Sie in einem beliebigen Intect-Modul auf **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .
1. Anmeldedaten für Intact eingeben

   * Firmen-ID
   * Benutzer-ID
   * Kennwort

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## Integrieren von Modulen und ihren Feldern

Bei der Konfiguration [!DNL Intacct] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Eingabefelder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]](#make-a-custom-api-call)
* [[!UICONTROL Suchdatensätze]](#search-records)

### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen] {#make-a-custom-api-call}

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Intacct] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Intacct] Module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Verbindung</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Kontos für die Verbindung mit [!DNL Workfront Fusion] 2.0, siehe <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Verbindung in Workfront Fusion einrichten</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body XML</td> 
   <td> <p>Schließen Sie nur die XML im Hauptteil ein. Die Anfrage enthält automatisch Authentifizierungskopfzeilen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Suchdatensätze]

Dieses Suchmodul ruft eine Liste von Datensätzen ab, die bestimmten Suchkriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Verbindung</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Kontos für die Verbindung mit [!DNL Workfront Fusion] 2.0, siehe <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Verbindung in Workfront Fusion einrichten</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den zu suchenden Datensatztyp aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Suchkriterien</p> </td> 
   <td> 
    <ul> 
     <li> <p>Wählen Sie das Feld aus, nach dem Sie suchen möchten</p> </li> 
     <li> <p>Wählen Sie den Operator aus, den Sie für die Suche verwenden möchten</p> </li> 
     <li> <p>Geben Sie den Wert ein, nach dem Sie suchen möchten</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ergebnissatz</td> 
   <td>Wählen Sie aus, ob Sie alle übereinstimmenden Datensätze oder nur den ersten übereinstimmenden Datensatz zurückgeben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach</td> 
   <td>Wählen Sie das Feld aus, nach dem die Ergebnisse sortiert werden sollen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reihenfolge</td> 
   <td>Wählen Sie aus, ob Sie eine aufsteigende oder absteigende Sortierung vornehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ausgaben</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Groß-/Kleinschreibung</td> 
   <td>Aktivieren Sie diese Option, um bei Ihrer Abfrage die Groß-/Kleinschreibung zu beachten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Abfrage an private Entitäten</td> 
   <td>Aktivieren Sie diese Option, damit das Modul private Entitäten durchsuchen kann.</td> 
  </tr> 
 </tbody> 
</table>
