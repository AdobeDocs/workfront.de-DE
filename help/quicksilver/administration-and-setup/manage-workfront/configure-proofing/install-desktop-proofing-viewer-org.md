---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installieren des Desktop Proofing Viewers für Ihr Unternehmen
description: Der Desktop Proofing Viewer, der hauptsächlich für die Prüfung interaktiver Inhalte entwickelt wurde, ist eine Anwendung, die auf dem lokalen Computer jedes Benutzers installiert werden muss. Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie diese Installation durchführen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# Installieren des Desktop Proofing Viewers für Ihr Unternehmen

Der Desktop Proofing Viewer, der hauptsächlich für die Prüfung interaktiver Inhalte entwickelt wurde, ist eine Anwendung, die auf dem lokalen Computer jedes Benutzers installiert werden muss. Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie diese Installation durchführen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium oder Select</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>In Ihrem Profil für Testberechtigungen muss "Administrator"ausgewählt sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurieren des Testversand-Zugriffs eines Benutzers</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Systemanforderungen

Der Desktop Proofing Viewer wird unter den folgenden Betriebssystemen unterstützt:

* Windows 7 und höher, 32-Bit und 64-Bit
* Mac OS X 10.9 und höher, 64 Bit

## Voraussetzungen

Damit Benutzer den Desktop Proofing Viewer verwenden können, müssen Sie

* Konfigurieren Sie das System so, dass der Desktop Proofing Viewer als Standardansicht für interaktive Testsendungen vor der Installation gestartet wird.

## Konfigurieren des Desktop Proofing Viewers als Standard für interaktive Testsendungen

Nachdem Sie den Desktop Proofing Viewer für Ihr Unternehmen installiert haben, können Sie ihn als Standard-Viewer für interaktive Testsendungen festlegen.

1. Klicken Sie in Workfront auf das Hauptmenü ![](assets/main-menu-icon.png)und dann auf Testversand klicken ![](assets/proofing-in-main-menu.png) , um auf Workfront Testversand zuzugreifen.

1. Klicken **Kontoeinstellungen** in der Nähe der oberen rechten Ecke von Workfront Proof klicken Sie auf das **Einstellungen** Registerkarte.

1. under **Standardangaben für Testsendungen** am Ende der **Desktop Proofing Viewer für interaktive Testsendungen** Zeile, klicken Sie auf **Einrichtung**.

   ![](assets/proof-defaults-350x265.png)

1. Klicken **Aktiviert und Standard** Klicken Sie auf **Speichern**.

## Installieren des Testversand-Viewers für Ihre Benutzer

* [Installieren des Desktop Proofing Viewers auf Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installieren des Desktop Proofing Viewers unter Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installieren des Desktop Proofing Viewers auf Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Führen Sie auf dem Computer des Benutzers einen der folgenden Schritte aus, um die App herunterzuladen:

   * Wenn Sie die Produktionsumgebung verwenden, klicken Sie auf  [Mac Production Download für den Desktop Proofing Viewer.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * Wenn Sie die Vorschau-Umgebung verwenden, klicken Sie auf  [Herunterladen der Mac-Vorschau für den Desktop-Proofing-Viewer.](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. Öffnen Sie die Datei, die Sie gerade heruntergeladen haben, um die Installation zu starten.
1. Klicken Sie im angezeigten Installationsfeld auf **Weiter** Klicken Sie auf **Installieren**.

   ![00000776.png](assets/00000776-350x244.png)

1. Stellen Sie sicher, dass alle Benutzer die Installation abgeschlossen haben, indem Sie im Bereich &quot;Dokumente&quot;in Workfront einen interaktiven Testversand öffnen.

### Installieren des Desktop Proofing Viewers unter Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Führen Sie auf dem Computer des Benutzers einen der folgenden Schritte aus, um die App herunterzuladen:

   * Klicken Sie in der Produktionsumgebung auf [Windows Production-Download für den Desktop Proofing Viewer.](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * Klicken Sie in der Vorschau-Umgebung auf [Herunterladen der Windows-Vorschau für den Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Öffnen Sie die Datei, die Sie gerade heruntergeladen haben, um die Installation zu starten.
1. Klicken Sie im angezeigten Sicherheitswarnungsfeld auf **Ausführen**.

   ![screen_shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Der Desktop Proofing Viewer wird installiert und ausgeführt.

1. (Bedingt) Wenn Sie die Anwendung mit Internet Explorer installieren, aktualisieren Sie die Startseite im Browser, nachdem die Anwendung installiert wurde.
1. Stellen Sie sicher, dass alle Benutzer die Installation abgeschlossen haben, indem Sie im Bereich &quot;Dokumente&quot;in Workfront einen interaktiven Testversand öffnen.
