---
title: Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn Sie einem benutzerdefinierten Formular ein neues benutzerdefiniertes Feld oder Widget hinzufügen, kann standardmäßig jeder im System, der Zugriff auf benutzerdefinierte Formulare hat, die Eigenschaften für dieses Element bearbeiten, z. B. seinen Titel und API-Namen. Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1eda36eb74aca2b731f2632eac3aae60e6b8ef9d
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 5%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets

Wenn Sie einem benutzerdefinierten Formular ein neues benutzerdefiniertes Feld oder Widget hinzufügen, kann standardmäßig jeder im System, der Zugriff auf benutzerdefinierte Formulare hat, die Eigenschaften für dieses Element bearbeiten, z. B. seinen Titel und API-Namen. Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Freigeben aus der Liste von Formularen und Feldern:

   1. Klicken Sie auf **Felder**, um den Bereich Felder zu öffnen.
   1. Wählen Sie das Feld aus, das Sie freigeben möchten, und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).

1. Freigeben über den Formular-Designer:
   1. Ein benutzerdefiniertes Formular öffnen oder ein neues benutzerdefiniertes Formular erstellen.
   1. Wählen Sie im Formular-Designer das Feld aus, das Sie freigeben möchten, und klicken Sie dann **rechts im Bereich zur Feldbearbeitung auf** Freigeben.

1. Beginnen Sie im Freigabefeld unter **Zugriff gewähren auf** mit der Eingabe des Namens des Benutzers, Teams, Aufgabengebiets, der Gruppe, des Unternehmens oder des Geschäftsprofils, für den Sie das Element freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Wenn Sie genauer sagen möchten, wie Sie das Element freigeben, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

   * **Anzeigen**: Klicken Sie auf das Symbol **Erweiterte Einstellungen** ![Symbol „Erweiterte Einstellungen“](assets/configure-options-icon.png), um anzugeben, ob die Benutzer das Element zu einem benutzerdefinierten Formular hinzufügen oder für andere Benutzer freigeben können sollen.
   * **Verwalten**: Ermöglicht den Zugriff auf die Bearbeitung des benutzerdefinierten Felds und dessen Anzeige sowohl in der Feldbibliothek als auch im Formular-Designer. Klicken Sie auf **Symbol** Erweiterte Einstellungen![, ](assets/configure-options-icon.png) anzugeben, ob die Benutzer das Element aus dem System löschen oder für andere Benutzer freigeben können sollen.

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Wählen Sie eine systemweite Freigabeoption für das Feld aus:

   * **Jeder Benutzer im System kann bearbeiten** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe dafür nicht einschränken, kann jeder im System, der Zugriff auf benutzerdefinierte Formulare hat, es anzeigen und seine Eigenschaften bearbeiten.

   * **Jeder im System kann Folgendes anzeigen**

     Alle Personen im System, die Zugriff auf benutzerdefinierte Formulare haben, können das Feld anzeigen, es jedoch nicht bearbeiten.

   * **Nur eingeladene Personen können darauf zugreifen**

     Beschränkt den Zugriff nur auf die, die Sie der Liste hinzugefügt haben.

   ![Freigabeoptionen](assets/share-field-in-designer.png)

1. Klicken Sie auf **Speichern**.

## geerbter Zugriff auf benutzerdefinierte Felder und Widgets, wenn ein benutzerdefiniertes Formular freigegeben wird

Wenn jemand ein benutzerdefiniertes Formular für eine Gruppe, ein Aufgabengebiet, ein Team, eine Firma oder ein Geschäftsprofil freigibt, erben die Empfänger den Ansichtszugriff auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, vorgesehen funktionieren kann. Dies gilt auch für Empfänger, die Bearbeitungszugriff auf das Formular haben.

Sie können ermitteln, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget geerbt hat, und den Zugriff darauf entfernen.

>[!NOTE]
>
>Wenn ein Empfänger Verwaltungszugriff auf ein benutzerdefiniertes Feld oder Widget im freigegebenen benutzerdefinierten Formular hat, wird dieser Zugriff für den Empfänger beibehalten.

### Finden Sie heraus, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget geerbt hat {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Klicken Sie **Felder** und wählen Sie dann das Widget „Feld“, „Bild“ oder „Zugriff“ aus.
1. Klicken Sie in dem angezeigten Feld auf **Vererbte Berechtigungen** und zeigen Sie die angezeigten Namen an.
1. Klicken Sie **Abbrechen**.

### Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt [Entfernen des Zugriffs auf ein benutzerdefiniertes Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form) im Artikel [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).


