---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Umgang mit Fehlern wiederholen in [!DNL Adobe Workfront Fusion]
description: In einigen Fällen ist es nützlich, ein fehlerhaftes Modul mehrmals erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Umgang mit Fehlern wiederholen in [!DNL Adobe Workfront Fusion]

In einigen Fällen ist es nützlich, ein fehlerhaftes Modul erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.

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

## Problemumgehungen für [!UICONTROL Wiederholen] Richtlinie zur Fehlerbehebung

[!UICONTROL Adobe Workfront Fusion] bietet derzeit die [!UICONTROL Wiederholen] Fehlerbearbeitungsrichtlinie, obwohl zwei Problemumgehungen verwendet werden können, um deren Funktionalität zu imitieren. Weitere Informationen finden Sie unter [Richtlinien für die Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Verwenden Sie die [!UICONTROL Break] Richtlinie

1. Aktivieren Sie im Bereich mit den Szenario-Einstellungen die **[!UICONTROL Speichern nicht abgeschlossener Ausführungen zulassen]** -Option.

   Weitere Informationen finden Sie unter [Das Bedienfeld für die Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Hängen Sie eine Fehler-Handler-Route an das Modul an, wie unter [Umgang mit Fehlern in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. Verknüpfen Sie die [!UICONTROL Break] -Anweisung zur Route des Fehler-Handlers hinzu und konfigurieren Sie sie.

   Weitere Informationen finden Sie unter [Richtlinien zur Fehlerbehandlung in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nachteile

* Das Wiederholungsintervall beträgt mindestens eine Minute.
* Wenn das Modul mehrere Bundles verarbeitet und die Verarbeitung eines Bundles fehlschlägt, wird die partielle Ausführung (nur das Bundle, das den Fehler verursacht hat) in den Ordner der unvollständigen Ausführungen verschoben und für weitere Versuche gemäß der Variablen [!UICONTROL Break] Richtlinieneinstellungen. Die aktuelle Ausführung wird jedoch fortgesetzt und das Modul verarbeitet die nachfolgenden Bundles weiter. Sie können den[!UICONTROL Sequenzielle Verarbeitung]&quot; in der [!UICONTROL Szenario-Einstellungen] , um zu verhindern, dass das Szenario erneut ausgeführt wird, bis die im Ordner Unvollständige Ausführungen gespeicherte Ausführung erfolgreich aufgelöst wurde.

  Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Unvollständige Ausführungen anzeigen und auflösen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Verwenden Sie die [!UICONTROL Repeater] Modul

1. Verwenden Sie die **[!UICONTROL Repeater]** -Modul und legen Sie **[!UICONTROL Wiederholungen]** -Feld zur maximalen Anzahl von Versuchen.
1. Verknüpfen Sie das potenziell fehlerhafte Modul mit dem **[!UICONTROL Repeater]** -Modul.
1. Hängen Sie eine Fehler-Handler-Route an dieses Modul an (siehe [Umgang mit Fehlern in [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Verknüpfen Sie die **[!UICONTROL Instrumente] > [!UICONTROL Schlafen]** -Modul auf die Fehler-Handler-Route zu und legen Sie deren **[!UICONTROL Verzögerung]** auf die Anzahl der Sekunden zwischen den Versuchen.

1. Verknüpfen Sie die **[!UICONTROL Ignorieren]** Richtlinie nach **[!UICONTROL Instrumente] > [!UICONTROL Schlafen]** -Modul (siehe [Richtlinien für die Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Verknüpfen Sie die **[!UICONTROL Instrumente] > [!UICONTROL Variable festlegen]** -Modul nach dem potenziell fehlerhaften Modul platzieren und es so konfigurieren, dass das Ergebnis des Moduls in einer Variablen namens gespeichert wird, z. B. `Result`.

1. Verknüpfen Sie die **[!UICONTROL Array-Aggregator]** -Modul nach **[!UICONTROL Instrumente] > [!UICONTROL Variable festlegen]** und wählen Sie die **[!DNL Repeater]** -Modul im Feld &quot;Quellmodul&quot;ein.

1. Verknüpfen Sie die **[!UICONTROL Instrumente] > [!UICONTROL Variable abrufen]** -Modul **[!UICONTROL Array-Aggregator]** -Modul und konfigurieren Sie es, um den Wert der `Result` -Variable.

1. Fügen Sie die **[!UICONTROL Instrumente] > [!UICONTROL Variable abrufen]** -Modul zwischen **[!UICONTROL Repeater]** -Modul und dem potenziell fehlerhaften Modul verwenden und konfigurieren, um den Wert der `Result` -Variable.

1. Filter dazwischen einfügen **[!UICONTROL Instrumente] > [!UICONTROL Variable abrufen]** -Modul und dem potenziell fehlenden Modul nur dann fortgesetzt werden, wenn die `Result` nicht vorhanden ist.

>[!INFO]
>
>**Beispiel:** Im Folgenden finden Sie ein Beispielszenario mit der Variablen [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] -Modul steht für das potenziell fehlerhafte Modul:
>
>![](assets/http-make-request-350x116.png)
>
>Wenn das Ergebnis des potenziell fehlerhaften Moduls zu komplex für die Speicherung in einer einfachen Variablen ist, können Sie einen Datenspeicher verwenden, um das Ergebnis zu speichern/abzurufen. Der Datenspeicher würde nur einen Datensatz enthalten. Der Schlüssel des Datensatzes kann beispielsweise `Result`.
>
>Weitere Informationen zu Datenspeichern finden Sie unter [Datenspeicher in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Rückruf

Diese Problemumgehung kann etwas zu komplex erscheinen und ist auch im Hinblick auf den Betrieb anspruchsvoller.
