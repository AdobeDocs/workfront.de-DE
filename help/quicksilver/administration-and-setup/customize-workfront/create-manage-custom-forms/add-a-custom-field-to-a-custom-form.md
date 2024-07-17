---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular mit dem Legacy-Formular hinzufügen
description: Wenn Sie an einem benutzerdefinierten Formular arbeiten, können Sie ein neues benutzerdefiniertes Feld erstellen und es zu einem benutzerdefinierten Formular hinzufügen. Sie können auch ein benutzerdefiniertes Feld hinzufügen, das bereits einem anderen benutzerdefinierten Formular hinzugefügt wurde.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 2%

---

# Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular mit dem Legacy-Formular hinzufügen

<!-- Audited: 02/2024 -->

{{form-designer-default}}

Wenn Sie an einem benutzerdefinierten Formular arbeiten, können Sie ein neues benutzerdefiniertes Feld erstellen und es zu einem benutzerdefinierten Formular hinzufügen.

Sie können auch ein benutzerdefiniertes Feld hinzufügen, das bereits einem anderen benutzerdefinierten Formular hinzugefügt wurde. Anweisungen finden Sie unter [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Weitere Informationen zum Hinzufügen eines Asset-Widgets zu einem benutzerdefinierten Formular, bei dem es sich um einen Prozess handelt, der dem Hinzufügen eines benutzerdefinierten Felds ähnelt, finden Sie unter [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>In einem benutzerdefinierten Formular, das viele benutzerdefinierte Felder oder eine Vielzahl von Mehrfachauswahloptionen in benutzerdefinierten Feldern enthält, kann es vorkommen, dass Benutzer beim Hinzufügen oder Ändern von Werten in diesen Feldern langsamer arbeiten. Beispielsweise kann ein Formular mit 100 benutzerdefinierten Feldern oder benutzerdefinierten Feldern mit mehreren Auswahlen mit mehr als 200 Optionen langsamer sein, wenn Benutzer damit interagieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td>Administratorzugriff auf benutzerdefinierte Formulare </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen {#add-custom-field-to-custom-form}

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie in [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) beschrieben.
1. Wählen Sie die Registerkarte **Feld hinzufügen** aus.

   ![Registerkarte &quot;Feld hinzufügen&quot;](assets/add-a-field.jpg)

1. Wählen Sie bei ausgewähltem Symbol **Neues Feld** ![Neues Feld](assets/new-field.jpg) einen der folgenden Feldtypen aus:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Textfeld mit einzelner Zeile</td> 
      <td>Ermöglicht Benutzern die Eingabe einer einzelnen Textzeile in das Feld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Absatztextfeld</td> 
      <td>Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Textfeld mit Formatierung</td> 
      <td>Ermöglicht Benutzern die Eingabe mehrerer Textzeilen in das Feld und die Formatierung des Texts mit fett, kursiv, unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen. Dies ist für Workfront-Objekte auf der Startseite, im Bereich "Updates", in Listen und im Bereich "Details"verfügbar. Eine Zeichenbeschränkung von 15.000 ermöglicht viel Text und Formatierung.</p> <p>Dieser benutzerdefinierte Feldtyp wird in Filtern für Listen und Berichte nicht unterstützt.</p> <p>Informationen zum Zugriff auf dieses Feld über die API finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Speicherung von Rich-Text-Feldern in der API</a>.</p> <p><b>HINWEIS</b>: Textfelder mit Formatierung sind nicht für mobile Workfront-Apps verfügbar. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dropdown</td> 
      <td>Bietet eine Liste von Dropdown-Optionen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typeahead </td> 
      <td>Ermöglicht Benutzern die Eingabe des Namens eines Objekts, das in Workfront vorhanden ist. Eine Liste mit Vorschlägen wird angezeigt, wenn der Benutzer mit der Eingabe beginnt.
      Dieser Feldtyp unterstützt die folgenden Objekte:
      <ul><li>Benutzerin oder Benutzer</li>
      <li>Gruppe</li>
      <li>Aufgabengebiet</li>
      <li>Portfolio</li>
      <li>Programm</li>
      <li>Projekt</li>
      <li>Team</li>
      <li>Vorlage</li>
      <li>Firma</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechnet</td> 
      <td>Ermöglicht die Definition eines Ausdrucks und die Anzeige des Ergebnisses im benutzerdefinierten Formular. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datum</td> 
      <td>Zeigt einen Kalender an, in dem Benutzer Datum und Uhrzeit auswählen können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kontrollkästchen</td> 
      <td>Ermöglicht Benutzern die Auswahl mehrerer Optionen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Optionsschaltflächen</td> 
      <td>Erfordert, dass Benutzer nur eine Auswahl auswählen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibender Text</td> 
      <td>Ermöglicht das Einfügen von Anweisungen und das Verknüpfen mit Seiten außerhalb von Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abschnittsumbruch</td> 
      <td>Eine Abschnittspause ist eigentlich kein Feld. Sie können einen Abschnittsumbruch verwenden, um Ihre benutzerdefinierten Felder und Widgets in Abschnitte zu organisieren und bei Bedarf für jeden Abschnitt verschiedene Anzeige- und Bearbeitungsberechtigungen zu konfigurieren. Weitere Informationen zum Hinzufügen und Konfigurieren von Abschnittsumbrüchen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Hinzufügen eines Abschnittsumbruchs zu einem benutzerdefinierten Formular</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Felder, die mehrere Auswahlmöglichkeiten zulassen, wie das Kontrollkästchen und das Dropdown-Menü, sind in Berichten schwer zu grafisch und gruppieren. Um eine einfachere Diagrammerstellung und Gruppierung in Berichten zu ermöglichen, können Sie für jede Auswahl separate Felder erstellen (z. B. ein einzeiliges Textfeld).

1. Konfigurieren Sie auf der Registerkarte **Feldeinstellungen** die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem benutzerdefinierten Feld angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das benutzerdefinierte Feld, wenn Sie es zu verschiedenen Bereichen in Workfront hinzufügen, z. B. zu Berichten, Startseite und API-Interaktionen.</p> <p>Wenn Sie das benutzerdefinierte Feld zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> 
      <p><b>WICHTIG</b>:   
      <ul> 
      <li>Obwohl dies möglich ist, sollten Sie diesen Namen nicht ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Workfront begonnen haben. Wenn dies der Fall ist, erkennt das System das benutzerdefinierte Feld nicht mehr, in dem es jetzt in anderen Bereichen von Workfront referenziert werden kann. <p>Wenn Sie beispielsweise das benutzerdefinierte Feld zu einem Bericht hinzufügen und später seinen Namen ändern, erkennt Workfront es nicht im Bericht und funktioniert dort nicht mehr ordnungsgemäß, es sei denn, Sie fügen es dem Bericht unter Verwendung des neuen Namens erneut hinzu.</p> </li>
      <li> <p>Es wird empfohlen, keinen Namen einzugeben, der bereits für integrierte Workfront-Felder verwendet wurde.</p> </li>
      <li><p>Es wird empfohlen, das Punkt-/Punkt-Zeichen nicht im benutzerdefinierten Feldnamen zu verwenden, um Fehler bei der Verwendung des Felds in verschiedenen Bereichen von Workfront zu vermeiden.</p></li>
      </ul> <p>Jeder benutzerdefinierte Feldname muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. Weitere Informationen finden Sie unter <a href="#add-a-custom-field-to-a-custom-form">Hinzufügen eines benutzerdefinierten Felds zu einem benutzerdefinierten Formular</a> in diesem Artikel.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Anleitung</td> 
      <td> <p>Geben Sie zusätzliche Informationen zum benutzerdefinierten Feld ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Wählen Sie den Datentyp aus, der im benutzerdefinierten Feld erfasst werden soll. Sie können die Formatauswahl nach dem Speichern des Formulars ändern. Das neue Format muss jedoch den eingegebenen Wert unterstützen.</p>

   <p><strong>Beispiel:</strong> Wenn Sie einen numerischen Wert für ein Feld mit Textformat für mindestens ein Objekt speichern und das Format später in Zahl oder Währung ändern, tritt kein Fehler auf. </p>
      <p>Wenn Sie jedoch einen alphanumerischen Wert in einem Feld mit dem Textformat für mindestens ein Objekt speichern und dann versuchen, das Format in Zahl oder Währung zu ändern, wird ein Fehler ausgegeben, da der gespeicherte alphanumerische Wert nicht mit den Formaten Zahl oder Währung kompatibel ist. </p>

   <p><strong>Hinweis:</strong> Die Zeichenbeschränkung für Zahlenfelder beträgt 16. Sie können auch ein Textfeld verwenden, um Zahlen einzugeben und die Begrenzung zu vermeiden.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigetyp</td> 
      <td>(Nur Dropdown, Checkboxes und Optionsfelder) Wechseln Sie den gewünschten Optionstyp für das Feld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Nur Textfelder) Wählen Sie eine Breite für das Feld aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tageszeit anzeigen</td> 
      <td>(Nur Datumsfelder) Wählen Sie diese Option aus, wenn Sie die Tageszeit zusammen mit dem Datum im Feld anzeigen möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Referenzierter Objekttyp</td> 
      <td> <p>(Nur Eingabefelder) Wählen Sie den Objekttyp aus, den Sie mit dem Feld verknüpfen möchten.</p> <p>Nachdem Sie auf Übernehmen oder Speichern+Schließen geklickt haben, können Sie den Objekttyp für das Feld nicht mehr ändern.</p> <p><b>NOTE</b>:   
        <ul> 
         <li>Wenn Ihr Workfront-Administrator den Namen für Portfolios, Programme oder Projekte in der Benutzeroberfläche von Workfront angepasst hat, wird der standardmäßige Workfront-Name für das Objekt in dieser Dropdownliste und nicht der benutzerdefinierte Name angezeigt. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Hilfe dazu benötigen.<br></li> 
         <li>Die folgenden Objekttypen werden in den mobilen Apps von iOS und Android Workfront unterstützt: Benutzer, Unternehmen, Gruppe, Auftragsrolle, Portfolio, Programm, Projekt und Vorlage.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Filter hinzufügen</td> 
      <td> <p>(Nur Felder vom Typ voraus) Fügen Sie einen Filter für einen Objekttyp hinzu, um die Objekte einzuschränken, die Benutzer bei der Verwendung des Felds auswählen können. </p> <p>Sie können beispielsweise ein Feld so einschränken, dass Benutzernamen nur ausgewählt werden können, wenn sie die folgenden Kriterien erfüllen:</p> 
       <ul> 
        <li>Sie gehören zu einer oder mehreren Gruppen, die Sie angeben</li> 
        <li>Sie sind mit einer von Ihnen angegebenen Rolle oder Berufsbezeichnung verknüpft.</li> 
        <li>Sie gehören zur gleichen Gruppe wie die Person, die das Feld verwendet</li> 
       </ul> <p>Sie müssen den Filter für den ausgewählten Objekttyp mithilfe der Textmodus-Syntax definieren. Informationen zum Erstellen eines Filters mit dem Textmodus finden Sie unter <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Bearbeiten eines Filters mit dem Textmodus</a>.</p>
       <p><b>NOTE</b>:   
        <ul> 
         <li>Wenn Sie ein vorhandenes benutzerdefiniertes Formular bearbeiten, werden durch Hinzufügen eines Filters zu einem Feld vom TypAhead keine Objekte (außerhalb des Filterbereichs) entfernt, die Benutzer bereits über das Feld hinzugefügt haben.</li> 
         <li>Dieser Filter ist auf Mobilgeräten nicht verfügbar. Wenn Sie den Filter für ein Feld vom Typ voraus verwenden, wird das Feld auf den Mobilgeräten der Benutzer angezeigt, die vom Filter nicht betroffen sind.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibender Text</td> 
      <td>(Nur beschreibende Textfelder) Geben Sie den Text ein, der angezeigt werden soll, um Anweisungen oder einen Link auf das benutzerdefinierte Formular bereitzustellen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hyperlink</td> 
      <td>(Nur beschreibende Textfelder) Wenn Sie einen Hyperlink auf den eingegebenen beschreibenden Text anwenden möchten, fügen Sie ihn hier hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zu einem Pflichtfeld machen</td> 
      <td>Wählen Sie diese Option aus, wenn das Feld erforderlich sein soll, damit der Benutzer das benutzerdefinierte Formular ausfüllen kann. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feldänderungen in Aktualisierungs-Feeds nachverfolgen</td> 
      <td><p>Klicken Sie auf die Dropdown-Liste und wählen Sie dann die Objekttypen aus, bei denen die Werteänderungen des Felds automatisch verfolgt werden sollen.</p> 
      <p><b>HINWEIS</b>: Diese Option ist für Folgendes nicht verfügbar:</p> 
      <ul> 
      <li>Benutzerdefinierte Formulare, die den folgenden Objekttypen zugeordnet sind: Ausgaben, Firma, Iteration, Rechnungsdatensatz, Dokument und Gruppe.</li> 
      <li>Die folgenden Feldtypen: Berechneter, beschreibender Text und Abschnittsumbruch</li> 
      </ul>
      <p><b>WICHTIG</b>: Die Auswahl oder Deaktivierung eines Objekttyps wirkt sich auf alle benutzerdefinierten Formulare aus, die mit dem ausgewählten Objekttyp verknüpft sind und dieses Feld enthalten. Wenn Sie beispielsweise die Auswahl eines Objekttyps hier aufheben und das benutzerdefinierte Formular speichern, werden die Werteänderungen des Felds für diesen Objekttyp in keinem benutzerdefinierten Formular mehr verfolgt, das das Feld enthält.</p>
       <p>Nachdem Sie hier einen Objekttyp für ein Feld ausgewählt und das benutzerdefinierte Formular gespeichert haben, wird das Feld auf der Registerkarte "Benutzerdefinierte Felder"im Bereich "Feeds aktualisieren"unter "Einrichtung"angezeigt.</p> 
       <p>Wenn dieses Feld dagegen im Bereich "Feeds aktualisieren"unter "Einrichtung"gelöscht wird, wird der Objekttyp für diese Einstellung für alle benutzerdefinierten Formulare deaktiviert, die mit dem Objekttyp verknüpft sind und dieses Feld enthalten.</p> 
       <p>Weitere Informationen finden Sie im Abschnitt <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Felder hinzufügen, die Workfront verfolgen soll</a> im Artikel <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Systemaktualisierungen konfigurieren</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logik hinzufügen</td>
      <td>Geben Sie an, welche Felder im Formular angezeigt werden sollen, basierend auf den Auswahlen, die Benutzer in vorhandenen Feldern treffen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Hinzufügen der Anzeigelogik und Überspringen der Logik in ein benutzerdefiniertes Formular</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Auswahl </td> 
      <td> <p>(Nur Dropdown-, Kontrollkästchen- oder Optionsfelder; optional)</p> 
       <ol> 
        <li> <p>Klicken Sie auf <b>Optionen</b> und aktivieren Sie dann eine der folgenden Optionen:</p> 
           <ul> 
            <li><strong>Werte anzeigen</strong>: Zeigt die Werte jeder Auswahl im Feld an. Der Titel jeder Auswahl wird standardmäßig angezeigt.</li> 
            <li><strong>Sortieroptionen A-Z</strong>: Sortiert die Auswahlmöglichkeiten, die Sie dem Feld alphabetisch hinzufügen.</li> 
           </ul> 
        </li> 
        <li> <p>Klicken Sie für jede Auswahlmöglichkeit, die Sie für den Benutzer hinzufügen, auf das Zahnradsymbol <img src="assets/gear-icon-settings.png"> und wählen Sie dann eine der folgenden Optionen aus:</p> 
           <ul> 
            <li><strong>Standardmäßig auswählen</strong>: Wählen Sie im Feld standardmäßig die Auswahl aus.</li> 
            <li> <p><strong>Auswahl ausblenden</strong>: Blendet die Auswahl im Feld aus. Ausgeblendete Optionen stehen in Berichten weiterhin zur Verfügung.</p> </li> 
            <li> <p><strong>Auswahl entfernen</strong>: Entfernt die Auswahl aus dem Feld.</p> <p><b>WARNUNG</b>: Wenn Sie aktuelle Objekte haben, die diese Auswahl verwenden, entfernen Sie sie nicht aus dem Feld. Wenn Sie sie entfernen, gehen historische Daten verloren. Wählen Sie stattdessen die Option aus, um sie auszublenden. Dies verhindert, dass Benutzer sie in Zukunft auswählen.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Um den Anzeigetyp eines Felds im benutzerdefinierten Formular zu ändern, klicken Sie auf das Dropdown-Menü **Anzeigetyp** und dann auf den gewünschten Typ.

   Sie können zwischen den folgenden Feldanzeigetypen wechseln:

   * **Auswahlfelder**: Kontrollkästchen, Dropdown, Optionsfelder.
   * **Textfelder**: Einzelzeilentext, Absatztext-Feld. (Sie können ein Textfeld mit Formatierung nicht in einen anderen Anzeigetyp wechseln. Sie können sie jedoch entfernen und einen anderen Feldtyp hinzufügen.)

   Wenn Sie beispielsweise ein Kontrollkästchen-Feld erstellt haben, können Sie es in ein Dropdown-Feld oder ein Optionsfeld ändern. Wenn Sie ein einzeiliges Textfeld erstellt haben, können Sie es in ein Absatztext -Feld ändern.

   >[!NOTE]
   >
   >Beachten Sie Folgendes, wenn Sie den Anzeigetyp eines Felds von einem Kontrollkästchen- oder Dropdown-Feld mit Mehrfachauswahl (eine Dropdown-Liste, in der mehr als eine Option ausgewählt werden kann) in einen Feldtyp mit Einzelauswahl ändern möchten:
   >
   >* Wenn Sie zu &quot;Optionsfelder&quot;wechseln, behält Workfront alle Mehrfachauswahlwerte bei, die ein Benutzer in das Feld eingegeben hat, bis der Benutzer Daten in einem beliebigen Teil des Formulars ändert und speichert. An dieser Stelle werden alle Werte, die mit dem Feld vom Typ Mehrfachauswahl ausgewählt wurden, durch den ausgewählten Wert für Optionsfelder ersetzt.
   >* Wenn Sie zu einem Dropdown-Menü mit nur einer Auswahl wechseln, behält Workfront alle Mehrfachauswahlwerte bei, die ein Benutzer möglicherweise in das Feld eingegeben hat, bis der Benutzer die Werte im Feld ändert und speichert. An dieser Stelle werden alle Werte, die mit dem Feld vom Typ Mehrfachauswahl ausgewählt wurden, durch den ausgewählten Dropdown-Wert ersetzt.

1. (Optional) Wiederholen Sie die Schritte 3 bis 5, um weitere benutzerdefinierte Felder hinzuzufügen.

   Oder

   Fügen Sie Felder hinzu, die bereits für Ihre Organisation erstellt wurden, wie unter [Benutzerdefiniertes Feld oder Widget in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md) beschrieben.

   >[!NOTE]
   >
   >Sie können bis zu 500 Felder und Widgets in einem einzelnen benutzerdefinierten Formular hinzufügen. Je nach Komplexität eines Formulars kann die Leistung jedoch beeinträchtigt werden, wenn mehr als 100 Formulare vorhanden sind. Beispiele für komplexe Formulare sind Formulare mit kaskadierenden Parametern, berechnete benutzerdefinierte Datenfelder und Optionen mit mehreren Werten in einem einzelnen Feld.

1. Klicken Sie auf **Anwenden**.
1. Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Positionieren Sie benutzerdefinierte Felder und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Einen Abschnittsumbruch zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigerlogik hinzufügen und Logik in ein benutzerdefiniertes Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Benutzerdefiniertes Formular in der Vorschau anzeigen und ausfüllen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
