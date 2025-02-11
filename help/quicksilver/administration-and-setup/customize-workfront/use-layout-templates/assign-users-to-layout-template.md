---
title: Zuweisen von Benutzern zu einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie eine von Ihnen erstellte Layout-Vorlage allen Benutzenden, Aufgabengebieten, Teams oder Gruppen zuweisen, die sie verwenden müssen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# Zuweisen von Benutzern zu einer Layout-Vorlage

Sie können eine von Ihnen erstellte Layout-Vorlage allen Benutzern, Aufgabengebieten, Teams oder Gruppen zuweisen, die sie verwenden müssen.

Benutzenden, denen keine Layout-Vorlage zugewiesen ist, wird das Standard-Layout verwendet. Weitere Informationen zum Standard-Layout finden Sie unter [Über das Standard-Adobe Workfront-Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Benutzer können sich auch selbst eine Layout-Vorlage zuweisen, wie unter Ändern der Bereiche Meine Arbeit und Arbeitsanfragen mit Layout-Vorlagen beschrieben.

Sie können demselben Namen mehrere verschiedene Layout-Vorlagen zuweisen. Weitere Informationen dazu, welche Layout-Vorlage für einen Benutzer, eine Rolle, eine Gruppe oder ein Team aktiv ist, finden Sie [Zuweisungspriorität für Layout-Vorlagen](#layout-template-assignment-priority) weiter unten in diesem Artikel.

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zuweisen einer Layout-Vorlage zu Benutzern

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.

   >[!TIP]
   >
   >Wenn Sie mit der Layout-Vorlage zufrieden sind, empfehlen wir, sie zu testen, wie in [Testen einer neuen Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md) beschrieben.

1. Klicken **im oberen** der Seite auf „Zuweisen zu“.
1. Klicken Sie im angezeigten Feld auf **Benutzer, Aufgabengebiet, Team oder Gruppe hinzufügen**, geben Sie den Namen eines Benutzers, Aufgabengebiets, Teams oder einer Gruppe ein und klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Kürzlich hinzugefügte Namen werden mit blauem Hintergrund angezeigt. Dies ist hilfreich, wenn Sie eine vorhandene Layout-Vorlage bearbeiten, da Sie die soeben hinzugefügten Namen von den bereits in der Liste vorhandenen unterscheiden können.

   Rechts neben dem Namen eines Benutzers![ eines Aufgabengebiets, Teams oder einer Gruppe, ](assets/info-icon.png) bereits einer anderen Layout-Vorlage zugewiesen ist, wird ein Infosymbol (Infosymbol) angezeigt. Sie können den Mauszeiger über das Symbol bewegen, um den Namen dieser Layout-Vorlage anzuzeigen und zu entscheiden, ob Sie die vorhandene Zuweisung überschreiben möchten.

1. Wiederholen Sie die beiden vorherigen Schritte, um die Layout-Vorlage ggf. anderen Benutzern, Aufgabengebieten, Teams oder Gruppen zuzuweisen.

   Sie können bis zu 100 Benutzer gleichzeitig zuweisen.

1. Klicken Sie **Fertig** und dann unten links auf **Speichern**.

   Dieser Schritt schließt den Prozess der Erstellung und Zuweisung einer Layout-Vorlage ab.

## Zuweisungspriorität der Layoutvorlage {#layout-template-assignment-priority}

Sie und andere Workfront-Admins können demselben Benutzenden auf vier verschiedene Arten mehrere verschiedene Layout-Vorlagen zuweisen:

* An den einzelnen Benutzer
* Einem bestimmten Aufgabengebiet zuweisen, das der Benutzer hat
* Für ein bestimmtes Team ist der Benutzer aktiv.
* Für eine bestimmte Gruppe ist der Benutzer in

Es ist jedoch immer nur eine Layoutvorlage für den Benutzer sichtbar. Die sichtbare Vorlage wird durch die folgende Prioritätshierarchie bestimmt:

* **Einzelner Benutzer**: Die Layout-Vorlage, die der Person als einzelner Benutzer zugewiesen ist, überschreibt alle anderen. Sie können eine frühere Zuweisung überschreiben, die für einen einzelnen Benutzer vorgenommen wurde, indem Sie eine neue Zuweisung vornehmen. Die neueste Zuweisung hat Vorrang.
* **Primäres Aufgabengebiet**: Wenn der Person keine Layout-Vorlage als Einzelperson zugewiesen ist, wird ihr die Vorlage für ihr primäres Aufgabengebiet zugewiesen.

  Nur die Layout-Vorlage, die dem primären Aufgabengebiet eines Benutzers zugewiesen ist, ist für den Benutzer sichtbar. Vorlagen, die sekundären Aufgabengebieten zugewiesen wurden, die vom Benutzer verwaltet werden, sind nicht sichtbar.

* **Home-Team**: Wenn der Person keine Layout-Vorlage als einzelner Benutzer oder als Benutzer mit einem primären Aufgabengebiet zugewiesen ist, wird ihr die Vorlage angezeigt, die ihrem Home-Team zugewiesen ist.

  Nur die Vorlage, die dem Home-Team eines Benutzers zugewiesen ist, ist für den Benutzer sichtbar. Vorlagen, die anderen Teams zugewiesen wurden, bei denen ein Benutzer Mitglied ist, sind nicht sichtbar.

* **Hauptgruppe**: Wenn der Person keine Layout-Vorlage als einzelner Benutzer, als Benutzer mit einem primären Aufgabengebiet oder als Mitglied eines Haupt-Teams zugewiesen ist, wird die Vorlage angezeigt, die ihrer Hauptgruppe zugewiesen ist.

  Nur die Vorlage, die der Hauptgruppe eines Benutzers zugewiesen ist, ist für den Benutzer sichtbar. Vorlagen, die einer der anderen Gruppen zugewiesen sind, sind nicht sichtbar.

## Große Anzahl von Benutzern, die einer Layout-Vorlage zugewiesen sind

Wenn Sie eine Layout-Vorlage bearbeiten, die mehr als 2.000 Benutzern zugewiesen ist, und Änderungen daran vornehmen, werden nur die ersten 2.000 Benutzer in der Layout-Vorlage beibehalten und die von Ihnen vorgenommenen Änderungen sehen. Die Layout-Vorlage wird aus allen anderen Vorlagen entfernt.

Wenn Sie einer Layout-Vorlage mehr als 2.000 Benutzer zuweisen müssen, empfehlen wir eine der folgenden Aktionen:

* Organisieren Sie die Benutzer in Gruppen oder Teams und weisen Sie diesen Gruppen oder Teams die Layout-Vorlage zu. Weitere Informationen finden Sie unter [Gruppe erstellen](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) und [Teams erstellen und verwalten](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Weisen Sie den Benutzern Aufgabengebiete zu und weisen Sie die Layout-Vorlage ihrem primären Aufgabengebiet zu. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
