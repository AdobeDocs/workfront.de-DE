---
title: Freigeben von Finanzberechtigungen für ein Objekt
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen beim Zuweisen Ihrer Zugriffsstufe Zugriff auf die Anzeige oder Bearbeitung von Finanzdaten gewähren. Weitere Informationen finden Sie unter Zugriff auf Finanzdaten gewähren .
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Freigeben von Finanzberechtigungen für ein Objekt

{{highlighted-preview}}

Ihr Adobe Workfront-Administrator kann Ihnen beim Zuweisen Ihrer Zugriffsstufe Zugriff auf die Anzeige oder Bearbeitung von Finanzdaten gewähren. Weitere Informationen finden Sie unter [Zugriff auf Finanzdaten gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Neben der Zugriffsebene, auf die Benutzer zugreifen können, können Sie ihnen auch die Berechtigung zum Anzeigen oder Verwalten von Finanzen für bestimmte Projekte, Aufgaben oder Probleme gewähren, auf die Sie Zugriff haben.

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
Sie müssen über Folgendes verfügen, um Finanzdaten zu Objekten freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte, Aufgaben, Probleme und Finanzdaten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für Projekte, Aufgaben und Probleme, die mindestens View Finance-Berechtigungen enthalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Objekte freigeben und finanzielle Berechtigungen erteilen

Beachten Sie Folgendes bei der Erteilung von Finanzberechtigungen für Objekte:

* Sie können finanziellen Berechtigungen für Projekte, Aufgaben, Probleme, <span class="preview">und Ratenkarten</span> gewähren.
* Berechtigungen können vererbt werden: Wenn Sie über View Finance-Berechtigungen für ein Projekt verfügen, erben Sie automatisch View Finance-Berechtigungen für die Aufgaben und Probleme im Projekt.

So erteilen Sie einem Objekt finanzielle Berechtigungen:

1. Gehen Sie zu einer Aufgabe, einem Projekt oder einem Problem, die/das Sie für andere freigeben möchten.
1. Klicken Sie in der Nähe des Objektnamens auf das Menü Mehr ![](assets/more-icon.png) und dann auf **Freigabe**.

1. Geben Sie im Feld **Erteilen von `<Object name>` Zugriff auf** den Namen eines Benutzers, Teams, einer Rolle, einer Gruppe oder eines Unternehmens ein, für den/das Sie das Objekt freigeben möchten.

   >[!TIP]
   >
   >Sie können ein Objekt nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.

1. Wenn rechts neben dem ausgewählten Namen ein Dropdown-Menü angezeigt wird, klicken Sie auf eine der folgenden verfügbaren Optionen:

   * **Anzeigen**
   * **Contribute to it**
   * **Verwalten**

     ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

1. Klicken Sie im selben Dropdown-Menü auf **Erweiterte Einstellungen** und führen Sie dann einen der folgenden Schritte aus:

   * Wenn Sie eine der drei Optionen im vorherigen Schritt ausgewählt haben, stellen Sie sicher, dass **Finanzen anzeigen** ausgewählt ist.
   * Wenn Sie im vorherigen Schritt **Finanzen verwalten** ausgewählt haben, stellen Sie sicher, dass **Finanzen verwalten** ausgewählt ist.

1. Klicken Sie auf **Speichern**.

## Finanzielle Erlaubnis für alle Freigabeebenen

Die folgende Tabelle zeigt, welche finanziellen Berechtigungen Benutzer erhalten, wenn Sie ihnen Anzeige-, Contribute- oder Verwaltungsberechtigungen für Objekte erteilen: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktionen</strong> </th> 
   <th><strong>Verwalten</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>Anzeigen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Rechnungsdatensätze verwalten</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Verwalten/Anzeigen der Rollenabrechnung und der Kostensätze</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Verwalten/Anzeigen der Benutzerabrechnung und der Kostensätze</td> 
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
   <td><span class="preview">Ratenkarten verwalten</span></td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="preview">Anzeigen von Ratenkarten</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr>
  <tr> 
   <td>Anzeigen von Informationen nach Kosten in den Tools für die Ressourcenplanung</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Budgetmittel in den Tools für die Ressourcenplanung*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Anzeigen von Ressourcen in den Tools für die Ressourcenplanung*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Erfordert zusätzlichen Zugriff auf die Ressourcenverwaltung.

Informationen zum Zugriff auf die Ressourcenverwaltung finden Sie unter [Gewähren des Zugriffs auf die Ressourcenverwaltung](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
