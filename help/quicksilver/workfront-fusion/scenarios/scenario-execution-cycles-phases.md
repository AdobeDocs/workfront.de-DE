---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ausführung, Zyklen und Phasen des Szenarios in  [!DNL Adobe Workfront Fusion]
description: In diesem Artikel werden Ereignisse beschrieben, die während der Ausführung eines [!DNL Adobe Workfront Fusion] Szenarios auftreten, z. B. Initialisierung, Vorgänge, Commits und Rollbacks.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Ausführung, Zyklen und Phasen des Szenarios in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] ist ein Transaktionssystem, das relationalen Datenbanken ähnelt. Die Ausführung des Szenarios beginnt jeweils mit der Initialisierungsphase, läuft mit mindestens einem Zyklus, der aus den Vorgangs- und Übertragungs-/Rollback-Phasen besteht, und endet mit der Finalisierungsphase:

>[!INFO]
>
>**Beispiel**
>
>Initialisierung
>
>Zyklus 1
>
>Vorgang (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>Zyklus 2
>
>Vorgang (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>...
>
>Zyklus N
>
>Vorgang (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>Fertigstellung

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
  <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Initialisierung

Während der Initialisierungsphase werden alle erforderlichen Verbindungen (Verbindung zu einer Datenbank, E-Mail-Dienst usw.) erstellt. Sie werden auch überprüft, ob jedes Modul in der Lage ist, die beabsichtigten Vorgänge auszuführen.

## Zyklen

Jeder Zyklus stellt eine nicht teilbare Arbeitseinheit dar, die aus einer Reihe von Vorgängen besteht. Es ist möglich, die maximale Anzahl von Zyklen im Bedienfeld [!UICONTROL szenario settings] festzulegen. Die Standardnummer ist 1.

Weitere Informationen finden Sie unter [Das Bedienfeld mit den Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Vorgang

Während der Betriebsphase werden Lese- und/oder Schreibvorgänge durchgeführt:

* Der Lesevorgang besteht darin, Daten von einem Dienst abzurufen, der dann von anderen Modulen nach einem vordefinierten Szenario verarbeitet wird. Beispielsweise gibt das Modul [!UICONTROL Dropbox] >[!UICONTROL Dateien überwachen] neue Bundles (Dateien) zurück, die seit der letzten Ausführung des Szenarios erstellt wurden.
* Der Schreibvorgang besteht darin, Daten zur weiteren Verarbeitung an einen bestimmten Dienst zu senden. Beispielsweise lädt das Modul [!DNL Dropbox] >[!UICONTROL Datei hochladen] eine Datei in einen Ordner [!DNL Dropbox] hoch.

## Zusichern

Wenn die Operationsphase für alle Module erfolgreich ist, beginnt die Commit-Phase, in der alle von den Modulen ausgeführten Vorgänge übernommen werden. Das bedeutet, dass [!DNL Workfront Fusion] allen in der Betriebsphase beteiligten Diensten Informationen über ihren Erfolg sendet.

## Rollback

Tritt während der Vorgangs- oder Commitphase eines Moduls ein Fehler auf, wird die Phase abgebrochen und die Rollback-Phase gestartet, sodass alle Vorgänge während des angegebenen Zyklus nichtig sind. Einige Module unterstützen kein Rollback und Vorgänge, die von diesen Modulen ausgeführt werden, können nicht zurückgenommen werden. Weitere Informationen finden Sie im Abschnitt [ACID modules](#acid-modules) .

## Fertigstellung

Während der Fertigungsphase werden offene Verbindungen (z. B. FTP-Verbindungen, Datenbankverbindungen usw.) geschlossen und das Szenario ist abgeschlossen.

## ACID-Module

Alle [!DNL Workfront Fusion] -Module, die das Rollback unterstützen (auch als Transaktionsfunktionalität bezeichnet), sind mit dem ACID-Tag markiert.

![](assets/acid-modules-350x189.png)

Module, die nicht mit diesem Tag gekennzeichnet sind, können nicht in ihren ursprünglichen Zustand zurückgesetzt werden, wenn in anderen Modulen Fehler auftreten. Ein typisches Beispiel für ein Nicht-ACID-Modul ist die Aktion [!UICONTROL E-Mail] >[!UICONTROL E-Mail senden] . Nachdem die E-Mail gesendet wurde, können Sie den Versand nicht mehr rückgängig machen.
