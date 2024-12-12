---
title: Eine Ratenkarte an ein Projekt anhängen
description: Wenn Sie einem Projekt eine Ratenkarte anhängen, werden alle Rollen nach Standort und die zugehörigen Abrechnungsraten zum Projekt hinzugefügt.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Eine Ratenkarte an ein Projekt anhängen

{{highlighted-preview-article-level}}

Ratenkarten speichern mehrere Abrechnungsraten pro Auftragsrolle basierend auf dem Standort. Sie könnten eine berufliche Rolle mit Designer mit Sitz in Paris und eine zweite Designer mit Sitz in New York mit jeweils unterschiedlichen Abrechnungsraten haben. Für Auftragsrollen auf einer Ratenkarte ist jedoch kein Ort erforderlich. Eine Abrechnungsrate für eine Stellenrolle (und möglicherweise einen Ort) auf einer Ratenkarte kann auch effektive Daten enthalten.

Wenn Sie einem Projekt eine Ratenkarte anhängen, werden alle Rollen nach Standort und die zugehörigen Abrechnungsraten zum Projekt hinzugefügt.

>[!NOTE]
>
>Wenn Sie eine Preiskarte anhängen, werden die bestehenden Abrechnungsraten für das Projekt überschrieben.

Sie können die Abrechnungsraten von der Preiskarte direkt im Projekt bearbeiten. Dies wirkt sich nicht auf die auf der Standardratenkarte gespeicherten Tarife aus.

Informationen zum Erstellen von Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Allgemeine Informationen zum Außerkraftsetzen der Abrechnungssätze für Stellenrollen für Projekte und zur Berechnung der Projekterlöse finden Sie unter [Übersicht über die Außerbetriebnahme von Auftragsrollenabrechnungen und Berechnung der Umsätze für ein Projekt](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Administratorzugriff auf Stellenrollen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Eine Ratenkarte an ein Projekt anhängen

1. Wechseln Sie zum Projekt.
1. Klicken Sie im linken Bereich auf **Abrechnungsraten**. Möglicherweise müssen Sie zuerst auf **Mehr anzeigen** klicken.
1. Klicken Sie auf **Abrechnungsrate hinzufügen > Eine Ratenkarte anhängen**.

   Die Seite Ratenkarte anhängen wird geöffnet. Weitere Informationen finden Sie unter [Verwalten von Ratenkarten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Wählen Sie die Ratenkarte aus, die dem Projekt hinzugefügt werden soll, und klicken Sie auf **Anhängen**.

   Die Ratenkarte und alle ihre Auftragseingangsraten werden der Liste der Abrechnungssätze hinzugefügt.

   ![Dem Projekt hinzugefügte Ratenkarte](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Auf der Liste der Abrechnungssätze können Sie eine oder mehrere Auftragsrollen entfernen, die von einer Ratenkarte stammten. Wenn Sie eine Abrechnungsrate für Auftragsrollen aus dem Projekt entfernen, wird sie nicht von der Standardratenkarte entfernt.
