---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Dokumentenbericht mit Link zu einem Korrekturabzug'
description: 'Anzeigen: Dokumentbericht mit Link zu einem Korrekturabzug'
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# Anzeigen: Dokumentbericht mit Link zu einem Korrekturabzug

<!--Audited: 11/2024-->

In dieser Dokumentansicht können Sie einen Link zu einem Korrekturabzug der aktuellen Version des Dokuments einfügen.

![Dokument mit Korrekturabzugs-Link anzeigen](assets/view-document-with-proof-link-350x92.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
