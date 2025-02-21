---
title: Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn Sie einem benutzerdefinierten Formular ein neues benutzerdefiniertes Feld oder Widget hinzufügen, kann standardmäßig jeder Benutzer im System, der Zugriff auf benutzerdefinierte Formulare hat, die Eigenschaften für dieses Element bearbeiten, z. B. seine Beschriftung und seinen Namen. Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '1096'
ht-degree: 1%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets

Wenn Sie einem benutzerdefinierten Formular ein neues benutzerdefiniertes Feld oder Widget hinzufügen, kann standardmäßig jeder Benutzer im System, der Zugriff auf benutzerdefinierte Formulare hat, die Eigenschaften für dieses Element bearbeiten, z. B. seine Beschriftung und seinen Namen. Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets aus der Formularliste

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Klicken Sie auf **Felder**, um den Bereich Felder zu öffnen.
1. Wählen Sie das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf ![Freigabesymbol](assets/share-icon.png).
1. Geben Sie im nun angezeigten Feld Zugriff auf benutzerdefiniertes Feld an, für wen Sie das Element freigeben möchten und wie Sie es freigeben möchten:

   1. Beginnen Sie in der linken unteren Ecke des Felds **Zugriff auf benutzerdefinierte Felder** unter **Zugriff auf benutzerdefinierte Felder erteilen** mit der Eingabe des Namens eines Benutzers, Teams, Aufgabengebiets, einer Gruppe oder eines Unternehmens, für den bzw. die Sie das Element freigeben möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.

      ![Benutzerdefiniertes Feld - Zugriffsfeld](assets/share-field-give-access-to.jpg)

   1. Wenn Sie detaillierter festlegen möchten, wie Sie das Element freigeben möchten, klicken Sie auf die Dropdown-Liste rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

      ![Freigabeoptionen](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Anzeigen</td> 
         <td> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um anzugeben, ob die Benutzenden oder die Benutzenden ihren Zugriff nutzen können sollen, um das Element zu einem benutzerdefinierten Formular hinzuzufügen oder es für andere Benutzende freizugeben.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Verwalten</td> 
         <td> <p>Ermöglicht den Zugriff auf die Bearbeitung des benutzerdefinierten Felds und dessen Anzeige in der Feldbibliothek sowie auf der Seite, auf der Sie benutzerdefinierte Formulare erstellen.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um anzugeben, ob die Benutzenden oder die Benutzenden ihren Zugriff nutzen können sollen, um das Element aus dem System zu löschen oder es für andere Benutzende freizugeben.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Namen zur Liste hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie auf das Zahnradsymbol ![Einstellungssymbol](assets/gear-icon-settings.png) in der oberen rechten Ecke, wenn Sie eine systemweite Freigabeoption für das Feld auswählen möchten.

   Nicht alle der folgenden Optionen werden in diesem Dropdown-Menü gleichzeitig angezeigt. Die zweite wird beispielsweise nur angezeigt, wenn eine der beiden anderen ausgewählt ist.

   * **Machen Sie diese systemweit bearbeitbar, sodass sie jeder in Workfront bearbeiten kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe dafür nicht einschränken, kann jeder im System, der Zugriff auf benutzerdefinierte Formulare hat, es anzeigen und seine Eigenschaften bearbeiten.

   * **Systemweiten Bearbeitungszugriff entfernen**

     Beschränkt den Zugriff nur auf diejenigen, die Sie der Liste hinzugefügt haben.

   * **Machen Sie dies systemweit sichtbar, sodass jeder in Workfront es sehen kann**

1. Klicken Sie auf **Speichern**.

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets im Formular-Designer

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms**.
1. Ein benutzerdefiniertes Formular öffnen oder ein neues benutzerdefiniertes Formular erstellen.
1. Wählen Sie im Formular-Designer das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann **rechts im Bereich zur Feldbearbeitung auf** Freigeben.
1. Beginnen Sie in dem angezeigten Feld unter **Zugriff auf benutzerdefinierte Formulare gewähren** mit der Eingabe des Namens des Benutzers, Teams, Aufgabengebiets, der Gruppe oder des Unternehmens, für den bzw. die Sie das Element freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Wenn Sie genauer sagen möchten, wie Sie das Element freigeben, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Anzeigen</td> 
        <td> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob die Benutzer das Element zu einem benutzerdefinierten Formular hinzufügen oder für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Verwalten</td> 
        <td> <p>Ermöglicht den Zugriff auf die Bearbeitung des benutzerdefinierten Felds und dessen Anzeige sowohl in der Feldbibliothek als auch im Formular-Designer.</p> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob die Benutzer das Element aus dem System löschen oder für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Wählen Sie eine systemweite Freigabeoption für das Feld aus:

   * **Jeder Benutzer im System kann bearbeiten** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe dafür nicht einschränken, kann jeder im System, der Zugriff auf benutzerdefinierte Formulare hat, es anzeigen und seine Eigenschaften bearbeiten.

   * **Jeder im System kann Folgendes anzeigen**
   * **Nur eingeladene Personen können darauf zugreifen**

     Beschränkt den Zugriff nur auf die, die Sie der Liste hinzugefügt haben.

   ![Freigabeoptionen](assets/share-field-in-designer.png)

1. Klicken Sie auf **Speichern**.

## geerbter Zugriff auf benutzerdefinierte Felder und Widgets, wenn ein benutzerdefiniertes Formular freigegeben wird

Wenn jemand ein benutzerdefiniertes Formular für eine Gruppe, ein Aufgabengebiet, ein Team oder eine Firma freigibt, erben die Empfänger den Ansichtszugriff auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, vorgesehen funktionieren kann. Dies gilt auch für Empfänger, die Bearbeitungszugriff auf das Formular haben.

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

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt [Entfernen des Zugriffs auf ein benutzerdefiniertes Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) im Artikel [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
