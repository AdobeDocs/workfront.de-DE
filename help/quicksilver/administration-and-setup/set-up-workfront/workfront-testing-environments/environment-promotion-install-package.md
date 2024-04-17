---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installieren eines Umgebungsförderungspakets
description: Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein Umgebungsförderungspaket in einer Zielumgebung installieren.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# Installieren eines Umgebungsförderungspakets

>[!NOTE]
>
>Um ein Paket zu installieren, müssen Sie in der Umgebung angemeldet sein, in der Sie das Paket installieren möchten. Dies ist die Umgebung, in die Sie Objekte kopieren **nach**.

1. Gehen Sie zur Umgebung, in der Sie das Paket installieren möchten.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System** Wählen Sie im linken Navigationsbereich die Option **Umgebungsförderung**.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. Wählen Sie für jedes Objekt mit einer Kollision aus, wie die Kollision gelöst werden soll.

   Klicken Sie zum Beheben einer Kollision auf den Dropdown-Pfeil neben dem Objekttyp und wählen Sie die gewünschte Aktion aus.

   Weitere Informationen finden Sie unter [Kollisionen](#collisions) in diesem Artikel
1. Um das Paket in der neuen Umgebung bereitzustellen, klicken Sie auf **Bereitstellen** oben rechts auf dem Bildschirm.

## Kollisionen

Kollisionen treten auf, wenn ein Objekt, das Teil des Installationspakets ist, bereits in der Zielumgebung vorhanden ist. In diesem Fall können Sie auswählen, wie die Kollision gelöst werden soll. Kollisionen werden auf Objektebene aufgelöst.

Sie können Kollisionen anzeigen, indem Sie auf das Dropdown-Menü neben jedem Objekttyp klicken. Kollisionen werden in der Spalte Kollision angezeigt.

Um eine Kollision zu beheben, wählen Sie eine Aktion in der Spalte Aktion für Freigabe aus oder verwenden Sie die bereits angezeigte Standardaktion.

* **Erstellen mit neuem Namen**: Erstellen Sie ein neues Objekt in der Zielumgebung. Wenn das Objekt in der Zielumgebung vorhanden ist, können Sie ein neues Objekt mit einem neuen Namen erstellen. Wenn es nicht in der Zielumgebung vorhanden ist, können Sie das Objekt mit einem neuen Namen oder mit dem Namen erstellen, den das Objekt im Paket hat.
* **Vorhandene verwenden**: Das Objekt im Paket wird nicht installiert und das Objekt, das bereits in der Zielumgebung vorhanden war, bleibt unverändert.
* **Überschreiben**: Das Objekt im Paket ersetzt das vorhandene Objekt in der Zielumgebung.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Die Standardwerte sind `Create new` , wenn das Objekt nicht in der Zielumgebung vorhanden ist, und `Use existing` , wenn das Objekt in der Zielumgebung vorhanden ist. Sie können zur Standardzuordnung zurückkehren, indem Sie auf **Auf Standardzuordnung zurücksetzen**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
