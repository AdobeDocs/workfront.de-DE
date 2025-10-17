---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprints - Übersicht
description: Blueprints sind eine Reihe von Workfront-Objekten, die gängige Anwendungsfälle in Workfront abdecken. Sie können eine Blueprint herunterladen und installieren und dann die Objekte für Ihren spezifischen Anwendungsfall konfigurieren.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Blueprints - Übersicht

<!--Audited: 01/2024-->

Blueprints sind eine Reihe von Workfront-Objekten, die gängige Anwendungsfälle in Workfront abdecken. Sie können eine Blueprint herunterladen und installieren und dann die Objekte für Ihren spezifischen Anwendungsfall konfigurieren.

![Blueprints-Hauptseite](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>Beispiele:
>
>* **Einrichtung der Personalorganisation**
>
>   Dieser Blueprint enthält die Konfiguration von Organisationsstrukturen, um eine Personalabteilung zu bilden.
>
>* **Neue Mitarbeiter-IT-Checkliste hinzufügen**
>
>   Dieser Blueprint enthält eine Vorlage zum Organisieren von Onboarding-Aktivitäten für neue Mitarbeiter. Die Verwendung dieser Vorlage ermöglicht es IT-Teams, effizient zu arbeiten, was zu einer positiven neuen Mitarbeitererfahrung und einem schnelleren Weg zur Produktivität führt.
>
>* **Vererbte Instanzgrundlagen | Checkliste**
>
>    Dieser Blueprint enthält eine Projektvorlage (oder Checkliste), die Sie mit einer kurzen Liste mit Fragen, Ressourcen und Links überprüfen können, um einen Überblick über die Konfiguration Ihrer Workfront-Instanz zu erhalten. Verwenden Sie dies, wenn Sie kürzlich eine Workfront-Instanz geerbt haben und Anleitungen zum Starten benötigen.
>
>Informationen zur Überprüfung der aktuellen Blueprints finden Sie unter [Liste der verfügbaren Blueprints](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).


Blueprints bieten grundlegende Bausteine, mit denen Sie ein mit Ihnen wachsendes Arbeitsverwaltungssystem erstellen können. Systemadministratoren können den Blueprint-Katalog durchsuchen und einsatzbereite Projektvorlagen, Dashboards und Organisationsstrukturen installieren. Andere Benutzer können den Katalog durchsuchen und die Installation einer Blueprint anfordern. Weitere Informationen finden Sie unter [Durchsuchen des Blueprint-Katalogs und Anfordern der Installation von Blueprints](../../administration-and-setup/blueprints/browse-catalog.md).

Jeder Blueprint ist auf eine Abteilung und eine bestimmte Reifegrad-Ebene ausgerichtet, damit Sie bewährte Best Practices schneller in Ihr System implementieren können. Die unten beschriebenen Reifegrade sind in der Blueprint-Katalogkarte und den Details angegeben.

* **[!UICONTROL Managed]:** Vorlagen für verwaltete Projekte unterstützen die Einführung eines neuen Geschäftsprozesses, bevor Aktivitäten und Ergebnisse vollständig als Standardvorgang akzeptiert werden. Sie enthalten Aufgaben, mit denen sichergestellt werden kann, dass jeder Schritt des neuen Prozesses eingehalten wird.

* **[!UICONTROL Integriert]:** Integrierte Projektvorlagen gehen davon aus, dass Geschäftsfunktionen durch ein Standardverfahren unterstützt werden. Mitwirkende am Prozess kennen die Schritte und Aufgaben, die sie ausführen müssen, um den Prozess durchzuführen. Die Projektvorlagen zur Unterstützung dieses Prozesses enthalten weniger Aufgaben, um nur Meilensteine und andere wichtige Ergebnisse zu verfolgen, die für Berichtszwecke erforderlich sind.

## Finden der richtigen Blueprint

Mit den Filtern auf der rechten Seite des Katalogs können Sie Blueprints nach Anwendungsfall, Reifegrad, Installationsstatus und Typ durchsuchen. Sobald Sie eine Blueprint gefunden haben, die Sie interessiert, können Sie Details auf der Detailseite anzeigen.

### Blueprint-Typen

Der Blueprint-Typ zeigt an, was in der Blueprint enthalten ist. Der Typ wird unten auf der Blueprint-Karte im Katalog aufgeführt. Beachten Sie, dass eine Blueprint mehr als einen Typ haben kann.

Die folgenden Blueprint-Typen sind verfügbar:

* **Projektvorlagen**: Enthält Standardobjekte, die mit einer Projektvorlage verknüpft sind (Aufgaben, Probleme, Rollen und Teams), sowie einige Voreinstellungen in Bezug auf diese Objekte. Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).
* **Organisationsstrukturen**: Enthält Objekte, die mit der Struktur einer Organisation verknüpft sind (Unternehmen, Gruppen, Rollen und Teams). Weitere Informationen finden Sie unter [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).
* **Dashboards**: Enthält ein oder mehrere Dashboards für einen bestimmten Anwendungsfall, z. B. Implementierungs-Services.
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

Informationen zur Überprüfung der aktuellen Blueprints finden Sie unter [Liste der verfügbaren Blueprints](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### Details anzeigen

Jeder Blueprint enthält eine Detailseite. Auf dieser Seite haben Sie folgende Möglichkeiten:

* Anzeigen einer Zusammenfassung des Workflow-Inhalts
* Eine kurze Zusammenfassung des Blueprints lesen
* Anzeigen des Installationsverlaufs (klicken Sie auf **[!UICONTROL Details anzeigen]**, um die vollständige Liste der mit der Blueprint installierten Objekte anzuzeigen)
* Siehe Beschreibungen zu Rollen, Teams, Unternehmen und Gruppen
* Sehen Sie sich ein visuelles Beispiel des spezifischen Blueprints an, z. B. eine Projektvorlage (Sie können das vollständige Bild im Browser in der Vorschau anzeigen oder herunterladen)

![[!UICONTROL Blueprint-Details] Seite](assets/blueprint-details-page-2022.png)

## Blueprint installieren

Ein Workfront-Administrator kann Blueprints direkt in beliebigen Umgebungen (Produktions-, Vorschau- oder Sandbox-Umgebungen) installieren. Weitere Informationen finden Sie unter [Blueprint installieren](../../administration-and-setup/blueprints/blueprints-install.md) oder [Blueprint konfigurieren](../../administration-and-setup/blueprints/configure-template-package.md).

Nach der Installation sind Sie sich möglicherweise nicht sicher, welche Aktionen Sie als Nächstes durchführen sollten. Weitere Informationen finden Sie [Aktionen, die nach der Installation eines Blueprints durchgeführt werden sollen](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## Zusätzliche Hinweise zu Blueprints und Vorlagen

Blueprints ersetzen nicht die Funktionalität der Projektvorlagen in [!DNL Adobe Workfront]. Mit Blueprints können Sie neue Vorlagen schneller erstellen, um einen größeren Teil Ihrer Arbeit in [!DNL Workfront] zu organisieren.

Blueprints können nicht kopiert oder bearbeitet werden. Nachdem Sie die Projektmappe jedoch über einen Blueprint installiert haben, können Sie die aus dem Blueprint erstellte Projektvorlage, Aufgabengebiete oder Teams auf die gleiche Weise ändern, wie Sie diese Datensätze normalerweise in der [!DNL Workfront] aktualisieren. Wenn Sie eine Blueprint installieren, wird die Vorlage im Bereich [!UICONTROL Vorlagen] von [!DNL Workfront] gespeichert und die ursprüngliche Blueprint verbleibt im Bereich [!UICONTROL Blueprints]. Sie müssen keine Kopie der Vorlage erstellen, bevor Sie sie an Ihre Anforderungen anpassen.

Blueprints entfernen oder ersetzen keine in Ihrer Umgebung konfigurierten Elemente. Wenn Sie eine vorhandene Vorlage ersetzen möchten, indem Sie einen Blueprint installieren, der eine neue Vorlage erstellt, empfehlen wir, die vorherige Version zu deaktivieren, um Verwirrung unter Ihren Planern zu vermeiden, die Projekte aus Vorlagen erstellen.
