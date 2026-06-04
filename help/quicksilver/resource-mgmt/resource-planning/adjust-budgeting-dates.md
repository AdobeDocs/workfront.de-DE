---
product-area: resource-management
navigation-topic: resource-planning
title: Budgetierungsdaten im Ressourcenplaner anpassen
description: Wenn Sie feststellen, dass es zu einer Überallokation Ihrer Ressourcen kommt, nachdem Sie sie im Ressourcenplaner budgetiert haben, können Sie Was-wäre-wenn-Szenarien untersuchen, indem Sie die budgetierten Stunden, FTE oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre budgetierten Stunden, VZÄ oder Kosten anpassen.
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
TQID: https://experienceleague.adobe.com/GksjnlROYkPaLMrp8vMkvx8IBZ8CPy2A54KGB2GBnVs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 509
ht-degree: 9%

---

# Anpassen der Budgetierungsdaten im Ressourcenplaner

Wenn Sie feststellen, dass es zu einer Überallokation Ihrer Ressourcen kommt, nachdem Sie sie im Ressourcenplaner budgetiert haben, können Sie Was-wäre-wenn-Szenarien untersuchen, indem Sie die budgetierten Stunden, FTE oder Kosten in einen anderen Zeitrahmen verschieben. Basierend auf den Ergebnissen in diesen Szenarien können Sie dann Ihre budgetierten Stunden, VZÄ oder Kosten anpassen.

Überlastungen können auftreten, wenn die budgetierten Stunden, VZÄ oder Kosten Ihrer Ressourcen höher sind als die verfügbaren Stunden, VZÄ oder Kosten. Dadurch wird ein negativer Nettowert generiert.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcenmanagement bearbeiten, der den Zugriff auf die Bearbeitung von Prioritäten und Budgetstunden im Ressourcenplaner beinhaltet</p> <p>Zugriff auf Finanzdaten bearbeiten, einschließlich Zugriff auf „Kostensätze bearbeiten“ und „Allgemeine Finanzen bearbeiten“</p>
   <p>Zugriff auf Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Projekte, für die Sie Informationen budgetieren möchten, mit der Möglichkeit, Kostensätze zu bearbeiten und allgemeine Finanzen zu bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
