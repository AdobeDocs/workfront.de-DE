---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server-Module
description: Sie können [!DNL Adobe Workfront Fusion] , um eine Verbindung mit Microsoft SQL Server herzustellen.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server]-Module

Sie können [!DNL Adobe Workfront Fusion] zur Verbindung mit [!UICONTROL Microsoft SQL Server].

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

## Verwenden [!DNL Microsoft SQL Server] Module

Sie können Ihre benutzerdefinierte Logik direkt auf Ihrem Datenbankserver mithilfe gespeicherter Verfahren ausführen. [!DNL Adobe Workfront Fusion] lädt die Schnittstelle von Eingabe-/Ausgabeparametern und Datensatzgruppen dynamisch, sodass jeder Parameter oder Wert einzeln zugeordnet werden kann. Bevor Sie mit der Konfiguration Ihres Szenarios beginnen, stellen Sie sicher, dass das Konto, über das Sie eine Verbindung mit Ihrer Datenbank herstellen, über Lesezugriff auf `INFORMATION_SCHEMA.ROUTINES` und `INFORMATION_SCHEMA.PARAMETERS` Ansichten.

Wann [!DNL Fusion] stellt die Verbindung zu [!DNL SQL server] Ziel, [!DNL Fusion] Der Benutzer identifiziert den Host (den Domänennamen oder die IP-Adresse, unter der der Server gehostet wird) und den Port. [!DNL Fusion] kann eine Verbindung zu jedem verfügbaren Host und Port herstellen.

Informationen zu bestimmten IP-Adressen, die von [!DNL Workfront Fusion], siehe [IP-Adressen für den Zugriff [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Weitere Informationen zum Erstellen einer gespeicherten Prozedur finden Sie unter [!DNL Microsoft SQL Server] Dokumentation.

>[!NOTE]
>
>[!DNL Workfront Fusion] unterstützt nicht mehrere Datensätze. Nur der erste wird verarbeitet.

## Fehlerbehebung [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Zeitüberschreitung der Sperrwartezeit überschritten; Neustarten der Transaktion]

Dieser Fehler tritt auf, wenn Sie dieselben Daten mit mehreren Modulen ändern. Sie wird durch SQL-Transaktionen verursacht.

Wenn ein SQL-Modul ausgeführt wird, startet es eine Transaktion. Die Transaktion ist abgeschlossen, nachdem das Szenario vollständig ausgeführt wurde.

Wenn ein anderes Modul versucht, auf dieselben Daten zuzugreifen, muss es warten, bis die vorherige Transaktion abgeschlossen ist. Da die erste Transaktion abgeschlossen wird, nachdem das Szenario abgeschlossen ist, kann die zweite Transaktion nie beginnen.

### Lösung:

Aktivieren Sie die automatische Übertragung. Die automatische Übertragung beendet (gibt Zusagen) jede Transaktion unmittelbar nach der Ausführung des Moduls.

1. Klicken Sie auf [!UICONTROL Szenario-Einstellungen] icon ![](assets/scenario-settings-icon.png)unten auf dem Bildschirm.
1. Klicken Sie auf **[!UICONTROL Automatische Übertragung]** aktivieren.
1. Klicken **[!UICONTROL OK]** , um die Szenario-Einstellungen zu speichern.
