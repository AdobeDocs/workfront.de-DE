---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Behandlung von Wiederholungsfehlern in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Behandlung von Wiederholungsfehlern in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Problemumgehung für `retry` Fehlerbehandlung konfigurieren](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/retry.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einigen Fällen ist es nützlich, ein fehlerhaftes Modul erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler im Laufe der Zeit vergeht.

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

## Problemumgehungen für die [!UICONTROL Wiederholen]-Fehlerbehandlungsanweisung

[!UICONTROL Adobe Workfront Fusion] bietet derzeit nicht die [!UICONTROL Retry]-Fehlerbehandlungsdirektive, obwohl zwei Problemumgehungen angewendet werden können, um ihre Funktionalität nachzuahmen. Weitere Informationen finden Sie unter [Anweisungen für die Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Verwenden der [!UICONTROL Break]-Direktive

1. Aktivieren Sie im Bedienfeld Szenario-Einstellungen die Option **[!UICONTROL Speichern unvollständiger Ausführungen zulassen]**.

   Weitere Informationen finden Sie unter [Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Hängen Sie eine Fehler-Handler-Route an das Modul an, wie unter [Fehlerbehandlung in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md) beschrieben.
1. Verknüpfen Sie die [!UICONTROL break]-Direktive mit der Fehler-Handler-Route und konfigurieren Sie sie.

   Weitere Informationen finden Sie unter [Anweisungen für die Fehlerbehandlung in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nachteile

* Das Mindestintervall für weitere Zustellversuche beträgt eine Minute.
* Wenn das Modul mehrere Bundles verarbeitet und die Verarbeitung eines Bundles fehlschlägt, wird die partielle Ausführung (nur das Bundle, das den Fehler verursacht hat) in den Ordner „Unvollständige Ausführungen“ verschoben und für weitere Zustellversuche gemäß den Einstellungen der [!UICONTROL break]-Anweisung geplant. Die aktuelle Ausführung wird jedoch fortgesetzt und das Modul verarbeitet weiterhin die nachfolgenden Bundles. Sie können die Option &quot;[!UICONTROL Sequenzielle Verarbeitung]&quot; in den [!UICONTROL Szenarioeinstellungen“ aktivieren] um zu verhindern, dass das Szenario erneut ausgeführt wird, bis die im Ordner „Unvollständige Ausführungen“ gespeicherte Ausführung erfolgreich aufgelöst wurde.

  Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Verwenden des [!UICONTROL Repeater]-Moduls

1. Verwenden Sie das **[!UICONTROL Repeater]**-Modul und legen Sie sein **[!UICONTROL Repeats]**-Feld auf die maximale Anzahl der Versuche fest.
1. Verknüpfen Sie das Modul mit dem potenziell fehlerhaften **[!UICONTROL mit dem]**.
1. Fügen Sie diesem Modul eine Fehler-Handler-Route hinzu (siehe [Fehlerbehandlung in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Sleep]** mit der Fehler-Handler-Route und legen Sie **[!UICONTROL Feld Verzögerung]** auf die Anzahl der Sekunden zwischen den Versuchen fest.

1. Verknüpfen Sie die Direktive **[!UICONTROL Ignore]** nach dem Modul **[!UICONTROL Tools] > [!UICONTROL Sleep]** (siehe [Anweisungen zur Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Variable festlegen]** nach dem Modul, das möglicherweise fehlschlägt, und konfigurieren Sie es so, dass das Ergebnis des Moduls in einer Variablen gespeichert wird, die z. B. `Result` heißt.

1. Verknüpfen Sie das Modul **[!UICONTROL Array]** nach dem **[!UICONTROL Tools] > [!UICONTROL Variable festlegen]** und wählen Sie das Modul **[!DNL Repeater]** in seinem Feld Source-Modul aus.

1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Variable abrufen]** mit dem **[!UICONTROL Array-Aggregator]**-Modul und konfigurieren Sie es so, dass der Wert der `Result`-Variable abgerufen wird.

1. Fügen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL GET variable]** zwischen dem **[!UICONTROL Repeater]**-Modul und dem möglicherweise fehlerhaften Modul ein und konfigurieren Sie es so, dass es den Wert der `Result`-Variablen erhält.

1. Fügen Sie einen Filter zwischen diesem Modul **[!UICONTROL Tools] > [!UICONTROL Variable abrufen]** und dem Modul ein, das möglicherweise fehlschlägt, und fahren Sie nur fort, wenn die `Result` nicht vorhanden ist.

>[!INFO]
>
>**Beispiel:** Hier ist ein Beispielszenario, in dem das [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen]-Modul das potenziell fehlerhafte Modul darstellt:
>
>![](assets/http-make-request-350x116.png)
>
>Wenn das Ergebnis des potenziell fehlschlagenden Moduls zu komplex ist, um in einer einfachen Variablen gespeichert zu werden, können Sie einen Datenspeicher verwenden, um das Ergebnis zu speichern/abzurufen. Der Datenspeicher würde nur einen Datensatz enthalten. Der Schlüssel des Datensatzes kann beispielsweise `Result` sein.
>
>Weitere Informationen zu Datenspeichern finden Sie unter [Datenspeicher in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Nachteil

Diese Problemumgehung mag etwas zu komplex erscheinen und ist auch im Hinblick auf den Betrieb anspruchsvoller.
