---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Auflisten von Benutzern mit Proofing-Lizenz in Adobe Workfront
description: Sie können sehen, für welche Benutzenden in Adobe Workfront derzeit die Option „Benutzende können Korrekturabzüge generieren“ aktiviert ist, indem Sie einen der folgenden Schritte ausführen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Auflisten von Benutzern mit Proofing-Lizenz in Adobe Workfront

Sie können sehen, für welche Benutzenden in Adobe Workfront derzeit die Option „Benutzende können Korrekturabzüge generieren“ aktiviert ist, indem Sie einen der folgenden Schritte ausführen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen eines Benutzerberichts

Sie können einen Benutzerbericht erstellen, um anzuzeigen, welche Benutzenden Korrekturabzüge generieren können:

1. Navigieren Sie zum **Reporting**-Bereich.
1. Klicken Sie auf **Dropdown** Menü „Neuer Bericht“ und dann auf **Benutzerbericht**.

1. Klicken Sie auf **Registerkarte** Filter **auf „Filterregel hinzufügen**.

1. Erweitern Sie im Feld Verfügbar **Benutzer** und klicken Sie dann auf **Hat Korrekturabzugslizenz**.

1. Wählen Sie **Gleich** > **Wahr** aus.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Klicken Sie **Speichern+Schließen**.

   Der Bericht zeigt alle Benutzenden in Workfront an, denen eine Proofing-Lizenz zugewiesen ist.

## Ansicht „Personen“ aktualisieren

Sie können der Ansicht Personen eine neue Spalte hinzufügen, um anzuzeigen, welche Benutzer Korrekturabzüge erstellen können:

1. Gehen Sie in den **Personen** Bereich.
1. Klicken Sie auf die **Personen**.
1. Führen **im Dropdown** Menü „Ansicht“ einen der folgenden Schritte aus:

   * Um diese Informationen zu einer vorhandenen Ansicht hinzuzufügen, wählen Sie die Ansicht aus, die Sie anpassen möchten, und klicken Sie dann auf **Ansicht anpassen**.
   * Um diese Informationen einer neuen Ansicht hinzuzufügen, klicken Sie auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Erweitern Sie im Feld Verfügbar **Benutzer** und klicken Sie dann auf **Hat Korrekturabzugslizenz**.

1. Klicken Sie **Fertig** und anschließend auf **Ansicht speichern** oder **Als neue Ansicht speichern**.

   In der Ansicht wird **True** oder **False** angezeigt, je nachdem, ob der/dem Benutzenden eine Proofing-Lizenz zugewiesen ist.
