---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Unvollständige Ausführungen in [!DNL Adobe Workfront Fusion] anzeigen und auflösen
description: Der Ordner [!UICONTROL Unvollständige Ausführungen] speichert Szenario-Ausführungen, die aufgrund eines Fehlers nicht erfolgreich abgeschlossen wurden. Jede gespeicherte unvollständige Ausführung kann entweder manuell oder automatisch aufgelöst werden.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 5%

---

# Unvollständige Ausführungen in [!DNL Adobe Workfront Fusion] anzeigen und auflösen

Der Ordner [!UICONTROL Unvollständige Ausführungen] speichert Szenario-Ausführungen, die aufgrund eines Fehlers nicht erfolgreich abgeschlossen wurden. Jede gespeicherte unvollständige Ausführung kann entweder manuell oder automatisch aufgelöst werden.

>[!NOTE]
>
>Standardmäßig ist die Speicherung unvollständiger Ausführungen deaktiviert. Aktivieren Sie dazu in den erweiterten Szenario-Einstellungen die Option [!UICONTROL Speicherung unvollständiger Ausführungen zulassen] .
>
>Weitere Informationen zu den Szenario-Einstellungen finden Sie unter [Bedienfeld mit den Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## Unvollständige Ausführungen anzeigen

Wenn bei einem Modul während des Vorgangs ein Fehler auftritt, wird dem Ordner Unvollständige Ausführungen eine neue unvollständige Ausführung hinzugefügt. Jede unvollständige Ausführung enthält den Blueprint des Szenarios und alle Bundles, die dem fehlerhaften Modul zugeordnet werden können. Die Liste der unvollständigen Ausführungen kann durch Klicken auf die Registerkarte [!UICONTROL Unvollständige Ausführungen] auf der Detailseite des Szenarios geöffnet werden:

![](assets/incomplete-executions-tab-350x102.png)

Weitere Informationen finden Sie unter [Fehler, die zu unvollständigen Ausführungen führen](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>Die aktuelle Größenbeschränkung für den nicht aufgelösten unvollständigen Ausführungsordner pro Organisation beträgt 500 MB. Wenn Ihr Unternehmen diese Grenze überschreitet, wird möglicherweise der folgende Fehler angezeigt:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Weitere Informationen finden Sie unter [Datenverlust aktivieren](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [Das Bedienfeld mit den Szenario-Einstellungen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Unvollständige Ausführungen auflösen

Wenn eine neue unvollständige Ausführung gespeichert wird, können Sie sie wie folgt auflösen:

1. Klicken Sie auf die Registerkarte **[!UICONTROL Nicht abgeschlossene Ausführungen]**.
1. Suchen Sie die unvollständige Ausführung, die Sie auflösen möchten, und klicken Sie auf **[!UICONTROL Detail]**.


   Wenn Sie das Protokoll aller Vorgänge des Moduls sehen möchten, bevor Sie versuchen, die unvollständige Ausführung zu beheben, können Sie die unvollständige Ausführung im Ordner [!UICONTROL Verlauf] auflösen:

1. Klicken Sie auf die Registerkarte **[!UICONTROL Verlauf]**.
1. Suchen Sie das fehlgeschlagene Ausführungsprotokoll des Szenarios und klicken Sie auf **[!UICONTROL Details]**.
1. Öffnen Sie das Protokoll des Moduls, in dem alle Vorgänge des Moduls angezeigt werden.
1. Suchen Sie den fehlgeschlagenen Vorgang und klicken Sie auf **[!UICONTROL Auflösen]**:

   ![](assets/resolve-btn-350x188.png)

## Optionen für unvollständige Ausführungen

Die folgenden Optionen im Bedienfeld [!UICONTROL Szenario-Einstellungen] bestimmen, ob und wie die unvollständigen Ausführungen gespeichert werden:

* Speichern unvollständiger Ausführungen zulassen
* Sequenzielle Verarbeitung
* Datenverlust aktivieren

Weitere Informationen zu diesen Optionen finden Sie unter [Das Bedienfeld mit den Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Fehler, die zu unvollständigen Ausführungen führten

Es gibt mehrere Fehlerkategorien, die dazu führen, dass unvollständige Ausführungen gespeichert werden. Dazu können gehören:

* Validierungsfehler, die aus unvollständigen oder fehlerhaften Daten resultieren, hauptsächlich aufgrund eines fehlenden Elements, das erwartet wird, um alle Daten, die ein Modul durchlaufen, erfolgreich zu verarbeiten.
* Fehler, die auftreten, wenn das endgültige Ziel aufgrund eines temporären oder langfristigen Verbindungsfehlers nicht verfügbar ist (z. B. bei der Verbindung mit einem E-Mail- oder Remote-FTP-Server).

Tritt beim ersten Modul des Szenarios ein Fehler auf, wird die Ausführung sofort gestoppt und keine unvollständige Ausführung gespeichert.

Wenn bei einem anderen Modul ein Fehler auftritt und keine Fehler-Handler-Route angehängt ist, tritt einer der folgenden Fehler auf:

* Wenn der Fehlertyp `ConnectionError`, `RateLimitError`, `OutOfSpaceError` oder `ModuleTimeoutError` ist, wird ein unvollständiger Ausführungs-Datensatz mit automatischem Wiederholungsversuch gespeichert.
* Wenn der Fehlertyp `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` oder `MaxResultsExceededError` lautet, wird ein unvollständiger Ausführungs-Datensatz ohne automatische Wiederholung gespeichert.
* Bei allen anderen als den oben genannten Fehlertypen schlägt die Ausführung fehl.
