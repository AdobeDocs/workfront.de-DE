---
title: Objektüberschriften mithilfe einer Layoutvorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Felder zu konfigurieren, die Benutzern beim Öffnen einer Objektseite in der Objektüberschrift angezeigt werden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Objektüberschriften mithilfe einer Layoutvorlage anpassen

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Felder zu konfigurieren, die Benutzern beim Öffnen einer Objektseite in der Objektüberschrift angezeigt werden.

>[!IMPORTANT]
>
>Das Anpassen von Objektüberschriften ist derzeit für Projekte, Aufgaben und Probleme verfügbar.

![](assets/object-header-fields.png)

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:


<table>
  <tr>
   <td><strong>Adobe Workfront-Abo</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenz</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen auf Zugriffsebene</strong>
   </td>
   <td>Sie müssen ein Workfront- oder Gruppenadministrator sein.
<p>
   </td>
  </tr>
</table>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## Objektüberschriften anpassen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Im **Anpassen der Ansicht von Benutzern** Dropdown-Menü auswählen **Projekte**, **Aufgaben** oder **Probleme**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. Im [!UICONTROL Kopfzeilenfelder] -Bereich, bewegen Sie den Mauszeiger über die angezeigten Felder und führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf **x** Symbol zum Entfernen eines Felds

     Oder

   * Klicken Sie auf und halten Sie die **Grab** -Symbol, um das Feld an eine neue Position zu ziehen.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Sie können bis zu fünf Felder in der Kopfzeile eines Objekts haben.
Wenn Sie bereits fünf Felder ausgewählt haben, müssen Sie ein Feld entfernen, bevor Sie ein neues hinzufügen können.
1. Im **Feld hinzufügen** Geben Sie den Namen eines nicht bearbeitbaren Workfront-Felds ein, das Sie hinzufügen möchten, und wählen Sie es dann aus, wenn es in der Liste angezeigt wird. Das Feld wird direkt rechts neben dem Feld Feld hinzufügen hinzugefügt und wird als erstes Feld in der oberen linken Ecke der Kopfzeile des Objekts angezeigt.

   >[!TIP]
   >
   >* Sie können nur Felder hinzufügen, die im Bereich Übersicht des Bereichs Details des Objekts angezeigt werden und nicht bearbeitbar sind. Nicht bearbeitbare Felder sind Felder, die Benutzer nicht manuell bearbeiten können. Sie werden automatisch von Workfront berechnet.
   >
   >* Sie können bearbeitbare Felder hinzufügen, die bereits Teil der Standardkopfzeilen sind (z. B. Projekteigentümer, Status, Prozentsatz abgeschlossen, Zuweisungen).
   >
   >* Wenn Sie das Feld &quot;Gelöst von&quot;zur Kopfzeile eines Problems hinzufügen, ändert sich das Feld in &quot;Beheben von Problemen, Aufgaben oder Projekten&quot;, wenn mit dem Problem ein auflösendes Objekt verknüpft ist.


   ![](assets/add-field-to-header-in-lt-list.png)


1. (Optional) Ziehen Sie die hinzugefügten Felder in eine andere Reihenfolge per Drag-and-Drop.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.
