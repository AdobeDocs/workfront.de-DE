---
product-area: resource-management
navigation-topic: resource-planning
title: Anpassen der Budgetierungsdaten im Ressourcenplaner
description: Wenn Sie feststellen, dass Ihre Ressourcen nach der Budgetierung im Ressourcenplaner übermäßig verteilt sind, können Sie die Szenarien erkunden, in denen Sie die budgetierten Stunden, VZÄ oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre geplanten Stunden, FTE oder Kosten anpassen.
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# Anpassen der Budgetierungsdaten im Ressourcenplaner

Wenn Sie feststellen, dass Ihre Ressourcen nach der Budgetierung im Ressourcenplaner übermäßig verteilt sind, können Sie die Szenarien erkunden, in denen Sie die budgetierten Stunden, VZÄ oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre geplanten Stunden, FTE oder Kosten anpassen.

Überverteilungen können auftreten, wenn die Budgetierungszeiten, VZÄ oder Kosten Ihrer Ressourcen höher sind als die verfügbaren Stunden, VZÄ oder Kosten. Dadurch wird ein negativer Nettowert generiert.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf das Ressourcen-Management, das Zugriff auf die Option "Prioritäten bearbeiten"und die Budgetzeiten im Ressourcenplaner enthält.</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, für die Informationen zum Budget bereitgestellt werden sollen, mit der Möglichkeit, die Finanzen zu verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Budgetierungsdaten anpassen

1. Navigieren Sie zum Ressourcenplaner und wählen Sie **Anzeigen nach Projekt**.

   >[!NOTE]
   >
   >Sie können die Option Geplante Datumswerte anpassen nur verwenden, wenn Sie den Ressourcenplaner nach Projekt anzeigen.

1. Bewegen Sie den Mauszeiger über den Namen eines Projekts und klicken Sie auf die Schaltfläche **Mehr** Menü.
1. Klicken **Anpassen der Budgetierungsdaten**.\
   Die Zeitleiste für die Projektzuordnung wird angezeigt.\
   Der Zeitrahmen, in dem die Stunden derzeit in den Haushaltsplan eingesetzt werden, wird bei einem Haushaltskonflikt orange und bei keinem Konflikt blau hervorgehoben.

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. Ziehen Sie den markierten Zeitrahmen per Drag-and-Drop in einen anderen Zeitraum, um zu verstehen, wo es keine Budgetkonflikte für das ausgewählte Projekt gibt. Wenn Sie einen Zeitrahmen finden, in dem der Nettowert positiv ist, wird der hervorgehobene Zeitrahmen blau angezeigt.
1. Klicken Sie auf das &quot;x&quot;in der oberen rechten Ecke der Zeitleiste für die Projektzuordnung, um es zu schließen.
1. Entfernen Sie die geplanten Stunden aus der vorhandenen Timeline des Projekts und fügen Sie sie der Timeline hinzu, die die beste Verfügbarkeit anzeigt.
1. Klicken Sie auf **Speichern**.
1. (Bedingt und optional) Wenn sich die Zeitrahmen ohne Budgetkonflikte außerhalb der Zeitleiste des Projekts befinden, klicken Sie auf den Namen des Projekts, um auf das Projekt zuzugreifen.
1. (Bedingt und optional) Klicken Sie auf **Projekt bearbeiten**, bearbeiten Sie dann die **Geplantes Startdatum** oder **Geplantes Abschlussdatum** , um die Zeitleiste des Projekts für den Zeitrahmen ohne Budgetkonflikte zu ändern.\
   Weitere Informationen zum Bearbeiten von Projekten finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

1. (Bedingt und optional) Klicken Sie auf **Änderungen speichern**.
1. Kehren Sie zum Ressourcenplaner zurück und geben Sie die budgetierten Stunden, VZÄs oder Kosten im Zeitrahmen ohne Budgetkonflikte erneut ein.
1. Klicken Sie auf **Speichern**.
