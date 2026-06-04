---
title: Hinzufügen einer Tarifkarte zu einem Projekt
description: Wenn Sie einem Projekt eine Tarifkarte beifügen, werden alle Funktionen nach Standort und die zugehörigen Abrechnungssätze zum Projekt hinzugefügt.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
TQID: https://experienceleague.adobe.com/waVWQfq2YqgDXZx3wl0ahzuQx7UJ78S1kYY8xBgi5OQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 566
ht-degree: 8%

---

# Anfügen einer Tarifkarte an ein Projekt

Tarifkarten speichern mehrere Abrechnungssätze pro Aufgabengebiet, basierend auf Attributen. Sie könnten beispielsweise für Designer in Paris ein Aufgabengebiet für Agency A, für Agency B ein anderes Designer in Paris und für Agency B ein drittes Designer in New York haben, das keiner Agency zugewiesen ist, die jeweils unterschiedliche Abrechnungssätze aufweisen. Für Aufgabengebiete auf einer Tarifkarte sind jedoch keine Attribute erforderlich. Die Attribute dienen als Werkzeuge zur Festlegung detaillierterer Raten. Ein Abrechnungssatz auf einer Tarifkarte kann auch ein Gültigkeitsdatum sein, sodass der Satz an einem bestimmten Datum beginnt und endet.

Wenn Sie einem Projekt eine Tarifkarte beifügen, werden alle Funktionen und die zugehörigen Abrechnungssätze zum Projekt hinzugefügt.

>[!NOTE]
>
>Wenn Sie eine Tarifkarte anhängen, werden alle vorhandenen Tarifkarten-Abrechnungssätze für das Projekt überschrieben. Abrechnungssatzüberschreibungen, die dem Projekt direkt hinzugefügt wurden, werden nicht entfernt.

Weitere Informationen zum Erstellen von Tarifkarten finden Sie [Verwalten von Tarifkarten](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Allgemeine Informationen zum Überschreiben der Verrechnungssätze für Aufgabengebiete für Projekte und zur Berechnung des Projektumsatzes finden Sie unter [Übersicht über das Überschreiben von Verrechnungssätzen und die Berechnung des Umsatzes für ein Projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte, Finanzdaten und Tarifkarten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie die Berechtigungen für das Projekt mit den Berechtigungen zum Bearbeiten von Abrechnungssätzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anfügen einer Tarifkarte an ein Projekt

1. Gehen Sie zum Projekt.
1. Klicken Sie **linken** auf „Tarife“ und wählen Sie dann **Abrechnung**.
1. Klicken Sie **Abrechnungssatz hinzufügen > Tarifkarte anhängen**.

   Das **„Tarifkarte**&quot; wird geöffnet. Sie können in der Liste nach einer Tarifkarte suchen.

   ![Fügen Sie ein Tarifkartenfeld hinzu](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >Die Gruppe und das Unternehmen auf den Tarifkarten werden als Filter auf dieser Liste verwendet. Da Projekte auch Gruppen- und Firmenfelder enthalten, verwendet Workfront diese Werte, um die Liste der verfügbaren Tarifkarten auf die für den Projektkontext relevanten einzugrenzen, und nicht auf alle Tarifkarten im gesamten System.
   >
   >Die Übereinstimmung muss nicht exakt sein. Tarifkarten mit leeren Gruppen- und/oder Firmenwerten können je nach der Gruppen-/Firmenkonfiguration des Projekts weiterhin angezeigt werden. Wenn beispielsweise für ein Projekt eine Gruppe ausgewählt ist, die Firma jedoch leer ist, werden dieser Gruppe möglicherweise Tarifkarten zugeordnet, selbst wenn die Firma der Tarifkarte unterschiedlich oder leer ist.

1. Wählen Sie die Tarifkarte aus, die dem Projekt hinzugefügt werden soll, und klicken Sie auf **Anhängen**.

   Die Tarifkarte und alle zugehörigen Tarife für Aufgabengebiete werden der Liste Abrechnungssätze hinzugefügt.

   ![Tarifkarte zum Projekt hinzugefügt](assets/rate-card-on-project.png)

## Entfernen einer Tarifkarte aus einem Projekt

Wenn Sie eine Tarifkarte aus einem Projekt entfernen, werden alle ihre Tarife für Aufgabengebiete entfernt. Sie können keinen individuellen Tarif aus dem Projekt entfernen, der von einer Tarifkarte stammt.

Abrechnungssatzüberschreibungen für Benutzer oder Aufgabengebiete, die direkt zum Projekt hinzugefügt wurden, können entfernt werden, ohne dass die gesamte Tarifkarte entfernt werden muss.

1. Gehen Sie zum Projekt.
1. Klicken Sie **linken** auf „Tarife“ und wählen Sie dann **Abrechnung**.
1. Klicken Sie auf das **Entfernen**-Symbol ![Entfernen](assets/remove-icon.png).
1. Klicken **auf** Bestätigungsmeldung, um die Tarifkarte zu entfernen.

