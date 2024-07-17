---
title: Fügen Sie mit dem alten Formular-Builder Logik hinzu und überspringen Sie Logik zu einem benutzerdefinierten Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# Fügen Sie mit dem alten Formular-Builder Logik hinzu und überspringen Sie Logik zu einem benutzerdefinierten Formular

{{form-designer-default}}

Sie können festlegen, welche Abschnitte eines benutzerdefinierten Formulars angezeigt oder übersprungen werden sollen, je nach den Optionen, die ein Benutzer beim Ausfüllen vornimmt.

>[!NOTE]
>
>Die Logik gilt nur innerhalb eines Formulars und kann nicht auf einer Auswahl aus einem anderen Formular basieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Administratorzugriff für bestimmte Bereiche</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Überlegungen zur Verwendung der Anzeigelogik und der Logik zum Überspringen

* Um eine Anzeigerlogik zu einem benutzerdefinierten Feld, Widget oder Abschnittsumbruch hinzuzufügen, muss mindestens ein Auswahlfeld (Optionsfelder, Dropdown-Menüs oder Kontrollkästchen) vor dem Feld im Formular positioniert werden.

  Weitere Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Hinzufügen eines benutzerdefinierten Felds zu einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) und [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular mit dem alten Formular-Builder](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Sie können einem Widget oder einer Abschnittsumbruch keine Logik zum Überspringen hinzufügen. Sie können sie nur zu einem Multiple-Choice-Feld hinzufügen (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).

* Sie können einem benutzerdefinierten Feld sowohl die Anzeigenlogik als auch die Logik überspringen, wenn Folgendes für das benutzerdefinierte Feld zutrifft:

   * Es handelt sich um ein Multiple-Choice-Feld (Optionsfelder, Dropdown-Listen oder Kontrollkästchen).
   * Dem Feld wird ein Multiple-Choice-Feld vorangestellt
   * Danach folgt ein weiteres benutzerdefiniertes Feld

* Beim Kopieren von Formularen mit Anzeigenlogik oder Logik zum Überspringen wird die Logik in das neue benutzerdefinierte Formular kopiert.
* Bei der Massenbearbeitung von Objekten werden alle benutzerdefinierten Felder im Feld &quot;Objekte bearbeiten&quot;angezeigt, einschließlich der Felder, die übersprungen oder ausgeblendet werden.
* Beachten Sie Folgendes, wenn Sie eine Logikregel für die Anzeige eines benutzerdefinierten Formulars erstellen:

   * Benutzerdefinierte Felder, die nicht in einer Logikanweisung zur Anzeige enthalten sind, werden standardmäßig in einem benutzerdefinierten Formular angezeigt.
   * Sie können Logikanweisungen für mehrere Felder erstellen.
   * Wenn auf alle Felder unter einem Abschnittsumbruch eine Anzeigereihenfolge angewendet wird und sie alle aufgrund der Logik ausgeblendet sind, wird der gesamte Abschnitt im benutzerdefinierten Formular ausgeblendet.

## Erstellen eines benutzerdefinierten Beispielformulars mit Anzeige- und Übersprunglogik

Am besten erfahren Sie, wie Sie einem benutzerdefinierten Formular eine Anzeige- und Auslassungslogik hinzufügen, indem Sie das praktische Beispiel lesen, das in den beiden folgenden Abschnitten erläutert wird:

### Anzeigelogik {#display-logic}

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms**.

1. Erstellen Sie das benutzerdefinierte Beispielformular:

   1. Klicken Sie auf **Neues benutzerdefiniertes Formular** und dann in der Dropdownliste auf **Projekt** .

   1. Geben Sie in das Feld **Formulartitel** den Wert **Beispiel für ein benutzerdefiniertes Formular - Lernlogik für die Anzeige und überspringen der Logik** ein.

   1. Klicken Sie oben links auf **Feld hinzufügen** .
   1. Fügen Sie ein Dropdown-Feld mit dem Namen *Problemfeld* hinzu, indem Sie auf **Dropdown** klicken und dann im Feld **Beschriftung** das Feld **Problem** eingeben.

   1. Fügen Sie unter **Auswahlmöglichkeiten** die folgenden Auswahlmöglichkeiten in die Textfelder ein:

      Erforderliche Forschung

      Keine Forschung mehr

   1. Klicken Sie unten links auf **Speichern + Schließen** .

1. Wählen Sie das neue benutzerdefinierte Beispielformular &quot;**Muster - Anzeigenlogik lernen&quot;und überspringen Sie das benutzerdefinierte Formular &quot;Logik&quot;** und klicken Sie dann auf &quot;**Bearbeiten**&quot;.

1. Fügen Sie ein neues einzeiliges Textfeld mit dem Namen *Andere Forschung* hinzu, indem Sie auf **Einzeiliges Textfeld** klicken und dann im Feld **Beschriftung** die Option **Andere Forschung** eingeben.

1. Klicken Sie unten links im Bildschirm **Benutzerdefiniertes Formular bearbeiten** auf **Logik hinzufügen** .

1. Richten Sie in dem angezeigten Feld bei geöffneter Registerkarte **Logik anzeigen** die Logik für den Zeitpunkt ein, zu dem das Feld **Andere Forschung** im Formular angezeigt wird, indem Sie in der ersten Dropdown-Liste auf das Feld **Problem** klicken, in der zweiten Dropdown-Liste auf **Forschung erforderlich** und in der dritten Dropdown-Liste auf **Ausgewählt**.
1. Klicken Sie auf **Speichern** , um das Fenster **Feldlogik** zu schließen, und klicken Sie dann im Bereich **Feldeinstellungen** auf **Fertig** .

   Wenn jetzt jemand in der Dropdown-Liste **Feld &quot;Problem&quot;** die Option &quot;**Erforscht erforderlich**&quot; auswählt, wird das Feld **Andere Forschung** angezeigt.

1. Klicken Sie auf **Vorschau** , um sicherzustellen, dass die Logik wie gewünscht im Formular angezeigt wird.
1. Klicken Sie auf **Vorschau beenden** , wenn Sie feststellen, dass die Logik erwartungsgemäß funktioniert.
1. Klicken Sie im Fenster **Benutzerdefiniertes Formular bearbeiten** auf **Speichern + Schließen** , um das Formular zu speichern, und fahren Sie dann mit [Logik überspringen](#skip-logic) weiter.

### Logik überspringen {#skip-logic}

Logik überspringen funktioniert ähnlich wie die Anzeigelogik, fungiert jedoch als umgekehrt: Anstatt spezifische benutzerdefinierte Multiple-Choice-Felder basierend auf bestimmten Auswahlen anzuzeigen, legen Sie anhand der Auswahl des Benutzers fest, welche übersprungen werden sollen.

Um dies zu erfahren, arbeiten Sie weiter an dem benutzerdefinierten Beispielformular, das Sie im Abschnitt [Logik anzeigen](#display-logic) in diesem Artikel erstellt haben:

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Benutzerdefinierter Forms**.
1. Wählen Sie das Formular **Beispiel für ein benutzerdefiniertes Formular - Lernende Anzeigerogik und überspringen Sie die Logik**, die Sie in den oben genannten Schritten erstellt haben, und klicken Sie dann auf **Bearbeiten**.

1. Wählen Sie das von Ihnen erstellte Dropdown-Feld mit dem Namen *Problemfeld* aus.
1. Klicken Sie in der Seitenleiste **Feldeinstellungen** auf die Schaltfläche **Logik hinzufügen** .

1. Stellen Sie im Feld **Feldlogik** sicher, dass die Registerkarte **Logik überspringen** ausgewählt ist.

1. Setzen Sie das erste Dropdown-Menü auf **Keine weitere Suche** und das zweite Dropdown-Menü auf **Ausgewählt**.

1. Wählen Sie in der Dropdown-Liste **Springen Sie dann zu** die Option **Ende des Formulars**.

   Wenn jetzt jemand im Dropdown-Feld **Problemfeld** die Option **Keine weitere Suche** auswählt, wird das Formular direkt an das Ende des Formulars übersprungen, ohne das Feld **Andere Forschung** anzuzeigen.

1. Klicken Sie auf **Speichern**.
1. Klicken Sie auf **Vorschau** , um sicherzustellen, dass die Logik die gewünschte Anwendung findet.
1. Klicken Sie unten links im Formular auf **Fertig** .
