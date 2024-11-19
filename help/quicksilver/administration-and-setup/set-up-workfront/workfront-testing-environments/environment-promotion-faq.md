---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Häufig gestellte Fragen zur Umgebungsförderung
description: Erfahren Sie mehr über die häufig gestellten Fragen zur Workfront-Umgebungsförderung.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e9794262-80cc-4641-a5c6-7130cf008ba2
source-git-commit: 4ea4d7d8fd16d4c4d7c2fe5f7adb15c2b44b6705
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 3%

---

# Häufig gestellte Fragen zur Umgebungsförderung

Häufig werden die folgenden Fragen zur Umgebungsförderung gestellt:

## Wird domänenübergreifende Promotion unterstützt?

### Antwort

Die domänenübergreifende Förderung von Umgebungen wird derzeit nicht unterstützt. Sie müssen zwischen Umgebungen in derselben Domäne weiterleiten.

## Ist die Adobe Business Platform/IMS eine Voraussetzung für die Förderung der Umwelt?

### Antwort

Nein. Die Umgebungsförderung ist sowohl für IMS-fähige als auch für Nicht-IMS-Workfront-Instanzen verfügbar.

## Wie können wir feststellen, ob unsere Workfront-Instanz über eine Prime- oder Ultimate-Lizenz verfügt?

### Antwort

* Ein Workfront-Administrator kann die Lizenz Ihres Unternehmens ermitteln.

   1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** (6}Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf das Symbol **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).![
   1. Klicken Sie im linken Bereich auf **System** .
   1. Um Ihren Workfront-Plan anzuzeigen, wählen Sie **Lizenzen** aus.
Ihr Plan wird in der Nähe der oberen rechten Ecke der Seite angezeigt.
      ![](assets/locate-plan.png)

  Oder
* Wenden Sie sich an Ihren Workfront-Kundenbetreuer.

## Ist die Umweltförderung bidirektional?

### Antwort

Ja. Sie können beispielsweise von Sandbox zur Produktion oder von Produktion zur Sandbox weiterleiten.

## Wird Freigabe unterstützt?

### Antwort

Nein, die Freigabe wird derzeit nicht unterstützt.

## Ist das Paket-Rollback verfügbar?

### Antwort

Das Paket-Rollback ist für das neueste Paket innerhalb von 24 Stunden nach der Paketinstallation verfügbar.

## Gibt es eine Option, die Promotion einzelner Komponenten zu überspringen? Wo die Optionen `Use Existing`, `Overwrite` und `Save with a new Name` vorhanden sind, kann `Skip` hinzugefügt werden, damit Sie die Promotion einzelner Parameter überspringen können?

### Antwort


* &quot;Vorhandene verwenden&quot;entspricht &quot;Überspringen&quot;oder Ignorieren der Bereitstellung, da sie dem vorhandenen Objekt in der Zielumgebung zugeordnet ist und keine Änderungen vornimmt.
* Um Objekte zu überspringen, wird empfohlen,
Alle Objekte, die Sie nicht über das Promotion-Paket oder direkt aus der Quellumgebung installieren möchten. Nachdem Sie die Objekte entfernt haben, assemblieren Sie das Paket neu.
