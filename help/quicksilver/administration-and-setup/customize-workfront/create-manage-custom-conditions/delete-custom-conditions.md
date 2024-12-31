---
title: Löschen einer benutzerdefinierten Bedingung
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

# Löschen einer benutzerdefinierten Bedingung

Sie können eine benutzerdefinierte Bedingung löschen, wenn sie nicht mehr benötigt wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen einer benutzerdefinierten Bedingung

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Bedingungen**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgabe** oder **Problem**), auf der sich die Bedingung befindet, die Sie löschen möchten.

1. Bewegen Sie den Mauszeiger über die Bedingung, die Sie löschen möchten, und klicken Sie dann auf das **Löschen**-Symbol, ![](assets/delete.png) ganz rechts angezeigt wird.
1. Klicken Sie in der angezeigten Bestätigungsmeldung auf **Bedingung löschen**.

1. Wählen Sie **angezeigten Feld** Bedingung löschen“ in der Dropdown-Liste für alle Projekte, die die Bedingung verwendet haben, die Sie löschen möchten, eine neue Bedingung aus.

   Benutzerdefinierte Bedingungen sind in der Dropdown-Liste nur verfügbar, wenn sie mit derselben integrierten Bedingung übereinstimmen wie die, die Sie löschen möchten. Wenn Sie beispielsweise eine Bedingung löschen, die der Gefährdungsstufe entspricht, können nur benutzerdefinierte Bedingungen ausgewählt werden, die ebenfalls der Stufe Gefährdet entsprechen.

1. Klicken Sie **Bedingung löschen**.

>[!NOTE]
>
>Die integrierten Bedingungen „In Target“, „Gefährdet“ und „In Schwierigkeiten“ können nicht gelöscht werden. Sie können jedoch ihren Namen und ihre Farbe ändern.

Informationen zu benutzerdefinierten Bedingungen finden Sie unter [Benutzerdefinierte Bedingungen](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
