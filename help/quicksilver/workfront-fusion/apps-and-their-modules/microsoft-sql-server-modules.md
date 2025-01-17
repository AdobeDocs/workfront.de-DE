---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Microsoft SQL Server-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-sql-server-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Sie können [!DNL Adobe Workfront Fusion] verwenden, um eine Verbindung zu [!UICONTROL Microsoft SQL Server] herzustellen.

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



## Verbinden des [!DNL Microsoft SQL Server]-Services mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Microsoft SQL Server]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Einverständnisbildschirm für Berechtigungen alle Berechtigungen angezeigt, die zuvor der Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn ein Benutzer beispielsweise über die über den Excel-Connector gewährten Berechtigungen zum Lesen von Tabellen verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Einverständnisbildschirm für Berechtigungen sowohl die bereits erteilte Berechtigung zum Lesen von Tabellen als auch die neu erforderliche Berechtigung zum Schreiben von E-Mails an.

## Verwenden von [!DNL Microsoft SQL Server]

Sie können Ihre benutzerdefinierte Logik über gespeicherte Prozeduren direkt auf Ihrem Datenbank-Server ausführen. [!DNL Adobe Workfront Fusion] lädt dynamisch die Schnittstelle von Eingabe/Ausgabe-Parametern und Recordset , sodass jeder Parameter oder Wert einzeln zugeordnet werden kann. Bevor Sie mit der Konfiguration Ihres Szenarios beginnen, stellen Sie sicher, dass das Konto, das Sie für die Verbindung mit Ihrer Datenbank verwenden, Lesezugriff auf `INFORMATION_SCHEMA.ROUTINES`- und `INFORMATION_SCHEMA.PARAMETERS` hat.

Wenn [!DNL Fusion] die Verbindung zum [!DNL SQL server]-Ziel herstellt, identifiziert der [!DNL Fusion] den Host (den Domain-Namen oder die IP-Adresse, unter der der Server gehostet wird) und den Port. [!DNL Fusion] können eine Verbindung zu jedem verfügbaren Host und Port herstellen.

Informationen zu den von [!DNL Workfront Fusion] verwendeten IP-Adressen finden Sie unter [IP-Adressen für den Zugriff [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Weitere Informationen zum Erstellen einer gespeicherten Prozedur finden Sie in der [!DNL Microsoft SQL Server].

>[!NOTE]
>
>[!DNL Workfront Fusion] unterstützt nicht mehrere Recordsets. Nur der erste wird verarbeitet.

## Fehlerbehebung für Fehler [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Sperrwartezeitlimit überschritten; versuchen Sie, die Transaktion neu zu starten]

Dieser Fehler tritt auf, wenn Sie dieselben Daten mithilfe mehrerer Module ändern. Sie wird durch SQL-Transaktionen verursacht.

Wenn ein SQL-Modul ausgeführt wird, startet es eine Transaktion. Die Transaktion ist abgeschlossen, nachdem das Szenario vollständig ausgeführt wurde.

Wenn ein anderes Modul versucht, auf dieselben Daten zuzugreifen, muss es warten, bis die vorherige Transaktion abgeschlossen ist. Da die erste Transaktion abgeschlossen wird, nachdem das Szenario abgeschlossen ist, kann die zweite Transaktion nie beginnen.

### Lösung:

Aktivieren Sie die automatische Bestätigung. Der automatische Commit beendet (übergibt) jede Transaktion unmittelbar nach Abschluss der Modulausführung.

1. Klicken Sie auf [!UICONTROL  Symbol ]Szenarioeinstellungen![](assets/scenario-settings-icon.png) am unteren Bildschirmrand.
1. Aktivieren Sie **[!UICONTROL Kontrollkästchen]** Automatisch bestätigen“.
1. Klicken Sie **[!UICONTROL OK]**, um die Szenario-Einstellungen zu speichern.
