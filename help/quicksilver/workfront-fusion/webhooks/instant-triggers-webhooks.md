---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]
description: Viele Services stellen Webhooks bereit, mit denen sofortige Benachrichtigungen bereitgestellt werden können, sobald eine bestimmte Änderung im Service eintritt. Für die Verarbeitung dieser Benachrichtigungen empfehlen wir die Verwendung von Instant Trigger. In diesem Artikel werden die Verwendung und Funktionalität von Instant Triggers in Adobe Workfront Fusion beschrieben.
author: Becky
feature: Workfront Fusion
exl-id: 13b3a1bf-9856-4d2c-b1a5-13b044a7c2e5
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 0%

---

# Sofortige Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]

Viele Services stellen Webhooks bereit, mit denen sofortige Benachrichtigungen bereitgestellt werden können, sobald eine bestimmte Änderung im Service eintritt. Für die Verarbeitung dieser Benachrichtigungen empfehlen wir die Verwendung von Instant Trigger. Sie können diese in [!DNL Adobe Workfront Fusion] anhand ihres -Tags leicht erkennen:

![](assets/instant-350x256.png)

Wenn der Service keine Webhooks bereitstellt, müssen Sie Abruf-Trigger verwenden, um den Service regelmäßig abzufragen.

Eine Videoeinführung zu Webhooks in Workfront Fusion finden Sie unter:

* [Einführung in Webhooks](https://video.tv.adobe.com/v/3427025/){target=_blank}
* [Zwischen-Webhooks](https://video.tv.adobe.com/v/3427030/){target=_blank}

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

## Webhook-Warteschlange anzeigen

Alle Nachrichten von eingehenden Webhooks werden in der Warteschlange des Webhooks gespeichert.

1. Klicken Sie **[!UICONTROL Menü]** links auf „Webhooks“.
1. Suchen Sie den Webhook, für den Sie die Warteschlange anzeigen möchten.
1. Klicken Sie auf die Schaltfläche mit einem LKW-Symbol und der Anzahl der empfangenen Webhooks.

   ![](assets/webhooks-truck-icon.png)

   >[!NOTE]
   >
   >Eingehende Webhook-Daten werden immer in der Warteschlange gespeichert, unabhängig davon, wie Sie die Option [!UICONTROL Daten] festgelegt haben (beschrieben im [Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)). Sobald die Daten in einem Szenario verarbeitet werden, werden sie dauerhaft aus dem System gelöscht.

## Sofortige Trigger planen

Wenn Ihr Szenario einen sofortigen Trigger enthält, können Sie die sofortige Ausführung des Szenarios planen:

![](assets/schedule-setting-350x185.png)

In diesem Fall wird Ihr Szenario sofort ausgeführt, wenn [!DNL Workfront Fusion] neue Daten vom Service erhält. Nach Ausführung des Szenarios wird die Gesamtzahl der ausstehenden Webhooks in der Warteschlange gezählt, und das Szenario führt so viele Zyklen aus wie ausstehende Webhooks, wobei ein Webhook pro Zyklus verarbeitet wird. Weitere Informationen finden Sie unter [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

>[!NOTE]
>
>* Ein Zyklus ist nicht dasselbe wie eine Szenarioausführung. Innerhalb einer Szenario-Ausführung können mehrere Zyklen durchgeführt werden.
>* Wenn Sie ein Szenario ausführen, bei dem ein sofortiger Trigger geplant ist, gelten die folgenden Ausnahmen:
>
>     * Das Intervall zwischen zwei Ausführungen unterliegt nicht dem Mindestintervall gemäß Preisplan.
>
>       Wenn das Szenario beispielsweise seine Ausführung abgeschlossen hat, wird die Warteschlange des Webhooks erneut überprüft. Wenn Webhooks ausstehen, wird das Szenario sofort erneut ausgeführt und alle ausstehenden Webhooks werden erneut verarbeitet.
>   
>     * Die Einstellung Maximale Anzahl von Zyklen wird ignoriert und auf 100 gesetzt, was bedeutet, dass nicht mehr als 100 ausstehende Webhooks während einer einzelnen Szenario-Ausführung verarbeitet werden (mit der Rate von 1 Ereignis pro einem Zyklus).
>


Wenn Sie eine andere Zeitplaneinstellung als &quot;[!UICONTROL &quot; verwenden] wird das Szenario in den von Ihnen angegebenen Intervallen ausgeführt. Da während des Intervalls mehrere Webhooks in der Warteschlange gesammelt werden können, wird empfohlen, die [[!UICONTROL Maximale Anzahl von Zyklen]](../../workfront-fusion/scenarios/scenario-settings-panel.md#maximum) auf einen höheren Wert als den Standardwert 1 festzulegen, um mehr Webhooks in einer Szenario-Ausführung zu verarbeiten:

1. Klicken Sie auf [!UICONTROL  Symbol ]Szenario-Einstellungen![](assets/gear-icon-settings.png) am unteren Rand Ihres Szenarios.
1. Geben Sie in das ]****[!UICONTROL  Szenarioeinstellungen eine Zahl in das Feld **[!UICONTROL Maximale Anzahl von Zyklen]** ein, um die Anzahl der Webhooks aus der Warteschlange anzugeben, die bei jeder Ausführung des Szenarios ausgeführt werden sollen.

## Ratenbeschränkungen

Die aktuelle Ratenbeschränkung beträgt 5 Webhooks pro Sekunde. Wenn das Limit überschritten wird, wird ein 429-Status-Code zurückgegeben.

## Ablauf inaktiver Webhooks

Ein Webhook, der seit mehr als 120 Stunden keinem Szenario zugewiesen wurde, wird entfernt.

## Webhook-Payloads

[!DNL Workfront Fusion] speichert Webhook-Payloads 30 Tage lang. Wenn Sie mehr als 30 Tage nach der Erstellung auf eine Webhook-Payload zugreifen, wird der Fehler &quot;[!UICONTROL Datei konnte nicht aus dem Speicher gelesen werden“ ].

## Fehlerbehandlung

Wenn in Ihrem Szenario ein Fehler mit einem sofortigen Trigger auftritt, wird das Szenario:

* Beendet sofort , wenn das Szenario auf „Sofort[!UICONTROL  eingestellt ].
* Beendet nach drei fehlgeschlagenen Versuchen (drei Fehlern) - wenn das Szenario so ausgeführt wird, dass es wie geplant ausgeführt wird.

Wenn während der Ausführung des Szenarios ein Fehler auftritt, wird der Webhook während der Rollback-Phase des sofortigen Triggers wieder in die Warteschlange platziert. In einem solchen Fall haben Sie die Möglichkeit, das Szenario zu beheben und es erneut auszuführen. Weitere Informationen finden Sie unter [Rollback](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) im Artikel [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Wenn in Ihrem Szenario ein Webhook-Antwortmodul vorhanden ist, wird der Fehler an die Webhook-Antwort gesendet. Das Webhook-Antwortmodul wird immer zuletzt ausgeführt (in dem Fall, [!UICONTROL  die Option &quot;] Commit“ in den Szenario-Einstellungen nicht aktiviert ist). Weitere Informationen finden Sie unter [Reagieren auf Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md#respondi) im Artikel [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Benutzerdefinierte Webhooks

Sie können Ihre eigenen Webhooks erstellen. Weitere Informationen finden Sie unter [Webhooks](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md).

## Webhook-Deaktiviert

Webhooks werden automatisch deaktiviert, wenn einer der folgenden Punkte zutrifft:

* Der Webhook wurde seit mehr als 5 Tagen mit keinem Szenario verbunden
* Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

Deaktivierte Webhooks werden automatisch gelöscht und von der Registrierung entfernt, wenn sie mit keinem Szenario verbunden sind und sich seit mehr als 30 Tagen im Status Deaktiviert befinden.


