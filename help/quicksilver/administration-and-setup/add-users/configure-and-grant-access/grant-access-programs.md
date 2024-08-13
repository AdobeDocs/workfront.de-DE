---
title: Zugriff auf Programme gewähren
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf Programme in Workfront zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Zugriff auf Programme gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf Programme zu definieren, wie unter Überblick über die Zugriffsstufen [1} beschrieben.](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzerzugriff auf Programme mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche **Ansicht** oder **Bearbeiten** rechts neben &quot;Programme&quot;und wählen Sie dann die Fähigkeiten aus, die Sie unter **Feinabstimmung Ihrer Einstellungen** gewähren möchten.

   Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Programmen tun können, finden Sie im Abschnitt [Programme](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

   >[!NOTE]
   >
   >Wenn Sie eine Einstellung auf Zugriffsebene für einen bestimmten Objekttyp konfigurieren, wirkt sich diese Konfiguration nicht auf den Zugriff der Benutzer auf Objekte mit niedrigerem Rang aus. Sie können beispielsweise Benutzer daran hindern, Programme auf ihrer Zugriffsebene zu löschen. Dies schränkt sie jedoch nicht vom Löschen von Projekten ein, die schlechter platziert sind als Programme. Weitere Informationen zur Objekthierarchie finden Sie im Abschnitt [Interdependenz und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugang zu Programmen nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Programmen tun können, finden Sie im Abschnitt [Programme](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugang zu freigegebenen Programmen

Als Eigentümer oder Ersteller eines Programms können Sie es mit anderen Benutzern teilen, indem Sie ihnen Berechtigungen erteilen, wie unter [Programm freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) beschrieben.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp
