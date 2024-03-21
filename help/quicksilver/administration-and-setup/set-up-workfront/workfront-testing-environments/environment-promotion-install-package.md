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
source-git-commit: 610469811a937fde70a938af829b156e69cca391
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# Installieren eines Umgebungsförderungspakets


1. Gehen Sie zur Umgebung, in der Sie das Paket installieren möchten. Dies ist die Umgebung, in die Sie Objekte kopieren **nach**.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System** Wählen Sie im linken Navigationsbereich die Option **Umgebungsförderung**.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. Um das Paket zu installieren, klicken Sie auf **Installieren** oben rechts auf dem Bildschirm.
1. Ordnen Sie jedes Objekt im Paket dem entsprechenden Objekt in der Zielumgebung zu.

   Weitere Informationen finden Sie unter [Zuordnung](#mapping) in diesem Artikel


## Zuordnung

Jeder Objekttyp wird im linken Navigationsbereich und auf einer Karte angezeigt. Die Karte zeigt Objekte dieses Typs an und ob diese Objekte in der Zielumgebung vorhanden sind. Sie können bestimmen, wie diese Objekte in die Zielumgebung verschoben werden.

* Neu erstellen: Erstellen Sie ein neues Objekt in der Zielumgebung. Wenn das Objekt in der Zielumgebung vorhanden ist, können Sie ein neues Objekt mit einem neuen Namen erstellen. Wenn es nicht in der Zielumgebung vorhanden ist, können Sie das Objekt mit einem neuen Namen oder mit dem Namen erstellen, den das Objekt im Paket hat.
* Vorhandenes verwenden: Das Objekt im Paket wird nicht installiert und das bereits in der Zielumgebung vorhandene Objekt bleibt unverändert.
* Vorhandene überschreiben: (Derzeit nicht verfügbar) Das Objekt im Paket ersetzt das vorhandene Objekt in der Zielumgebung.
* Nicht verwenden: Das Objekt im Paket wird nicht in der Zielumgebung installiert. Wenn Sie Nicht verwenden auswählen, wird eine Fehlermeldung angezeigt, in der beschrieben wird, wie sich diese Auswahl auf andere Objekte oder Felder auswirkt.

Die Standardwerte sind `Create new` , wenn das Objekt nicht in der Zielumgebung vorhanden ist, und `Use existing` , wenn das Objekt in der Zielumgebung vorhanden ist. Sie können zur Standardzuordnung zurückkehren, indem Sie auf **Auf Standardzuordnung zurücksetzen**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
