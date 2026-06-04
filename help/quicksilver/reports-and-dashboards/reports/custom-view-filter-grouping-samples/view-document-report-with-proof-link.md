---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Dokumentenbericht mit Link zu einem Korrekturabzug'
description: 'Ansicht: Dokumentbericht mit Link zu einem Korrekturabzug'
author: Courtney
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/bRL7x0qjHQrwg-HfxtJcazG9GK0WifSsl13VL1K5hGs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 20%

---

# Ansicht: Dokumentbericht mit Link zu einem Korrekturabzug

<!--Audited: 11/2024-->

In dieser Dokumentansicht können Sie einen Link zu einem Korrekturabzug der aktuellen Version des Dokuments einfügen.

![Dokument mit Korrekturabzugs-Link anzeigen](assets/view-document-with-proof-link-350x92.png)

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
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dokumentbericht mit Link zu einem Korrekturabzug anzeigen

Um diese Ansicht anzuwenden:

1. Zu einer Liste von Dokumenten gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie **Wechseln Sie in den Textmodus** und dann **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Ersetzen Sie „Ihre Domain“ durch Ihre eigentliche Workfront-Domain. Wenn die Workfront-URL Ihres Unternehmens beispielsweise *Company.my.workfront.com* lautet, lautet Ihre Domain „Unternehmen“.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
1. (Optional) Um sicherzustellen, dass nur Dokumente mit Korrekturabzügen angezeigt werden, fügen Sie einen Filter hinzu, indem Sie Folgendes durchführen:

   1. Klicken Sie auf **Dropdown** Menü „Filter“ und dann auf **Neuer Filter**.
   1. Klicken Sie **Filterregel hinzufügen** und geben Sie „Testversand-Verantwortlicher“ ein. Wählen Sie dann **ID des Testversands** aus, wenn er in der Liste angezeigt wird.
   1. Wählen Sie **Filtermodifikator** Ist nicht leer“ aus.
   1. Klicken Sie auf **Filter speichern**.
   1. (Optional) Aktualisieren Sie den Filternamen und klicken Sie dann auf **Filter speichern**.

1. Klicken Sie auf den Link in der Spalte Korrekturabzugs-Link , um auf den Korrekturabzug der letzten Version des Dokuments zuzugreifen.
