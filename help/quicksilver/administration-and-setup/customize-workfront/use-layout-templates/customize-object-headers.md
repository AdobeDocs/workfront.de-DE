---
title: Objektüberschriften mithilfe einer Layout-Vorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Felder zu konfigurieren, die Benutzern beim Öffnen einer Objektseite in der Objektüberschrift angezeigt werden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Objektüberschriften mithilfe einer Layoutvorlage anpassen

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Felder zu konfigurieren, die Benutzern beim Öffnen einer Objektseite in der Objektüberschrift angezeigt werden.

>[!IMPORTANT]
>
>Das Anpassen von Objektüberschriften ist derzeit für Projekte, Aufgaben und Probleme verfügbar.

![](assets/object-header-fields.png)

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objektüberschriften anpassen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Wählen Sie im Dropdownmenü **Anpassen, was Benutzer sehen** die Option **Projekte**, **Aufgaben** oder **Probleme** aus.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Bewegen Sie im Abschnitt [!UICONTROL Kopfzeilenfelder] den Mauszeiger über die angezeigten Felder und führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf das Symbol **x** , um ein Feld zu entfernen.

     Oder

   * Klicken Sie auf das Symbol **Grab** und halten Sie es gedrückt, um das Feld an eine neue Position zu ziehen.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Sie können bis zu fünf Felder in der Kopfzeile eines Objekts haben.
Wenn Sie bereits fünf Felder ausgewählt haben, müssen Sie ein Feld entfernen, bevor Sie ein neues hinzufügen können.
1. Geben Sie im Feld **Feld hinzufügen** den Namen eines nicht bearbeitbaren Workfront-Felds ein, das Sie hinzufügen möchten, und wählen Sie es dann aus, wenn es in der Liste angezeigt wird. Das Feld wird direkt rechts neben dem Feld Feld hinzufügen hinzugefügt und wird als erstes Feld in der oberen linken Ecke der Kopfzeile des Objekts angezeigt.

   >[!TIP]
   >
   >* Sie können nur Felder hinzufügen, die im Bereich Übersicht des Bereichs Details des Objekts angezeigt werden und nicht bearbeitbar sind. Nicht bearbeitbare Felder sind Felder, die Benutzer nicht manuell bearbeiten können. Sie werden automatisch von Workfront berechnet.
   >
   >* Sie können bearbeitbare Felder hinzufügen, die bereits Teil der Standardkopfzeilen sind (z. B. Projekteigentümer, Status, Prozentsatz abgeschlossen, Zuweisungen).
   >
   >* Wenn Sie das Feld &quot;Gelöst von&quot;zur Kopfzeile eines Problems hinzufügen, ändert sich das Feld in &quot;Beheben von Problemen, Aufgaben oder Projekten&quot;, wenn mit dem Problem ein auflösendes Objekt verknüpft ist.


   ![](assets/add-field-to-header-in-lt-list.png)


1. (Optional) Ziehen Sie die hinzugefügten Felder in eine andere Reihenfolge per Drag &amp; Drop.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.
