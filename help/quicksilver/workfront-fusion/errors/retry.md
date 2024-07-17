---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Fehlerbehandlung in [!DNL Adobe Workfront Fusion] wiederholen
description: In einigen Fällen ist es nützlich, ein fehlerhaftes Modul mehrmals erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Fehlerbehandlung in [!DNL Adobe Workfront Fusion] wiederholen

In einigen Fällen ist es nützlich, ein fehlerhaftes Modul erneut auszuführen, wenn die Wahrscheinlichkeit besteht, dass der Grund für den Fehler mit der Zeit vergeht.

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
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

## Problemumgehungen zur Fehlerbehandlungsrichtlinie [!UICONTROL Retry]

[!UICONTROL Adobe Workfront Fusion] bietet derzeit nicht die Fehlerbearbeitungsrichtlinie [!UICONTROL Retry] , obwohl zwei Problemumgehungen verwendet werden können, um die Funktionalität zu imitieren. Weitere Informationen finden Sie unter [Richtlinien für die Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

### Verwenden der Anweisung [!UICONTROL Break]

1. Aktivieren Sie im Bereich mit den Szenario-Einstellungen die Option **[!UICONTROL Speicherung unvollständiger Ausführungen zulassen]** .

   Weitere Informationen finden Sie unter [Das Bedienfeld mit den Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. Verbinden Sie das Modul mit einer Fehler-Handler-Route, wie unter [Umgang mit Fehlern in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md) beschrieben.
1. Verbinden Sie die Anweisung [!UICONTROL Break] mit der Route des Fehler-Handlers und konfigurieren Sie sie.

   Weitere Informationen finden Sie unter [Richtlinien für die Fehlerbehandlung in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### Nachteile

* Das Wiederholungsintervall beträgt mindestens eine Minute.
* Wenn das Modul mehrere Bundles verarbeitet und die Verarbeitung eines Bundles fehlschlägt, wird die partielle Ausführung (nur das Bundle, das den Fehler verursacht hat) in den Ordner der unvollständigen Ausführungen verschoben und für weitere Versuche gemäß den Einstellungen der Anweisung [!UICONTROL Break] geplant. Die aktuelle Ausführung wird jedoch fortgesetzt und das Modul verarbeitet die nachfolgenden Bundles weiter. Sie können die Option &quot;[!UICONTROL Sequenzielle Verarbeitung]&quot; in den [!UICONTROL Szenario-Einstellungen] aktivieren, um zu verhindern, dass das Szenario erneut ausgeführt wird, bis die im Ordner Unvollständige Ausführungen gespeicherte Ausführung erfolgreich aufgelöst wurde.

  Weitere Informationen zu unvollständigen Ausführungen finden Sie unter [Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Verwenden des Moduls [!UICONTROL Repeater]

1. Verwenden Sie das Modul **[!UICONTROL Repeater]** und legen Sie für das Feld **[!UICONTROL Repeats]** die maximale Anzahl von Versuchen fest.
1. Verknüpfen Sie das potenziell fehlerhafte Modul mit dem Modul **[!UICONTROL Repeater]** .
1. Fügen Sie diesem Modul eine Fehler-Handler-Route hinzu (siehe [Umgang mit Fehlern in  [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)).
1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Schlachten]** mit der Route des Fehler-Handlers und legen Sie für das Feld **[!UICONTROL Verzögerung]** die Anzahl der Sekunden zwischen den Versuchen fest.

1. Verknüpfen Sie die Anweisung **[!UICONTROL Ignore]** nach dem Modul **[!UICONTROL Tools] > [!UICONTROL Schlaf]** (siehe [Richtlinien für die Fehlerbehandlung in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)).

1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Variable festlegen]** nach dem potenziell fehlerhaften Modul und konfigurieren Sie es so, dass das Ergebnis des Moduls in einer Variablen namens, z. B. `Result`, gespeichert wird.

1. Verknüpfen Sie das Modul **[!UICONTROL Array aggregator]** nach dem Modul **[!UICONTROL Tools] > [!UICONTROL Variable festlegen]** und wählen Sie im Feld &quot;Source-Modul&quot;das Modul **[!DNL Repeater]** aus.

1. Verknüpfen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Variable abrufen]** mit dem Modul **[!UICONTROL Array-Aggregator]** und konfigurieren Sie es so, dass der Wert der Variable `Result` abgerufen wird.

1. Fügen Sie das Modul **[!UICONTROL Tools] > [!UICONTROL Variable abrufen]** zwischen dem Modul **[!UICONTROL Repeater]** und dem potenziell fehlenden Modul ein und konfigurieren Sie es, um den Wert der Variable `Result` zu erhalten.

1. Fügen Sie einen Filter zwischen diesem Modul **[!UICONTROL Tools] > [!UICONTROL Variable abrufen]** ein und setzen Sie das potenziell fehlende Modul so ein, dass nur dann fortgesetzt wird, wenn die Variable `Result` nicht vorhanden ist.

>[!INFO]
>
>**Beispiel:** Hier ist ein Beispielszenario, bei dem das Modul [!UICONTROL HTTP] >[!UICONTROL Anfrage stellen] das potenziell fehlerhafte Modul darstellt:
>
>![](assets/http-make-request-350x116.png)
>
>Wenn das Ergebnis des potenziell fehlerhaften Moduls zu komplex für die Speicherung in einer einfachen Variablen ist, können Sie einen Datenspeicher verwenden, um das Ergebnis zu speichern/abzurufen. Der Datenspeicher würde nur einen Datensatz enthalten. Der Schlüssel des Datensatzes kann beispielsweise `Result` sein.
>
>Weitere Informationen zu Datenspeichern finden Sie unter [Datenspeicher in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### Rückruf

Diese Problemumgehung kann etwas zu komplex erscheinen und ist auch im Hinblick auf den Betrieb anspruchsvoller.
