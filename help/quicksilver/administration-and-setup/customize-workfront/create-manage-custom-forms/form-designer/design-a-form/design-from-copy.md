---
title: Erstellen eines Formulars aus einer Kopie
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Mit dem Formular-Designer können Sie ein benutzerdefiniertes Formular aus einer Kopie erstellen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
TQID: https://experienceleague.adobe.com/WaLGsLpGDMXGvNd7W-8JzmgJYiCaxSd-gaMoGy6j-Zc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 3e77f50ee2297a9c552e27bfcdf7f08a6a4c89b5
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 24%

---

# Erstellen eines Formulars aus einer Kopie

Sie können ein neues benutzerdefiniertes Formular entwerfen, das auf einem vorhandenen Formular basiert. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten zu diesen Objekten zu erfassen.

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

## Kopieren eines benutzerdefinierten Formulars, um ein neues zu erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **Benutzerdefinierte Forms.**
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie als Grundlage für ein neues benutzerdefiniertes Formular verwenden möchten, und klicken Sie dann auf ![Kopiersymbol](assets/copy-icon.png).
1. Geben Sie **Feld „Benutzerdefinierte**&quot; die folgenden Informationen ein:

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
      <td> <p>Wählen Sie im Feld <b>Formulartyp</b> die Objekttypen aus, mit denen das benutzerdefinierte Formular arbeiten soll, und klicken Sie auf das X neben den Typen, die Sie entfernen möchten. Typen, die bereits mit dem Formular verknüpft sind, sind in der Liste deaktiviert.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>Das Formular muss mit mindestens einem Objekttyp verknüpft sein.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Kopieren**.

   Wenn im ursprünglichen Formular berechnete Felder auf Felder verweisen, die mit einem Objekttyp inkompatibel sind, den Sie dem neuen Formular hinzufügen, werden Sie in einer Meldung aufgefordert, die Berechnungen in diesen Feldern zu ändern.

   Wenn eine Zugriffsoption für einen Abschnittsumbruch im ursprünglichen Formular nicht mit einem Objekttyp kompatibel ist, den Sie dem neuen hinzufügen, werden Sie in einer Meldung aufgefordert, die Option anzupassen.

1. Wählen Sie das soeben kopierte Formular aus und klicken Sie dann auf ![Symbol „Bearbeiten](assets/edit-icon.png).
1. Nehmen Sie Änderungen am Formular vor, wie in den folgenden Abschnitten des Artikels [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) erläutert:

   * [Wiederverwenden eines vorhandenen Feldes oder Widgets, das bereits in einem anderen benutzerdefinierten Formular verwendet wurde](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Hinzufügen von Textfeldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Hinzufügen von berechneten Feldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Hinzufügen von Optionsfeldern, Kontrollkästchen-Gruppen und Dropdown-Listen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Datumsfelder hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-date-fields)
   * [Hinzufügen von Bildern, PDFs und Videos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Hinzufügen von Adobe XD-Dateien](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [Hinzufügen von Planung-Verbindungsfeldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. (Optional) Fügen Sie nach dem Klicken auf **Speichern und schließen** das Formular an das Objekt an, in dem Sie es verwenden möchten, wie in [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt“ &#x200B;](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
