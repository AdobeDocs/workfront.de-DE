---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Übersicht über das Adobe Workfront Fusion-Szenario
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: 13d6230d-51f6-4f68-8697-30f8ce6c8599
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Übersicht über Szenarien

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert [!DNL Adobe Workfront Fusion] zusätzlich zu einer [!DNL Adobe Workfront license].

>[!IMPORTANT]
>
>[!DNL Workfront Fusion] Szenarien sollten nicht mit [!DNL Workfront Scenario Planner] Szenarien. Informationen zu [!DNL Workfront Scenario Planner] Szenarien, siehe [Die [!DNL Scenario Planner] Übersicht](../../scenario-planner/scenario-planner-overview.md).

Die Rolle von [!DNL Adobe Workfront Fusion] ist es, Ihre Prozesse zu automatisieren, sodass Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Diensten, um ein Szenario zu erstellen, in dem Ihre Daten automatisch übertragen und transformiert werden. Das Szenario, in dem Sie Watches für Daten in einer App oder einem Dienst erstellen und diese Daten verarbeiten, um das gewünschte Ergebnis zu liefern.

Ein Szenario besteht aus einer Reihe von Modulen, die angeben, wie Daten in einer App umgewandelt oder zwischen Apps und Webdiensten übertragen werden sollen.

## Beispiel: Automatisieren von Prozessen in [!DNL Adobe Workfront]

>[!NOTE]
>
>Diese Funktion ist für die folgenden Lizenzen verfügbar:
>
>* [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]
>* [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration]
>


[!DNL Workfront Fusion] ermöglicht Ihnen die Automatisierung einfacher oder komplexer Workflows in [!DNL Workfront], wodurch Zeit gespart und sichergestellt wird, dass der Prozess konsistent ausgeführt wird.

In diesem Beispiel wird das Szenario Trigger, wenn sich ein bestimmtes Feld in einer Aufgabe oder einem Problem in [!DNL Workfront]. Wenn das Szenario ausgelöst wird, ruft es Informationen im zugehörigen Projekt ab und erstellt ein maßgeschneidertes Update für eine Person, die einer bestimmten Rolle im Projekt zugewiesen ist.

![](assets/fusion-template-example-350x102.png)

## Beispiel: Verbinden [!DNL Workfront] zu einer anderen App oder einem Webdienst

>[!NOTE]
>
>Diese Funktion ist für die folgende Lizenz verfügbar:
>
>* [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration]
>


[!DNL Workfront Fusion] Sie können auch eine Verbindung zu anderen Apps und Webdiensten herstellen. Sie können auf Daten aus anderen Anwendungen zugreifen, diese importieren, bearbeiten oder exportieren und sie in Workfront oder miteinander integrieren. Viele Anwendungen verfügen über dedizierte [!DNL Workfront Fusion] Connectoren. Wenn für die Anwendung, auf die Sie zugreifen möchten, kein dedizierter Connector vorhanden ist, können Sie [!DNL Workfront Fusion]s [!UICONTROL HTTP] oder [!UICONTROL SOAP] -Module, um über die API eine Verbindung zur Anwendung herzustellen.

In diesem Beispiel wird das Szenario Trigger, wenn ein Benutzer einem [!DNL Excel] Tabelle. Das Szenario überprüft, ob sich der Benutzer in [!DNL Workfront]. Wenn nicht, wird der Benutzer im Szenario in [!DNL Workfront] und fügt ihre Workfront-Benutzer-ID wieder in die Tabelle ein.

![](assets/fusion-integration-example--350x171.png)

Eine Liste der dedizierten Connectoren finden Sie unter [Apps und ihre Module](../../workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

>[!IMPORTANT]
>
>[!DNL Adobe Workfront Fusion] kann eine Verbindung zu fast jedem Webdienst herstellen. Wenn die App, mit der Sie arbeiten möchten, nicht über eine dedizierte [!DNL Workfront Fusion] -Connector können Sie die folgenden Module verwenden, um eine direkte Verbindung zum Webdienst herzustellen:
>
>* [[!UICONTROL HTTP] Module](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)
>* [[!UICONTROL SOAP] Modul](../../workfront-fusion/apps-and-their-modules/soap-module.md)
>* [[!UICONTROL JSON] Module](../../workfront-fusion/apps-and-their-modules/json-modules.md)
>

