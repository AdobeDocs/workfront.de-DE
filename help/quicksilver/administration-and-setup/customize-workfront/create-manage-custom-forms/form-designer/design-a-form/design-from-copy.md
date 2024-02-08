---
title: Entwerfen eines Formulars aus einer Kopie mit dem Formularentwickler
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular aus einer Kopie mit dem Formularentwickler entwerfen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 9cdafc6a38a8b2b2dd337c695ba01d54515b00e5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Entwerfen eines Formulars aus einer Kopie mit dem Formularentwickler

{{highlighted-preview}}

Sie können ein neues benutzerdefiniertes Formular entwerfen, das auf einem vorhandenen basiert. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten zu diesen Objekten zu erfassen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Kopieren Sie ein benutzerdefiniertes Formular, um ein neues zu erstellen

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierter Forms.**
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie als Grundlage für ein neues benutzerdefiniertes Formular verwenden möchten, und klicken Sie dann auf **Kopieren** <span class="preview">oder ![Kopiersymbol](assets/copy-icon.png).</span>
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

1. Wählen Sie das soeben kopierte Formular aus und klicken Sie auf **Bearbeiten** <span class="preview">oder ![Symbol Bearbeiten](assets/edit-icon.png).</span>
1. Nehmen Sie Änderungen am Formular vor, wie in den folgenden Abschnitten des [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) Artikel:

   * [Vorhandenes Feld oder Widget in einem anderen benutzerdefinierten Formular wiederverwenden](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [Textfelder hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [Berechnete Felder hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [Optionsfelder, Kontrollkästchengruppen und Dropdown-Listen hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [Typevorschau- und Datumsfelder hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [Bilder, PDF und Videos hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [Hinzufügen von Adobe XD-Dateien](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Optional) Nachdem Sie auf **Speichern+Schließen**, fügen Sie das Formular an das Objekt an, in dem Sie es verwenden möchten, wie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
