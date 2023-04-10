---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Integrationsmethoden von Adobe Workfront
description: Sie können [!DNL Adobe Workfront] mit Drittanbieteranwendungen. Diese Integrationen können die Nützlichkeit von [!DNL Workfront] und passen Sie sie an die Bedürfnisse Ihrer Organisation an. Sie können eine oder alle dieser Integrationen verwenden, je nachdem, welche für eine bestimmte Aufgabe am nützlichsten ist.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# Integrationsmethoden von Adobe Workfront

Sie können [!DNL Adobe Workfront] mit Drittanbieteranwendungen sowie anderen [!DNL Adobe] Produkte. Diese Integrationen können die Nützlichkeit von [!DNL Workfront] und passen Sie sie an die Bedürfnisse Ihrer Organisation an. Sie können eine oder alle dieser Integrationen verwenden, je nachdem, welche für eine bestimmte Aufgabe am nützlichsten ist.

## Integrierte Integrationen

Workfront bietet verschiedene Integrationen, die Sie direkt über Workfront oder eine andere Anwendung konfigurieren können, indem Sie das Workfront-Add-In für diese Anwendung installieren. Diese integrierten Integrationen decken viele gängige Anwendungsfallszenarien ab und konzentrieren sich auf die Erweiterung und Verbindung von Benutzererlebnissen für Endbenutzer.

Die integrierten Workfront-Integrationen konzentrieren sich im Wesentlichen auf die persönliche Produktivität und Zusammenarbeit. Diese Integrationen reduzieren die Unterbrechungen im Workflow eines Benutzers, sodass dieser Workfront-Benachrichtigungen erhält, auf Informationen zugreifen und mit Workfront-Arbeitselementen arbeiten kann, ohne die integrierte Anwendung verlassen zu müssen.

Die Vorteile integrierter Integrationen können Folgendes umfassen:

* Viele dieser integrierten Integrationen sind kostenfrei verfügbar. (Für andere ist ein zusätzlicher Kauf erforderlich.)
* Integrierte Integrationen decken viele der gängigsten Apps ab, die von Unternehmen verwendet werden, z. B. [!DNL Slack], [!DNL Google Drive]oder [!DNL Adobe] Produkte wie [!DNL Adobe Creative Cloud] oder [!DNL Adobe Experience Manager] Assets. Wenn Ihr Unternehmen diese Apps bereits verwendet, erfolgt die Integration reibungslos in den vorhandenen Workflow Ihrer Benutzer.
* Integration [!DNL Workfront] mit einer häufig verwendeten Anwendung kann die Akzeptanz bei Ihren Benutzern erhöhen.

>[!INFO]
>
>**Beispiel:**
>
>Mit dem [!DNL Workfront for Microsoft Teams integration], können Benachrichtigungen in [!DNL Microsoft Teams] über [!DNL Workfront] Arbeitselemente. Ohne Abfahren [!DNL Microsoft Teams], können Sie Aktionen ausführen, wie z. B. das Genehmigen, Kommentieren oder Ändern des Status von Arbeitselementen. Alle Änderungen, die Sie an Arbeitselementen aus [!DNL Microsoft Teams] werden in [!DNL Workfront] sowie

Weitere Informationen zu integrierten Integrationen, einschließlich einer Liste der derzeit verfügbaren integrierten Integrationen, finden Sie unter [[!DNL Adobe Workfront] Übersicht über integrierte Integrationen](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Benutzerdefinierte OAuth2-Anwendungen

Adobe [!DNL Workfront] Administratoren können OAuth2-Anwendungen für Ihre Instanz von erstellen. [!DNL Workfront], die anderen Anwendungen den Zugriff erlauben [!DNL Workfront]. Ihre Benutzer können dann anderen Anwendungen Berechtigungen erteilen, um auf ihre [!DNL Workfront] Daten. Auf diese Weise können Sie Workfront mit Anwendungen Ihrer Wahl integrieren, einschließlich Ihrer eigenen internen Anwendungen.

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich &quot;Erstellen einer App&quot;auf den Prozess der Erstellung einer solchen Zugriffsverknüpfung zwischen einer App und einem Server wie Workfront.

Vorteile der Erstellung eines [!UICONTROL OAuth2] kann Folgendes umfassen:

* Benutzer können diese Integrationen direkt in [!DNL Workfront], ähnlich wie bei integrierten Integrationen.
* Einrichten oder Verwenden einer [!UICONTROL OAuth2] erfordert keine zusätzlichen technischen Kenntnisse, z. B. die Kenntnis der [!DNL Workfront] API.
* Ihr Unternehmen kann Software verwenden, die nicht als [!DNL Workfront] integrierte Anwendung. Sie können diese Software dennoch mit [!DNL Workfront] durch Verwendung von [!UICONTROL OAuth2] -Anwendung, auch wenn die Software für Ihr Unternehmen geschützt ist.

Weitere Informationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] bietet eine öffentliche API (Anwendungsprogrammierschnittstelle), mit der Sie Ihr Workfront-Erlebnis erweitern und erweitern können. Das Ziel für [!DNL Workfront] Die API besteht darin, die Erstellung eigener Integrationen mit [!DNL Workfront] durch Einführung einer REST-fähigen Architektur, die über HTTP funktioniert. Die [!DNL Workfront] Die API benötigt einige technische Kenntnisse, ist aber ein sehr leistungsstarkes Tool zum Abrufen, Erstellen und Ändern von Daten. Sie können API-Aufrufe anpassen, um sehr spezifische Funktionen auszuführen.

Darüber hinaus [!DNL Workfront] bietet eine API zur Ereignisabonnement. Wenn eine Aktion auf einer [!DNL Workfront] -Objekt, das von Ereignisanmeldungen unterstützt wird, können Sie [!DNL Workfront] , um eine Antwort an Ihren gewünschten Endpunkt zu senden. Das bedeutet, dass Anwendungen von Drittanbietern Aktualisierungen von erhalten können [!DNL Workfront] Interaktionen über die [!DNL Workfront] API kurz nach ihrem Auftreten.

Vorteile der Verwendung der [!DNL Workfront] Die API kann Folgendes umfassen:

* Sie können die [!DNL Workfront] API zum Herstellen einer Verbindung zu fast jedem anderen Webdienst oder jeder Anwendung, der bzw. die eine öffentliche API anbietet. Es ist daher möglich, [!DNL Workfront] mit nahezu jedem Webdienst oder jeder Anwendung, den/die Sie verwenden möchten.
* Die [!DNL Workfront] Die Flexibilität der API erstreckt sich auch auf die proprietäre Software Ihres Unternehmens. Sie können [!DNL Workfront] Daten aus Ihrer eigenen Software.
* Da APIs so häufig von Software verwendet werden, sind Ihre internen Entwickler mit ihnen wahrscheinlich vertraut. [!DNL Workfront] verwendet eine REST-ful-API, den häufigsten API-Typ, wodurch es für Ihre Entwickler noch einfacher wird, schnell zu arbeiten.

>[!INFO]
>
>**Beispiel:**
>
>Der folgende API-Aufruf gibt einen Kommentar zum Aktualisierungsstream der Aufgabe mit der angegebenen ID ein.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Weitere Informationen zum [!DNL Workfront] API, siehe [API-Grundlagen](../wf-api/general/api-basics.md).

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignisabonnement-API](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] ermöglicht die Automatisierung von Workflows. Mit dem [!DNL Workfront Fusion for Work Automation and Integration] -Lizenz können Sie diese Automatisierungen für mehrere Apps und Webdienste erstellen und Szenarien erstellen, in denen die Apps zusammenarbeiten, um eine Aufgabe auszuführen. Ein Szenario ist eine visuelle Darstellung der Aufgabe oder des Workflows, die mit Modulen erstellt wird, die diskrete Aufgaben wie &quot;Dokument herunterladen&quot;oder &quot;Projekt erstellen&quot;sind. Sie ketten die Module zusammen, um den Workflow zu definieren. Der Workflow wird dann automatisch ausgeführt, wenn eine Trigger-Bedingung erfüllt ist.

Vorteile [!DNL Workfront Fusion] kann Folgendes umfassen:

* [!DNL Workfront Fusion] erfordert nicht so viel technisches Wissen wie die API, da die visuelle Benutzeroberfläche beim Verständnis und Einrichten des Workflows hilft. Dies bedeutet, dass sie von Einzelanwendern außerhalb eines Entwicklungsteams verwendet werden kann, was Ihrer Organisation Zeit und Geld sparen kann.
* Seit [!DNL Workfront Fusion] funktioniert über die API und kann auf die meisten Apps und Webdienste zugreifen. Viele Apps verfügen über Module zum Ausführen von API-Aufrufen oder Sie können die HTTP-, SOAP- oder JSON-Module verwenden, um mit Webdiensten zu interagieren, für die keine dedizierten [!DNL Workfront Fusion] Connector.

>[!INFO]
>
>**Beispiel:**
>
>Folgendes [!DNL Workfront] -Modul in [!DNL Workfront Fusion] ist so eingerichtet, dass dem ausgewählten Projekt ein Kommentar hinzugefügt wird. Nachdem das Modul ausgeführt wurde, ist der Kommentar im Aktualisierungsstream des Projekts in Workfront sichtbar.
>
>![](assets/fusion-example-comment-350x416.png)

Weitere Informationen finden Sie unter [!DNL Workfront Fusion], siehe [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
