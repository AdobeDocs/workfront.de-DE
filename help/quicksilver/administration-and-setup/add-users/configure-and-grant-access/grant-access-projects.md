---
title: Projektzugriff gewähren
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Projekte in Workfront zu definieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Projektzugriff gewähren

<!-- Audited: 12/2023 -->

Als Adobe Workfront-Administrator können Sie mithilfe einer Zugriffsebene den Zugriff eines Benutzers auf Projekte definieren, wie in den folgenden Artikeln beschrieben:
* [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)
* [Übersicht über die neuen Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)

Informationen zur Verwendung benutzerdefinierter Zugriffsebenen zur Verwaltung des Benutzerzugriffs auf andere Objekttypen in Workfront finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
  </tr>

<tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerzugriff auf Projekte mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche **Ansicht** oder **Bearbeiten** rechts neben &quot;Projekte&quot;und wählen Sie dann die Fähigkeiten aus, die Sie unter **Feinabstimmung Ihrer Einstellungen** gewähren möchten.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Benutzer mit einer Work-Lizenz verfügen über eingeschränkte Projektrechte. Sie können zu einem Projekt beitragen, aber kein Projekt verwalten.
   >* Benutzer mit einer Überprüfungslizenz haben Anzeigerechte für Projekte aus konvertierten Problemen, ihre Anzeigerechte sind jedoch eingeschränkt.
   >* Informationen zu Berechtigungen, die Benutzer beim Freigeben von Projekten für andere gewähren können, finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Wenn Sie eine Einstellung auf Zugriffsebene für einen bestimmten Objekttyp konfigurieren, wirkt sich diese Konfiguration nicht auf den Zugriff der Benutzer auf Objekte mit niedrigerem Rang aus. Sie können beispielsweise Benutzer daran hindern, Projekte auf ihrer Zugriffsebene zu löschen. Dies schränkt sie jedoch nicht vom Löschen von Aufgaben ein, die niedriger sind als Projekte. Weitere Informationen zur Objekthierarchie finden Sie im Abschnitt [Interdependenz und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optional) Klicken Sie rechts neben der Option &quot;Erstellen&quot;auf **Freigabestandardwerte festlegen** und dann auf **Regel hinzufügen** , um eine Freigaberegel für neue Projekte hinzuzufügen.

   Wenn der Benutzer mit dieser Zugriffsebene ein Projekt erstellt, wird das Projekt automatisch für die Benutzer freigegeben, die Sie im Menü auf der linken Seite auswählen.

   ![](assets/project-sharing-menu.png)

   Im Menü auf der rechten Seite geben Sie an, wie das Projekt für diese Benutzer freigegeben werden soll:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Wenn ein Benutzer mit dieser Zugriffsebene eine Projektzugriffsvorlage verwendet, setzt die Vorlage die Freigabeeinstellungen auf der Zugriffsebene außer Kraft. Weitere Informationen zu Projektzugriffsvorlagen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   Sie können diesen Schritt wiederholen, um so viele Regeln für die Projektfreigabe hinzuzufügen, wie für die Zugriffsebene erforderlich sind.

1. Klicken Sie auf das X, um das Feld **Einstellungen optimieren** zu schließen.
1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Berichte, Dashboards und Kalender nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Projekte](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Projekte

Als Eigentümer oder Ersteller eines Problems können Sie es mit anderen Benutzern teilen, indem Sie ihnen Berechtigungen erteilen, wie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) beschrieben.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp
