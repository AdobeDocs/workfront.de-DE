---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server-Module
description: Sie können [!DNL Adobe Workfront Fusion] verwenden, um eine Verbindung zum Microsoft SQL Server herzustellen.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] Module

Sie können [!DNL Adobe Workfront Fusion] verwenden, um eine Verbindung zu [!UICONTROL Microsoft SQL Server] herzustellen.

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Verbinden des [!DNL Microsoft SQL Server]-Dienstes mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Microsoft SQL Server]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

## Verwenden von [!DNL Microsoft SQL Server] -Modulen

Sie können Ihre benutzerdefinierte Logik direkt auf Ihrem Datenbankserver mithilfe gespeicherter Verfahren ausführen. [!DNL Adobe Workfront Fusion] lädt die Oberfläche von Eingabe-/Ausgabeparametern und Datensatzgruppen dynamisch, sodass jeder Parameter oder Wert einzeln zugeordnet werden kann. Bevor Sie mit der Konfiguration Ihres Szenarios beginnen, stellen Sie sicher, dass das Konto, über das Sie eine Verbindung mit Ihrer Datenbank herstellen, Lesezugriff auf die Ansichten `INFORMATION_SCHEMA.ROUTINES` und `INFORMATION_SCHEMA.PARAMETERS` hat.

Wenn [!DNL Fusion] die Verbindung zum [!DNL SQL server]-Ziel herstellt, identifiziert der [!DNL Fusion] -Benutzer den Host (den Domänennamen oder die IP-Adresse, unter der der Server gehostet wird) und den Port. [!DNL Fusion] kann eine Verbindung zu jedem verfügbaren Host und Port herstellen.

Informationen zu bestimmten IP-Adressen, die von [!DNL Workfront Fusion] verwendet werden, finden Sie unter [IP-Adressen für den Zugriff auf [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md) .

Weitere Informationen zum Erstellen einer gespeicherten Prozedur finden Sie in der Dokumentation zu [!DNL Microsoft SQL Server] .

>[!NOTE]
>
>[!DNL Workfront Fusion] unterstützt nicht mehrere Datensätze. Nur der erste wird verarbeitet.

## Fehlerbehebung für Fehler [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Zeitüberschreitung der Sperrwartezeit überschritten; Neustarten der Transaktion]

Dieser Fehler tritt auf, wenn Sie dieselben Daten mit mehreren Modulen ändern. Sie wird durch SQL-Transaktionen verursacht.

Wenn ein SQL-Modul ausgeführt wird, startet es eine Transaktion. Die Transaktion ist abgeschlossen, nachdem das Szenario vollständig ausgeführt wurde.

Wenn ein anderes Modul versucht, auf dieselben Daten zuzugreifen, muss es warten, bis die vorherige Transaktion abgeschlossen ist. Da die erste Transaktion abgeschlossen wird, nachdem das Szenario abgeschlossen ist, kann die zweite Transaktion nie beginnen.

### Lösung:

Aktivieren Sie die automatische Übertragung. Die automatische Übertragung beendet (gibt Zusagen) jede Transaktion unmittelbar nach der Ausführung des Moduls.

1. Klicken Sie unten auf dem Bildschirm auf das Symbol [!UICONTROL Szenarioeinstellungen] ![](assets/scenario-settings-icon.png).
1. Klicken Sie auf das Kontrollkästchen **[!UICONTROL Automatisches Übertragen]** .
1. Klicken Sie auf **[!UICONTROL OK]** , um die Szenario-Einstellungen zu speichern.
