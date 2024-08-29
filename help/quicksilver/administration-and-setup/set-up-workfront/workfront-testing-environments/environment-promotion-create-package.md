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
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: e9df34c206dd65ccc2edec00087248eb4ed16f54
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets

Sie müssen ein Paket in der Umgebung erstellen, aus dem Sie die Objekte **aus** kopieren möchten. Wenn Sie beispielsweise ein Projekt in Ihrer Sandbox für benutzerdefinierte Aktualisierung konfigurieren und es in Ihrer Produktionsumgebung bewerben, müssen Sie das Paket in Ihrer Sandbox für benutzerdefinierte Aktualisierung erstellen.

>[!IMPORTANT]
>
>Wenn Ihre Sandbox für benutzerdefinierte Aktualisierung aktualisiert wird, während Sie das Objekt für die Umgebungsförderung konfigurieren, geht diese Konfiguration bei der Aktualisierung verloren. Es wird empfohlen, die benutzerdefinierte Aktualisierungs-Sandbox nur dann zu aktualisieren, wenn alle ausstehenden Umgebungsförderungsobjekte und -pakete erfolgreich beworben wurden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime oder Ultimate (nur neue Pläne)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenses</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationen auf Zugriffsebene
   </td>
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Package erstellen

1. Wechseln Sie zu der Umgebung, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, in die Sie Objekte **aus** kopieren.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** (6}Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf das Symbol **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).![
1. Wählen Sie im linken Navigationsbereich **System** und dann **Umgebungsförderung**.
1. Klicken Sie auf **Paket erstellen**.

   Die Seite Neues Promotion-Paket wird geöffnet.

1. Geben Sie im Feld **Paketname** einen Namen für das Paket ein.
1. Geben Sie im Feld **Beschreibung** eine Beschreibung für dieses Paket ein.
1. Um dem Paket ein Objekt hinzuzufügen, klicken Sie im linken Navigationsbereich auf **Objekte hinzufügen** und wählen Sie den Typ des Objekts aus, das Sie hinzufügen möchten.
1. Wählen Sie ein oder mehrere Objekte aus der Liste aus oder geben Sie den Namen in die Suchleiste ein und wählen Sie das Objekt aus, wenn es in der Liste angezeigt wird. Sie können mehrere Objekte in der Liste auswählen.
1. Klicken Sie auf **Hinzufügen (X Objekte)** , um die ausgewählten Objekte zum Paket hinzuzufügen.

   >[!INFO]
   >
   >**Beispiel**
   >
   >Wenn Sie drei Projekte zum Hinzufügen zum Projekt ausgewählt haben, lautet die Schaltfläche &quot;**3 Projekte hinzufügen**&quot;.

   Die hinzugefügten Objekte werden im Bereich Paketinhalt rechts auf der Seite angezeigt.

1. Wiederholen Sie die Schritte 7 bis 9, um einen weiteren Objekttyp hinzuzufügen.
1. (Optional) Um ein Objekt aus dem Paket zu entfernen, bewegen Sie den Mauszeiger über das Objekt im Bereich Paketinhalt und klicken Sie dann auf das X neben dem Objekt.
1. Nachdem Sie alle gewünschten Objekte zum Paket hinzugefügt haben, klicken Sie auf **Speichern und schließen** , um das Paket zu speichern, ohne es zusammenzustellen.

   Oder

   Klicken Sie auf **Speichern und Assemblieren** , um das Paket zu speichern und zusammenzustellen.

   >[!NOTE]
   >
   >* Die Schaltflächen Speichern und Schließen und Speichern und Zusammenführen sind verfügbar, wenn ein Paket sowohl einen Namen mit fünf oder mehr Zeichen als auch mindestens ein Objekt enthält.
   >* Sie können kein Paket zusammenstellen, das sich in einem Installationsstatus wie &quot;Testen&quot;oder &quot;Aktiv&quot;befindet.

## Bearbeiten oder Zusammenführen eines vorhandenen Pakets

1. Wechseln Sie zu der Umgebung, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, in die Sie Objekte **aus** kopieren.
1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** (6}Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf das Symbol **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).![
1. Wählen Sie im linken Navigationsbereich **System** und dann **Umgebungsförderung**.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. (Bedingt) Um deaktivierte Pakete anzuzeigen, aktivieren Sie die Option **Eingestellte Pakete anzeigen** .
1. (Optional) Um den Inhalt einschließlich aller Objekte und ihrer Unterobjekte anzuzeigen, klicken Sie im Abschnitt **Inhalt** auf den Dropdown-Pfeil neben dem Objekttyp.
1. (Optional) Klicken Sie auf **Bereitstellungen**, um die vorherigen Installations- und Installationsversuche dieses Pakets anzuzeigen.
1. (Optional) Um das Paket zu bearbeiten, klicken Sie oben rechts im Bildschirm auf **Paket bearbeiten** .
1. Um das Paket zu installieren, klicken Sie oben rechts im Bildschirm auf **Installieren** .

   Anweisungen zum Installieren eines Pakets finden Sie unter [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
