---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets
description: Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein Umgebungsförderungspaket erstellen, das Sie dann in einer anderen Umgebung installieren können.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: e03573640fd8af9c811cef4cf176cc4f37d757fc
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets

Sie müssen ein Paket in der Umgebung erstellen, in das Sie Objekte kopieren möchten **von**. Wenn Sie beispielsweise ein Projekt in Ihrer Sandbox für benutzerdefinierte Aktualisierung konfigurieren und es in Ihrer Produktionsumgebung bewerben, müssen Sie das Paket in Ihrer Sandbox für benutzerdefinierte Aktualisierung erstellen.

>[!IMPORTANT]
>
>Wenn Ihre Sandbox für benutzerdefinierte Aktualisierung aktualisiert wird, während Sie das Objekt für die Umgebungsförderung konfigurieren, geht diese Konfiguration bei der Aktualisierung verloren. Es wird empfohlen, die benutzerdefinierte Aktualisierungs-Sandbox nur dann zu aktualisieren, wenn alle ausstehenden Umgebungsförderungsobjekte und -pakete erfolgreich beworben wurden.

## Package erstellen

1. Wechseln Sie zu der Umgebung, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, in die Sie Objekte kopieren **von**.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System** Wählen Sie im linken Navigationsbereich die Option **Umgebungsförderung**.
1. Klicks **Paket erstellen**.

   Die Seite Neues Promotion-Paket wird geöffnet.

1. Im **Paketname** ein, geben Sie einen Namen für das Paket ein.
1. Im **Beschreibung** Geben Sie eine Beschreibung für dieses Paket ein.
1. Um dem Paket ein Objekt hinzuzufügen, klicken Sie auf **Objekte hinzufügen** Wählen Sie im linken Navigationsbereich den Objekttyp aus, den Sie hinzufügen möchten.
1. Wählen Sie ein oder mehrere Objekte aus der Liste aus oder geben Sie den Namen in die Suchleiste ein und wählen Sie das Objekt aus, wenn es in der Liste angezeigt wird. Sie können mehrere Objekte in der Liste auswählen.
1. Klicks **Hinzufügen (X Objekte)** , um die ausgewählten Objekte zum Paket hinzuzufügen.

   >[!INFO]
   >
   >**Beispiel**
   >
   >Wenn Sie drei Projekte zum Hinzufügen zum Projekt ausgewählt haben, lautet die Schaltfläche **3 Projekte hinzufügen**.

   Die hinzugefügten Objekte werden im Bereich Paketinhalt rechts auf der Seite angezeigt.

1. Wiederholen Sie die Schritte 7 bis 9, um einen weiteren Objekttyp hinzuzufügen.
1. (Optional) Um ein Objekt aus dem Paket zu entfernen, bewegen Sie den Mauszeiger über das Objekt im Bereich Paketinhalt und klicken Sie dann auf das X neben dem Objekt.
1. Nachdem Sie alle gewünschten Objekte zum Paket hinzugefügt haben, klicken Sie auf **Speichern und schließen** , um das Paket zu speichern, ohne es zusammenzustellen.

   Oder

   Klicks **Speichern und Assemblieren** , um das Paket zu speichern und zusammenzustellen.

   >[!NOTE]
   >
   >* Die Schaltflächen Speichern und Schließen und Speichern und Zusammenführen sind verfügbar, wenn ein Paket sowohl einen Namen mit fünf oder mehr Zeichen als auch mindestens ein Objekt enthält.
   >* Sie können kein Paket zusammenstellen, das sich in einem Installationsstatus wie &quot;Testen&quot;oder &quot;Aktiv&quot;befindet.

## Bearbeiten oder Zusammenführen eines vorhandenen Pakets

1. Wechseln Sie zu der Umgebung, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, in die Sie Objekte kopieren **von**.
1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System** Wählen Sie im linken Navigationsbereich die Option **Umgebungsförderung**.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. (Bedingt) Um deaktivierte Pakete anzuzeigen, aktivieren Sie die **Eingestellte Pakete anzeigen** -Option.
1. (Optional) Um den Inhalt einschließlich aller Objekte und ihrer Unterobjekte anzuzeigen, klicken Sie auf den Dropdown-Pfeil neben dem Objekttyp in der **Inhalt** Abschnitt.
1. (Optional) Um frühere Installationen und Installationsversuche für dieses Paket anzuzeigen, klicken Sie auf **Bereitstellungen**.
1. (Optional) Klicken Sie zum Bearbeiten des Pakets auf **Paket bearbeiten** oben rechts auf dem Bildschirm.
1. Um das Paket zu installieren, klicken Sie auf **Installieren** oben rechts auf dem Bildschirm.

   Anweisungen zum Installieren eines Pakets finden Sie unter [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
