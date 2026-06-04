---
title: Freigeben von Finanzberechtigungen für ein Objekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Finanzdaten gewähren. Weitere Informationen finden Sie unter Gewähren des Zugriffs auf Finanzdaten.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/IVsfFJKauKvgOzXMP8rxHos8LDhqWYnThoyZeaiMCv0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 542
ht-degree: 14%

---

# Freigeben von Finanzberechtigungen für ein Objekt

Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Finanzdaten gewähren. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten der Finanzen für bestimmte Projekte, Aufgaben oder Probleme erteilen, auf die Sie Zugriff haben.

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Finanzdaten tun können, finden Sie im Abschnitt [Finanzdaten](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriffsanforderungen

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Standard</p> 
   <p>Abo</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme und Finanzdaten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> Zeigen Sie Berechtigungen oder höhere Berechtigungen für Projekte, Aufgaben und Probleme an, die mindestens „Abrechnungssätze anzeigen“, „Kostensätze anzeigen“ und „Allgemeine Finanzberechtigungen anzeigen“ umfassen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objekt freigeben und finanzielle Berechtigungen erteilen

Beachten Sie Folgendes, wenn Sie Objekten Finanzberechtigungen erteilen:

* Sie können Projekten, Aufgaben und Problemen finanzielle Berechtigungen erteilen.
* Berechtigungen können geerbt werden: Wenn Sie über die Berechtigung „Allgemeine Finanzen anzeigen“ für ein Projekt verfügen, übernehmen Sie automatisch die Berechtigungen „Allgemeine Finanzen anzeigen“ für die Aufgaben und Probleme im Projekt.
* Durch das Gewähren von Berechtigungen für Abrechnungs- und Kostensätze kann der Benutzer die Sätze für dieses Objekt anzeigen oder bearbeiten. Mit den Berechtigungen für allgemeine Finanzen kann der Benutzer allgemeine Finanzfelder (die nicht mit Abrechnungs- oder Kostensätzen in Verbindung stehen) für das Objekt anzeigen oder bearbeiten.

So erteilen Sie einem Objekt finanzielle Berechtigungen:

1. Wechseln Sie zu einer Aufgabe, einem Projekt oder einem Problem, die/das Sie für andere freigeben möchten.
1. Klicken Sie in der Nähe des Objektnamens auf **Freigeben**.

1. Geben Sie **Feld `<Object name>` Zugriff auf** den Namen eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens ein, für den bzw. die Sie das Objekt freigeben möchten.

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie eine der folgenden Optionen:

   * **Anzeigen**
   * **Beitragen**
   * **Verwalten**

1. Klicken Sie im gleichen Dropdown-Menü auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe und führen Sie dann einen der folgenden Schritte aus:

   * Wählen Sie für jede Berechtigungsstufe **Abrechnungssätze anzeigen**, **Kostensätze anzeigen** und **Allgemeine Finanzen anzeigen** aus.
   * Wählen **nur** Berechtigungen die Optionen **Abrechnungssätze bearbeiten**, **Kostensätze bearbeiten** und **Allgemeine Finanzen bearbeiten**.

1. Klicken Sie auf **Speichern**.

## Finanzielle Berechtigung für alle Freigabeebenen

Die folgende Tabelle zeigt, welche Finanzberechtigungen Benutzende erhalten, wenn Sie ihnen Berechtigungen zum Anzeigen, Mitwirken oder Verwalten für Objekte erteilen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktionen</strong> </th> 
   <th><strong>Verwalten</strong> </th> 
   <th><strong>Beitragen</strong> </th> 
   <th><strong>Anzeigen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Rechnungsnachweise verwalten</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Abrechnungstarife bearbeiten</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Kostensätze bearbeiten</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Allgemeine Finanzen bearbeiten</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Abrechnungstarife anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Kostensätze anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Allgemeine Finanzen anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Informationen nach Kosten in den Ressourcenplanungs-Tools anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Budgetressourcen in den Tools für die Ressourcenplanung*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Ressourcen in den Ressourcenplanungs-Tools anzeigen*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Erfordert zusätzlichen Zugriff auf die Ressourcenverwaltung.

Informationen zum Zugriff auf die Ressourcenverwaltung finden Sie unter [Zugriff auf die Ressourcenverwaltung gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
