---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]
description: In diesem Artikel werden Ereignisse beschrieben, die während  [!DNL Adobe Workfront Fusion]  Ausführung eines Szenarios auftreten, z. B. Initialisierung, Vorgänge, Commits und Rollbacks.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 1%

---

# Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] ist ein Transaktionssystem, das relationalen Datenbanken ähnelt. Jede Szenarioausführung beginnt mit der Initialisierungsphase, wird mit mindestens einem Zyklus fortgesetzt, der aus den Vorgangs- und Commit-/Rollback-Phasen besteht, und endet mit der Finalisierungsphase:

>[!INFO]
>
>**Beispiel**
>
>Initialisierung
>
>#1
>
>Betrieb (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>#2
>
>Betrieb (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>…
>
>#N
>
>Betrieb (Lesen oder Schreiben)
>
>Commit oder Rollback
>
>Fertigstellung

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Initialisierung

Während der Initialisierungsphase werden alle erforderlichen Verbindungen (Verbindung zu einer Datenbank, E-Mail-Service usw.) erstellt. Sie werden auch überprüft, ob jedes Modul in der Lage ist, die beabsichtigten Vorgänge auszuführen.

## Zyklen

Jeder Zyklus stellt eine unteilbare Arbeitseinheit dar, die aus einer Reihe von Vorgängen besteht. Die maximale Anzahl von Zyklen kann im Bedienfeld „Szenario[!UICONTROL Einstellungen“ ] werden. Die Standardzahl ist 1.

Weitere Informationen finden Sie unter [Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Vorgang

Während der Betriebsphase wird Lese- und/oder Schreibvorgang ausgeführt:

* Der Lesevorgang besteht darin, Daten von einem Service zu erhalten, die dann von anderen Modulen gemäß einem vordefinierten Szenario verarbeitet werden. Beispielsweise gibt das Modul [!UICONTROL Dropbox] >[!UICONTROL Dateien beobachten] neue Bundles (Dateien) zurück, die seit der letzten Szenario-Ausführung erstellt wurden.
* Der Schreibvorgang besteht darin, Daten zur weiteren Verarbeitung an einen bestimmten Dienst zu senden. Beispielsweise lädt das Modul [!DNL Dropbox] > [!UICONTROL Datei hochladen] eine Datei in einen [!DNL Dropbox] Ordner hoch.

## Zusichern

Wenn die Vorgangsphase für alle Module erfolgreich ist, beginnt die Commit-Phase, während der alle von den Modulen ausgeführten Vorgänge übergeben werden. Das bedeutet, dass [!DNL Workfront Fusion] Informationen über den Erfolg an alle an der Betriebsphase beteiligten Dienste sendet.

## Rollback

Wenn während der Vorgangs- oder Commit-Phase auf einem Modul ein Fehler auftritt, wird die Phase abgebrochen und die Rollback-Phase gestartet, wodurch alle Vorgänge während des angegebenen Zyklus ungültig werden. Einige Module unterstützen kein Rollback, und Vorgänge, die von diesen Modulen ausgeführt werden, können nicht zurückgenommen werden. Weitere Informationen finden Sie im [ACID-Module](#acid-modules) Abschnitt.

## Fertigstellung

Während der Finalisierungsphase werden offene Verbindungen (z. B. FTP-Verbindungen, Datenbankverbindungen usw.) geschlossen und das Szenario ist abgeschlossen.

## ACID-Module

Alle [!DNL Workfront Fusion], die Rollback unterstützen (auch als Transaktion bezeichnet), sind mit dem ACID-Tag gekennzeichnet.

![](assets/acid-modules-350x189.png)

Module, die nicht mit diesem Tag markiert sind, können nicht in ihren Ausgangszustand zurückgesetzt werden, wenn in anderen Modulen Fehler auftreten. Ein typisches Beispiel für ein Nicht-ACID-Modul ist die Aktion [!UICONTROL E] > [!UICONTROL E-Mail senden]. Nach dem Versand der E-Mail kann der Versand nicht mehr rückgängig gemacht werden.
