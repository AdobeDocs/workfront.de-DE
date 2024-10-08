---
product-area: resource-management
navigation-topic: resource-planning
title: Anpassen der Budgetierungsdaten im Ressourcenplaner
description: Wenn Sie feststellen, dass Ihre Ressourcen nach der Budgetierung im Ressourcenplaner übermäßig verteilt sind, können Sie die Szenarien erkunden, in denen Sie die budgetierten Stunden, VZÄ oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre geplanten Stunden, FTE oder Kosten anpassen.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Anpassen der Budgetierungsdaten im Ressourcenplaner

Wenn Sie feststellen, dass Ihre Ressourcen nach der Budgetierung im Ressourcenplaner übermäßig verteilt sind, können Sie die Szenarien erkunden, in denen Sie die budgetierten Stunden, VZÄ oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre geplanten Stunden, FTE oder Kosten anpassen.

Überverteilungen können auftreten, wenn die Budgetierungszeiten, VZÄ oder Kosten Ihrer Ressourcen höher sind als die verfügbaren Stunden, VZÄ oder Kosten. Dadurch wird ein negativer Nettowert generiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
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
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf das Ressourcen-Management, das Zugriff auf die Option "Prioritäten bearbeiten"und die Budgetzeiten im Ressourcenplaner enthält.</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, für die Informationen zum Budget bereitgestellt werden sollen, mit der Möglichkeit, die Finanzen zu verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Budgetierungsdaten anpassen

1. Wechseln Sie zum Ressourcenplaner und wählen Sie **Nach Projekt anzeigen** aus.

   >[!NOTE]
   >
   >Sie können die Option Geplante Datumswerte anpassen nur verwenden, wenn Sie den Ressourcenplaner nach Projekt anzeigen.

1. Bewegen Sie den Mauszeiger über den Namen eines Projekts und klicken Sie dann auf das Menü **Mehr** .
1. Klicken Sie auf **Budgetierungsdaten anpassen**.\
   Die Zeitleiste für die Projektzuordnung wird angezeigt.\
   Der Zeitrahmen, in dem die Stunden derzeit in den Haushaltsplan eingesetzt werden, wird bei einem Haushaltskonflikt orange und bei keinem Konflikt blau hervorgehoben.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Ziehen Sie den markierten Zeitrahmen per Drag-and-Drop in einen anderen Zeitraum, um zu verstehen, wo es keine Budgetkonflikte für das ausgewählte Projekt gibt. Wenn Sie einen Zeitrahmen finden, in dem der Nettowert positiv ist, wird der hervorgehobene Zeitrahmen blau angezeigt.
1. Klicken Sie auf das &quot;x&quot;in der oberen rechten Ecke der Zeitleiste für die Projektzuordnung, um es zu schließen.
1. Entfernen Sie die geplanten Stunden aus der vorhandenen Timeline des Projekts und fügen Sie sie der Timeline hinzu, die die beste Verfügbarkeit anzeigt.
1. Klicken Sie auf **Speichern**.
1. (Bedingt und optional) Wenn sich die Zeitrahmen ohne Budgetkonflikte außerhalb der Zeitleiste des Projekts befinden, klicken Sie auf den Namen des Projekts, um auf das Projekt zuzugreifen.
1. (Bedingt und optional) Klicken Sie auf **Projekt bearbeiten** und bearbeiten Sie dann das geplante Startdatum **3} oder das geplante Abschlussdatum** 5}, um die Timeline des Projekts für den Zeitraum ohne Budgetkonflikte zu ändern.****\
   Weitere Informationen zum Bearbeiten von Projekten finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Bedingt und optional) Klicken Sie auf **Änderungen speichern**.
1. Kehren Sie zum Ressourcenplaner zurück und geben Sie die budgetierten Stunden, VZÄs oder Kosten im Zeitrahmen ohne Budgetkonflikte erneut ein.
1. Klicken Sie auf **Speichern**.
