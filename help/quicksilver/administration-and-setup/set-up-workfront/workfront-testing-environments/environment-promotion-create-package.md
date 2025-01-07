---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets
description: Die Funktion zum Hochstufen der Umgebung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Erfahren Sie, wie Sie ein Umgebungs-Promotion-Paket erstellen, das Sie dann in einer anderen Umgebung installieren können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 839b53afb9233ef0e36e981b243c8b2593b45f0f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets

Sie müssen ein Paket in der Umgebung erstellen, aus der Sie Objekte (**)** möchten. Wenn Sie beispielsweise ein Projekt in Ihrer benutzerdefinierten Aktualisierungs-Sandbox-Umgebung konfigurieren und es in Ihre Produktionsumgebung übertragen, müssen Sie das Paket in Ihrer benutzerdefinierten Aktualisierungs-Sandbox-Umgebung erstellen.

>[!IMPORTANT]
>
>Wenn Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisiert wird, während Sie das Objekt für die Umgebungsweiterleitung konfigurieren, geht diese Konfiguration bei der Aktualisierung verloren. Es wird empfohlen, die benutzerdefinierte Aktualisierungs-Sandbox nur zu aktualisieren, wenn alle ausstehenden Objekte und Pakete zur Umgebungsförderung erfolgreich beworben wurden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] Plan</strong>
   </td>
   <td> Prime oder Ultimate (nur neue Pläne)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] Lizenzen</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Erstellen eines Pakets

1. Wechseln Sie zu der Umgebung, in der Sie das Paket erstellen möchten. Dies ist die Umgebung, aus der Sie Objekte ****.
1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **** Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **linken Navigationsbereich die Option** System“ und dann **Umgebungs-Promotion** aus.
1. Klicken Sie **Paket erstellen**.

   Die Seite Neues Promotion-Paket wird geöffnet.

1. Geben Sie **Feld „Paketname** einen Namen für das Paket ein.
1. Geben **im Feld** eine Beschreibung für dieses Paket ein.
1. Um ein -Objekt zum Paket hinzuzufügen, wählen Sie in der linken Navigationsleiste den Typ des -Objekts aus, das Sie hinzufügen möchten.
1. Wählen Sie ein oder mehrere Objekte aus der angezeigten Liste aus, oder geben Sie den Namen in die Suchleiste ein, und wählen Sie das Objekt aus, wenn es in der Liste angezeigt wird. Sie können mehrere Objekte in der Liste auswählen.

   Die Liste enthält bis zu 500 Objekte des ausgewählten Objekttyps. Um ein Objekt zu finden, das sich nicht auf der Liste befindet, verwenden Sie die Suchleiste.
1. Klicken Sie auf **Hinzufügen (X Objekte)**, um die ausgewählten Objekte zum Paket hinzuzufügen.

   >[!INFO]
   >
   >**Beispiel**
   >
   >Wenn Sie drei Projekte zum Hinzufügen zum Projekt ausgewählt haben, lautet die Schaltfläche **3 Projekte hinzufügen**.

   Die Objekte, die Sie hinzugefügt haben, werden im Bereich Paketinhalt rechts auf der Seite angezeigt.

1. Um einen anderen Objekttyp hinzuzufügen, wiederholen Sie die Schritte 7-9.
1. (Optional) Um ein Objekt aus dem Paket zu entfernen, bewegen Sie den Mauszeiger über das Objekt im Bereich Paketinhalt und klicken Sie dann auf das X neben dem Objekt.
1. Nachdem Sie alle gewünschten Objekte zum Paket hinzugefügt haben, klicken Sie auf **Speichern und schließen** um das Paket zu speichern, ohne es zusammenzustellen.

   Oder

   Klicken Sie **Speichern und**), um das Paket zu speichern und zusammenzustellen.

   >[!NOTE]
   >
   >* Die Schaltflächen Speichern und schließen sowie Speichern und Zusammenstellen sind verfügbar, wenn ein Paket sowohl einen Namen mit fünf oder mehr Zeichen als auch mindestens ein Objekt enthält, das hinzugefügt wurde.
   >* Sie können kein Paket zusammenstellen, das sich in einem installierbaren Status wie „Testen“ oder „Aktiv“ befindet.

## Bearbeiten oder Zusammenführen eines vorhandenen Pakets

Ein Paket muss `DRAFT` Status haben, damit es bearbeitet werden kann.

1. Wechseln Sie zu der Umgebung, in der Sie das Paket bearbeiten möchten. Dies ist die Umgebung, in der das Paket ursprünglich erstellt wurde.
1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **** Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **linken Navigationsbereich die Option** System“ und dann **Umgebungs-Promotion** aus.
1. Wählen Sie das Paket aus der angezeigten Liste aus.
1. (Bedingt) Um deaktivierte Pakete anzuzeigen, aktivieren Sie die Option **Eingestellte Pakete anzeigen**.
1. (Optional) Um den Inhalt einschließlich aller Objekte und ihrer Unterobjekte anzuzeigen, klicken Sie auf den Dropdown-Pfeil neben dem Objekttyp im Abschnitt **Inhalte**.
1. (Optional) Um frühere Installationen und Installationsversuche dieses Pakets anzuzeigen, klicken Sie auf &quot;**&quot;**.
1. (Optional) Um das Paket zu bearbeiten, klicken **oben** auf dem Bildschirm auf „Paket bearbeiten“.
Ein Paket muss `DRAFT` Status haben, damit es bearbeitet werden kann. Um das Paket in `DRAFT` Status zu verschieben, klicken Sie im Feld **Status** auf `Draft`. Sie können dann mit der Bearbeitung des Pakets fortfahren.
1. Um das Paket zu installieren **klicken Sie** oben rechts auf dem Bildschirm auf „Installieren“.

   Anweisungen zur Installation eines Pakets finden Sie unter [Installieren eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).

## Erstellen eines Pakets aus einem Objektvergleich

Sie können ein Paket direkt aus einem Objektvergleich erstellen.

1. Erstellen Sie einen Objektvergleich, wie in [Objekte zwischen Umgebungen vergleichen](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md) beschrieben.
1. Wählen Sie im generierten Vergleich die Objekte aus, die Sie in das Paket aufnehmen möchten.
1. Klicken **oben rechts** Bildschirm auf „Paket erstellen“.
1. Geben Sie einen Namen und eine Beschreibung für das Paket ein.
1. Klicken Sie **Fenster** erstellen auf „Paket erstellen“.

   Das Paket wird generiert.
