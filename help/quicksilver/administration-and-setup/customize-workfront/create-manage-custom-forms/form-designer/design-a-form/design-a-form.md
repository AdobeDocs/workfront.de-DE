---
title: Erstellen eines benutzerdefinierten Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Formular-Designer entwerfen. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten über diese Objekte zu erfassen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 9fcfea189bfc8827e41098823402f5e392b36d1b
workflow-type: tm+mt
source-wordcount: '7040'
ht-degree: 5%

---

# Erstellen eines benutzerdefinierten Formulars

<!-- Audited: 6/2025 -->

{{preview-fast-release-general}}

Sie können ein benutzerdefiniertes Formular mit dem Formular-Designer in Adobe Workfront entwerfen. Sie können benutzerdefinierte Formulare an verschiedene Workfront-Objekte anhängen, um Daten über diese Objekte zu erfassen.

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
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beginnen Sie mit dem Entwurf eines benutzerdefinierten Formulars

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms** und wählen Sie dann **Forms**.

1. Klicken Sie auf **Neues benutzerdefiniertes Formular.**
1. Wählen Sie aus, an welche Objekttypen Sie das benutzerdefinierte Formular anhängen möchten, und klicken Sie dann auf **Weiter**.

   ![Auswählen von Objekttypen](assets/new-custom-form-select-objects.png)

1. Geben **im Bereich &quot;** hinzufügen“ den benutzerdefinierten Formulartitel ein.
1. (Optional) Wenn Sie dem Formular weitere Objekttypen hinzufügen möchten, damit es mit weiteren Objekten verbunden werden kann, klicken Sie auf das **Hinzufügen**-Symbol ![Objekte hinzufügen](assets/add-objects-icon.png) neben **Objekttypen** und wählen Sie dann im angezeigten Menü den gewünschten Typ aus. Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   Nachdem Sie mehr als ein Objekt zum Formular hinzugefügt haben, können Sie auf das X auf einem Objekttyp klicken, um es aus dem Formular zu löschen.

   >[!CAUTION]
   >
   >Beim Löschen eines benutzerdefinierten Formulars werden auch alle benutzerdefinierten Daten in den mit dem Formular verknüpften Objekten gelöscht. Die gelöschten Daten können nicht wiederhergestellt werden. Alternativ können Sie ein benutzerdefiniertes Formular deaktivieren, das Sie nicht mehr verwenden. Dadurch werden alle zugehörigen historischen Daten beibehalten.
   >
   >Weitere Informationen finden Sie unter [Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) und [Deaktivieren oder Reaktivieren eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Als Nächstes können Sie damit beginnen, Ihrem benutzerdefinierten Formular Felder hinzuzufügen. Weitere Informationen finden Sie in den folgenden Abschnitten:
   * [Vorhandenes Feld oder Widget wiederverwenden, das bereits in einem anderen benutzerdefinierten Formular verwendet wurde](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Hinweise zu Feldnamen und Kennzeichnungen](#notes-on-field-names-and-labels)
   * [Textfelder hinzufügen](#add-text-fields)
   * [Hinzufügen von berechneten Feldern](#add-calculated-fields)
   * [Hinzufügen von Optionsfeldern, Kontrollkästchen-Gruppen und Dropdown-Listen](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [Felder für automatische Textvervollständigung und Datum hinzufügen](#add-typeahead-and-date-fields)
   * [Hinzufügen externer Suchfelder](#add-external-lookup-fields)
   * [Bilder, PDFs und Videos hinzufügen](#add-images-pdfs-and-videos)
   * [Native Workfront-Felder hinzufügen](#add-workfront-native-fields)
   * [Adobe XD-Dateien hinzufügen](#add-adobe-xd-files)
   * [Planning-Verbindungsfelder hinzufügen](#add-planning-connection-fields)

## Hinzufügen neuer oder vorhandener Felder zum benutzerdefinierten Formular

Sie können neue oder vorhandene Felder beim Entwerfen Ihres benutzerdefinierten Formulars verwenden.

Benutzerdefinierte Formulare sind auf 500 Felder beschränkt. Ein Zähler unten links zeigt an, wie viele Felder im Formular verwendet werden, und er ist immer sichtbar, wenn Sie im Formular-Designer scrollen.

### Vorhandenes Feld oder Widget wiederverwenden, das bereits in einem anderen benutzerdefinierten Formular verwendet wurde

1. Klicken Sie oben links im Bildschirm auf &quot;**&quot;**.

1. Ziehen Sie das gewünschte Feld oder Widget auf die Arbeitsfläche. Wiederholen Sie diesen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   >[!NOTE]
   >
   >Sie können bis zu 500 Felder und Widgets in einem einzelnen benutzerdefinierten Formular hinzufügen. Je nach Komplexität eines Formulars kann es jedoch zu Leistungseinbußen kommen, wenn mehr als 100 auf dem Formular vorhanden sind.
   >
   >
   >Beispiele für komplexe Formulare sind Formulare mit kaskadierenden Parametern, berechneten benutzerdefinierten Datenfeldern und mehreren Wertoptionen in einem einzigen Feld.

   >[!NOTE]
   >
   >Wenn Sie ein vorhandenes Feld als inaktiv markieren, wird es von diesem Zeitpunkt an nicht mehr für die Verwendung in Berichtselementen und benutzerdefinierten Formularen verfügbar. Wenn das inaktive Feld derzeit in einem Bericht oder Formular verwendet wird, bleiben das Feld und seine historischen Daten erhalten.

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Hinweise zu Feldnamen und Kennzeichnungen {#notes-on-field-names-and-labels}

Die Bezeichnung ist für die meisten Felder verfügbar. Dies ist eine beschreibende Beschriftung, die über dem Feld oder Widget im benutzerdefinierten Formular angezeigt wird. Sie können den Titel jederzeit ändern.

>[!NOTE]
>
>Vermeiden Sie die Verwendung von Sonderzeichen in dieser Beschriftung, da sie in Berichten nicht korrekt angezeigt werden.

Für jedes Feld ist ein Name erforderlich. Mit diesem Namen identifiziert das System das benutzerdefinierte Feld, wenn Sie es verschiedenen Bereichen in Workfront hinzufügen, z. B. Berichten, der Startseite und API-Interaktionen. Wenn Sie das Feld oder Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.

Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden.

>[!NOTE]
>
>Obwohl dies möglich ist, empfehlen wir, diesen Namen nicht zu ändern, nachdem Sie oder andere Benutzende mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Andernfalls erkennt das System das benutzerdefinierte Feld nicht mehr, in dem jetzt in anderen Bereichen von Workfront darauf verwiesen werden kann.
>Wenn Sie beispielsweise ein benutzerdefiniertes Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es im Bericht nicht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter dem neuen Namen erneut hinzu.
>
>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wird.
>
>Es wird empfohlen, im benutzerdefinierten Feldnamen keinen Punkt bzw. Punkt zu verwenden, um Fehler zu vermeiden, wenn das Feld in verschiedenen Bereichen von Workfront verwendet wird.

Die folgenden Sonderzeichen werden in benutzerdefinierten Feldbezeichnungen und -namen nicht unterstützt.

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Textfelder hinzufügen

Sie können einem benutzerdefinierten Formular mehrere verschiedene Textfelder hinzufügen.

+++ Erweitern Sie , um Beschreibungen der verfügbaren Textfelder anzuzeigen.

* **Einzeiliges Textfeld**: Ermöglicht Benutzern, eine einzelne Textzeile in das Feld einzugeben.
* **Absatzfeld**: Ermöglicht Benutzern, mehrere Textzeilen in das Feld einzugeben.
* <span class="preview">**Rich-Text**: Ermöglicht Benutzern, mehrere Textzeilen in das Feld einzugeben und den Text mit fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierung, Tiefgestellt und hochgestellt, Hyperlinks, Blockanführungszeichen, Überschriften und Tabellen zu formatieren. Eine Zeichenbeschränkung von 15.000 bietet viel Platz für Text und Formatierung.</span>

  <span class="preview">Der Rich-Text-Feldtyp ersetzt den Text durch den Feldtyp Formatierung . Sie können vorhandenen Text mit Formatierungsfeldern schnell in Rich-Text konvertieren, indem Sie auf die Schaltfläche **In Rich-Text konvertieren** in den Feldoptionen auf der rechten Seite klicken.</span>

* **Textfeld mit Formatierung**: Ermöglicht Benutzern, mehrere Textzeilen in das Feld einzugeben und den Text mit fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierungen, Hyperlinks und Blockanführungszeichen zu formatieren. Eine Zeichenbeschränkung von 15.000 ermöglicht viel Text und Formatierung.

  Dieser benutzerdefinierte Feldtyp wird in Filtern in Listen und Berichten nicht unterstützt.

  Informationen zum Zugriff auf dieses Feld über die API finden Sie unter [Rich-Text-Feldspeicher in der API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Textfelder mit Formatierung sind für Workfront Mobile Apps nicht verfügbar (in kommenden Versionen verfügbar).

* **Beschreibungstext**: Ermöglicht das Einfügen von Anweisungen und Links zu Seiten außerhalb von Workfront.

+++

Hinzufügen eines Textfelds:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite eines der folgenden Textfelder und ziehen Sie es in einen Bereich der Arbeitsfläche:

   * Einzeiliger Text
   * Absatz
   * <span class="preview">Rich-Text</span>
   * Text mit Formatierung
   * Beschreibender Text

   ![Feld in Abschnitt ziehen](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table>
    <tr>
    <td>Eingabe in</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
    <tr>
    <td>Größe</td>
    <td><p>(Optional) Ändern Sie die Größe der Textfelder im Formular.<p>
   </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    <li><span class="preview">Rich Text</span></li>
    <li>Text mit Formatierung</li>
    <li>Beschreibender Text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Label</td>
    <td><p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.<p>
    <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p></td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    <li><span class="preview">Rich Text</span></li>
    <li>Text mit Formatierung</li>
    </ul></td>
    </tr>
    <tr>
     <td>Name</td>
    <td><p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
    <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p>
    </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    <li><span class="preview">Rich Text</span></li>
    <li>Text mit Formatierung</li>
    <li>Beschreibender Text</li>
    </ul></td>
    </tr>
    <tr>
    <td>Anleitung</td>
    <td>Geben Sie zusätzliche Informationen zum Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    <li><span class="preview">Rich Text</span></li>
    <li>Text mit Formatierung</li>
    </ul></td>
    </tr>
    <tr>
    <td>Format</td>
    <td><p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>Hinweis</b>:   
    <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlen- oder Währungsformat auswählen.</li> 
    <li>Wenn Sie Zahl oder Währung auswählen, kürzt das System automatisch Zahlen, die mit 0 beginnen.</li>
    <li>Die Zeichenbeschränkung für Zahlenfelder ist 16. Sie können auch ein Textfeld verwenden, um Zahlen einzugeben und das Limit zu vermeiden.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    </ul></td>
    </tr>
    <tr>
    <td>Anzeigetyp</td>
    <td>Zwischen einzeiligen und Absatztextfeldern wechseln.</td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hyperlink</td>
    <td> Wenn Sie einen Hyperlink auf den eingegebenen beschreibenden Text anwenden möchten, fügen Sie ihn hier hinzu. Der beschreibende Text wird als Link auf Objekten angezeigt, an die das Formular angehängt ist.</td>
    <td><ul><li>Beschreibender Text</li></ul></td>
    </tr>
    <tr>
     <td>Aktiv</td>
     <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     <td><ul>
     <li>Einzeiliger Text</li>
     <li>Absatz</li>
     <li><span class="preview">Rich Text</span></li>
     <li>Text mit Formatierung</li>
     <li>Beschreibender Text</li></ul></td>
    </tr>
    <tr> 
      <td>Zu einem Pflichtfeld machen</td>
      <td><p>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann.</p></td>
    <td><ul>
    <li>Einzeiliger Text</li>
    <li>Absatz</li>
    <li><span class="preview">Rich Text</span></li>
    <li>Text mit Formatierung</li>
    </ul></td> 
    </tr> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![copy icon](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Hinzufügen von berechneten Feldern

In einem benutzerdefinierten Formular können Sie ein berechnetes benutzerdefiniertes Feld hinzufügen, das vorhandene Daten verwendet, um neue Daten zu generieren, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.

Informationen zum Hinzufügen eines berechneten Felds finden Sie unter [Hinzufügen berechneter Felder mit dem Formular-Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Hinzufügen von Optionsfeldern, Kontrollkästchen-Gruppen und Dropdown-Listen

Sie können Optionsfelder, Kontrollkästchengruppen, Dropdown-Listen und Dropdown-Listen mit Mehrfachauswahl zu einem benutzerdefinierten Formular hinzufügen.

+++ Erweitern Sie , um Beschreibungen der verfügbaren Felder anzuzeigen.

* **Optionsfelder**: Erfordert, dass Benutzer nur eine Auswahl auswählen.
* **Kontrollkästchen-Gruppe**: Ermöglicht Benutzern die Auswahl mehrerer Auswahlmöglichkeiten.
* **Dropdown-Liste mit Einzelauswahl**: Bietet eine Liste mit Dropdown-Optionen.
* **Mehrfachauswahl-Dropdown**: Ermöglicht Benutzern die Auswahl mehrerer Auswahlmöglichkeiten aus einer Dropdown-Liste.

+++

>[!NOTE]
>
>Felder, die mehrere Auswahlmöglichkeiten zulassen, z. B. die Kontrollkästchen-Gruppe und das Mehrfachauswahl-Dropdown-Menü, sind in Berichten schwer zu kartieren und zu gruppieren. Um Diagramme und Gruppierungen in Berichten zu erleichtern, können Sie für jede Auswahl separate Felder erstellen (z. B. ein einzeiliges Textfeld).

So fügen Sie Optionsfelder, Kontrollkästchengruppen und Dropdown-Listen hinzu:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich der Arbeitsfläche:

   * Optionsfelder
   * Kontrollkästchen-Gruppe
   * Einfachauswahl-Dropdown
   * Mehrfachauswahl-Dropdown

   ![Ziehen Sie ein Feld auf die Arbeitsfläche](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Eingabe in</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
    <tr> 
     <td role="rowheader">Label</td> 
     <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Name</td> 
     <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
    <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td>
     <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Anleitung</td> 
    <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Format</td> 
    <td> <p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p> <p><b>Hinweis</b>:   
     <ul> 
    <li>Dieses Feld kann nach dem Speichern des Formulars nicht mehr bearbeitet werden. Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlen- oder Währungsformat auswählen.<br></li> 
    <li>Wenn Sie Zahl oder Währung auswählen, kürzt das System automatisch Zahlen, die mit 0 beginnen.</li>
    <li>Die Zeichenbeschränkung für Zahlenfelder ist 16. Sie können auch ein Textfeld verwenden, um Zahlen einzugeben und das Limit zu vermeiden.</li>
     </ul></p></td> 
     <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Anzeigetyp</td> 
    <td>Wechseln zwischen Optionsfeldern, Kontrollkästchen-Gruppen, Einfach-Auswahl-Dropdown-Listen oder Mehrfachauswahl-Dropdown-Listen für das Feld.</td> 
    <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
    </tr> 
    <td role="rowheader">Auswahl </td> 
    <td> 
    <p>Wählen Sie eine der folgenden Optionen aus:</p> 
    <ul> 
    <li><strong>Werte anzeigen</strong>: Zeigt die Werte jeder Auswahl im Feld an. Der Titel jeder Auswahl wird standardmäßig angezeigt.</li>
   <li><strong>Auswahl A-Z sortieren</strong>: Sortiert die Auswahlmöglichkeiten, die Sie dem Feld hinzufügen.</li>
    </ul>
     <p>Klicken Sie für jede Auswahl, die Sie dem Benutzer hinzufügen, auf das Zahnradsymbol <img src="assets/gear-icon-settings.png"> und wählen Sie dann eine der folgenden Optionen aus:</p> 
    <ul> 
    <li><strong>Standardmäßig auswählen</strong>: Wählen Sie im Feld die Standardauswahl aus.</li> 
    <li> <p><strong>Auswahl ausblenden</strong>: Blendet die Auswahl im Feld aus. Ausgeblendete Auswahlmöglichkeiten bleiben in Berichten verfügbar.</p> </li> 
    <li> <p><strong>Auswahl entfernen</strong>: Entfernen der Auswahl aus dem Feld.</p> <p><b>Warnung</b>: Wenn Sie aktuelle Objekte haben, die diese Auswahl verwenden, entfernen Sie sie nicht aus dem Feld. Durch Entfernen gehen historische Daten verloren. Wählen Sie stattdessen die Option aus, um sie auszublenden, sodass die Benutzer sie in Zukunft nicht mehr auswählen können.</p> </li> 
    </ul>   
    <p><b>Hinweis:</b> Es gibt keine Begrenzung dafür, wie viele Auswahlmöglichkeiten Sie auswählen können. </p>    
    </td> 
    <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul>
    </td>
     </tr>
    <tr>
     <td>Aktiv</td>
     <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     <td><ul>
     <li>Optionsfelder</li>
     <li>Kontrollkästchen-Gruppe</li>
     <li>Einfachauswahl-Dropdown</li>
     <li>Mehrfachauswahl-Dropdown</li></ul></td>
    </tr>
    <tr> 
    <td role="rowheader">Zu einem Pflichtfeld machen</td> 
    <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
    <td><ul>
    <li>Optionsfelder</li>
    <li>Kontrollkästchen-Gruppe</li>
    <li>Einfachauswahl-Dropdown</li>
    <li>Mehrfachauswahl-Dropdown</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![Symbol „Kopieren“](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Felder für automatische Textvervollständigung und Datum hinzufügen

Sie können einem benutzerdefinierten Formular Felder für automatische Textvervollständigung und Datum hinzufügen.

+++ Erweitern Sie , um Beschreibungen der verfügbaren Felder anzuzeigen.

* **typeahead**: Ermöglicht Benutzern, den Namen eines Objekts einzugeben, das in Workfront vorhanden ist. Eine Liste mit Vorschlägen wird angezeigt, wenn Benutzende mit der Eingabe beginnen. Dieser Feldtyp unterstützt die folgenden Objekte:
   * Benutzerin oder Benutzer
   * Gruppe
   * Aufgabengebiet
   * Portfolio
   * Programm
   * Projekt
   * Team
   * Vorlage
   * Firma
* **Datum**: Zeigt einen Kalender an, in dem Benutzer ein Datum und eine Uhrzeit auswählen können.

+++

So fügen Sie Felder für automatische Textvervollständigung und Datum hinzu:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich der Arbeitsfläche.

   * Typeahead
   * Datum

   ![Feld in Abschnitt ziehen](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Feldeinstellung</td>
    <td>Beschreibung</td>
    <td>Verfügbar für </td>
    </tr>
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
      <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td>
    <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tageszeit anzeigen</td> 
      <td>Wählen Sie diese Option aus, wenn Sie die Tageszeit zusammen mit dem Datum im Feld anzeigen möchten.</td> 
         <td><ul>
    <li>Datum</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Referenzierter Objekttyp</td> 
      <td> <p>Wählen Sie den Objekttyp aus, den Sie mit dem Feld verknüpfen möchten.</p> <p>Nachdem Sie auf <b>Anwenden</b> oder <b>Speichern und schließen</b> geklickt haben, können Sie den Objekttyp für das Feld nicht mehr ändern.</p> <p><b>Hinweis</b>:   
        <ul> 
         <li>Wenn Ihr Workfront-Administrator den Namen für Portfolios, Programme oder Projekte in der Workfront-Benutzeroberfläche angepasst hat, wird in dieser Dropdown-Liste der standardmäßige Workfront-Name für das Objekt angezeigt, nicht der benutzerdefinierte Name. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Hilfe benötigen.<br></li> 
         <li>Die folgenden Objekttypen werden in iOS und Android Workfront Mobile Apps unterstützt: Benutzer, Unternehmen, Gruppe, Aufgabengebiet, Portfolio, Programm, Projekt und Vorlage.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Filter hinzufügen</td>
      <td><p>Fügen Sie einen Filter für einen Objekttyp hinzu, um die Objekte zu begrenzen, die Benutzer auswählen können, wenn sie das Feld verwenden. </p> <p>Sie können beispielsweise ein Feld so beschränken, dass Benutzernamen nur ausgewählt werden können, wenn sie die folgenden Kriterien erfüllen:</p> 
       <ul> 
        <li>Sie gehören zu einer oder mehreren Gruppen, die Sie angeben.</li> 
        <li>Sie sind mit einer von Ihnen angegebenen Funktion oder einem von Ihnen angegebenen Titel verknüpft.</li> 
        <li>Sie gehören zur selben Gruppe wie die Person, die das Feld verwendet.</li> 
       </ul>
       <p>Sie müssen den Filter für den ausgewählten Objekttyp mithilfe der Textmodus-Syntax definieren. Weitere Informationen zum Erstellen eines Filters im Textmodus finden Sie unter <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Bearbeiten eines Filters im Textmodus</a>.</p>
       <p><b>Tipp</b> Sie können einen Bericht erstellen, um Ihren Filter zu testen, bevor Sie den Filter direkt zum Feld mit automatischer Textvervollständigung hinzufügen. Auf diese Weise können Sie überprüfen, ob der Filter die richtigen Objekte zurückgibt. Anschließend können Sie im Bericht in den Textmodus wechseln, die Textmodusanweisung kopieren und zum Typeahead-Filter hinzufügen.</p>
       <p><b>Hinweis</b>:
       <ul> 
        <li>Wenn Sie ein vorhandenes benutzerdefiniertes Formular bearbeiten, werden beim Hinzufügen eines Filters zu einem Feld mit automatischer Textvervollständigung keine Objekte entfernt (außerhalb des Bereichs des Filters), die Benutzende bereits mithilfe des Felds hinzugefügt haben.</li> 
        <li>Dieser Filter ist auf Mobilgeräten nicht verfügbar. Wenn Sie den Filter für ein Feld mit automatischer Textvervollständigung verwenden, wird das Feld auf den Mobilgeräten der Benutzenden angezeigt, ohne vom Filter betroffen zu sein.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Typeahead</li>
       </ul>
      </td>
     </tr>
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
      <td><ul>
      <li>Typeahead</li>
      <li>Datum</li></ul></td>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td> 
      <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Datum</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![copy icon](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Hinzufügen externer Suchfelder

Ein externes Suchfeld ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können eine oder mehrere dieser Optionen aus der Dropdown-Liste auswählen, je nachdem, ob das externe Suchfeld ein Einzel- oder Mehrfachauswahlfeld ist. Die externen Suchfelder sind auch in Listen und Berichten verfügbar.

Beispiele für die Verwendung des externen Suchfelds zum Aufrufen derselben Instanz von Workfront oder einer öffentlichen API finden Sie unter [Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* Externe Suchfelder werden im Outlook-Plug-in nicht unterstützt.
>* Externe Suchfelder sind nicht in Listen verfügbar, wenn das Feld eine Abhängigkeit von einem anderen Feld aufweist.

So fügen Sie eine externe Suche hinzu:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite nach **Externe Suche** oder **Externe Suche mit Mehrfachauswahl** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.
1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen für das benutzerdefinierte Feld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Beschriftung und Name sind jedoch nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
      <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td>
     </tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td>
      <td><p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll.</p>
      <p><strong>Hinweis:</strong></p>
      <ul><li>Sie können den Formattyp nach dem Speichern des Formulars ändern, mit einer Einschränkung: Alle vorhandenen Werte auf Objekten müssen in den neuen Typ konvertiert werden können. (Wenn beispielsweise der Formattyp Text lautet und ein Objekt den Wert „abc“ speichert, können Sie das Feld nicht konvertieren und erhalten die Fehlermeldung, dass das System „abc“ nicht in Zahl/Währung konvertieren kann.) Wenn Sie Ihr Feld in mathematischen Berechnungen verwenden möchten, stellen Sie sicher, dass Sie ein Zahlen- oder Währungsformat auswählen.</li>
      <li>Wenn Sie Zahl oder Währung auswählen, kürzt das System automatisch Zahlen, die mit 0 beginnen.</li>
      <li>Die Zeichenbeschränkung für Zahlenfelder ist 16. Sie können auch ein Textfeld verwenden, um Zahlen einzugeben und das Limit zu vermeiden.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Basis-API-URL</td> 
      <td><p>Geben Sie die URL für die API ein oder fügen Sie sie ein.</p><p>Die API-URL muss einen JSON-Inhalt der Optionen zurückgeben, die Sie in der Dropdown-Liste anzeigen möchten. Sie können das Feld JSON-Pfad verwenden, um die spezifischen Werte aus der zurückgegebenen JSON als Dropdown-Optionen auszuwählen.</p><p>Bei der Eingabe der API-URL können Sie optional die folgenden Werte in die URL eingeben:</p>
      <ul>
      <li>$$HOST - Stellt den aktuellen Workfront-Host dar und kann verwendet werden, um API-Aufrufe an die Workfront-API durchzuführen bzw. zu suchen. Wenn dieser Platzhalter verwendet wird, wird die Authentifizierung verarbeitet und die Benutzer müssen keine Authentifizierungs-Header senden. (Benutzerinnen und Benutzer können beispielsweise Aufgaben mithilfe des Basis-URL-<code>$$HOST/attask/api/task/search</code> suchen. Dadurch können sie Aufgaben suchen und Werte aus einer zurückgegebenen Aufgabenliste auswählen.)</li>
      <li><p>$$QUERY - Stellt den Suchtext dar, den der Endbenutzer in das Feld eingibt, und ermöglicht Ihnen die Implementierung der Abfragefilterung für Ihre Endbenutzer. (Der Benutzer sucht nach dem Wert in der Dropdown-Liste.)</p>
      <p>Wenn die API, auf die Sie verweisen, dies zulässt, können Sie auch Modifikatoren in Ihre Suchanfrage einbeziehen, um zu ermitteln, wie die Suche funktionieren sollte. Beispielsweise können Sie Folgendes als Basis-API-URL verwenden, damit Benutzer nach allen Workfront-Projekten suchen können, die bestimmten Text enthalten: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Weitere Informationen zu den Workfront-Suchmodifikatoren finden Sie unter <a href="/help/quicksilver/wf-api/general/api-basics.md">API-Grundlagen</a>.</p>
      <p><strong>Hinweis:</strong> Wenn Sie $$QUERY nicht verwenden und der Text der Benutzenden in das Suchfeld eingeben, werden die bereits verfügbaren Optionen eingeschränkt. Wenn Sie jedoch $$QUERY verwenden und der Benutzer etwas eingibt, wird ein neuer Netzwerkaufruf an Ihre API durchgeführt. Wenn Ihre API also mehr als 2.000 Werte enthält und die API Abfragen unterstützt, können Sie mit $$QUERY nicht nur nach den vorhandenen 2.000 Werten, sondern auch nach der ursprünglichen API mit den eingeschränkten Optionen suchen.</p></li>
      <li><p>{fieldName} - Wobei fieldName ein benutzerdefiniertes oder natives Feld in Workfront ist. Auf diese Weise können Sie kaskadierende Dropdown-Optionsfilter implementieren, wenn Sie den Wert eines bereits ausgewählten Felds an das externe Suchfeld übergeben, um Optionen nach unten zu filtern. (Das Feld Region existiert beispielsweise bereits im Formular und Sie grenzen die Liste der Länder von der API auf die Länder ein, die sich in einer bestimmten Region befinden.)</p>
      <p>Bei einem externen Suchfeld, das (unter Verwendung der {fieldName} Syntax) eine Abhängigkeit von anderen Feldern aufweist, sind die von der API zurückgegebenen Optionen auf die Optionen beschränkt, die mit den in den anderen Feldern eingegebenen Zeichenfolgen oder Werten übereinstimmen. (Diese Funktion wird in Listen und Berichten nicht unterstützt.)</p></li>
      <li>{referenceObject}.{fieldName} : Wobei das Feld Teil eines Objekts ist. Diese Syntax ähnelt benutzerdefinierten Ausdrücken. (Beispiel: portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>Tipp:</strong> Lesen Sie die Dokumentation für die API, mit der Sie arbeiten, und die spezifischen Abfragen, die Sie definieren können.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP-Methode</td> 
      <td>Wählen Sie <strong> Methode </strong>GET<strong>, POST</strong> oder <strong>PUT</strong>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON-Pfad</td>
      <td><p>Geben Sie den JSON-Pfad für die API ein oder fügen Sie ihn ein.</p> <p>Diese Option ermöglicht das Extrahieren von Daten aus der von der API-URL zurückgegebenen JSON. Sie dient als Möglichkeit, festzulegen, welche Werte aus dem JSON-Code in den Dropdown-Optionen angezeigt werden.</p><p>Wenn Ihre API-URL beispielsweise JSON im folgenden Format zurückgibt, können Sie "$.data[*].name“ verwenden, um USA und Kanada als Dropdown-Optionen auszuwählen:</br>
      <pre>
      &lbrace;
       Daten: &lbrace;
         { name: „USA“},
         { name: „Canada“}
       &rbrace;
      &rbrace;
      </pre>
      </p>
     <p>Weitere Informationen zum JSON-Pfad und zum Schreiben des richtigen JSON-Pfads finden Sie unter <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Header</td>
      <td><p>Klicken Sie <strong>Kopfzeile hinzufügen</strong> und geben Sie dann das für die Authentifizierung mit der API erforderliche Schlüssel-Wert-Paar ein oder fügen Sie es ein.</p><p><strong>Hinweis:</strong> Die Header-Felder sind kein sicherer Ort zum Speichern von Anmeldeinformationen, und Sie sollten darauf achten, was Sie eingeben und speichern.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Mehrfachauswahl-Dropdown</td>
      <td><p>Wählen Sie diese Option aus, damit der/die Benutzende mehr als einen Wert in der Dropdown-Liste auswählen kann.</p></td>
     </tr>
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td>
      <td><p>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann.</p></td>
     </tr>       
    </tbody>
   </table>

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

>[!NOTE]
>
>Bei den folgenden Elementen handelt es sich um technische Einschränkungen des Aufrufs an die externe API:
>
>* Maximale Anzahl von Optionen: 2000 (es werden nur die ersten 2000 eindeutigen Optionen aus der zurückgegebenen JSON-Datei angezeigt)
>* Zeitüberschreitung: 30 Sekunden
>* Anzahl weiterer Versuche: 3
>* Wartezeit zwischen weiteren Zustellversuchen: 500 ms
>* Erwartete Antwortstatus: 2xx

### Bilder, PDFs und Videos hinzufügen

Sie können Bilder, PDFs und Videos zu einem benutzerdefinierten Formular hinzufügen. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können das Bild, die PDF oder das Video nur in den folgenden Bereichen sehen:

* Der Bereich Details des Objekts (z. B. für ein Projekt der Bereich Projektdetails ).
* Das Bearbeitungsfeld für das Objekt, wenn es das neue Erscheinungsbild von Adobe Workfront aufweist (z. B. die Felder Projekt bearbeiten und Aufgabe bearbeiten ).

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ Erweitern Sie , um Beschreibungen der verfügbaren Felder anzuzeigen.

* **Image**: Ermöglicht Benutzern das Hinzufügen von Bilddateien.
* **PDF**: Ermöglicht Benutzern das Hinzufügen von PDFs
* **Videos**: Ermöglicht Benutzern das Hinzufügen von Videodateien.

+++

So fügen Sie Bilder, PDFs oder Videos hinzu:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite eines der folgenden Felder und ziehen Sie es in einen Bereich der Arbeitsfläche.

   * Bild
   * PDF
   * Video

   ![Feld in Abschnitt ziehen](assets/drag-field-to-section.png)

1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie die Anzeigegröße des Widgets nach Bedarf.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Beschriftung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben Sie die URL des Widgets ein, in dem es im Internet gespeichert ist, oder fügen Sie sie ein.</p> 
      <p>Wenn Sie ein Video-Widget hinzufügen, können Sie dies derzeit tun, indem Sie Folgendes in das URL-Feld einfügen:</p> 
      <ul> 
      <li> <p>Link zu YouTube oder Vimeo</p> </li> 
      <li> <p>Videolink auf Google Drive</p> </li> 
      <li> <p>Link zum Video mit MP4- und MOV-Erweiterung</p> </li> 
      <li> <p>Link zu Video, das bereits in den Bereich Dokumente in Ihrer Workfront-Instanz hochgeladen wurde. Anweisungen finden Sie unter <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich Dokumente</a> in diesem Artikel.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     </tr>
    </tbody> 
   </table>

   >[!NOTE]
   >Bei PDFs wird empfohlen, „Groß“ für die Anzeigegröße des Widgets zu verwenden.
   >Der PDF-Viewer eines Browsers wirkt sich auf die Anzeige für Benutzende aus. Wenn die PDF-Anzeige nicht optimal ist, müssen diese möglicherweise ihre Fenstergröße und ihren Browser-Zoom-Prozentsatz anpassen.

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![copy icon](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

#### Hinzufügen eines Videos zu einem benutzerdefinierten Formular aus dem Bereich Dokumente{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wenn Sie auf diese Weise ein Video zu einem benutzerdefinierten Formular hinzufügen, gelten die im Bereich Dokumente festgelegten Berechtigungen für das Video, wenn Benutzer auf das Formular auf einem Objekt zugreifen.

1. Gehen Sie zum Video im Bereich Dokumente und generieren Sie einen Korrekturabzug dafür, wie in [Erstellen eines interaktiven Korrekturabzugs für eine Website oder andere Web-Inhalte](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md) beschrieben.
1. Öffnen Sie den Korrekturabzug.
1. Klicken Sie mit der rechten Maustaste auf eine beliebige Stelle im Video und wählen Sie **Videoadresse kopieren**.
1. Fügen Sie im benutzerdefinierten Formular, in dem Sie das Video-Widget hinzufügen, die kopierte Adresse in das Feld **URL** ein.
1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Native Workfront-Felder hinzufügen

Sie können Ihren benutzerdefinierten Formularen native Workfront-Felder hinzufügen. Wenn das benutzerdefinierte Formular an ein Objekt angehängt wird, wird das Feld aus den Objektdaten gefüllt. Beispielsweise ruft das Feld Beschreibung in einem benutzerdefinierten Formular, das an ein Projekt angehängt ist, die Projektbeschreibung ab. (Wenn keine Daten verfügbar sind, kann das Feld „K. A.“ anzeigen.)

+++ Erweitern Sie , um die Liste der unterstützten nativen Felder anzuzeigen.

In dieser Tabelle sind die verfügbaren nativen Felder für bestimmte Workfront-Objekte in einem benutzerdefinierten Formular aufgeführt.

| Feldname | Projekt | Aufgabe | Problem | Vorlage | Vorlagenaufgabe | Portfolio | Programm | Gruppe |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Tatsächliches Abschlussdatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Tatsächliche Dauer | ✓ |   |   |   |   |   |   |   |
| Tatsächliche Stunden | ✓ |   | ✓ |   |   |   |   |   |
| Tatsächliches Startdatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Firma | ✓ |   |   | ✓ |   |   |   |   |
| Bedingung | ✓ | ✓ | ✓ |   |   |   |   |   |
| Bedingungstyp | ✓ |   |   | ✓ |   |   |   |   |
| Beschreibung | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Dauer |   | ✓ |   |   | ✓ |   |   |   |
| Dauertyp |   | ✓ |   |   | ✓ |   |   |   |
| Dauer - Einheit |   | ✓ |   |   | ✓ |   |   |   |
| Eingegeben von | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Eingabedatum | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| Gruppe | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Zuletzt aktualisiert von | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Datum der letzten Aktualisierung | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Name | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Besitzer | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| Geplantes Abschlussdatum | ✓ | ✓ | ✓ |   |   |   |   |   |
| Geplante Dauer | ✓ |   |   | ✓ |   |   |   |   |
| Geplante Stunden | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| Geplantes Startdatum | ✓ |   |   |   |   |   |   |   |
| Portfolio | ✓ |   |   | ✓ |   |   | ✓ |   |
| Priorität | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Programm | ✓ |   |   | ✓ |   |   |   |   |
| Voraussichtliches Abschlussdatum | ✓ | ✓ |   |   |   |   |   |   |
| Geplante Dauer in Minuten |   | ✓ |   |   |   |   |   |   |
| Voraussichtlicher Starttermin | ✓ | ✓ |   |   |   |   |   |   |
| Referenznummer | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| Zeitplanmodus | ✓ |   |   | ✓ |   |   |   |   |
| Schweregrad |   |   | ✓ |   |   |   |   |   |
| Sponsor | ✓ |   |   | ✓ |   |   |   |   |
| Status | ✓ | ✓ |   |   |   |   |   |   |
| Story-Punkte |   | ✓ |   |   |   |   |   |   |
| Vorlage | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite nach **Nativer Feldverweis** und ziehen Sie ihn in einen Abschnitt auf der Arbeitsfläche.
1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen für das benutzerdefinierte Feld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie die Anzeigegröße des Felds nach Bedarf.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td>
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Feld. Wenn Sie das Feld zum ersten Mal konfigurieren und die Bezeichnung eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
      <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Referenzfeld</td> 
      <td><p>(Erforderlich) Wählen Sie ein natives Workfront-Feld aus.<p><p>Für die Objekte des Formulars sind nur native Felder verfügbar. Wenn beispielsweise die Liste Objekttypen oben im Formular-Designer „Projekt“ anzeigt, können Sie native Felder für Projekte auswählen, jedoch keine Felder, die speziell für Aufgaben verwendet werden.</p></td>
     </tr>
     <tr>
      <td role="rowheader">Filter hinzufügen</td>
      <td><p>Fügen Sie einen Filter für das Referenzfeld hinzu, um die Liste der Elemente zu begrenzen, aus denen Benutzerinnen und Benutzer bei der Verwendung des Felds auswählen können. </p> <p>Sie können beispielsweise ein Feld so beschränken, dass Benutzernamen nur ausgewählt werden können, wenn sie die folgenden Kriterien erfüllen:</p> 
       <ul>
        <li>Sie gehören zu einer oder mehreren Gruppen, die Sie angeben.</li> 
        <li>Sie sind mit einer von Ihnen angegebenen Funktion oder einem von Ihnen angegebenen Titel verknüpft.</li> 
        <li>Sie gehören zur selben Gruppe wie die Person, die das Feld verwendet.</li> 
       </ul>
       <p>Sie müssen den Filter für das von Ihnen ausgewählte Referenzfeld mithilfe der Textmodussyntax definieren. Weitere Informationen finden Sie unter <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Bearbeiten eines Filters im Textmodus</a>.</p>
       <p><b>Hinweis</b>:
       <ul> 
        <li>Die Filteroption ist nur verfügbar, wenn Sie auf ein natives Feld mit automatischer Textvervollständigung verweisen, z. B. Portfolio, Unternehmen oder Inhaber.</li>
        <li>Wenn Sie ein vorhandenes benutzerdefiniertes Formular bearbeiten, werden beim Hinzufügen eines Filters zu einem nativen Feld keine Objekte entfernt (außerhalb des Bereichs des Filters), die Benutzende bereits mithilfe des Felds hinzugefügt haben.</li> 
        <li>Dieser Filter ist auf Mobilgeräten nicht verfügbar. Wenn Sie den Filter für ein natives Feld verwenden, wird das Feld auf den Mobilgeräten der Benutzer angezeigt, ohne vom Filter betroffen zu sein.</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td>
      <td><p>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Adobe XD-Dateien hinzufügen

Sie können einen Adobe XD-Prototyp direkt zu einem benutzerdefinierten Formular hinzufügen. Benutzende, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können die Adobe XD-Datei nur in den folgenden Bereichen sehen:

* Der Bereich Details des Objekts (z. B. für ein Projekt der Bereich Projektdetails)
* Das Bearbeitungsfeld für das Objekt, wenn es das neue Erscheinungsbild von Adobe Workfront aufweist (z. B. die Felder Projekt bearbeiten und Aufgabe bearbeiten )

Hinzufügen einer Adobe XD-Datei:

1. Suchen Sie auf **Registerkarte** Neues Feld“ auf der linken Bildschirmseite nach **Adobe XD** und ziehen Sie es in einen Abschnitt auf der Arbeitsfläche.
1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie die Anzeigegröße des Widgets nach Bedarf.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Beschriftung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Beschriftung keine Sonderzeichen, da diese in Berichten nicht korrekt angezeigt werden. Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget. Wenn Sie das Widget zum ersten Mal konfigurieren und die Beschriftung eingeben, wird das Feld Name automatisch ausgefüllt, damit es übereinstimmt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p>
    <p>Weitere Informationen finden Sie unter <a href="design-a-form.md#notes-on-field-names-and-labels">Hinweise zu Feldnamen und Beschriftungen</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben Sie einen gültigen XD-Prototyp-Link ein oder fügen Sie ihn ein.</p> 
      <p><b>Hinweis</b>: Die Einstellung „Link-Zugriff“ auf der Registerkarte Freigeben in Adobe XD muss auf „Jeder, der über den Link verfügt“ festgelegt sein. Andernfalls können Benutzende den Prototyp nicht anzeigen. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr>
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     </tr>
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder oder Widgets hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![copy icon](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

### Planning-Verbindungsfelder hinzufügen

>[!IMPORTANT]
>
>Die Informationen in diesem Abschnitt beziehen sich auf Adobe Workfront Planning, eine zusätzliche Funktion von Adobe Workfront.
>
>Sie benötigen zusätzliche Pakete, um auf Workfront Planning zugreifen zu können.
>
>Eine vollständige Liste der Anforderungen für den Zugriff auf Workfront Planning finden Sie unter [Zugriffsübersicht für Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Weitere Informationen zur Workfront-Planung finden Sie unter [Erste Schritte mit Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md).

Sie können Datensätze, die über Workfront Planning verbunden sind, in einem benutzerdefinierten Feld eines Workfront-Objekts anzeigen, indem Sie dem benutzerdefinierten Formular eines Objekts ein benutzerdefiniertes Feld für die Planning-Verbindung hinzufügen.

Sie können das Feld Planning-Verbindung zu den benutzerdefinierten Formularen aller Objekte hinzufügen. Sie können verbundene Datensätze jedoch nur in den benutzerdefinierten Formularen anzeigen, die mit Workfront-Objekten verknüpft sind und über Workfront Planning verbunden werden können.

>[!NOTE]
>
>Benutzer, die Informationen im benutzerdefinierten Feld anzeigen, müssen Zugriff auf Workfront Planning und auf die Arbeitsbereiche haben, die die mit Workfront-Objekten verbundenen Datensatztypen enthalten.

So fügen Sie ein Feld für eine Planungsverbindung hinzu:

1. Suchen Sie in der **&#x200B;**&#x200B;Neues Feld auf der linken Bildschirmseite nach **Planning-Verbindung** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.
1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen für das benutzerdefinierte Feld:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie die Anzeigegröße des Widgets nach Bedarf.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>Wichtig</b>: Verwenden Sie in dieser Kennzeichnung keine Sonderzeichen.</p> 
      <p>Es wird empfohlen, einen Titel auszuwählen, anhand dessen Sie leicht erkennen können, woher der Planungsdatensatz stammt. Fügen Sie Informationen wie den Namen des Arbeitsbereichs oder den Namen des Datensatztyps hinzu. </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td>
      <td> <p>(Erforderlich) Der Name gibt an, wie das System das Feld identifiziert. Wenn Sie das Feld zum ersten Mal konfigurieren und die Bezeichnung eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden nicht synchronisiert. Dadurch haben Sie die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzerinnen und Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>(Empfohlen) Geben Sie zusätzliche Informationen zum Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p>
      <p>Hier können Sie detaillierte Informationen über den Datensatz und die Objekte hinzufügen, die Sie verbinden. </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objekttyp</td> 
      <td><p>(Erforderlich) Wählen Sie einen Workfront-Objekttyp aus, der mit einem Datensatztyp in Workfront Planning verbunden ist.</p>
      Sie können aus den folgenden Objekttypen auswählen:
      <ul><li> Projekt</li>
      <li> Portfolio</li><li> Programm</li><li> Firma</li><li> Gruppe</li></ul>
       <p>Es sind nur Workfront-Objekttypen für die Objekttypen des Formulars verfügbar.</p> <p> Wenn beispielsweise in der Liste „Objekttypen“ oben im Formular-Designer „Projekt“ angezeigt wird, können Sie in diesem Feld nur „Projekt“ und nicht „Portfolios“ auswählen. Portfolios können aber auch mit Datensatztypen verbunden werden.</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Arbeitsbereich</td> 
      <td> <p>(Erforderlich) Wählen Sie den Arbeitsbereich Planung aus, aus dem die Datensätze stammen, die in Workfront angezeigt werden sollen.</p> <p> Es werden nur Arbeitsbereiche angezeigt, die mit den im Feld Objekttyp ausgewählten Objekttypen verbunden sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eintragstyp</td> 
      <td><p>(Erforderlich) Wählen Sie den Workfront Planning-Datensatztyp aus, der über eine Verbindung mit dem Workfront-Objekttyp verfügt.</p><p>Es werden nur Datensatztypen angezeigt, die Verbindungen zu dem im Feld Objekttyp ausgewählten Objekttyp haben. </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Verbindungsfeld</td> 
      <td><p>(Erforderlich) Wählen Sie das Verbindungsfeld zwischen dem ausgewählten Planungs-Datensatztyp, den Sie auf den Workfront-Objekten anzeigen möchten, und dem Workfront-Objekttyp aus. </p> <p> <b>Hinweis</b>: Sie können mehrere Verbindungsfelder zwischen demselben Objekt und Datensatztyp haben, aber Sie können nur ein Feld auswählen.</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">Eintragstypfelder</td> 
      <td><p>(Optional) Wählen Sie aus dem verbundenen Datensatztyp bis zu 7 Suchfelder aus, die im benutzerdefinierten Formular angezeigt werden sollen. Das primäre Feld ist standardmäßig ausgewählt und kann nicht bearbeitet werden. </p> <p> Die ausgewählten Felder des verbundenen Datensatzes werden in einer Tabellenansicht im benutzerdefinierten Formular angezeigt. Wenn das Formular mit einem Workfront-Objekt verbunden ist, ist die Tabellenansicht schreibgeschützt. </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
     <tr>
      <td>Aktiv</td>
      <td><p>Diese Option ist standardmäßig aktiviert.<p><p>Wenn Sie ein Feld als inaktiv festlegen, wird es aus Berichten, Filtern und Ansichten ausgeschlossen und ist nicht mehr in der Feldbibliothek für benutzerdefinierte Formulare verfügbar.</p></td>
     </tr>
      </tbody> 
   </table>

1. (Optional) Wiederholen Sie die vorherigen Schritte, um weitere Felder hinzuzufügen.

   ODER

   Um ein Feld zu kopieren, bewegen Sie den Mauszeiger über ein Feld und klicken Sie auf das Kopiersymbol.

   ![copy icon](assets/copy-field.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   ODER

   Klicken Sie **Speichern und schließen**.

   Sie können das Formular jetzt an ein Objekt anhängen, das über Workfront Planning verbunden ist, und einen der folgenden Schritte ausführen:

   * Anzeigen von Workfront Planning-Datensatztypen, die mit dem Workfront-Objekt verbunden sind, falls vorhanden.
   * Verbinden von Datensätzen mit dem Workfront-Objekt oder Trennen von Datensätzen.

   Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen aus Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

### Hinzufügen von Benutzeroberflächenerweiterungen

Eine App kann mithilfe des Feldtyps UI-Erweiterungen in ein benutzerdefiniertes Workfront-Formular eingebettet werden. Um Benutzeroberflächenerweiterungen zu erstellen, benötigen Sie Zugriff auf Adobe App Builder in der Adobe Developer Console. Weitere Informationen finden Sie unter [Einbetten einer App mit einem benutzerdefinierten Workfront](/help/quicksilver/app-builder/app-builder.md#embed-an-app-using-a-workfront-custom-form) im Artikel [Erstellen benutzerdefinierter Programme für Workfront mit Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Organisieren und Vorschau eines Formulars mit dem Formular-Designer

Informationen zum Organisieren eines benutzerdefinierten Formulars mit Abschnittsumbrüchen und zum Anzeigen einer Vorschau des Formulars finden Sie unter [Organisieren und Vorschau eines Formulars mit dem Formular-Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).



