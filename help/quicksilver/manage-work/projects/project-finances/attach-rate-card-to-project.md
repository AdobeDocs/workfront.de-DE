---
title: Eine Ratenkarte an ein Projekt anhängen
description: Wenn Sie einem Projekt eine Ratenkarte anhängen, werden alle Rollen nach Standort und die zugehörigen Abrechnungsraten zum Projekt hinzugefügt.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Eine Ratenkarte an ein Projekt anhängen

{{highlighted-preview-article-level}}

Ratenkarten speichern mehrere Abrechnungsraten pro Auftragsrolle basierend auf dem Standort. Sie könnten eine berufliche Rolle in Designer mit Sitz in Paris und einen zweiten Designer mit Sitz in New York mit jeweils unterschiedlichen Abrechnungsraten haben. Für Auftragsrollen auf einer Ratenkarte ist jedoch kein Ort erforderlich. Eine Abrechnungsrate für eine Stellenrolle (und möglicherweise einen Ort) auf einer Ratenkarte kann auch effektive Daten enthalten.

Wenn Sie einem Projekt eine Ratenkarte anhängen, werden alle Rollen nach Standort und die zugehörigen Abrechnungsraten zum Projekt hinzugefügt.

>[!NOTE]
>
>Wenn Sie eine Preiskarte anhängen, werden die bestehenden Abrechnungsraten für das Projekt überschrieben.

Sie können die Abrechnungsraten von der Preiskarte direkt im Projekt bearbeiten. Dies wirkt sich nicht auf die auf der Standardratenkarte gespeicherten Tarife aus.

Informationen zum Erstellen von Ratenkarten finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Allgemeine Informationen über die Überschreitung der Abrechnungssätze für Stellenausschreibungen für Projekte und die Berechnung der Projekterlöse finden Sie unter [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Standard</p><p>Oder</p><p>Veralteter Plan: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Administratorzugriff für Job-Rollen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Eine Ratenkarte an ein Projekt anhängen

1. Wechseln Sie zum Projekt.
1. Klicken **Abrechnungssätze** im linken Bereich. Möglicherweise müssen Sie zuerst klicken **Mehr anzeigen**.
1. Klicken **Abrechnungsrate hinzufügen > Eine Ratenkarte anhängen**.

   Die Seite Ratenkarte anhängen wird geöffnet. Weitere Informationen finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Wählen Sie die zum Projekt hinzuzufügende Ratenkarte aus und klicken Sie auf **Attach**.

   Die Ratenkarte und alle ihre Auftragseingangsraten werden der Liste der Abrechnungssätze hinzugefügt.

   ![Dem Projekt hinzugefügte Ratenkarte](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Auf der Liste der Abrechnungssätze können Sie eine oder mehrere Auftragsrollen entfernen, die von einer Ratenkarte stammten. Wenn Sie eine Abrechnungsrate für Auftragsrollen aus dem Projekt entfernen, wird sie nicht von der Standardratenkarte entfernt.

