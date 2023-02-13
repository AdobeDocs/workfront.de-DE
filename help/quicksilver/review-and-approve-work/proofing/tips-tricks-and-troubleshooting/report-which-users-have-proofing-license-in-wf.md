---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Benutzer mit einer Testlizenz in Adobe Workfront auflisten
description: Sie können auf eine der folgenden Arten anzeigen, für welche Benutzer in Adobe Workfront derzeit die Option "Benutzer kann Testsendungen generieren"aktiviert ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Benutzer mit einer Testlizenz in Adobe Workfront auflisten

Sie können auf eine der folgenden Arten anzeigen, für welche Benutzer in Adobe Workfront derzeit die Option &quot;Benutzer kann Testsendungen generieren&quot;aktiviert ist.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Veralteter Plan: Select oder Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppierungen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Benutzerbericht erstellen

Sie können einen Benutzerbericht erstellen, um zu sehen, welche Benutzer Testsendungen generieren können:

1. Navigieren Sie zu **Berichterstellung** Bereich.
1. Klicken Sie auf **Neuer Bericht** Dropdown-Menü, und klicken Sie auf **Benutzerbericht**.

1. Im **Filter** Registerkarte, klicken Sie auf **Filterregel hinzufügen**.

1. Erweitern Sie im verfügbaren Feld **Benutzer** Klicken Sie auf **Hat Testlizenz**.

1. Auswählen **Gleich** > **True**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Klicken **Speichern+Schließen**.

   Der Bericht zeigt alle Benutzer in Workfront an, denen eine Testlizenz zugewiesen wurde.

## Personenansicht aktualisieren

Sie können in der Personenansicht eine neue Spalte hinzufügen, um zu sehen, welche Benutzer Testsendungen generieren können:

1. Navigieren Sie zu **Personen** Bereich.
1. Klicken Sie auf **Personen** Registerkarte.
1. Im **Ansicht** Führen Sie einen der folgenden Schritte aus:

   * Um diese Informationen zu einer vorhandenen Ansicht hinzuzufügen, wählen Sie die Ansicht aus, die Sie anpassen möchten, und klicken Sie dann auf **Ansicht anpassen**.
   * Um diese Informationen einer neuen Ansicht hinzuzufügen, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen**.
1. Erweitern Sie im verfügbaren Feld **Benutzer** Klicken Sie auf **Hat Testlizenz**.

1. Klicken **Fertig** Klicken Sie auf **Ansicht speichern** oder **Als neue Ansicht speichern**.

   Die Ansicht wird angezeigt **True** oder **False** abhängig davon, ob dem Benutzer eine Testlizenz zugewiesen wurde.
