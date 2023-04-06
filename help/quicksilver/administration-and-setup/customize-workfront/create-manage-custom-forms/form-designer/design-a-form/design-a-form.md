---
title: Entwerfen eines Formulars mit dem Formularentwickler
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler entwerfen.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '3803'
ht-degree: 4%

---


# Entwerfen eines Formulars mit dem Formularentwickler

Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler entwerfen. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten zu diesen Objekten zu erfassen.

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
   <td>
   <p>Aktueller Plan: Standard</p>
   <p>oder</p>
   <p>Veralteter Plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Erstellen eines benutzerdefinierten Formulars

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Benutzerdefinierte Forms** im linken Bereich.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klicken **Neues benutzerdefiniertes Formular.**
1. Wählen Sie die Objekttypen aus, an die das benutzerdefinierte Formular angehängt werden soll, und klicken Sie dann auf **Weiter**.

   ![](assets/choose-object-type.jpg)

1. Im **Titel ist erforderlich** Bereich, geben Sie den Titel des benutzerdefinierten Formulars ein.
1. (Optional) Wenn Sie dem Formular weitere Objekttypen hinzufügen möchten, damit es an weitere Objekte angehängt werden kann, klicken Sie auf die Schaltfläche **Hinzufügen** icon ![](assets/add-objects-icon.png) after **Objekttypen** und wählen Sie dann den gewünschten Typ im angezeigten Menü aus. Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   Sie können auch auf das X für einen Objekttyp klicken, um ihn aus dem Formular zu löschen.

   >[!CAUTION]
   >
   >Beim Löschen eines benutzerdefinierten Formulars werden auch alle benutzerdefinierten Daten zu den mit dem Formular verknüpften Objekten gelöscht. Die gelöschten Daten können nicht wiederhergestellt werden. Ziehen Sie stattdessen die Deaktivierung eines benutzerdefinierten Formulars in Betracht. Wenn Sie ein benutzerdefiniertes Formular deaktivieren, das Sie nicht mehr verwenden, behalten Sie alle zugehörigen historischen Daten bei.
   >
   >Weitere Informationen finden Sie unter [Löschen von Objekttypen in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. Als Nächstes können Sie Ihrem benutzerdefinierten Formular Felder hinzufügen. Siehe die folgenden Abschnitte:
   * [Vorhandenes Feld oder Widget in einem anderen benutzerdefinierten Formular wiederverwenden](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Textfelder hinzufügen](#add-text-fields)
   * [Berechnete Felder hinzufügen](#add-calculated-fields)
   * [Optionsfelder, Kontrollkästchengruppen und Dropdown-Listen hinzufügen](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Typevorschau- und Datumsfelder hinzufügen](#add-typeahead-and-date-fields)
   * [Bilder, PDF und Videos hinzufügen](#add-images-pdfs-and-videos)
   * [Hinzufügen von Adobe XD-Dateien](#add-adobe-xd-files)

## Hinzufügen neuer oder vorhandener Felder zum benutzerdefinierten Formular

Sie können beim Entwerfen Ihres benutzerdefinierten Formulars neue oder vorhandene Felder verwenden.

## Vorhandenes Feld oder Widget in einem anderen benutzerdefinierten Formular wiederverwenden

1. Klicken Sie oben links im Bildschirm auf **Feldbibliothek**.

1. Ziehen Sie das Feld oder Widget in das benutzerdefinierte Formular.
1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   >[!NOTE]
   >
   >Sie können bis zu 500 Felder und Widgets in einem einzelnen benutzerdefinierten Formular hinzufügen. Je nach Komplexität eines Formulars kann die Leistung jedoch beeinträchtigt werden, wenn mehr als 100 Formulare vorhanden sind.
   >
   >
   >Beispiele für komplexe Formulare sind Formulare mit kaskadierenden Parametern, berechnete benutzerdefinierte Datenfelder und Optionen mit mehreren Werten in einem einzelnen Feld.

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

### Textfelder hinzufügen

Sie können einem benutzerdefinierten Formular mehrere verschiedene Textfelder hinzufügen.

+++ **Erweitern, um Beschreibungen der verfügbaren Textfelder anzuzeigen**

* **Einzelzeilentext-Feld**: Ermöglicht Benutzern die Eingabe einer einzelnen Textzeile in das Feld.
* **Absatztext-Feld**: Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld.
* **Textfeld mit Formatierung**: Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld und die Formatierung des Texts mit fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen. Eine Zeichenbeschränkung von 15.000 ermöglicht viel Text und Formatierung.

   Informationen zum Zugriff auf dieses Feld über die API finden Sie unter Rich-Text-Feldspeicherung in der API.

   >[!NOTE]
   >
   >Textfelder mit Formatierung sind nicht für mobile Workfront-Apps verfügbar (in den kommenden Versionen verfügbar).

* **Beschreibender Text**: Ermöglicht das Einfügen von Anweisungen und das Verknüpfen mit Seiten außerhalb von Workfront.

+++

So fügen Sie ein Textfeld hinzu:

1. Suchen Sie auf der linken Bildschirmseite eines der folgenden Textfelder und ziehen Sie es in einen Bereich auf der Arbeitsfläche:

   * Einzelzeilentext:
   * Absatztext
   * Textfeld mit Formatierung
   * Beschreibender Text

   ![](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Bildschirmseite die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table>
    <tr>
    <td>Eingabe in</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
    <tr>
    <td>Größe</td>
    <td><p>Ändern Sie die Größe der Textfelder im Formular.<p>
   </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    <li>Text mit Formatierung</li>
    <li>Beschreibender Text - In Kürze verfügbar</li>
    </ul></td>
    </tr>
    <tr>
    <td>Bezeichnung</td>
    <td><p>Geben Sie eine beschreibende Bezeichnung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.<p>
    <p>WICHTIG: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p></td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    <li>Text mit Formatierung</li>
    </ul></td>
    </tr>
    <tr>
     <td>Name</td>
    <td><p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
    <p><b>WICHTIG</b>:   
      <ul> 
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Ist dies der Fall, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
    </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    <li>Text mit Formatierung</li>
    <li>Beschreibender Text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Anweisungen</td>
    <td>Geben Sie weitere Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    <li>Text mit Formatierung</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>NOTIZ</b>:   
    <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie das Format Zahl oder Währung auswählen.<br></li> 
    <li>Wenn Sie "Zahl"oder "Währung"auswählen, schneidet das System automatisch Zahlen ab, die mit 0 beginnen.</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    </ul></td>
    </tr>
    <tr>
    <td>Anzeigetyp</td>
    <td>Zwischen einzelnen Zeilen- und Absatztextfeldern wechseln.</td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Text des Absatzes</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td> Wenn Sie einen Hyperlink auf den eingegebenen Text anwenden möchten, fügen Sie ihn hier hinzu. Der beschreibende Text wird als Link auf Objekten angezeigt, an die das Formular angehängt ist.</td>
    <td><ul><li>Beschreibender Text</li></ul></td>
    </tr>
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   oder

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Kopiersymbol](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

### Berechnete Felder hinzufügen

In einem benutzerdefinierten Formular können Sie ein berechnetes benutzerdefiniertes Feld hinzufügen, das vorhandene Daten verwendet, um neue Daten zu generieren, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.

Informationen zum Hinzufügen eines berechneten Felds finden Sie unter [Berechnete Felder mit dem Formularentwickler hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Radiobuttons, Checkboxes und Dropdown-Listen hinzufügen

Sie können einem benutzerdefinierten Formular Radiobuttons, Checkboxes und Dropdown-Listen hinzufügen.

+++ **Erweitern , um Beschreibungen der verfügbaren Felder anzuzeigen**

* **Optionsfelder**: Erfordert, dass Benutzer nur eine Auswahl auswählen.
* **Kontrollkästchengruppe**: Ermöglicht Benutzern die Auswahl mehrerer Optionen.
* **Dropdown**: Bietet eine Liste von Dropdown-Optionen.

+++

So fügen Sie Optionsfelder und Kontrollkästchen hinzu:

1. Suchen Sie auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich auf der Arbeitsfläche.

   * Optionsschaltflächen
   * Kontrollkästchen-Gruppe
   * Dropdown

   ![](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Bildschirmseite die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Eingabe in</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
    <tr> 
     <td role="rowheader">Bezeichnung</td> 
     <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Name</td> 
     <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das benutzerdefinierte Feld, wenn Sie es zu verschiedenen Bereichen in Workfront hinzufügen, z. B. zu Berichten, Startseite und API-Interaktionen.</p> <p>Wenn Sie das benutzerdefinierte Feld zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
    <p><b>WICHTIG</b>:   
     <ul> 
    <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Ist dies der Fall, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
    <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
     <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
     </ul> <p>Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. Weitere Informationen finden Sie unter <a href="#Add" class="MCXref xref">Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen</a> in diesem Artikel.</p> </td>
     <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Anweisungen</td> 
    <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>NOTIZ</b>:   
     <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie das Format Zahl oder Währung auswählen.<br></li> 
    <li>Wenn Sie "Zahl"oder "Währung"auswählen, schneidet das System automatisch Zahlen ab, die mit 0 beginnen.</li> 
     </ul></p></td> 
     <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Anzeigetyp</td> 
    <td>Zwischen Optionsfeldern, Kontrollkästchengruppen oder Dropdown-Listen für das Feld wechseln.</td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Zu einem erforderlichen Feld machen</td> 
    <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Auswahlmöglichkeiten </td> 
    <td> 
    <ol> 
    <li> <p>Klicken <b>Optionen</b>, aktivieren Sie dann einen der folgenden Schritte:</p> 
    <ul> 
    <li><strong>Werte anzeigen</strong>: Zeigt die Werte jeder Auswahl im Feld an. Der Titel jeder Auswahl wird standardmäßig angezeigt.</li> 
     <li><strong>Sortierungsoptionen A-Z</strong>: Sortiert die Auswahlmöglichkeiten, die Sie dem Feld alphabetisch hinzufügen.</li> 
    </ul> 
    </li> 
    <li> <p>Klicken Sie für jede Auswahlmöglichkeit, die Sie für den Benutzer hinzufügen, auf das Zahnradsymbol <img src="assets/gear-icon-settings.png">und wählen Sie dann eine der folgenden Optionen aus:</p> 
    <ul> 
    <li><strong>Standardmäßig auswählen</strong>: Wählen Sie im Feld standardmäßig die gewünschte Option aus.</li> 
    <li> <p><strong>Auswahl ausblenden</strong>: Blenden Sie die Auswahl im Feld aus. Ausgeblendete Optionen stehen in Berichten weiterhin zur Verfügung.</p> </li> 
    <li> <p><strong>Auswahl entfernen</strong>: Entfernen Sie die Auswahl aus dem Feld.</p> <p><b>WARNUNG</b>: Wenn Sie aktuelle Objekte haben, die diese Auswahl verwenden, entfernen Sie sie nicht aus dem Feld. Wenn Sie sie entfernen, gehen historische Daten verloren. Wählen Sie stattdessen die Option aus, um sie auszublenden. Dies verhindert, dass Benutzer sie in Zukunft auswählen.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   oder

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Kopiersymbol](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

### Typevorschau- und Datumsfelder hinzufügen

Sie können einem benutzerdefinierten Formular Typeahead- und Datumsfelder hinzufügen.

+++ **Erweitern , um Beschreibungen der verfügbaren Felder anzuzeigen**

* **Typahead**: Ermöglicht Benutzern die Eingabe des Namens eines Objekts, das in Workfront vorhanden ist. Eine Liste mit Vorschlägen wird angezeigt, wenn der Benutzer mit der Eingabe beginnt. Dieser Feldtyp unterstützt die folgenden Objekte:
   * Benutzerin oder Benutzer
   * Gruppe
   * Aufgabengebiet
   * Portfolio
   * Programm
   * Projekt
   * Team
   * Vorlage
   * Firma
* **Datumsfeld**: Zeigt einen Kalender an, in dem Benutzer Datum und Uhrzeit auswählen können.

+++

So fügen Sie Typeahead-Datumsfelder hinzu:

1. Suchen Sie auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich auf der Arbeitsfläche.

   * Typeahead
   * Datumsfeld

   ![](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Bildschirmseite die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Feldeinstellung</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das benutzerdefinierte Feld, wenn Sie es zu verschiedenen Bereichen in Workfront hinzufügen, z. B. zu Berichten, Startseite und API-Interaktionen.</p> <p>Wenn Sie das benutzerdefinierte Feld zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
      <p><b>WICHTIG</b>:   
      <ul> 
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Ist dies der Fall, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
      </ul> <p>Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. Weitere Informationen finden Sie unter <a href="#Add" class="MCXref xref">Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen</a> in diesem Artikel.</p> </td>
         <td><ul>
    <li>Typeahead</li>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Anweisungen</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tageszeit anzeigen</td> 
      <td>Aktivieren Sie diese Option, wenn Sie die Tageszeit zusammen mit dem Datum im Feld anzeigen möchten.</td> 
         <td><ul>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Referenzierter Objekttyp</td> 
      <td> <p>Wählen Sie den Objekttyp aus, den Sie mit dem Feld verknüpfen möchten.</p> <p>Nachdem Sie auf "Anwenden"oder "Speichern und schließen"geklickt haben, können Sie den Objekttyp für das Feld nicht mehr ändern.</p> <p><b>NOTIZ</b>:   
        <ul> 
         <li>Wenn Ihr Workfront-Administrator den Namen für Portfolios, Programme oder Projekte in der Benutzeroberfläche von Workfront angepasst hat, wird der standardmäßige Workfront-Name für das Objekt in dieser Dropdown-Liste und nicht der benutzerdefinierte Name angezeigt. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Hilfe dazu benötigen.<br></li> 
         <li>Die folgenden Objekttypen werden in den mobilen Apps von iOS und Android Workfront unterstützt: Benutzer, Firma, Gruppe, Auftragsrolle, Portfolio, Programm, Projekt und Vorlage.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem erforderlichen Feld machen</td> 
      <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   oder

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Kopiersymbol](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

### Bilder, PDF und Videos hinzufügen

Sie können einem benutzerdefinierten Formular Bilder, PDF und Videos hinzufügen. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können das Bild, die PDF oder das Video nur in den folgenden Bereichen anzeigen:

* Der Detailbereich des Objekts (z. B. für ein Projekt, den Bereich Projektdetails )
* Das Feld &quot;Bearbeiten&quot;für das Objekt, wenn das neue Adobe Workfront-Erlebnis wie &quot;Projekt bearbeiten&quot;und &quot;Aufgabe bearbeiten&quot;angezeigt wird

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Erweitern , um Beschreibungen der verfügbaren Felder anzuzeigen**

* **Bild**: Ermöglicht Benutzern das Hinzufügen von _____ Bilddateien.
* **PDF**: Ermöglicht Benutzern das Hinzufügen von PDF
* **Videos**: Ermöglicht Benutzern das Hinzufügen von ____ Videodateien.

+++

So fügen Sie Bilder, PDF oder Videos hinzu:

1. Suchen Sie auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich auf der Arbeitsfläche.

   * Bild
   * PDF
   * Video

   ![](assets/drag-field-to-section.png)

1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget.</p> <p>Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> <p><b>WICHTIG</b>: Obwohl dies möglich ist, empfehlen wir, diesen Namen nicht zu ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Widget beginnen. Ist dies der Fall, erkennt das System das Widget nicht mehr, wo es jetzt in anderen Bereichen von Workfront referenziert wird. </p> <p>Jeder Widget-Name muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben oder fügen Sie die URL des Widgets ein, in dem es im Internet gespeichert ist.</p> 
      <p>Wenn Sie ein Video-Widget hinzufügen, können Sie dies derzeit tun, indem Sie Folgendes in das URL-Feld hinzufügen:</p> 
      <ul> 
      <li> <p>YouTube- oder Vimeo-Link</p> </li> 
      <li> <p>Videolink "Google Drive"</p> </li> 
      <li> <p>Link zum Video mit MP4- und MOV-Erweiterung</p> </li> 
      <li> <p>Link zu Video, das bereits in den Bereich "Dokumente"in Ihrer Workfront-Instanz hochgeladen wurde. Anweisungen finden Sie unter <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich "Dokumente"</a> in diesem Artikel.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anweisungen</td> 
      <td> <p>Geben Sie weitere Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größe</td> 
      <td>Ändern Sie die Anzeigegröße des Widgets nach Bedarf.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   oder

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Kopiersymbol](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

#### **Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich &quot;Dokumente&quot;**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wenn Sie einem benutzerdefinierten Formular auf diese Weise ein Video hinzufügen, gelten nur die für das benutzerdefinierte Formular festgelegten Berechtigungen für das Video, wenn Benutzer auf das Formular eines Objekts zugreifen, nicht die Berechtigungen, die für das Video im Bereich &quot;Dokumente&quot;festgelegt wurden.

1. Gehen Sie zum Video im Bereich Dokumente und generieren Sie einen Testversand dafür, wie beschrieben in [Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öffnen Sie den Testversand.
1. Klicken Sie mit der rechten Maustaste auf eine beliebige Stelle im Video und wählen Sie **Videoadresse kopieren**.
1. Fügen Sie die kopierte Adresse in das benutzerdefinierte Formular ein, in das Sie das Video-Widget einfügen. **URL** ankreuzen.
1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

### Hinzufügen von Adobe XD-Dateien

Sie können einen Adobe XD-Prototyp direkt zu einem benutzerdefinierten Formular hinzufügen. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können die Adobe XD-Datei nur in den folgenden Bereichen anzeigen:

* Der Detailbereich des Objekts (z. B. für ein Projekt, den Bereich Projektdetails )
* Das Feld &quot;Bearbeiten&quot;für das Objekt, wenn das neue Adobe Workfront-Erlebnis wie &quot;Projekt bearbeiten&quot;und &quot;Aufgabe bearbeiten&quot;angezeigt wird

So fügen Sie eine Adobe XD-Datei hinzu:

1. Suchen Sie auf der linken Bildschirmseite nach **Adobe XD** und ziehen Sie es in einen Bereich auf der Arbeitsfläche.
1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget. Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
    <p><b>WICHTIG</b>:   
      <ul> 
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Ist dies der Fall, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben Sie einen gültigen XD Prototyplink ein oder fügen Sie ihn ein.</p> 
      <p>Hinweis: Die Einstellung Link-Zugriff auf die Registerkarte Freigabe in Adobe XD muss auf Jeder mit dem Link festgelegt sein. Andernfalls können Benutzer den Prototyp nicht anzeigen. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anweisungen</td> 
      <td> <p>Geben Sie weitere Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie bei Bedarf die Anzeigegröße des Widgets.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   oder

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Kopiersymbol](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicken **Speichern und schließen**.

## Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler

Informationen zum Organisieren und Anzeigen einer Vorschau des Formulars finden Sie unter [Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).