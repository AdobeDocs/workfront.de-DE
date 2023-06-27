---
title: MariaDB-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL MariaDB], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 1%

---

# [!DNL MariaDB]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL MariaDB], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL MariaDB] -Module, müssen Sie über eine [!DNL MariaDB] -Konto.

## Verbinden [!DNL MariaDB] nach [!DNL Workfront Fusion]

Sie können eine Verbindung zu Ihrem [!DNL MariaDB] direkt in einer [!DNL MariaDB] -Modul.

1. In jeder [!DNL MariaDB] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Konfigurieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verbindungsname]</p> </td> 
      <td> <p>Geben Sie einen Namen für die neue Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Geben Sie die IP-Adresse oder den Hostnamen Ihrer Datenbankinstanz ein. Auf diesen Host muss von außerhalb Ihres Netzwerks aus zugegriffen werden können.</p> <p>Beispiel: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>Der Standardanschluss ist 3306. Wenn Sie einen nicht standardmäßigen Port verwenden, setzen Sie diese Nummer auf Ihren Port. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Datenbankname]</td> 
      <td>Geben Sie den Namen der Datenbank ein, mit der Sie interagieren möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Benutzername]</td> 
      <td>Geben Sie Ihren Benutzernamen ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kennwort]</td> 
      <td>Geben Sie Ihr Kennwort ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL MariaDB] Module und ihre Felder

Bei der Konfiguration [!DNL MariaDB] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL MariaDB] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Ausführen einer Abfrage (erweitert)

Dieses Aktionsmodul ruft basierend auf einer von Ihnen angegebenen Abfrage Informationen aus Ihrer Datenbank ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden der [!DNL MariaDB] Konto [!DNL Workfront Fusion], siehe <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL MariaDB] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfrage]</td> 
   <td> <p>Geben Sie die SQL-Abfrage ein, die das Modul zum Abrufen von Daten verwenden soll.</p> <p>Wichtig: Die in der Abfrage verwendeten Variablen werden nicht bereinigt. Stellen Sie sicher, dass Sie Variablen ordnungsgemäß bereinigen, um SQL-Injections zu verhindern.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Zeilen aus einer Tabelle auswählen (erweitert)]

Dieses Modul liest Datensätze aus Ihrer Datenbank.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden der [!DNL MariaDB] Konto [!DNL Workfront Fusion], siehe <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL MariaDB] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabelle]</td> 
   <td> <p>Wählen Sie die Tabelle aus, die die Datensätze enthält, die Sie lesen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Richten Sie den Filter ein, nach dem Sie Zeilen auswählen möchten</p> 
    <ul> 
     <li> <p>Wählen Sie das Feld aus, nach dem Sie suchen möchten</p> </li> 
     <li> <p>Wählen Sie den Operator aus, den Sie für die Suche verwenden möchten</p> </li> 
     <li> <p>Geben Sie den Wert ein oder ordnen Sie ihn zu, nach dem Sie suchen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierung] </td> 
   <td> <p>Klicken Sie für jede Ebene, nach der die Ergebnisse sortiert werden sollen, auf <strong>[!UICONTROL Element hinzufügen]</strong>und wählen Sie dann das Feld aus, nach dem die Ergebnisse sortiert werden sollen, und geben Sie an, ob die Sortierung aufsteigend oder absteigend sein soll</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>
