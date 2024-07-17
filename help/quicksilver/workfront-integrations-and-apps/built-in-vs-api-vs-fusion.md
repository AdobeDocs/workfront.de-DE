---
content-type: reference
product-area: workfront-integrations
keywords: native,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Integrationsmethoden von Adobe Workfront
description: Sie können [!DNL Adobe Workfront] in Anwendungen von Drittanbietern integrieren. Diese Integrationen können das Dienstprogramm von [!DNL Workfront] erweitern und an die Anforderungen Ihres Unternehmens anpassen. Sie können eine oder alle dieser Integrationen verwenden, je nachdem, welche für eine bestimmte Aufgabe am nützlichsten ist.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Integrationsmethoden von Adobe Workfront

Sie können [!DNL Adobe Workfront] in Drittanbieteranwendungen sowie andere [!DNL Adobe] -Produkte integrieren. Diese Integrationen können das Dienstprogramm [!DNL Workfront] erweitern und an die Anforderungen Ihres Unternehmens anpassen. Sie können eine oder alle dieser Integrationen verwenden, je nachdem, welche für eine bestimmte Aufgabe am nützlichsten ist.

## Integrierte Integrationen

Workfront bietet verschiedene Integrationen, die Sie direkt über Workfront oder eine andere Anwendung konfigurieren können, indem Sie das Workfront-Add-In für diese Anwendung installieren. Diese integrierten Integrationen decken viele gängige Anwendungsfallszenarien ab und konzentrieren sich auf die Erweiterung und Verbindung von Benutzererlebnissen für Endbenutzer.

Die integrierten Workfront-Integrationen konzentrieren sich im Wesentlichen auf die persönliche Produktivität und Zusammenarbeit. Diese Integrationen reduzieren die Unterbrechungen im Workflow eines Benutzers, sodass dieser Workfront-Benachrichtigungen erhält, auf Informationen zugreifen und mit Workfront-Arbeitselementen arbeiten kann, ohne die integrierte Anwendung verlassen zu müssen.

Die Vorteile integrierter Integrationen können unter anderem folgende sein:

* Viele dieser integrierten Integrationen sind kostenfrei verfügbar. (Andere benötigen einen zusätzlichen Kauf.)
* Integrierte Integrationen decken viele der gängigsten Apps ab, die von Unternehmen verwendet werden, z. B. [!DNL Slack], [!DNL Google Drive] oder [!DNL Adobe] Produkte wie die Assets [!DNL Adobe Creative Cloud] oder [!DNL Adobe Experience Manager]. Wenn Ihr Unternehmen diese Apps bereits verwendet, erfolgt die Integration reibungslos in den vorhandenen Workflow Ihrer Benutzer.
* Die Integration von [!DNL Workfront] in eine häufig verwendete Anwendung kann die Akzeptanz bei Ihren Benutzern erhöhen.

>[!INFO]
>
>**Beispiel:**
>
>Mit dem [!DNL Workfront for Microsoft Teams integration] können Sie Benachrichtigungen in [!DNL Microsoft Teams] über Ihre [!DNL Workfront] Arbeitselemente erhalten. Ohne &quot;[!DNL Microsoft Teams]&quot;zu verlassen, können Sie Aktionen wie das Genehmigen, Kommentieren oder Ändern des Status von Arbeitselementen durchführen. Alle Änderungen, die Sie an Arbeitselementen von [!DNL Microsoft Teams] vornehmen, werden ebenfalls in [!DNL Workfront] übernommen.

Weitere Informationen zu integrierten Integrationen, einschließlich einer Liste der derzeit verfügbaren integrierten Integrationen, finden Sie unter [[!DNL Adobe Workfront] Übersicht über integrierte Integrationen](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Benutzerdefinierte OAuth2-Anwendungen

Adobe [!DNL Workfront] -Administratoren können OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront] erstellen, die anderen Anwendungen den Zugriff auf [!DNL Workfront] ermöglichen. Ihre Benutzer können dann diesen anderen Anwendungen Berechtigungen für den Zugriff auf ihre [!DNL Workfront] -Daten erteilen. Auf diese Weise können Sie Workfront mit Anwendungen Ihrer Wahl integrieren, einschließlich Ihrer eigenen internen Anwendungen.

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich &quot;Erstellen einer App&quot;auf den Prozess der Erstellung einer solchen Zugriffsverknüpfung zwischen einer App und einem Server wie Workfront.

Die Vorteile der Erstellung einer [!UICONTROL OAuth2] -Anwendung können Folgendes umfassen:

* Benutzer können diese Integrationen ähnlich wie integrierte Integrationen direkt in [!DNL Workfront] verwenden.
* Für das Einrichten oder Verwenden einer [!UICONTROL OAuth2] -Anwendung sind keine zusätzlichen technischen Kenntnisse erforderlich, z. B. die Kenntnis der [!DNL Workfront] -API.
* Ihr Unternehmen kann Software verwenden, die nicht als integrierte [!DNL Workfront] -Anwendung angeboten wird. Sie können diese Software weiterhin mit [!DNL Workfront] integrieren, indem Sie eine [!UICONTROL OAuth2] -Anwendung verwenden, selbst wenn die Software für Ihr Unternehmen geschützt ist.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] bietet eine öffentliche API (Anwendungsprogrammierschnittstelle), mit der Sie Ihr Workfront-Erlebnis erweitern und erweitern können. Ziel der [!DNL Workfront]-API ist es, die Erstellung eigener Integrationen mit [!DNL Workfront] zu vereinfachen, indem eine REST-basierte Architektur eingeführt wird, die über HTTP ausgeführt wird. Die [!DNL Workfront]-API benötigt einige technische Kenntnisse, ist aber ein sehr leistungsstarkes Tool zum Abrufen, Erstellen und Ändern von Daten. Sie können API-Aufrufe anpassen, um sehr spezifische Funktionen auszuführen.

Zusätzlich bietet [!DNL Workfront] eine API zur Ereignisanmeldung. Wenn eine Aktion für ein [!DNL Workfront] -Objekt erfolgt, das von Ereignisabonnements unterstützt wird, können Sie [!DNL Workfront] so konfigurieren, dass eine Antwort an den gewünschten Endpunkt gesendet wird. Das bedeutet, dass Anwendungen von Drittanbietern Aktualisierungen von [!DNL Workfront] -Interaktionen über die [!DNL Workfront] -API erhalten können, kurz nachdem sie aufgetreten sind.

Die Verwendung der [!DNL Workfront] -API bietet unter anderem folgende Vorteile:

* Sie können die [!DNL Workfront] -API verwenden, um eine Verbindung zu fast jedem anderen Webdienst oder jeder App herzustellen, der bzw. die eine öffentliche API anbietet. Daher ist es möglich, [!DNL Workfront] in nahezu jeden Webdienst oder jede Anwendung zu integrieren, den/die Sie verwenden möchten.
* Die Flexibilität der [!DNL Workfront]-API erstreckt sich auch auf die proprietäre Software Ihres Unternehmens. Sie können [!DNL Workfront] -Daten aus Ihrer eigenen Software verwenden und ändern.
* Da APIs so häufig von Software verwendet werden, sind Ihre internen Entwickler mit ihnen wahrscheinlich vertraut. [!DNL Workfront] verwendet eine REST-ful-API, den häufigsten API-Typ, wodurch es für Ihre Entwickler sogar noch einfacher wird, schnell auf den neuesten Stand zu kommen.

>[!INFO]
>
>**Beispiel:**
>
>Der folgende API-Aufruf gibt einen Kommentar zum Aktualisierungsstream der Aufgabe mit der angegebenen ID ein.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Weitere Informationen zur [!DNL Workfront]-API finden Sie unter [API-Grundlagen](../wf-api/general/api-basics.md).

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Ereignisabonnement-API](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

Mit [!DNL Workfront Fusion] können Sie Workflows automatisieren. Mit der [!DNL Workfront Fusion for Work Automation and Integration] -Lizenz können Sie diese Automatisierungen für mehrere Apps und Webdienste erstellen und Szenarien erstellen, in denen die Apps zusammenarbeiten, um eine Aufgabe auszuführen. Ein Szenario ist eine visuelle Darstellung der Aufgabe oder des Workflows, die mit Modulen erstellt wird, die diskrete Aufgaben wie &quot;Dokument herunterladen&quot;oder &quot;Projekt erstellen&quot;sind. Sie ketten die Module zusammen, um den Workflow zu definieren. Der Workflow wird dann automatisch ausgeführt, wenn eine Trigger-Bedingung erfüllt ist.

Vorteile von [!DNL Workfront Fusion] können Folgendes umfassen:

* [!DNL Workfront Fusion] benötigt nicht so viel technisches Wissen wie die API, da die visuelle Oberfläche beim Verständnis und Einrichten des Workflows hilft. Dies bedeutet, dass sie von Einzelanwendern außerhalb eines Entwicklungsteams verwendet werden kann, was Ihrer Organisation Zeit und Geld sparen kann.
* Da [!DNL Workfront Fusion] über die API funktioniert, kann es auf die meisten Apps und Webdienste zugreifen. Viele Apps verfügen über Module zum Ausführen von API-Aufrufen. Alternativ können Sie die HTTP-, SOAP- oder JSON-Module verwenden, um mit Webdiensten zu interagieren, die keinen dedizierten [!DNL Workfront Fusion]-Connector haben.

>[!INFO]
>
>**Beispiel:**
>
>Das folgende [!DNL Workfront]-Modul in [!DNL Workfront Fusion] ist so eingerichtet, dass dem ausgewählten Projekt ein Kommentar hinzugefügt wird. Nachdem das Modul ausgeführt wurde, ist der Kommentar im Aktualisierungsstream des Projekts in Workfront sichtbar.
>
>![](assets/fusion-example-comment-350x416.png)

Weitere Informationen zu [!DNL Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
