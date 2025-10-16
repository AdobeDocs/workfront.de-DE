---
title: Hinzufügen einer Tarifkarte zu einem Projekt
description: Wenn Sie einem Projekt eine Tarifkarte beifügen, werden alle Funktionen nach Standort und die zugehörigen Abrechnungssätze zum Projekt hinzugefügt.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Tarifkarte an ein Projekt anhängen

{{highlighted-preview-article-level}}

Tarifkarten speichern mehrere Abrechnungssätze pro Aufgabengebiet, basierend auf dem Standort. Sie könnten ein Aufgabengebiet für Designer mit Sitz in Paris und ein zweites Designer mit Sitz in New York haben, jedes mit unterschiedlichen Abrechnungssätzen. Für Aufgabengebiete auf einer Tarifkarte ist jedoch kein Standort erforderlich. Ein Abrechnungssatz für ein Aufgabengebiet (und möglicherweise den Standort) auf einer Tarifkarte kann auch Gültigkeitsdaten enthalten.

Wenn Sie einem Projekt eine Tarifkarte beifügen, werden alle Funktionen nach Standort und die zugehörigen Abrechnungssätze zum Projekt hinzugefügt.

>[!NOTE]
>
>Durch das Anhängen einer Tarifkarte werden alle vorhandenen Abrechnungssätze für das Projekt überschrieben.

Sie können die Abrechnungssätze direkt im Projekt über die Tarifkarte bearbeiten. Dies hat keinen Einfluss auf die auf der Standardtarifkarte gespeicherten Tarife.

Weitere Informationen zum Erstellen von Tarifkarten finden Sie [Verwalten von Tarifkarten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Allgemeine Informationen zum Überschreiben von Abrechnungssätzen für Aufgabengebiete für Projekte und zur Berechnung des Projektumsatzes finden Sie unter [Übersicht über das Überschreiben von Abrechnungssätzen für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Administratorzugriff für Aufgabengebiete</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie Berechtigungen für das Projekt, das die Option Finanzdaten bearbeiten enthält. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tarifkarte an ein Projekt anhängen

1. Gehen Sie zum Projekt.
1. Klicken **im linken** auf „Abrechnungssätze“.
1. Klicken Sie **Abrechnungssatz hinzufügen > Tarifkarte anhängen**.

   Die Seite Tarifkarte anhängen wird geöffnet. Weitere Informationen finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Wählen Sie die Tarifkarte aus, die dem Projekt hinzugefügt werden soll, und klicken Sie auf **Anhängen**.

   Die Tarifkarte und alle zugehörigen Tarife für Aufgabengebiete werden der Liste Abrechnungssätze hinzugefügt.

   ![Tarifkarte zum Projekt hinzugefügt](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >In der Liste Abrechnungssätze können Sie ein oder mehrere Aufgabengebiete entfernen, die aus einer Tarifkarte stammen. Wenn Sie einen Abrechnungssatz für das Aufgabengebiet aus dem Projekt entfernen, wird er nicht aus der Standardratenkarte entfernt.
