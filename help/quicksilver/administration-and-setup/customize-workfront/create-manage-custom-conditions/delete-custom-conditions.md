---
title: Benutzerdefinierte Bedingung löschen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Sie können eine benutzerdefinierte Bedingung löschen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Benutzerdefinierte Bedingung löschen

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierte Bedingung löschen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Projektvoreinstellungen** > **Bedingungen**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgabe** oder **Problem**), wobei sich die Bedingung, die Sie löschen möchten, befindet.

1. Bewegen Sie den Mauszeiger über die Bedingung, die Sie löschen möchten, und klicken Sie auf die Schaltfläche **Löschen** icon ![](assets/delete.png) das ganz rechts erscheint.
1. Klicken Sie in der angezeigten Bestätigungsmeldung auf **Bedingung löschen**.

1. Im **Bedingung löschen** wird eine neue Bedingung in der Dropdown-Liste für alle Projekte ausgewählt, die die zu löschende Bedingung verwendet haben.

   Benutzerdefinierte Bedingungen sind nur dann in der Dropdownliste verfügbar, wenn sie mit derselben integrierten Bedingung übereinstimmen, die Sie löschen. Wenn Sie beispielsweise eine Bedingung löschen, die mit &quot;Risiko&quot;übereinstimmt, können nur benutzerdefinierte Bedingungen ausgewählt werden, die auch mit &quot;Risiko&quot;übereinstimmen.

1. Klicken **Bedingung löschen**.

>[!NOTE]
>
>Sie können die integrierten Bedingungen, die sich auf Target, Risiko und In Schwierigkeiten befinden, nicht löschen. Sie können jedoch Namen und Farben ändern.

Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
