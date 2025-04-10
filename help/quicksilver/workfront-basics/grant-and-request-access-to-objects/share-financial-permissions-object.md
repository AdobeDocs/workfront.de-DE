---
title: Freigeben von Finanzberechtigungen für ein Objekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Finanzdaten gewähren. Weitere Informationen finden Sie unter Gewähren des Zugriffs auf Finanzdaten.
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 1%

---

# Freigeben von Finanzberechtigungen für ein Objekt

Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Finanzdaten gewähren. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten der Finanzen für bestimmte Projekte, Aufgaben oder Probleme erteilen, auf die Sie Zugriff haben.

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Finanzdaten tun können, finden Sie im Abschnitt [Finanzdaten](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriffsanforderungen

<!--drafted for P&P:

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
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.
Sie müssen über Folgendes verfügen, um Finanzdaten zu Objekten freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme und Finanzdaten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für Projekte, Aufgaben und Probleme, die mindestens „Finanzen anzeigen“-Berechtigungen enthalten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Objekt freigeben und finanzielle Berechtigungen erteilen

Beachten Sie Folgendes, wenn Sie Objekten Finanzberechtigungen erteilen:

* Sie können Projekten, Aufgaben und Problemen finanzielle Berechtigungen erteilen.
* Berechtigungen können vererbt werden: Wenn Sie über Anzeigefinanzierungsberechtigungen für ein Projekt verfügen, übernehmen Sie automatisch die Anzeigefinanzierungsberechtigungen für die Aufgaben und Probleme im Projekt.

So erteilen Sie einem Objekt finanzielle Berechtigungen:

1. Wechseln Sie zu einer Aufgabe, einem Projekt oder einem Problem, die/das Sie für andere freigeben möchten.
1. Klicken Sie in der Nähe des Objektnamens auf die ![](assets/more-icon.png) Mehr und dann auf **Freigabe**.

1. Geben **im Feld `<Object name>` Zugriff auf** den Namen eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens ein, für den bzw. die Sie das Objekt freigeben möchten.

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Wenn rechts neben dem ausgewählten Namen ein Dropdown-Menü angezeigt wird, klicken Sie auf eine der folgenden verfügbaren Optionen:

   * **Anzeigen**
   * **Mitwirken**
   * **Verwalten**

1. Klicken Sie im gleichen Dropdown-Menü auf **Erweiterte Einstellungen** und führen Sie dann einen der folgenden Schritte aus:

   * Wenn Sie im vorherigen Schritt eine der drei Optionen ausgewählt haben, stellen Sie sicher, dass **Finanzen anzeigen** ausgewählt ist.
   * Wenn Sie im vorherigen Schritt **Finanzen verwalten** ausgewählt haben, stellen Sie sicher, dass **Finanzen verwalten** ausgewählt ist.

1. Klicken Sie auf **Speichern**.

## Finanzielle Berechtigung für alle Freigabeebenen

Die folgende Tabelle zeigt, welche finanziellen Berechtigungen Benutzende erhalten, wenn Sie ihnen Berechtigungen zum Anzeigen, Mitwirken oder Verwalten für Objekte erteilen: 

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
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Funktionsbezogene Fakturierung und Kostensätze verwalten/anzeigen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzerfakturierung und Kostensätze verwalten/anzeigen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Finanzen anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
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
   <td> </td> 
   <td> </td> 
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
