---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Installieren des Desktop Proofing Viewers für Ihr Unternehmen
description: Der Desktop Proofing Viewer, der hauptsächlich für das Proofing interaktiver Inhalte entwickelt wurde, ist eine Anwendung, die auf dem lokalen Computer jedes Benutzers installiert werden muss. Als Adobe Workfront- oder Workfront Proof-Administrator können Sie diese Installation durchführen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
TQID: https://experienceleague.adobe.com/fFf7rX8YWJzj8VTTnvN305UjDo5UV-LjZezuCa-LLAk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 605
ht-degree: 8%

---

# Installieren des Desktop Proofing Viewers für Ihr Unternehmen

<!--Audited: 05/2024-->

Der Desktop Proofing Viewer, der hauptsächlich für das Proofing interaktiver Inhalte entwickelt wurde, ist eine Anwendung, die auf dem lokalen Computer jedes Benutzers installiert werden muss. Als Adobe Workfront- oder Workfront Proof-Administrator können Sie diese Installation durchführen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium oder Select</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>In Ihrem Profil für Korrekturabzugsberechtigungen muss „Administrator“ ausgewählt sein. Weitere Informationen finden Sie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurieren des Proofing-Zugriffs von Benutzenden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Systemanforderungen

Der Desktop Proofing Viewer wird von den folgenden Betriebssystemen unterstützt:

* Windows 7 und höher, 32 Bit und 64 Bit
* Mac OS X 10.9 und höher, 64-Bit

## Voraussetzungen

Damit Benutzer den Desktop Proofing Viewer verwenden können, müssen Sie das System so konfigurieren, dass der Desktop Proofing Viewer als Standardansicht für interaktive Korrekturabzüge vor der Installation gestartet wird.

## Desktop Proofing Viewer als Standard für interaktive Korrekturabzüge konfigurieren

Nachdem Sie den Desktop Proofing Viewer für Ihr Unternehmen installiert haben, können Sie ihn als Standard-Viewer für interaktive Korrekturabzüge festlegen.

{{step1-to-proofing}}

1. Klicken **oben rechts** Workfront Proof auf „Kontoeinstellungen“ und dann auf die Registerkarte **Einstellungen**.

1. Klicken **unter** Testversand-Standardeinstellungen“ am Ende der Zeile **Desktop Proofing Viewer für interaktives**&quot; auf **Setup**.

   ![Standardeinstellungen für Korrekturabzüge](assets/proof-defaults.png)

1. Klicken Sie auf **Aktiviert und Standard** und dann auf **Speichern**.

## Installieren des Desktop Proofing Viewers für Ihre Benutzer

* [Installieren des Desktop Proofing Viewers auf Mac](#installing-the-desktop-proofing-viewer-on-mac)
* [Installieren des Desktop Proofing Viewers unter Windows](#installing-the-desktop-proofing-viewer-on-windows)

### Installieren des Desktop Proofing Viewers auf Mac {#installing-the-desktop-proofing-viewer-on-mac}

1. Führen Sie auf dem Computer des Benutzers einen der folgenden Schritte aus, um die App herunterzuladen:

   * Wenn Sie die Produktionsumgebung verwenden, klicken Sie auf [Mac-Produktionsdownload für den Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * Wenn Sie die Vorschau-Umgebung verwenden, klicken Sie auf [Mac-Vorschau-Download für den Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. Öffnen Sie die soeben heruntergeladene Datei, um die Installation zu starten.
1. Klicken Sie im angezeigten Installationsfenster auf **Fortfahren** und dann auf **Installieren**.

   ![Installationskasten](assets/install-wf-proof-box.png)

1. Stellen Sie sicher, dass jeder Benutzer die Installation abschließt, indem Sie einen interaktiven Korrekturabzug im Bereich Dokumente in Workfront öffnen.

### Installieren des Desktop Proofing Viewers unter Windows {#installing-the-desktop-proofing-viewer-on-windows}

1. Führen Sie auf dem Computer des Benutzers einen der folgenden Schritte aus, um die App herunterzuladen:

   * Klicken Sie in der Produktionsumgebung auf [Windows-Produktions-Download für den Desktop Proofing Viewer](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * Klicken Sie in der Vorschau-Umgebung auf [Windows-Vorschau für den Desktop Proofing Viewer](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. Öffnen Sie die soeben heruntergeladene Datei, um die Installation zu starten.
1. Klicken Sie im angezeigten Warnfeld auf **Ausführen**.

   ![screen_shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   Desktop Proofing Viewer wird installiert und ausgeführt.

1. (Bedingt) Wenn Sie die Anwendung über Internet Explorer installieren, aktualisieren Sie die Startseite im Browser, nachdem die Anwendung installiert wurde.
1. Stellen Sie sicher, dass jeder Benutzer die Installation abschließt, indem Sie einen interaktiven Korrekturabzug im Bereich Dokumente in Workfront öffnen.
