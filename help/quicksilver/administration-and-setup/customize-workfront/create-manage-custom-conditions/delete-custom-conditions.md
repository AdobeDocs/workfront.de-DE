---
title: Benutzerdefinierte Bedingung löschen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Sie können eine benutzerdefinierte Bedingung löschen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Benutzerdefinierte Bedingung löschen

Sie können eine benutzerdefinierte Bedingung löschen, wenn sie nicht mehr benötigt wird.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Bedingung löschen

{{step-1-to-setup}}

1. Klicken Sie auf **Projekteinstellungen** > **Bedingungen**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgabe** oder **Problem**), in dem sich die Bedingung befindet, die Sie löschen möchten.

1. Bewegen Sie den Mauszeiger über die Bedingung, die Sie löschen möchten, und klicken Sie dann auf das Symbol **Löschen** ![](assets/delete.png), das ganz rechts angezeigt wird.
1. Klicken Sie in der angezeigten Bestätigungsmeldung auf **Bedingung löschen**.

1. Wählen Sie im angezeigten Feld **Bedingung löschen** eine neue Bedingung in der Dropdown-Liste für alle Projekte aus, die die zu löschende Bedingung verwendet haben.

   Benutzerdefinierte Bedingungen sind nur dann in der Dropdownliste verfügbar, wenn sie mit derselben integrierten Bedingung übereinstimmen, die Sie löschen. Wenn Sie beispielsweise eine Bedingung löschen, die mit &quot;Risiko&quot;übereinstimmt, können nur benutzerdefinierte Bedingungen ausgewählt werden, die auch mit &quot;Risiko&quot;übereinstimmen.

1. Klicken Sie auf **Bedingung löschen**.

>[!NOTE]
>
>Sie können die integrierten Bedingungen, die sich auf Target, Risiko und In Schwierigkeiten befinden, nicht löschen. Sie können jedoch Namen und Farben ändern.

Weitere Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
