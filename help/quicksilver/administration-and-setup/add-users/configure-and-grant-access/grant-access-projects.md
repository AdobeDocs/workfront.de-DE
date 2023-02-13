---
title: Projektzugriff gewähren
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Projekte in Workfront zu definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Projektzugriff gewähren

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf Projekte definieren, wie hier beschrieben: [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Informationen zur Verwendung benutzerdefinierter Zugriffsebenen zur Verwaltung des Benutzerzugriffs auf andere Objekttypen in Workfront finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerzugriff auf Projekte mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie hier beschrieben: [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Ansicht** oder **Bearbeiten** auf der rechten Seite der Projekte klicken, und wählen Sie dann die Fähigkeiten aus, die Sie unter **Einstellungen anpassen**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Benutzer mit einer Work-Lizenz verfügen über eingeschränkte Projektrechte. Sie können zu einem Projekt beitragen, aber kein Projekt verwalten.
   >* Benutzer mit einer Überprüfungslizenz haben Anzeigerechte für Projekte aus konvertierten Problemen, ihre Anzeigerechte sind jedoch eingeschränkt.
   >* Informationen zu Berechtigungen, die Benutzer gewähren können, wenn sie Projekte für andere freigeben, finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Wenn Sie eine Einstellung auf Zugriffsebene für einen bestimmten Objekttyp konfigurieren, wirkt sich diese Konfiguration nicht auf den Zugriff der Benutzer auf Objekte mit niedrigerem Rang aus. Sie können beispielsweise Benutzer daran hindern, Projekte auf ihrer Zugriffsebene zu löschen. Dadurch werden sie jedoch nicht daran gehindert, Aufgaben zu löschen, die im Vergleich zu Projekten untergeordneter sind. Weiterführende Informationen zur Objekthierarchie finden Sie im Abschnitt . [Abhängigkeit und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).


1. (Optional) Klicken Sie auf **Standardwerte für die Freigabe festlegen** rechts neben der Option Erstellen und **Regel hinzufügen** , um eine Freigaberegel für neue Projekte hinzuzufügen.

   Wenn der Benutzer mit dieser Zugriffsebene ein Projekt erstellt, wird das Projekt automatisch für die Benutzer freigegeben, die Sie im Menü auf der linken Seite auswählen.

   ![](assets/project-sharing-menu.png)

   Im Menü auf der rechten Seite geben Sie an, wie das Projekt für diese Benutzer freigegeben werden soll:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Wenn ein Benutzer mit dieser Zugriffsebene eine Projektzugriffsvorlage verwendet, setzt die Vorlage die Freigabeeinstellungen auf der Zugriffsebene außer Kraft. Weitere Informationen zu Projektzugriffsvorlagen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   Sie können diesen Schritt wiederholen, um so viele Regeln für die Projektfreigabe hinzuzufügen, wie für die Zugriffsebene erforderlich sind.

1. Klicken Sie auf das X, um die **Einstellungen anpassen** ankreuzen.
1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Berichte, Dashboards und Kalender nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Projekte](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Projekte

Als Eigentümer oder Ersteller eines Problems können Sie es mit anderen Benutzern teilen, indem Sie ihnen Berechtigungen erteilen, wie hier beschrieben: [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp
