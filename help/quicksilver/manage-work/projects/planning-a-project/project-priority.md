---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Verstehen und Aktualisieren von Projektprioritäten
description: Es gibt mehrere Möglichkeiten, Prioritäten für Projekte zu verwenden, und sie kommunizieren nicht miteinander. Es wird empfohlen, eine Projektpriorität auszuwählen, die Ihren Anforderungen entspricht, und bei der Kategorisierung der Bedeutung Ihrer Projekte darauf zu verweisen.
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/3w01CpdcPcJ2YreI2xpk0-NMpMteCIcD4jVKGAVAPWE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 614
ht-degree: 7%

---

# Verstehen und Aktualisieren von Projektprioritäten

Es gibt mehrere Möglichkeiten, Prioritäten für Projekte zu verwenden, und sie kommunizieren nicht miteinander. Es wird empfohlen, eine Projektpriorität auszuwählen, die Ihren Anforderungen entspricht, und bei der Kategorisierung der Bedeutung Ihrer Projekte darauf zu verweisen.

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
   <td><p>Standard</p> 
   <p>Abo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Typen von Projektpriorität in Adobe Workfront

Im Folgenden finden Sie Prioritätstypen, mit denen Sie Projekte in Adobe Workfront nach Rang ordnen können:

* **Das Feld Projektpriorität**: Sie können einem Projekt manuell eine Priorität zuweisen. In diesem Artikel wird beschrieben, wie Sie einem Projekt manuell eine Priorität zuweisen.

  Weitere Informationen finden Sie im Abschnitt [Überlegungen zur Projektpriorität](#considerations-about-project-priority) in diesem Artikel.

* **Die Priorität eines Projekts in Portfolio Optimizer**, wenn das Projekt mit einem Portfolio verknüpft ist:

  Weitere Informationen zur Priorität eines Projekts in Portfolio Optimizer finden Sie im Artikel [Priorisieren von Projekten in Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

* **Die Priorität eines Projekts im Ressourcenplaner**: Sie können Projekte im Ressourcenplaner manuell priorisieren, um anzugeben, welche Projekte zuerst Ressourcen erhalten sollen.

  Weitere Informationen zur Priorisierung von Projekten im Ressourcenplaner finden Sie im Abschnitt „Projektplanungspriorität“ im Artikel [Ressourcenplaner - Navigationsübersicht](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Überlegungen zur Projektpriorität {#considerations-about-project-priority}

Sie können Projekten in Workfront eine Priorität zuordnen. Wenn eine Priorität für das Projekt angegeben wird, wird allen im System mitgeteilt, wie wichtig dieses Projekt ist.

Beachten Sie bei der Auswahl einer Priorität für Ihre Projekte Folgendes:

* Ihr Workfront-Administrator definiert die in Workfront verfügbaren Prioritäten. Nachdem sie eingerichtet wurden, können Sie sie mit Projekten im Feld Priorität verknüpfen.

  Weitere Informationen zum Erstellen von Prioritäten in Workfront finden Sie im Artikel [Erstellen und Anpassen von Prioritäten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

* Wenn Sie das Feld Priorität eines Projekts aktualisieren, wird diese Priorität nicht an Portfolio Optimizer oder den Ressourcenplaner übertragen. Das Feld Priorität des Projekts ist lediglich eine manuelle Markierung, die Sie auf das Projekt setzen, um anderen Benutzern seine Bedeutung zu verdeutlichen.
* Der Prioritätswert eines Projekts wird hauptsächlich zu Berichtszwecken verwendet.

  Sie können beispielsweise nach allen Projekten suchen, die den Prioritätswert „Dringend“ aufweisen, wenn Sie dieses Feld in einem Projektfilter verwenden.
* Aufgaben und Probleme haben ebenfalls Prioritäten, aber die Aufgaben-, Problem- und Projektprioritäten arbeiten unabhängig voneinander und beeinflussen sich nicht automatisch gegenseitig. Sie können in einem Projekt mit niedriger Priorität ein Problem mit hoher Priorität oder eine Aufgabe mit mittlerer Priorität haben.
* Sie können die Priorität von Projekten in den folgenden Bereichen von Workfront aktualisieren:

   * Im Dialogfeld **Projekt bearbeiten**.
   * Auf der **Projektdetails** Registerkarte eines Projekts.
   * In einer Projektliste oder einem Bericht.

## Aktualisieren des Feldes Projektpriorität

1. Wechseln Sie zu dem Projekt, dessen Priorität Sie aktualisieren möchten.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/qs-edit-icon.png) in der oberen rechten Ecke des Bereichs Projektdetails und dann auf **Übersicht**.

1. Wählen **im Feld** eine der folgenden Optionen aus:

   * Keine
   * Niedrig
   * Normal

     Dies ist die Standardpriorität.

   * Hoch
   * Dringend

   ![Prioritätenliste eines Projekts](assets/project-priority-picker-list.png)

1. Klicken Sie auf **Änderungen speichern**.

   Sie müssen mit anderen Benutzern kommunizieren und verstehen, was jede Prioritätsstufe für das Projekt bedeutet.
