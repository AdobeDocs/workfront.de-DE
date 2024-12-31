---
title: MariaDB-Module
description: In  [!DNL Adobe Workfront Fusion]  Szenario können Sie Workflows automatisieren, die  [!DNL MariaDB] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# [!DNL MariaDB]

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL MariaDB] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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

Um [!DNL MariaDB]-Module verwenden zu können, müssen Sie über ein [!DNL MariaDB]-Konto verfügen.

## [!DNL MariaDB] mit [!DNL Workfront Fusion] verbinden

Sie können direkt aus einem [!DNL MariaDB]-Modul heraus eine Verbindung zu Ihrem [!DNL MariaDB]-Konto herstellen.

1. Klicken Sie in einem [!DNL MariaDB] Modul **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung].
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
      <td> <p>Geben Sie die IP-Adresse oder den Hostnamen Ihrer Datenbankinstanz ein. Dieser Host muss von außerhalb Ihres Netzwerks zugänglich sein.</p> <p>Beispiel: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>Der Standard-Port ist 3306. Wenn Sie einen nicht standardmäßigen Port verwenden, setzen Sie diese Nummer auf Ihren Port. </td> 
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

1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

## [!DNL MariaDB] Module und ihre Felder

Beim Konfigurieren [!DNL MariaDB] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL MariaDB] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Ausführen einer Abfrage (erweitert)

Dieses Aktionsmodul ruft basierend auf einer von Ihnen angegebenen Abfrage Informationen aus Ihrer Datenbank ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL MariaDB]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL MariaDB] mit [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Abfrage]</td> 
   <td> <p>Geben Sie die SQL-Abfrage ein, mit der das Modul Daten abrufen soll.</p> <p>Wichtig: In der Abfrage verwendete Variablen werden nicht bereinigt. Stellen Sie sicher, dass Sie Variablen ordnungsgemäß bereinigen, um SQL-Injections zu verhindern.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Zeilen aus einer Tabelle auswählen (erweitert)]

Dieses Modul liest Einträge aus Ihrer Datenbank.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL MariaDB]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL MariaDB] mit [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Tabelle]</td> 
   <td> <p>Wählen Sie die Tabelle aus, die die Datensätze enthält, die Sie lesen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td> <p>Richten Sie den Filter ein, nach dem Sie Zeilen auswählen möchten</p> 
    <ul> 
     <li> <p>Wählen Sie das Feld aus, nach dem Sie suchen möchten</p> </li> 
     <li> <p>Wählen Sie den Operator aus, den Sie für Ihre Suche verwenden möchten</p> </li> 
     <li> <p>Geben Sie den Wert ein, nach dem Sie suchen möchten, oder ordnen Sie ihn zu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL sort] </td> 
   <td> <p>Klicken Sie für jede Ebene, nach der Ihre Ergebnisse sortiert werden sollen, auf <strong>[!UICONTROL Element hinzufügen]</strong> und wählen Sie dann das Feld aus, nach dem Sie die Ergebnisse sortieren möchten, und ob Sie auf- oder absteigend sortieren möchten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>
