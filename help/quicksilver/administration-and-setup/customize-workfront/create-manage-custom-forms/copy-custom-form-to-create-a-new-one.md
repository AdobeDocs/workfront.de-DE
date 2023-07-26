---
user-type: administrator
product-area: system-administration
keywords: create,custom,form,copy,base,another
navigation-topic: create-and-manage-custom-forms
title: Kopieren Sie ein benutzerdefiniertes Formular, um ein neues mit dem alten Builder zu erstellen
description: Sie können ein neues benutzerdefiniertes Formular erstellen, das auf einem vorhandenen basiert.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Kopieren Sie ein benutzerdefiniertes Formular, um ein neues mit dem alten Builder zu erstellen

Sie können ein neues benutzerdefiniertes Formular erstellen, das auf einem vorhandenen basiert.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Kopieren Sie ein benutzerdefiniertes Formular, um ein neues zu erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicks **Benutzerdefinierter Forms.**
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie als Grundlage für ein neues benutzerdefiniertes Formular verwenden möchten, und klicken Sie dann auf **Kopieren**.
1. Im **Benutzerdefinierte Formularkopie** Geben Sie die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Formularname</td> 
      <td>Geben Sie einen Namen für das kopierte Formular ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Formulartypen </p> </td> 
      <td> <p>Im <b>Formulartyp</b> Wählen Sie die Objekttypen aus, mit denen das benutzerdefinierte Formular verwendet werden soll, und klicken Sie auf das X neben allen Typen, die Sie entfernen möchten. Typen, die bereits mit dem Formular verknüpft sind, sind in der Liste deaktiviert.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>Das Formular muss mindestens einem Objekttyp zugeordnet sein.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Formular kopieren**.

   Wenn berechnete Felder im Originalformular auf Felder verweisen, die nicht mit einem Objekttyp kompatibel sind, den Sie dem neuen Formular hinzufügen, werden Sie aufgefordert, die Berechnungen in diesen Feldern zu ändern.

   Wenn eine Zugriffsoption für einen Abschnittsumbruch im Originalformular nicht mit einem Objekttyp kompatibel ist, den Sie zum neuen hinzufügen, werden Sie in einer Meldung aufgefordert, die Option anzupassen.

1. Wählen Sie das soeben kopierte Formular aus und klicken Sie auf **Bearbeiten**.
1. Nehmen Sie Änderungen am Formular vor, wie in den folgenden Artikeln beschrieben:

   * [Kopieren Sie ein benutzerdefiniertes Formular, um ein neues mit dem alten Formular-Builder zu erstellen](#Add2)
   * [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Positionieren Sie benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular mit dem Legacy-Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Verwenden Sie ein vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular mit dem alten Formular-Builder erneut.](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Fügen Sie mit dem alten Formular-Builder Logik hinzu und überspringen Sie Logik zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Erstellen Sie eine Vorschau und füllen Sie ein benutzerdefiniertes Formular mit dem alten Formular-Builder aus.](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Optional) Nachdem Sie auf **Speichern+Schließen**, fügen Sie das Formular an das Objekt an, in dem Sie es verwenden möchten, wie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
