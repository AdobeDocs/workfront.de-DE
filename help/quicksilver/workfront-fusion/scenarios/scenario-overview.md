---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Übersicht über das Adobe Workfront Fusion-Szenario
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Übersicht über [!DNL Adobe Workfront Fusion] Szenario

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Szenario - Übersicht](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/scenario-overview.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] benötigt zusätzlich zu einer [!DNL Adobe Workfront license] eine [!DNL Adobe Workfront Fusion].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] Szenarien sollten nicht mit [!DNL Workfront Scenario Planner] Szenarien verwechselt werden. Weitere Informationen zu [!DNL Workfront Scenario Planner] finden Sie unter [The [!DNL Scenario Planner] overview](../../scenario-planner/scenario-planner-overview.md).

Die Rolle von [!DNL Adobe Workfront Fusion] besteht darin, Ihre Prozesse zu automatisieren, damit Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Services, um ein Szenario zu erstellen, das Ihre Daten automatisch überträgt und transformiert. Das Szenario, in dem Sie Daten in einer App oder einem Service erstellen, überwacht und verarbeitet diese Daten, um das gewünschte Ergebnis zu liefern.

Ein Szenario besteht aus einer Reihe von Modulen, die angeben, wie Daten innerhalb einer App transformiert oder zwischen Apps und Web-Services übertragen werden sollen.

## Übersicht über Szenarioelemente

Ein Szenario besteht aus verschiedenen Elementen. Die Verwendung der Dokumentation wird durch das Verständnis der Terminologie dieser Elemente erleichtert.

### Szenario

Ein **Szenario** ist eine vom Benutzer erstellte Reihe automatisierter Schritte, mit denen Daten verschoben und bearbeitet werden. Der Begriff „Szenario“ bezieht sich auf die gesamte Gruppe verbundener Schritte.

![Szenario](assets/entire-scenario-scenario.png)

### Trigger

Ein Szenario beginnt mit einem **Trigger**. Der Trigger sucht nach neuen und aktualisierten Daten und startet das Szenario, wenn bestimmte im Modul konfigurierte Bedingungen zutreffen. Trigger können so konfiguriert werden, dass ein Szenario nach einem Zeitplan (Abrufen) oder bei jeder Datenänderung (sofortig) gestartet wird.

![Trigger ](assets/scenario-trigger.png)

### Modul

Auf den Trigger folgt eine Reihe **Module**. Ein Modul stellt einen einzelnen Schritt in einem Szenario dar, das eine bestimmte Aktion ausführt. Module werden konfiguriert und miteinander verkettet, um Szenarien zu erstellen.

![MODULE](assets/scenario-module.png)

### Route

Ein Szenario kann in &quot;**&quot; unterteilt**. Eine Route ist ein Abschnitt des Szenarios, der für ein bestimmtes Datenpaket verwendet werden kann oder nicht. Routen werden mithilfe eines Routermoduls und von Filtern eingerichtet.

![Route](assets/scenario-route.png)

### Szenario-Segment

Ein Szenario-Segment ist ein Abschnitt eines Szenarios, das aus einer Reihe zusammenhängender Module besteht, die alle mit derselben Anwendung verbunden sind. Szenario-Segmente stellen oft einen kurzen Workflow im Programm dar.

![Szenario-Segment](assets/scenario-segment.png)

### Connector

Ein Connector ist ein Satz von Modulen für eine bestimmte Anwendung. Workfront Fusion bietet Connectoren für viele gängige Arbeitsanwendungen wie Workfront, Salesforce und Jira sowie generische Connectoren, die für jeden Webservice verwendet werden können.

![Connectoren](assets/scenario-connectors.png)



## Beispiel: Automatisieren von Prozessen in [!DNL Adobe Workfront]

>[!NOTE]
>
>Diese Funktion ist für die folgenden Lizenzen verfügbar:
>
>* [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]
>* [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und -integration]

[!DNL Workfront Fusion] können Sie einfache oder komplexe Workflows innerhalb von [!DNL Workfront] automatisieren, was Zeit spart und sicherstellt, dass der Prozess konsistent ausgeführt wird.

In diesem Beispiel tritt ein Trigger auf, wenn sich ein angegebenes Feld in einer Aufgabe oder einem Problem in [!DNL Workfront] ändert. Nach der Auslösung ruft das Szenario Informationen im zugehörigen Projekt ab und erstellt eine maßgeschneiderte Aktualisierung für eine Person, die einer bestimmten Rolle im Projekt zugewiesen wurde.

![](assets/fusion-template-example-350x102.png)

## Beispiel: Verbinden von [!DNL Workfront] mit einer anderen App oder einem anderen Webservice

>[!NOTE]
>
>Diese Funktion ist für die folgende Lizenz verfügbar:
>
>* [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und -integration]
>

[!DNL Workfront Fusion] können auch eine Verbindung zu anderen Apps und Web-Services herstellen. Sie können auf Daten aus anderen Programmen zugreifen, diese importieren, bearbeiten oder exportieren und dabei in Workfront oder miteinander integrieren. Viele Anwendungen verfügen über dedizierte [!DNL Workfront Fusion]. Wenn für die Anwendung, auf die Sie zugreifen möchten, kein dedizierter Connector vorhanden ist, können Sie die [!UICONTROL HTTP]- oder [!UICONTROL SOAP]-Module von [!DNL Workfront Fusion] verwenden, um über die API eine Verbindung zur Anwendung herzustellen.

In diesem Beispiel tritt beim Szenario ein Trigger auf, wenn ein(e) Benutzende(r) zu einer [!DNL Excel] Tabelle hinzugefügt wird. Das Szenario prüft, ob sich der Benutzer in [!DNL Workfront] befindet. Andernfalls wird der Benutzer in [!DNL Workfront] erstellt und seine Workfront-Benutzer-ID wird wieder in die Tabelle eingefügt.

![](assets/fusion-integration-example--350x171.png)

Eine Liste der dedizierten Connectoren finden Sie unter [Apps und ihre Module](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] kann eine Verbindung zu fast jedem Webdienst herstellen. Wenn die App, mit der Sie arbeiten möchten, keinen dedizierten [!DNL Workfront Fusion]-Connector hat, können Sie die folgenden Module verwenden, um eine direkte Verbindung zum Webservice herzustellen:
>
>* [[!UICONTROL HTTP]-Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP]-Modul](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON]-Module](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>
