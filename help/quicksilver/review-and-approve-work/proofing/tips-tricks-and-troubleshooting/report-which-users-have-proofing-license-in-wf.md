---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Auflisten von Benutzenden mit Proofing-Lizenz in Adobe Workfront
description: Sie können sehen, für welche Benutzenden in Adobe Workfront derzeit die Option „Benutzende können Korrekturabzüge generieren“ aktiviert ist, indem Sie einen der folgenden Schritte ausführen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
TQID: https://experienceleague.adobe.com/9P5Bp9TrJ1ECSwpK7C4AW4rQlTQOBH4U7-CPYl92RKU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 20%

---

# Auflisten von Benutzenden mit Proofing-Lizenz in Adobe Workfront

Sie können sehen, für welche Benutzenden in Adobe Workfront derzeit die Option „Benutzende können Korrekturabzüge generieren“ aktiviert ist, indem Sie einen der folgenden Schritte ausführen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
