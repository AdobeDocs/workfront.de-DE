---
title: Zuweisen von Benutzern zu einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie einer beliebigen Benutzer, Rolle, Gruppe oder Gruppe, die diese Vorlage verwenden möchten, eine von Ihnen erstellte Layoutvorlage zuweisen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# Benutzer einer Layoutvorlage zuweisen

Sie können eine von Ihnen erstellte Layoutvorlage jedem Benutzer, jeder Auftragsrolle, jedem Team oder jeder Gruppe zuweisen, der/die sie verwenden muss.

Für Benutzer, denen keine Layoutvorlage zugewiesen ist, wird das Standardlayout verwendet. Weitere Informationen zum Standardlayout finden Sie unter [Über das standardmäßige Adobe Workfront-Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Benutzer können sich auch eine Layoutvorlage zuweisen, wie unter Die Bereiche Meine Arbeit und Arbeitsanforderungen mit Layoutvorlagen ändern beschrieben.

Sie können mehrere verschiedene Layoutvorlagen demselben Namen zuweisen. Weitere Informationen dazu, welche Layoutvorlage für einen Benutzer, eine Rolle, eine Gruppe oder ein Team aktiv ist, finden Sie weiter unten in diesem Artikel unter [Priorität der Layoutvorlagenzuweisung](#layout-template-assignment-priority) .

Weitere Informationen zu Layoutvorlagen finden Sie unter [Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzern eine Layoutvorlage zuweisen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.

   >[!TIP]
   >
   >Wenn Sie mit Ihrer Layoutvorlage zufrieden sind, empfehlen wir Ihnen, diese zu testen, wie unter [Testen einer neuen Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md) beschrieben.

1. Klicken Sie im oberen Abschnitt der Seite auf **Zuweisen zu** .
1. Klicken Sie in dem angezeigten Feld auf &quot;**Benutzer, Auftragsrolle, Team oder Gruppe hinzufügen&quot;**&quot;, geben Sie den Namen eines Benutzers, einer Auftragsrolle, eines Teams oder einer Gruppe ein und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Kürzlich hinzugefügte Namen werden mit blauem Hintergrund angezeigt. Dies ist hilfreich, wenn Sie eine vorhandene Layoutvorlage bearbeiten, da Sie die Namen, die Sie gerade hinzugefügt haben, von denen unterscheiden können, die sich bereits in der Liste befanden.

   Rechts neben dem Namen eines Benutzers, einer Rolle, eines Teams oder einer Gruppe, dem/der bereits eine andere Layoutvorlage zugewiesen ist, wird das Info-Symbol ![](assets/info-icon.png) angezeigt. Sie können den Mauszeiger über das Symbol bewegen, um den Namen dieser Layoutvorlage anzuzeigen und zu entscheiden, ob Sie die vorhandene Zuweisung überschreiben möchten.

1. Wiederholen Sie die beiden vorherigen Schritte, um die Layoutvorlage anderen Benutzern, Auftragsrollen, Teams oder Gruppen nach Bedarf zuzuweisen.

   Sie können bis zu 100 Benutzer gleichzeitig zuweisen.

1. Klicken Sie auf **Fertig** und dann unten links auf **Speichern** .

   Dieser Schritt schließt die Erstellung und Zuweisung einer Layoutvorlage ab.

## Priorität der Zuweisung von Layout-Vorlagen {#layout-template-assignment-priority}

Sie und andere Workfront-Administratoren können demselben Benutzer auf vier verschiedene Arten verschiedene Layoutvorlagen zuweisen:

* An den einzelnen Benutzer
* Für eine bestimmte Rolle des Benutzers
* Für ein bestimmtes Team ist der Benutzer aktiviert
* Für eine bestimmte Gruppe ist der Benutzer

Es ist jedoch immer nur eine Layout-Vorlage für den Benutzer sichtbar. Die angezeigte Vorlage wird durch die folgende Prioritätshierarchie bestimmt:

* **Individueller Benutzer**: Die Layout-Vorlage, die der Person als einzelner Benutzer zugewiesen wurde, setzt alle anderen außer Kraft. Sie können eine vorherige Zuweisung, die für einen einzelnen Benutzer vorgenommen wurde, überschreiben, indem Sie eine neue Zuweisung vornehmen. Die neueste Zuweisung hat Vorrang.
* **Primäre Auftragsrolle**: Wenn der Person keine Layoutvorlage als Einzelbenutzer zugewiesen wurde, wird ihnen die Vorlage angezeigt, die für ihre primäre Auftragsrolle zugewiesen ist.

  Nur die Layout-Vorlage, die der Rolle &quot;Hauptauftrag&quot;eines Benutzers zugewiesen ist, ist für den Benutzer sichtbar. Vorlagen, die sekundären, vom Benutzer gespeicherten Auftragsrollen zugewiesen wurden, sind nicht sichtbar.

* **Home team**: Wenn der Person weder als einzelner Benutzer noch als Benutzer mit der Rolle &quot;primärer Job&quot;eine Layoutvorlage zugewiesen wurde, wird ihnen die ihrem Home-Team zugewiesene Vorlage angezeigt.

  Nur die Vorlage, die dem Home-Team eines Benutzers zugewiesen wurde, ist für den Benutzer sichtbar. Für andere Teams zugewiesene Vorlagen, denen ein Benutzer angehört, sind nicht sichtbar.

* **Home group**: Wenn der Person weder eine Layoutvorlage als einzelner Benutzer, noch als Benutzer mit der Rolle &quot;primärer Job&quot;oder als Mitglied eines Home-Teams zugewiesen wird, sehen sie die Vorlage, die ihrer Home-Gruppe zugewiesen ist.

  Nur die Vorlage, die der Gruppe Startseite eines Benutzers zugewiesen ist, ist für den Benutzer sichtbar. Vorlagen, die einer ihrer anderen Gruppen zugewiesen sind, sind nicht sichtbar.

## Große Anzahl von Benutzern, die einer Layoutvorlage zugewiesen sind

Wenn Sie eine Layout-Vorlage bearbeiten, die mehr als 2000 Benutzern zugewiesen ist, und Änderungen daran vornehmen, werden nur die ersten 2000 Benutzer in der Layoutvorlage beibehalten und die vorgenommenen Änderungen angezeigt. Die Layout-Vorlage wird von allen anderen entfernt.

Wenn Sie mehr als 2000 Benutzer einer Layoutvorlage zuweisen müssen, empfehlen wir, einen der folgenden Schritte auszuführen:

* Organisieren Sie die Benutzer in Gruppen oder Teams und weisen Sie diesen Gruppen oder Teams die Layoutvorlage zu. Weitere Informationen finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Erstellen und Verwalten von Teams](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Weisen Sie den Benutzern Vorgangsrollen zu und weisen Sie ihnen die Layoutvorlage ihrer primären Auftragsrolle zu. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
