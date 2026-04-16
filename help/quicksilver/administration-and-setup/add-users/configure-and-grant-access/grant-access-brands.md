---
title: Zugriff auf Markenberechtigungen gewähren
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie Markenberechtigungen konfigurieren, indem Sie eine Benutzergruppe in der Admin Console erstellen und das Produktprofil GenStudio System Manager zuweisen.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 7%

---

# Zugriff auf Markenberechtigungen gewähren

Benutzern werden die Berechtigungen zum Erstellen, Bearbeiten und Veröffentlichen von Adobe GenStudio-System-Managern gewährt, wenn sie zu einer Benutzergruppe hinzugefügt werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console-Berechtigungen</td> 
   <td> <p>Sie müssen Systemadministrator in der Adobe Admin Console sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anforderungen

* Für Ihre Workfront-Instanz müssen einheitliche Genehmigungen aktiviert sein.

* Ihr Unternehmen muss über GenStudio Foundation verfügen.
   * Content Reviewer in Workfront bietet die in GenStudio Foundation verfügbaren Funktionen für Asset-Prüfungs- und Genehmigungs-Workflows. Sie müssen nicht direkt auf GenStudio Foundation zugreifen, um Ihre Arbeit abzuschließen. Ihr Zugriff auf GenStudio Foundation-Funktionen über Content Reviewer fällt unter die Bedingungen Ihres Workfront-Vertrags.
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.
Weitere Informationen zur Unterzeichnung des Abkommens finden Sie unter [Unterzeichnung des Adobe Gen AI-Abkommens](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Konfigurieren der Markenberechtigungen in der Admin Console

### Schritt 1: Erstellen einer Benutzergruppe

Erstellen Sie eine neue Benutzergruppe in der Admin Console, um Berechtigungen für die Markenerstellung und -bearbeitung zu verwalten.

### Schritt 2: Zuweisen eines Produktprofils zur Benutzergruppe

Die mit dem zugewiesenen Profil verknüpfte Berechtigung gibt allen Benutzenden in dieser Gruppe GenStudio Brands Berechtigungen (Marken erstellen, aktualisieren und löschen).

So weisen Sie ein Profil zu:

1. Navigieren Sie zur neu erstellten Benutzergruppe.
1. Klicken Sie auf **Registerkarte Zugewiesene** .
1. Klicken Sie **Profil zuweisen**.
1. Wählen Sie im Popup **Adobe GenStudio** aus der Produktliste aus und klicken Sie dann auf **Apply**.
1. Wählen Sie das Profil **Adobe GenStudio Foundation Editors** aus.
1. Klicken Sie auf **Übernehmen**.
1. Klicken Sie auf **Speichern**.

### Schritt 3: Benutzer zur Benutzergruppe hinzufügen

Um Benutzern Berechtigungen zum Erstellen, Bearbeiten und Veröffentlichen von Marken zuzuweisen, fügen Sie sie der Benutzergruppe hinzu.

>[!NOTE]
>
>Sie müssen mindestens einen Benutzer hinzufügen, bevor Sie die Gruppe wie in Schritt 4 beschrieben zu einem Projekt hinzufügen.

Hinzufügen von Benutzern:

1. Navigieren Sie zu **Admin Console** > **Benutzer** > **Benutzergruppen**.
1. Wählen Sie Ihre Benutzergruppe aus.
1. Benutzer nach Benutzernamen oder E-Mail-Adresse hinzufügen.
1. Auswahl aus vorgeschlagenen Treffern für bestehende Benutzer.

### Schritt 4: Erstellen eines Brands-Projekts

Ein Projekt bietet einen Speicherort, an dem Benutzer Marken-Assets speichern können.

Erstellen eines Projekts:

1. Navigieren Sie zur Registerkarte **Datenspeicherung** in Admin Console.
1. Klicken Sie auf **Projekte**.
1. Klicken Sie **Projekt erstellen**.
1. Geben Sie im Popup den Projektnamen ein: **Adobe GenStudio Brands**.

   >[!IMPORTANT]
   >
   >Geben Sie den Projektnamen genau wie gezeigt ein. Fügen Sie keine zusätzlichen Leerzeichen hinzu und ändern Sie die Groß-/Kleinschreibung nicht.

1. Klicken Sie auf **Erstellen**.

### Schritt 5: Benutzergruppe zum Projekt einladen

Fügen Sie die Benutzergruppe zum Brands-Projekt hinzu, damit sie auf Assets zugreifen und sie verwalten kann.

1. Fügen Sie im **Zum Projekt**) die von Ihnen erstellte Benutzergruppe hinzu.
1. Wählen Sie **Kann bearbeiten** aus.
1. Klicken Sie auf **Einladen**.

### Ergebnis

Benutzer in der Gruppe haben jetzt die Berechtigung, Marken-Assets in Workfront zu erstellen, zu bearbeiten und zu veröffentlichen.

## &#x200B;2. Gewähren des Zugriffs auf Workfront-Zugriffsebenen für Marken

Sie müssen alle Schritte im vorherigen Abschnitt abschließen, bevor Sie einzelnen Benutzern Zugriff auf die Zugriffsebenen von Marken in Workfront gewähren.

>[!IMPORTANT]
>
>* Nur Benutzende, die der Benutzergruppe mit dem GenStudio System Manager-Produktprofil in der Admin Console zugewiesen sind, können Marken in Workfront erstellen, bearbeiten und veröffentlichen, auch wenn andere Benutzende in ihren Zugriffsebenen-Einstellungen Zugriff auf Marken aktiviert haben.
>* Benutzende, die zur Zugriffsebene mit aktiviertem Markenzugriff hinzugefügt wurden, aber nicht zur Benutzergruppe in der Admin Console hinzugefügt wurden, können nur Marken anzeigen.


So gewähren Sie Zugriff auf die Zugriffsebenen von Marken in Workfront:

{{step-1-to-setup}}

1. Klicken **im linken** auf „Zugriffsebenen“.
1. Suchen Sie die Zugriffsebene, die Sie bearbeiten möchten, und klicken Sie dann auf das Bearbeitungssymbol ![Bearbeiten-Symbol](assets/edit-icon.png), um sie zu bearbeiten.

   Oder

   Klicken Sie **Neue Zugriffsebene**, um eine neue Zugriffsebene zu erstellen. Weitere Informationen zum Erstellen von Zugriffsebenen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Scrollen Sie nach unten **Zusätzliche Einschränkungen festlegen** und wählen Sie dann **Benutzer dürfen auf Marken zugreifen** aus.
   ![Einstellung „Zugriff auf Marken zulassen“](assets/access-for-brands.png)
1. Klicken Sie auf **Speichern**.

Nachdem Sie Marken konfiguriert haben, können Sie einen Content Reviewer erstellen, der Assets im Überprüfungs- und Genehmigungs-Workflow anhand der Markenrichtlinien überprüft. Weitere Informationen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).
