---
title: Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 1%

---

# Konfigurieren der Freigabe für benutzerdefinierte Felder und Widgets

Wenn Sie ein neues benutzerdefiniertes Feld oder Widget zu einem benutzerdefinierten Formular hinzufügen, kann standardmäßig jeder Benutzer im System mit Zugriff auf benutzerdefinierte Formulare die Eigenschaften für dieses Element bearbeiten (z. B. Titel und Name). Sie können dies ändern, indem Sie steuern, für wen es freigegeben werden kann.

Weitere Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets aus der Formularliste

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Klicken Sie auf **Felder** , um den Bereich Felder zu öffnen.
1. Wählen Sie das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann auf das Symbol ![Freigeben](assets/share-icon.png).
1. Geben Sie im angezeigten Feld Benutzerdefinierter Feldzugriff an, für wen Sie das Element freigeben möchten und wie Sie es freigeben möchten:

   1. Geben Sie in der linken unteren Ecke des Felds **Benutzerdefinierter Feldzugriff** unter **Geben Sie benutzerdefinierten Feldzugriff auf** ein, beginnen Sie mit der Eingabe des Namens eines Benutzers, Teams, Auftrags, einer Gruppe oder eines Unternehmens, für das bzw. das Sie das Element freigeben möchten, und klicken Sie dann auf den Namen, wenn es angezeigt wird.

      ![Feld für benutzerdefinierten Feldzugriff](assets/share-field-give-access-to.jpg)

   1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben möchten, klicken Sie auf die Dropdownliste rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

      ![Freigabeoptionen](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Anzeigen</td> 
         <td> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um festzulegen, ob der Benutzer oder die Benutzer über seinen Zugriff in der Lage sein sollen, das Element zu einem benutzerdefinierten Formular hinzuzufügen oder es für andere Benutzer freizugeben.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Verwalten</td> 
         <td> <p>Ermöglicht Zugriff auf das Bearbeiten des benutzerdefinierten Felds und dessen Anzeige in der Feldbibliothek und auf der Seite, auf der Sie benutzerdefinierte Formulare erstellen.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um festzulegen, ob der Benutzer oder die Benutzer über seinen Zugriff das Element aus dem System löschen oder für andere Benutzer freigeben kann.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie oben rechts auf das Zahnradsymbol ![Einstellungssymbol](assets/gear-icon-settings.png), wenn Sie eine systemweite Freigabeoption für das Feld wählen möchten.

   Nicht alle der folgenden Optionen werden in diesem Dropdown-Menü gleichzeitig angezeigt. Beispielsweise wird die zweite nur angezeigt, wenn eine der beiden anderen ausgewählt ist.

   * **Sorgen Sie dafür, dass dieser Inhalt systemweit bearbeitet werden kann, damit er von allen Benutzern in Workfront bearbeitet werden kann** (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Entfernen des systemweiten Bearbeitungszugriffs**

     Beschränkt den Zugriff auf nur die, die Sie der Liste hinzugefügt haben.

   * **Machen Sie dies systemweit sichtbar, damit jeder in Workfront es sehen kann**

1. Klicken Sie auf **Speichern**.

## Konfigurieren der Freigabe eines benutzerdefinierten Felds oder Widgets aus dem Formularentwickler

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Öffnen Sie ein benutzerdefiniertes Formular oder erstellen Sie ein neues benutzerdefiniertes Formular.
1. Wählen Sie im Formularentwickler das Element aus, für das Sie die Freigabe konfigurieren möchten, und klicken Sie dann im Feld-Bearbeitungsbereich auf der rechten Seite auf **Freigeben** .
1. Geben Sie in dem angezeigten Feld unter **Gewähren des benutzerdefinierten Formularzugriffs auf** den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/das Sie das Element freigeben möchten, und drücken Sie dann bei der Anzeige des Namens die Eingabetaste **3}.**
1. Wenn Sie genauer wissen möchten, wie Sie das Element freigeben, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und verwenden Sie dann eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Anzeigen</td> 
        <td> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob die Benutzer das Element zu einem benutzerdefinierten Formular hinzufügen oder für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Verwalten</td> 
        <td> <p>Ermöglicht Zugriff auf das Bearbeiten des benutzerdefinierten Felds und dessen Anzeige sowohl in der Feldbibliothek als auch im Formularentwickler.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob die Benutzer das Element aus dem System löschen oder für andere Benutzer freigeben können sollen.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Optional) Wiederholen Sie die Schritte 5 bis 6, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wählen Sie eine systemweite Freigabeoption für das Feld aus:

   * **Jeder im System kann** bearbeiten (Standardoption)

     Wenn Sie ein benutzerdefiniertes Feld oder Widget hinzufügen und die Freigabe nicht einschränken, können alle Benutzer im System, die Zugriff auf benutzerdefinierte Formulare haben, es anzeigen und seine Eigenschaften bearbeiten.

   * **Jeder im System kann** anzeigen.
   * **Nur eingeladene Personen können auf** zugreifen

     Beschränkt den Zugriff auf nur die Elemente, die Sie der Liste hinzugefügt haben.

   ![Freigabeoptionen](assets/share-field-in-designer.png)

1. Klicken Sie auf **Speichern**.

## Vererbter Zugriff auf benutzerdefinierte Felder und Widgets bei der Freigabe eines benutzerdefinierten Formulars

Wenn ein Benutzer ein benutzerdefiniertes Formular für eine Gruppe, eine Rolle, ein Team oder ein Unternehmen freigegeben hat, erben die Empfänger den Zugriff auf die Ansicht auf alle benutzerdefinierten Felder und Widgets, die sich im Formular befinden. Diese Zugriffsebene auf diese Elemente im Formular wird immer beibehalten, damit das Formular für die Empfänger wie von der Person, die es erstellt hat, gewünscht funktionieren kann. Dies gilt auch für Empfänger, die Zugriff auf das Formular haben.

Sie können ermitteln, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat, und den Zugriff darauf entfernen.

>[!NOTE]
>
>Wenn ein Empfänger Zugriff auf ein benutzerdefiniertes Feld oder Widget im freigegebenen benutzerdefinierten Formular verwalten hat, wird dieser Zugriff für den Empfänger beibehalten.

### Erfahren Sie, wer Zugriff auf ein benutzerdefiniertes Feld oder Widget erhalten hat. {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.
1. Klicken Sie auf **Felder** und wählen Sie dann das Feld, Bild oder Zugriffs-Widget aus.
1. Klicken Sie im angezeigten Feld auf **Vererbte Berechtigungen** und zeigen Sie die angezeigten Namen an.
1. Klicken Sie auf **Abbrechen**.

### Entfernen des Zugriffs auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular, das freigegeben wurde {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Wenn Sie den Zugriff auf ein benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular entfernen müssen, das freigegeben wurde, müssen Sie die Freigabe des Formulars aufheben. Anweisungen finden Sie im Abschnitt [Zugriff auf ein benutzerdefiniertes Formular entfernen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) im Artikel [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) .
