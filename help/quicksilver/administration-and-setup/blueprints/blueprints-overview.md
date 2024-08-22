---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprints-Übersicht
description: Blueprints sind Sets von Workfront-Objekten, die häufige Anwendungsfälle in Workfront behandeln. Sie können einen Blueprint herunterladen und installieren und dann die Objekte für Ihren spezifischen Anwendungsfall konfigurieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Blueprints - Übersicht

<!--Audited: 01/2024-->

Blueprints sind Sets von Workfront-Objekten, die häufige Anwendungsfälle in Workfront behandeln. Sie können einen Blueprint herunterladen und installieren und dann die Objekte für Ihren spezifischen Anwendungsfall konfigurieren.

![](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Beispiele:
>
>* **Einrichtung der Personalorganisation**
>
>   Dieser Entwurf enthält die Konfiguration von Organisationsstrukturen, die auf eine Personalabteilung erweitert werden sollen.
>
>* **Neue IT-Checkliste für Mitarbeiter hinzufügen**
>
>   Dieser Blueprint enthält eine Vorlage zur Organisation neuer Onboarding-Aktivitäten für Mitarbeiter. Durch die Verwendung dieser Vorlage können IT-Teams effizient arbeiten, was zu einer positiven neuen Mitarbeitererfahrung und einer schnelleren Verfolgung der Produktivität führt.
>
>* **Vererbte Instanzgrundlagen | Checkliste**
>
>    Dieser Blueprint enthält eine Projektvorlage (oder Checkliste), die Sie mit einer kurzen Liste von Fragen, Ressourcen und Links überprüfen können, um ein klares Verständnis der Konfiguration Ihrer Workfront-Instanz zu erhalten. Verwenden Sie dies, wenn Sie kürzlich eine Workfront-Instanz geerbt haben und eine Anleitung zum Starten benötigen.
>
>Informationen zum Überprüfen der aktuellen Blueprints finden Sie unter [Liste der verfügbaren Blueprints](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


Blueprints stellen grundlegende Bausteine bereit, mit denen Sie ein Arbeitsverwaltungssystem erstellen können, das mit Ihnen wächst. Systemadministratoren können den Blueprints-Katalog durchsuchen und gebrauchsfertige Projektvorlagen, Dashboards und Organisationsstrukturen installieren. Andere Benutzer können den Katalog durchsuchen und die Installation eines Blueprints anfordern. Weitere Informationen finden Sie unter [Katalog mit Blueprints durchsuchen und Installation von Blueprints anfordern](../../administration-and-setup/blueprints/browse-catalog.md).

Jeder Blueprint richtet sich an eine Abteilung und ein spezifisches Laufzeitniveau, damit Sie bewährte Best Practices schneller in Ihr System implementieren können. Die im Folgenden beschriebenen Laufzeitstufen sind in der Blueprint-Katalogkarte und den Details angegeben.

* **[!UICONTROL Managed]:** Verwaltete Projektvorlagen unterstützen die Übernahme eines neuen Geschäftsprozesses, bevor Aktivitäten und Ergebnisse vollständig als Standardverfahren akzeptiert werden. Sie enthalten Aufgaben, die sicherstellen, dass jeder Schritt des neuen Prozesses befolgt wird.

* **[!UICONTROL Integrierte Projektvorlagen]:** Bei integrierten Projektvorlagen wird davon ausgegangen, dass Geschäftsfunktionen durch ein standardmäßiges Betriebsverfahren unterstützt werden. Mitwirkende kennen die Schritte und Aufgaben, die sie ausführen müssen, um den Prozess zu verfolgen. Die Projektvorlagen zur Unterstützung dieses Prozesses enthalten weniger Aufgaben, um nur Meilensteine und andere wichtige Ergebnisse zu verfolgen, die für Berichterstellungszwecke erforderlich sind.

## Den richtigen Blueprint finden

Sie können Blueprints nach Anwendungsfall, Reifegrad, Installationsstatus und Typ mit den Filtern auf der rechten Seite des Katalogs durchsuchen. Sobald Sie einen für Sie interessanten Blueprint gefunden haben, können Sie Details auf der Detailseite anzeigen.

### Blueprint-Typen

Der Blueprint-Typ zeigt, was im Blueprint enthalten ist. Der Typ wird unten auf der Blueprint-Karte im Katalog aufgeführt. Beachten Sie, dass ein Blueprint mehr als einen Typ haben kann.

Die folgenden Blueprint-Typen sind verfügbar:

* **Projektvorlagen**: Umfasst Standardobjekte, die mit einer Projektvorlage verknüpft sind (Aufgaben, Probleme, Rollen und Teams), sowie einige Voreinstellungen für diese Objekte. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).
* **Organisationsstrukturen**: Umfasst Objekte, die mit der Struktur einer Organisation verknüpft sind (Unternehmen, Gruppen, Rollen und Teams). Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).
* **Dashboards**: Umfasst ein oder mehrere Dashboards für einen bestimmten Anwendungsfall, z. B. Implementierungsdienste.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Informationen zum Überprüfen der aktuellen Blueprints finden Sie unter [Liste der verfügbaren Blueprints](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Details anzeigen

Jeder Blueprint enthält eine Detailseite. Auf dieser Seite haben Sie folgende Möglichkeiten:

* Zusammenfassung des Workflow-Inhalts anzeigen
* Eine kurze Zusammenfassung des Blueprints lesen
* Installationsverlauf anzeigen (klicken Sie auf **[!UICONTROL Siehe Details]** , um die vollständige Liste der mit dem Blueprint installierten Objekte anzuzeigen)
* Anzeigen von Rollen, Teams, Unternehmen und Gruppen
* Sehen Sie sich ein visuelles Beispiel für den jeweiligen Blueprint an, z. B. eine Projektvorlage (Sie können das vollständige Bild im Browser anzeigen oder herunterladen).

![[!UICONTROL Blueprint-Details] Seite](assets/blueprint-details-page-2022.png)

## Blueprint installieren

Ein Workfront-Administrator kann einen Blueprint direkt in allen Umgebungen (Produktions-, Vorschau- oder Sandbox-Umgebungen) installieren. Weitere Informationen finden Sie unter [Installieren eines Blueprints](../../administration-and-setup/blueprints/blueprints-install.md) oder [Konfigurieren eines Blueprints](../../administration-and-setup/blueprints/configure-template-package.md).

Nach der Installation sind Sie möglicherweise nicht sicher, welche Maßnahmen die nächsten Schritte am besten sind. Weitere Informationen finden Sie unter [Aktionen, die nach der Installation eines Blueprints ausgeführt werden sollen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Zusätzliche Hinweise zu Blueprints und Vorlagen

Blueprints ersetzen nicht die Funktionalität der Projektvorlagen in [!DNL Adobe Workfront]. Mit Blueprints können Sie neue Vorlagen schneller erstellen, um mehr Ihrer Arbeit in [!DNL Workfront] zu organisieren.

Ein Blueprint kann nicht kopiert oder bearbeitet werden. Nachdem Sie die Lösung jedoch über einen Blueprint installiert haben, können Sie die Projektvorlage, die Auftragsrollen oder die aus dem Blueprint erstellten Teams auf die gleiche Weise ändern, wie Sie diese Datensätze normalerweise in der Oberfläche von [!DNL Workfront] aktualisieren. Wenn Sie einen Blueprint installieren, wird die Vorlage im Bereich [!UICONTROL Vorlagen] von [!DNL Workfront] gespeichert und der ursprüngliche Blueprint bleibt im Bereich [!UICONTROL Blueprints]. Sie müssen keine Kopie der Vorlage erstellen, bevor Sie mit der Anpassung an Ihre Anforderungen beginnen.

Blueprints entfernen oder ersetzen keine in Ihrer Umgebung konfigurierten Elemente. Wenn Sie eine vorhandene Vorlage ersetzen möchten, indem Sie einen Blueprint installieren, der eine neue Vorlage erstellt, empfehlen wir, die vorherige Version zu deaktivieren, um Verwirrung bei Ihren Planern zu vermeiden, die Projekte aus Vorlagen erstellen.
