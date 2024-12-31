---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]
description: Der Ordner [!UICONTROL Unvollständige Ausführungen] speichert Szenario-Ausführungen, die aufgrund eines Fehlers nicht erfolgreich abgeschlossen wurden. Jede gespeicherte unvollständige Ausführung kann entweder manuell oder automatisch aufgelöst werden.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 53582d36ef2256f6073705ce3eabe8cd61c9b2cc
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 5%

---

# Anzeigen und Auflösen unvollständiger Ausführungen in [!DNL Adobe Workfront Fusion]

Der Ordner [!UICONTROL Unvollständige Ausführungen] speichert Szenario-Ausführungen, die aufgrund eines Fehlers nicht erfolgreich abgeschlossen wurden. Jede gespeicherte unvollständige Ausführung kann entweder manuell oder automatisch aufgelöst werden.

>[!NOTE]
>
>Standardmäßig ist das Speichern unvollständiger Ausführungen deaktiviert. Um sie zu aktivieren, aktivieren Sie die Option [!UICONTROL Speichern unvollständiger Ausführungen zulassen] in den erweiterten Einstellungen des Szenarios.
>
>Weitere Informationen zu Szenarioeinstellungen finden Sie unter [Das Bedienfeld „Szenarioeinstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Anzeigen unvollständiger Ausführungen

Wenn bei einem Modul während seines Vorgangs ein Fehler auftritt, wird eine neue unvollständige Ausführung zum Ordner Unvollständige Ausführungen hinzugefügt. Jede unvollständige Ausführung enthält den Blueprint des Szenarios und alle Bundles, die dem fehlgeschlagenen Modul zugeordnet werden können. Die Liste der unvollständigen Ausführungen kann durch Klicken auf die Registerkarte [!UICONTROL Unvollständige Ausführungen] auf der Seite mit den Szenario-Details geöffnet werden.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

Weitere Informationen finden Sie unter [Fehler, die zu unvollständigen Ausführungen führen](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>Die aktuelle Größenbeschränkung des nicht aufgelösten Ordners „Unvollständige Ausführungen“ pro Organisation beträgt 500 MB. Wenn Ihre Organisation dieses Limit überschreitet, wird möglicherweise der folgende Fehler angezeigt:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Weitere Informationen finden Sie unter [Datenverlust aktivieren](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) im [Bedienfeld „Szenarioeinstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Unvollständige Ausführungen auflösen

Wenn eine neue unvollständige Ausführung gespeichert wird, können Sie sie wie folgt auflösen:

1. Klicken Sie auf die **[!UICONTROL Unvollständige Ausführungen]**.
1. Suchen Sie die unvollständige Ausführung, die Sie auflösen möchten, und klicken Sie auf **[!UICONTROL Detail]**.


   Wenn Sie das Protokoll aller Modulvorgänge anzeigen möchten, bevor Sie versuchen, die unvollständige Ausführung aufzulösen, können Sie die unvollständige Ausführung über den Ordner [!UICONTROL Verlauf] auflösen:

1. Klicken Sie auf die **[!UICONTROL Verlauf]**.
1. Suchen Sie das fehlgeschlagene Ausführungsprotokoll des Szenarios und klicken Sie auf **[!UICONTROL Details]**.
1. Öffnen Sie das Protokoll des Moduls, in dem alle Vorgänge des Moduls angezeigt werden.
1. Suchen Sie den fehlgeschlagenen Vorgang und klicken Sie auf **[!UICONTROL Auflösen]**:

   ![](assets/resolve-btn-350x188.png)

## Optionen im Zusammenhang mit unvollständigen Ausführungen

Die folgenden Optionen im Bedienfeld [!UICONTROL Szenarioeinstellungen] bestimmen, ob und wie die unvollständigen Ausführungen gespeichert werden:

* Speichern unvollständiger Ausführungen zulassen
* Sequenzielle Verarbeitung
* Datenverlust aktivieren

Weitere Informationen zu diesen Optionen finden Sie unter [Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Fehler führen zu unvollständigen Ausführungen

Es gibt verschiedene Kategorien von Fehlern, die zur Speicherung unvollständiger Ausführungen führen. Dazu können gehören:

* Validierungsfehler, die aus unvollständigen oder fehlerhaften Daten resultieren, hauptsächlich aufgrund eines fehlenden Elements, das erwartet wird, um alle Daten, die ein Modul durchlaufen, erfolgreich zu verarbeiten.
* Fehler, die durch die Nichtverfügbarkeit des endgültigen Ziels aufgrund eines temporären oder langfristigen Verbindungsfehlers auftreten (z. B. während der Verbindung zu einem E-Mail- oder FTP-Remote-Server).

Tritt beim ersten Modul des Szenarios ein Fehler auf, wird die Ausführung sofort gestoppt und keine unvollständige Ausführung gespeichert.

Wenn ein Fehler bei einem anderen Modul auftritt und keine Fehler-Handler-Route angehängt ist, tritt einer der folgenden Fälle auf:

* Wenn der Fehlertyp `ConnectionError`, `RateLimitError`, `OutOfSpaceError` oder `ModuleTimeoutError` ist, wird ein unvollständiger Ausführungseintrag mit automatischem Wiederholungsversuch gespeichert.
* Wenn der Fehlertyp `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` oder `MaxResultsExceededError` lautet, wird ein unvollständiger Ausführungsdatensatz ohne automatische Wiederholung gespeichert.
* Bei allen anderen als den oben genannten Fehlertypen schlägt die Ausführung fehl.
