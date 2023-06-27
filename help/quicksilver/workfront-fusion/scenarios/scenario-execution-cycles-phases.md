---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]
description: In diesem Artikel werden Ereignisse beschrieben, die auftreten, während ein [!DNL Adobe Workfront Fusion] ausgeführt wird, z. B. Initialisierung, Vorgänge, Commits und Rollbacks.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] ist ein Transaktionssystem, das mit relationalen Datenbanken vergleichbar ist. Die Ausführung des Szenarios beginnt jeweils mit der Initialisierungsphase, läuft mit mindestens einem Zyklus, der aus den Vorgangs- und Übertragungs-/Rollback-Phasen besteht, und endet mit der Finalisierungsphase:

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

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Initialisierung

Während der Initialisierungsphase werden alle erforderlichen Verbindungen (Verbindung zu einer Datenbank, E-Mail-Dienst usw.) erstellt. Sie werden auch überprüft, ob jedes Modul in der Lage ist, die beabsichtigten Vorgänge auszuführen.

## Zyklen

Jeder Zyklus stellt eine nicht teilbare Arbeitseinheit dar, die aus einer Reihe von Vorgängen besteht. Es ist möglich, die maximale Anzahl von Zyklen im [!UICONTROL Szenario-Einstellungen] Bereich. Die Standardnummer ist 1.

Weitere Informationen finden Sie unter [Das Bedienfeld für die Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Vorgang

Während der Betriebsphase werden Lese- und/oder Schreibvorgänge durchgeführt:

* Der Lesevorgang besteht darin, Daten von einem Dienst abzurufen, der dann von anderen Modulen nach einem vordefinierten Szenario verarbeitet wird. Beispiel: die [!UICONTROL Dropbox] >[!UICONTROL Dateien überwachen] -Modul gibt neue Bundles (Dateien) zurück, die seit der letzten Ausführung des Szenarios erstellt wurden.
* Der Schreibvorgang besteht darin, Daten zur weiteren Verarbeitung an einen bestimmten Dienst zu senden. Beispiel: die [!DNL Dropbox] >[!UICONTROL Datei hochladen] -Modul eine Datei in eine [!DNL Dropbox] Ordner.

## Zusichern

Wenn die Betriebsphase für alle Module erfolgreich ist, beginnt die Commit-Phase, in der alle von den Modulen ausgeführten Vorgänge übernommen werden. Das bedeutet: [!DNL Workfront Fusion] sendet Informationen über den Erfolg an alle in der Betriebsphase beteiligten Dienste.

## Rollback

Tritt während der Vorgangs- oder Commitphase eines Moduls ein Fehler auf, wird die Phase abgebrochen und die Rollback-Phase gestartet, sodass alle Vorgänge während des angegebenen Zyklus nichtig sind. Einige Module unterstützen kein Rollback und Vorgänge, die von diesen Modulen ausgeführt werden, können nicht zurückgenommen werden. Weitere Informationen finden Sie unter [ACID-Module](#acid-modules) Abschnitt.

## Fertigstellung

Während der Fertigungsphase werden offene Verbindungen (z. B. FTP-Verbindungen, Datenbankverbindungen usw.) geschlossen und das Szenario ist abgeschlossen.

## ACID-Module

Alle [!DNL Workfront Fusion] -Module, die das Rollback unterstützen (auch als Transaktionsfunktionalität bezeichnet), sind mit dem ACID-Tag markiert.

![](assets/acid-modules-350x189.png)

Module, die nicht mit diesem Tag gekennzeichnet sind, können nicht in ihren ursprünglichen Zustand zurückgesetzt werden, wenn in anderen Modulen Fehler auftreten. Ein typisches Beispiel für ein Nicht-ACID-Modul ist die [!UICONTROL Email] >[!UICONTROL E-Mail senden] Aktion. Nachdem die E-Mail gesendet wurde, können Sie den Versand nicht mehr rückgängig machen.
