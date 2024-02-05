---
title: Formular mit dem Formularentwickler erstellen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler entwerfen.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 4120b44a1be1fc8cf7da26ac441c8e51fa8b48ac
workflow-type: tm+mt
source-wordcount: '5096'
ht-degree: 3%

---

# Formular mit dem Formularentwickler erstellen

Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler entwerfen. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten zu diesen Objekten zu erfassen.

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
   <td>
   <p>Neuer Plan: Standard</p>
   <p>oder</p>
   <p>Aktueller Plan: Plan</p></td> 
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

1. Klicks **Benutzerdefinierte Forms** im linken Bereich.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klicks **Neues benutzerdefiniertes Formular.**
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

## Hinzufügen neuer oder vorhandener Felder zu Ihrem benutzerdefinierten Formular

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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

### Textfelder hinzufügen

Sie können einem benutzerdefinierten Formular mehrere verschiedene Textfelder hinzufügen.

+++ **Erweitern, um Beschreibungen der verfügbaren Textfelder anzuzeigen**

* **Einzeiliges Textfeld**: Ermöglicht Benutzern die Eingabe einer einzelnen Textzeile in das Feld.
* **Absatztext-Feld**: Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld.
* **Textfeld mit Formatierung**: Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld und die Formatierung des Texts mit fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen. Eine Zeichenbeschränkung von 15.000 ermöglicht viel Text und Formatierung.

  Informationen zum Zugriff auf dieses Feld über die API finden Sie unter Rich-Text-Feldspeicherung in der API.

  >[!NOTE]
  >
  >Textfelder mit Formatierung sind nicht für mobile Workfront-Apps verfügbar (in den kommenden Versionen verfügbar).

* **Beschreibender Text**: Hier können Sie Anweisungen einfügen und Links zu Seiten außerhalb von Workfront erstellen.

+++

Hinzufügen eines Textfelds:

1. Suchen Sie auf der linken Bildschirmseite eines der folgenden Textfelder und ziehen Sie es in einen Bereich auf der Arbeitsfläche:

   * Einzelzeilentext
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
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
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
    <td>Anleitung</td>
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
    <td><p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>NOTE</b>:   
    <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlenformat oder ein Währungsformat auswählen.<br></li> 
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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

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

>[!NOTE]
>
>Felder, die mehrere Auswahlmöglichkeiten zulassen, wie z. B. die Kontrollkästchen-Gruppe und Dropdown-Liste, sind in Berichten schwer grafisch zu gestalten und zu gruppieren. Um eine einfachere Diagrammerstellung und Gruppierung in Berichten zu ermöglichen, können Sie für jede Auswahl separate Felder erstellen (z. B. ein einzeiliges Textfeld).

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
    <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
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
    <td role="rowheader">Anleitung</td> 
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
    <td> <p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>NOTE</b>:   
     <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlenformat oder ein Währungsformat auswählen.<br></li> 
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
    <td>Wechseln Sie zwischen Optionsfeldern, Kontrollkästchengruppen, Dropdown-Listen oder Dropdown-Listen mit Mehrfachauswahl für das Feld.</td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Zu einem Pflichtfeld machen</td> 
    <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
    <td><ul>
    <li>Optionsschaltflächen</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Dropdown</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Auswahl </td> 
    <td> 
    <ol> 
    <li> <p>Klicks <b>Optionen</b>, aktivieren Sie dann einen der folgenden Schritte:</p> 
    <ul> 
    <li><strong>Werte anzeigen</strong>: Zeigt die Werte jeder Auswahl im Feld an. Der Titel jeder Auswahl wird standardmäßig angezeigt.</li> 
     <li><strong>Sortierungsoptionen A-Z</strong>: Sortiert die Auswahlmöglichkeiten, die Sie im Feld alphabetisch hinzufügen.</li> 
    </ul> 
    </li> 
    <li> <p>Klicken Sie für jede Auswahlmöglichkeit, die Sie für den Benutzer hinzufügen, auf das Zahnradsymbol <img src="assets/gear-icon-settings.png">und wählen Sie dann eine der folgenden Optionen aus:</p> 
    <ul> 
    <li><strong>Standardmäßig auswählen</strong>: Wählen Sie im Feld standardmäßig die gewünschte Option aus.</li> 
    <li> <p><strong>Auswahl ausblenden</strong>: Blendet die Auswahl im Feld aus. Ausgeblendete Optionen stehen in Berichten weiterhin zur Verfügung.</p> </li> 
    <li> <p><strong>Auswahl entfernen</strong>: Entfernt die Auswahl aus dem Feld.</p> <p><b>WARNUNG</b>: Wenn Sie aktuelle Objekte haben, die diese Auswahl verwenden, entfernen Sie sie nicht aus dem Feld. Wenn Sie sie entfernen, gehen historische Daten verloren. Wählen Sie stattdessen die Option aus, um sie auszublenden. Dies verhindert, dass Benutzer sie in Zukunft auswählen.</p> </li> 
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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

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
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
      </ul> <p>Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. Weitere Informationen finden Sie unter <a href="#Add" class="MCXref xref">Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen</a> in diesem Artikel.</p> </td>
         <td><ul>
    <li>Typeahead</li>
    <li>Datumsfeld</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
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
      <td> <p>Wählen Sie den Objekttyp aus, den Sie mit dem Feld verknüpfen möchten.</p> <p>Nachdem Sie auf Übernehmen oder Speichern+Schließen geklickt haben, können Sie den Objekttyp für das Feld nicht mehr ändern.</p> <p><b>NOTE</b>:   
        <ul> 
         <li>Wenn Ihr Workfront-Administrator den Namen für Portfolios, Programme oder Projekte in der Benutzeroberfläche von Workfront angepasst hat, wird der standardmäßige Workfront-Name für das Objekt in dieser Dropdown-Liste und nicht der benutzerdefinierte Name angezeigt. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Hilfe dazu benötigen.<br></li> 
         <li>Die folgenden Objekttypen werden in den mobilen Apps von iOS und Android Workfront unterstützt: Benutzer, Unternehmen, Gruppe, Auftragsrolle, Portfolio, Programm, Projekt und Vorlage.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td> 
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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

### Externe Suchfelder hinzufügen

Ein externes Suchfeld ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können eine oder mehrere dieser Optionen aus der Dropdown-Liste auswählen. Das externe Suchfeld ist auch in Listen und Berichten verfügbar.

>[!NOTE]
>
>Die externe Suchfunktion ist für Dokument- oder Benutzerobjekte nicht verfügbar.

So fügen Sie eine externe Suche hinzu:

1. Suchen Sie auf der linken Bildschirmseite nach **Externe Suche** und ziehen Sie es in einen Bereich auf der Arbeitsfläche.
1. Konfigurieren Sie rechts im Bildschirm die Optionen für das benutzerdefinierte Feld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das benutzerdefinierte Feld.</p> <p>Wenn Sie das benutzerdefinierte Feld zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
      <p><b>WICHTIG</b>:   
      <ul> 
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
      </ul> <p>Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. Weitere Informationen finden Sie unter <a href="#Add" class="MCXref xref">Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen</a> in diesem Artikel.</p> </td>
     </tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p>
      <p><strong>NOTE:</strong></p>
      <ul><li>Sie können den Formattyp nach dem Speichern des Formulars ändern, mit einer Einschränkung: Alle vorhandenen Werte für Objekte müssen in der Lage sein, in den neuen Typ zu konvertieren. (Wenn der Formattyp beispielsweise Text ist und ein Objekt den Wert "abc"speichert, können Sie das Feld nicht konvertieren und erhalten eine Fehlermeldung, dass das System "abc"nicht in Zahl/Währung konvertieren kann.) Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlenformat oder ein Währungsformat auswählen.</li>
      <li>Wenn Sie "Zahl"oder "Währung"auswählen, schneidet das System automatisch Zahlen ab, die mit 0 beginnen.</li></ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Basis-API-URL</td> 
      <td><p>Geben Sie die URL für die API ein oder fügen Sie sie ein.</p><p>Die API-URL muss einen JSON-Inhalt der Optionen zurückgeben, die Sie im Dropdown-Menü anzeigen möchten. Sie können das Feld JSON-Pfad verwenden, um die spezifischen Werte aus den zurückgegebenen JSON-Optionen auszuwählen, die Dropdown-Optionen sein sollen.</p><p>Beim Eingeben der API-URL können Sie optional die folgenden Werte in die URL übergeben:</p>
      <ul>
      <li>$$HOST - Dies stellt den aktuellen Workfront-Host dar und kann verwendet werden, um /search API-Aufrufe an die Workfront-API durchzuführen. Wenn dieser Platzhalter verwendet wird, wird die Authentifizierung verarbeitet und Benutzer müssen keine Authentifizierungskopfzeilen senden. (Beispielsweise können Benutzer Aufgaben mithilfe der Basis-URL suchen <code>$$HOST/attask/api/task/search</code> und ermöglicht die Suche nach Aufgaben und die Auswahl von Werten aus einer zurückgegebenen Aufgabenliste.)</li>
      <li><p>$$QUERY - Dies stellt den Suchtext dar, den der Endbenutzer in das Feld eingibt, und ermöglicht Ihnen die Implementierung der Abfragefilterung für Ihre Endbenutzer. (Der Benutzer sucht im Dropdown-Menü nach dem Wert.)</p>
      <p>Wenn die API, auf die Sie verweisen, dies zulässt, können Sie in Ihre Suchabfrage auch Modifikatoren einfügen, um festzustellen, wie die Suche funktionieren soll. Beispielsweise können Sie Folgendes als Basis-API-URL verwenden, um Personen die Suche nach Workfront-Projekten zu ermöglichen, die bestimmten Text enthalten: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Weitere Informationen zu den Workfront-Suchmodifikatoren finden Sie unter <a href="/help/quicksilver/wf-api/general/api-basics.md">API-Grundlagen</a>.</p>
      <p><strong>NOTE:</strong> Wenn Sie $$QUERY nicht verwenden und der Benutzer Text in das Suchfeld eingibt, werden die bereits vorhandenen Auswahlmöglichkeiten eingegrenzt. Wenn Sie jedoch $$QUERY verwenden und der Benutzer alles eingibt, wird ein neuer Netzwerkaufruf an Ihre API durchgeführt. Wenn Sie mehr als 2000 Werte in Ihrer API haben und die API Abfragen unterstützt, können Sie $$QUERY verwenden, um nicht nur aus den vorhandenen 2000 Werten zu suchen, sondern auch aus der ursprünglichen API mit den eingeschränkten Optionen.</p></li>
      <li><p>{fieldName} - Dabei ist fieldName ein benutzerdefiniertes oder natives Feld in Workfront. Auf diese Weise können Sie Dropdown-Optionsfilter für die Kaskadierung implementieren, wenn Sie den Wert eines bereits ausgewählten Felds an das Feld Externe Suche übergeben, um Optionen nach unten zu filtern. (Beispielsweise ist das Feld Region bereits im Formular vorhanden und Sie schränken eine Liste von Ländern von der API auf Länder ein, die sich in einer bestimmten Region befinden.)</p>
      <p>Für ein externes Suchfeld mit einer Abhängigkeit von anderen Feldern (mithilfe der {fieldName} -Syntax), sind die von der API zurückgegebenen Optionen auf die Optionen beschränkt, die mit den in den anderen Feldern eingegebenen Zeichenfolgen oder Werten übereinstimmen. (Diese Funktion wird in Listen und Berichten nicht unterstützt.)</p></li>
      <li>{referenceObject}.{fieldName} - Wenn das Feld Teil eines Objekts ist. Diese Syntax ähnelt benutzerdefinierten Ausdrücken. (Beispiel: portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>NOTE:</strong> Lesen Sie die Dokumentation für die API, mit der Sie arbeiten, für die spezifischen Abfragen, die Sie definieren können.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP-Methode</td> 
      <td>Auswählen <strong>Get</strong>, <strong>Post</strong>oder <strong>Put</strong> für die -Methode.</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON-Pfad</td>
      <td><p>Geben Sie den JSON-Pfad für die API ein oder fügen Sie ihn ein.</p> <p>Diese Option ermöglicht das Extrahieren von Daten aus der JSON-Datei, die von der API-URL zurückgegeben wird. Es dient dazu, festzulegen, welche Werte aus dem JSON-Bereich in den Dropdown-Optionen angezeigt werden.</p><p>Wenn Ihre API-URL beispielsweise JSON in diesem Format zurückgibt:</br>
      <pre>
      { data: { name: "USA"}, { name: "Canada"} }
      </pre>
      </p>
      <p>dann können Sie "$.data[*].name"verwenden, um USA und Kanada als Dropdown-Optionen auszuwählen.</p> <p>Weitere Informationen zum JSON-Pfad und zum Sicherstellen des richtigen JSON-Pfads finden Sie unter <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Kopfzeilen</td>
      <td><p>Klicks <strong>Kopfzeile hinzufügen</strong>und geben Sie das Schlüssel-Wert-Paar ein oder fügen Sie es ein, das für die Authentifizierung mit der API erforderlich ist.</p><p><strong>NOTE:</strong> Die Felder "Kopfzeile"sind kein sicherer Ort zum Speichern von Anmeldeinformationen. Achten Sie darauf, was Sie eingeben und speichern.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Mehrfachauswahl-Dropdown</td>
      <td><p>Wählen Sie diese Option aus, damit der Benutzer mehr als einen Wert in der Dropdown-Liste auswählen kann.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td>
      <td><p>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann.</p></td>
     </tr>       
    </tbody>
   </table>

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

>[!NOTE]
>
>Die folgenden Elemente sind technische Einschränkungen des Aufrufs an die externe API:
>
>* Maximale Anzahl an Optionen: 2000 (nur die ersten 2000 eindeutigen Optionen aus der zurückgegebenen JSON werden angezeigt)
>* Zeitüberschreitung: 3 Sekunden
>* Anzahl weiterer Versuche: 3
>* Wartezeit zwischen Wiederholungen: 500 ms
>* Erwartete Antwortstatus: 2xx

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
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget.</p> <p>Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> <p><b>WICHTIG</b>: Obwohl dies möglich ist, empfehlen wir, diesen Namen nicht zu ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Widget begonnen haben. Ist dies der Fall, erkennt das System das Widget nicht mehr, wo es jetzt in anderen Bereichen von Workfront referenziert wird. </p> <p>Jeder Widget-Name muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. </p> </td> 
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
      <td role="rowheader">Anleitung</td> 
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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

#### **Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich &quot;Dokumente&quot;**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wenn Sie einem benutzerdefinierten Formular auf diese Weise ein Video hinzufügen, gelten nur die für das benutzerdefinierte Formular festgelegten Berechtigungen für das Video, wenn Benutzer auf das Formular eines Objekts zugreifen, nicht die Berechtigungen, die für das Video im Bereich &quot;Dokumente&quot;festgelegt wurden.

1. Gehen Sie zum Video im Bereich Dokumente und generieren Sie einen Testversand dafür, wie beschrieben in [Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öffnen Sie den Testversand.
1. Klicken Sie mit der rechten Maustaste auf eine beliebige Stelle im Video und wählen Sie **Videoadresse kopieren**.
1. Fügen Sie die kopierte Adresse in das benutzerdefinierte Formular ein, in das Sie das Video-Widget einfügen. **URL** ankreuzen.
1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

### Hinzufügen von Adobe XD-Dateien

Sie können einen Adobe XD-Prototyp direkt zu einem benutzerdefinierten Formular hinzufügen. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können die Adobe XD-Datei nur in den folgenden Bereichen anzeigen:

* Der Detailbereich des Objekts (z. B. für ein Projekt, den Bereich Projektdetails )
* Das Feld &quot;Bearbeiten&quot;für das Objekt, wenn das neue Adobe Workfront-Erlebnis wie &quot;Projekt bearbeiten&quot;und &quot;Aufgabe bearbeiten&quot;angezeigt wird

Hinzufügen einer Adobe XD-Datei:

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
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
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
      <td role="rowheader">Anleitung</td> 
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

1. Klicken Sie zum Speichern der Änderungen auf **Anwenden** und fahren Sie mit einem anderen Abschnitt fort, um mit der Erstellung des Formulars fortzufahren.

   oder

   Klicks **Speichern und schließen**.

## Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler

Informationen zum Organisieren und Anzeigen einer Vorschau des Formulars finden Sie unter [Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
