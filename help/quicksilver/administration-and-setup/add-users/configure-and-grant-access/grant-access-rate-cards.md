---
title: Zugriff auf Finanzdaten gewähren
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Finanzdaten in Workfront über seine Zugriffsebene definieren.
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: dfc6344303f33a9c3c89837b759235612e54904e
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 10%

---


# Zugriff auf Tarifkarten gewähren

{{highlighted-preview-article-level}}

Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers definieren, um Karten über die Zugriffsebene des Benutzers zu bewerten, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Informationen zu Tarifkarten finden Sie unter [Tarifkarten verwalten](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Gewähren des Zugriffs auf Tarifkarten

Beachten Sie Folgendes, wenn Sie Benutzenden Zugriff auf Tarifkarten in Workfront gewähren:

* Benutzer müssen Bearbeitungszugriff auf Tarifkarten, Projekte und Finanzdaten haben, um eine Tarifkarte an ein Projekt anhängen zu können.
* Benutzer ohne Zugriff auf Tarifkarten und Bearbeitungszugriff auf Finanzdaten können keine Tarifkarte an ein Projekt anhängen, aber sie können andere Abrechnungssätze für das Projekt bearbeiten, die aus anderen Quellen stammen.

## Konfigurieren des Benutzerzugriffs zum Bewerten von Karten mit einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der **Ansicht** oder **Bearbeiten** rechts neben den Tarifkarten und wählen Sie dann die Funktionen aus, die Sie unter **Einstellungen optimieren** gewähren möchten.

   ![Anpassung des Kartenzugriffs](assets/rate-card-access-fine-tune.png)

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren“ aufgeführt sind](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Tarifkarten

Sie können eine Tarifkarte für andere Benutzer freigeben, indem Sie ihnen die entsprechenden Berechtigungen erteilen, wie unter [Tarifkarte freigeben](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md) beschrieben.

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers durch eine Kombination zweier Dinge bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt erteilen
* Die Zugriffsebenen-Einstellungen des Empfängers für den Objekttyp
