---
product-area: resource-management
navigation-topic: resource-planning
title: Budgetierungsdaten im Ressourcenplaner anpassen
description: Wenn Sie feststellen, dass es zu einer Überallokation Ihrer Ressourcen kommt, nachdem Sie sie im Ressourcenplaner budgetiert haben, können Sie Was-wäre-wenn-Szenarien untersuchen, indem Sie die budgetierten Stunden, FTE oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre budgetierten Stunden, VZÄ oder Kosten anpassen.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# Budgetierungsdaten im Ressourcenplaner anpassen

Wenn Sie feststellen, dass es zu einer Überallokation Ihrer Ressourcen kommt, nachdem Sie sie im Ressourcenplaner budgetiert haben, können Sie Was-wäre-wenn-Szenarien untersuchen, indem Sie die budgetierten Stunden, FTE oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre budgetierten Stunden, VZÄ oder Kosten anpassen.

Überlastungen können auftreten, wenn die budgetierten Stunden, VZÄ oder Kosten Ihrer Ressourcen höher sind als die verfügbaren Stunden, VZÄ oder Kosten. Dadurch wird ein negativer Nettowert generiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
    <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcenmanagement bearbeiten, der den Zugriff auf die Bearbeitung von Prioritäten und Budgetstunden im Ressourcenplaner beinhaltet</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Projekte, für die Sie Informationen budgetieren möchten, mit der Möglichkeit, Finanzen zu verwalten.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Budgetierungsdaten anpassen

1. Gehen Sie zum Ressourcenplaner und wählen Sie **Nach Projekt anzeigen**.

   >[!NOTE]
   >
   >Sie können die Option Budgetierte Termine anpassen nur verwenden, wenn Sie den Ressourcenplaner nach Projekt anzeigen.

1. Bewegen Sie den Mauszeiger über den Namen eines Projekts und klicken Sie dann auf das Menü **Mehr**.
1. Klicken Sie **Budgetierungsdaten anpassen**.\
   Die Zeitleiste für die Projektzuordnung wird angezeigt.\
   Der Zeitrahmen, in dem die Stunden derzeit budgetiert sind, wird bei einem Budgetierungskonflikt orange und bei keinen Konflikten blau hervorgehoben.

   ![Budgetierungsdaten anpassen](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Ziehen Sie den hervorgehobenen Zeitrahmen per Drag-and-Drop in eine andere Zeit, um zu verstehen, wo es keine Budgetkonflikte für das ausgewählte Projekt gibt. Wenn Sie einen Zeitrahmen finden, bei dem der Nettowert positiv ist, wird der hervorgehobene Zeitrahmen in Blau geändert.
1. Klicken Sie auf das „x“ in der oberen rechten Ecke der Zeitleiste für die Projektzuordnung, um sie zu schließen.
1. Entfernen Sie die budgetierten Stunden aus der vorhandenen Zeitleiste des Projekts und fügen Sie sie zur Zeitleiste hinzu, die die größte Verfügbarkeit zeigt.
1. Klicken Sie auf **Speichern**.
1. (Bedingt und optional) Wenn sich die Zeitrahmen ohne Budgetkonflikte außerhalb der Zeitleiste des Projekts befinden, klicken Sie auf den Namen des Projekts, um auf das Projekt zuzugreifen.
1. (Bedingt und optional) Klicken Sie auf **Projekt bearbeiten** und bearbeiten Sie dann das **Geplantes Startdatum** oder das **Geplantes Abschlussdatum**, um die Zeitleiste des Projekts für den Zeitrahmen ohne Budgetkonflikte zu ändern.\
   Weitere Informationen zum Bearbeiten von Projekten finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Bedingt und optional) Klicken Sie auf **Änderungen speichern**.
1. Kehren Sie zum Ressourcenplaner zurück und geben Sie die budgetierten Stunden, FTEs oder Kosten ohne Budgetkonflikte erneut in den Zeitrahmen ein.
1. Klicken Sie auf **Speichern**.
