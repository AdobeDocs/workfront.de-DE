---
title: Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: In einem benutzerdefinierten Formular können Sie ein berechnetes benutzerdefiniertes Feld erstellen, das Berechnungen generiert. Erstellen Sie dazu eine Anweisung, die Datenausdrücke und die Namen vorhandener Felder verwendet, bei denen es sich um benutzerdefinierte Felder, berechnete benutzerdefinierte Datenfelder und integrierte Workfront-Felder handeln kann. Diese Anweisung berechnet die eingegebenen Daten und zeigt das Ergebnis im neuen berechneten benutzerdefinierten Feld an.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '2863'
ht-degree: 0%

---

# Hinzufügen berechneter Daten zu einem benutzerdefinierten Formular mit dem Legacy-Formular

<!--Audited: 01/2024-->

In einem benutzerdefinierten Formular können Sie ein berechnetes benutzerdefiniertes Feld hinzufügen, das vorhandene Daten verwendet, um neue Daten zu generieren, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.

Erstellen Sie dazu eine Anweisung, die Datenausdrücke und die Namen vorhandener Felder verwendet, bei denen es sich um benutzerdefinierte Felder, berechnete benutzerdefinierte Datenfelder und integrierte Adobe Workfront-Felder handeln kann.

Diese Anweisung berechnet die eingegebenen Daten und zeigt das Ergebnis im neuen berechneten benutzerdefinierten Feld an.

Ein berechnetes benutzerdefiniertes Feld kann Folgendes enthalten:

* Ein einfacher Verweis auf ein einzelnes integriertes Feld.

  >[!INFO]
  >
  > **Beispiel:** Um den Umsatz zu berechnen, der durch Projekte und Aufgaben generiert wurde, können Sie ein berechnetes benutzerdefiniertes Feld erstellen, das das integrierte Feld &quot;Tatsächlicher Umsatz&quot;enthält. Wenn ein Benutzer das benutzerdefinierte Formular an ein Projekt oder eine Aufgabe anhängt, wird der Umsatz für das Projekt oder die Aufgabe im Feld angezeigt.

* Ein Ausdruck, der auf ein oder mehrere Felder verweist. Dabei kann es sich um benutzerdefinierte Felder, andere berechnete benutzerdefinierte Felder und integrierte Felder handeln.

  >[!INFO]
  >
  >**Beispiel:** Um den durch Projekte und Aufgaben generierten Gewinn zu berechnen, können Sie ein berechnetes benutzerdefiniertes Feld namens Profit erstellen, das einen mathematischen Ausdruck enthält, der Kosten vom Umsatz abzieht.
  >
  >Dazu können Sie den mathematischen Ausdruck SUB (subtract) mit den integrierten Workfront-Feldern Tatsächliche Kosten und tatsächliche Umsätze verwenden.
  >
  >In den folgenden Schritten sehen Sie, wie dieses Beispiel ausgeführt werden kann.

Informationen zum Erstellen benutzerdefinierter Formulare für Ihre Organisation und zum Verständnis des Typs der Felder, die Sie ihnen zuordnen können, finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Aktuell: Plan</p>
   Oder
   <p>Neu: Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </p> </td> 
  </tr>  
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden. Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Berechnetes Feld zu einem benutzerdefinierten Formular hinzufügen {#add-a-calculated-field-to-a-custom-form}

Sie können sowohl integrierte Workfront-Felder als auch benutzerdefinierte Felder verwenden, die Sie bereits im Ausdruck eines berechneten benutzerdefinierten Felds erstellt haben.

>[!IMPORTANT]
>
>Bevor Sie ein berechnetes benutzerdefiniertes Feld erstellen, identifizieren Sie die vorhandenen Felder, die Sie einbeziehen möchten, damit Sie sicher sind, dass die für die Berechnung erforderlichen Daten in Workfront vorhanden sind.

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Im **Feld hinzufügen** Registerkarte, klicken **Berechnet**.

   Im Anzeigebereich auf der rechten Seite zeigt das Feld den Füllwert 12345 an. Dies ist ein Hinweis, der Sie daran erinnert, dass es sich bei dem Feld um ein berechnetes benutzerdefiniertes Feld handelt, während Sie das benutzerdefinierte Formular erstellen oder bearbeiten. Wenn das Formular an ein Objekt angehängt ist und Benutzer es ausfüllen, sehen sie das Ergebnis der Berechnung im Feld und nicht den Wert 12345.

1. Geben Sie die folgenden Informationen für das berechnete Feld an:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td>Geben Sie eine Beschriftung für das Feld ein. Dies ist es, was Benutzer sehen, wenn sie das benutzerdefinierte Formular verwenden. Das Feld <b>Name</b>, der automatisch ausgefüllt wird und mit der Beschriftung übereinstimmt, wird von Workfront in Berichten referenziert. Dies ist ein Pflichtfeld.</td> 
     </tr>

   <tr> 
   <td role="rowheader">Name</td> 
   <td>Standardmäßig entspricht der Name eines Felds dem Titel. Sie können jedoch den Namen eines Felds so ändern, dass er sich von dem Titel eines Felds unterscheidet. Das Feld <b>Name</b> wird von Workfront in Berichten referenziert. Dies ist ein Pflichtfeld.</td> 
   </tr>

   <tr> 
     <td role="rowheader" id="instructions">Anleitung</td> 
      <td> <p>Fügen Sie Text hinzu, um zusätzliche Informationen über das Feld und die Formel darin bereitzustellen.</p>
      <p>Sie können hier auch die Formel einfügen, die bei der Berechnung des benutzerdefinierten Felds verwendet wird. In diesem Fall sollten Sie zunächst die Berechnung des benutzerdefinierten Felds aktualisieren, dann den endgültigen Ausdruck aus dem Feld Berechnung kopieren und in das Feld Anweisungen einfügen. </p>


   Dies kann auf folgende Weise nützlich sein:
   <ul> 
      <li> <p>Erinnern Sie sich daran, was die Formel ist und wie sie funktioniert. Dies ist besonders hilfreich, wenn Sie dieses berechnete benutzerdefinierte Feld für mehrere Formulare verwenden möchten.</p> </li> 
       <li> <p>Als QuickInfo können Benutzer sehen, wenn sie den Mauszeiger über das Feld bewegen. Sie können hier jeden Text hinzufügen, den Sie in der QuickInfo sehen möchten.</p> </li> 
       </ul>
       <p>Wenn Sie nicht möchten, dass Benutzer die Formel in der QuickInfo sehen, was für sie verwirrend sein kann, fügen Sie sie nicht zum Feld Anweisungen hinzu. Verwenden Sie stattdessen die Einstellung "Formel in Anweisungen anzeigen", um die Formel ein- oder auszublenden, wie in diesem Artikel beschrieben. <a href="#build-the-calculation-for-your-calculated-custom-field">Erstellen Sie die Berechnung für Ihr berechnetes benutzerdefiniertes Feld</a> in diesem Artikel.</p>

   <p>Informationen zur Verwendung desselben berechneten benutzerdefinierten Felds in einem neuen Formular finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden</a>.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Das Format, in dem die Ergebnisse des Felds gespeichert und angezeigt werden sollen.</p> <p>Wenn Sie das Feld in mathematischen Berechnungen verwenden möchten, verwenden Sie immer eine <strong>Zahl</strong> oder <strong>Währung</strong> Format. Wenn Sie "Zahl"oder "Währung"auswählen, schneidet das System automatisch Zahlen ab, die mit 0 beginnen.</p> 
      <p><b>WICHTIG</b>: <p>Bevor Sie ein Format auswählen, sollten Sie das richtige Format für das neue Feld berücksichtigen. Das Formatfeld kann nach dem Speichern des benutzerdefinierten Formulars nicht mehr bearbeitet werden. Die Auswahl des falschen Formats könnte sich auf zukünftige Berechnungen und aggregierte Werte in Berichts- und Listengruppierungen auswirken.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Aktualisieren Sie weiterhin die benutzerdefinierten Feldinformationen, wie im Abschnitt beschrieben. [Erstellen Sie die Berechnung für Ihr berechnetes benutzerdefiniertes Feld](#build-the-calculation-for-your-calculated-custom-field) in diesem Artikel.

## Erstellen Sie die Berechnung für Ihr berechnetes benutzerdefiniertes Feld {#build-the-calculation-for-your-calculated-custom-field}

1. Erstellen Sie das berechnete benutzerdefinierte Feld, wie im Abschnitt beschrieben. [Berechnetes Feld zu einem benutzerdefinierten Formular hinzufügen](#add-a-calculated-field-to-a-custom-form) in diesem Artikel.

1. Klicks **Maximieren** , um die **Berechnungs-Editor** und erstellen Sie Ihre Berechnung.

   >[!INFO]
   >
   >**Beispiel:** Anhand des Beispiels in der Einführung zu diesem Artikel können Sie ein berechnetes benutzerdefiniertes Feld namens &quot;Gewinn&quot;in einem benutzerdefinierten Formular für Projekte und Aufgaben erstellen. Dieses Feld könnte eine Berechnung enthalten, die den Unterschied zwischen tatsächlichem Umsatz und tatsächlichen Kosten anzeigt:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >In diesem Beispiel `SUB` ist der Ausdruck und die referenzierten Felder sind `actualRevenue` und `actualCost`.

   Eine Berechnung beginnt normalerweise mit einem Ausdruck, gefolgt von Klammern, die die Felder enthalten, auf die Sie verweisen möchten, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird. Informationen zu den verfügbaren Ausdrücken finden Sie unter [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Jedes Feld muss von geschweiften Klammern umgeben sein, wie im Abschnitt beschrieben [Syntax in berechneten benutzerdefinierten Feldern erforderlich](#syntax-required-in-calculated-custom-fields) in diesem Artikel. Wenn Sie mit der Eingabe des Namens eines Felds beginnen, unterbreitet das System Vorschläge und Sie können einen Vorschlag auswählen, um ihn in Ihre Berechnung einzufügen.

   >[!NOTE]
   >
   >   In einer Berechnung können keine Felder der folgenden Typen referenziert werden: 
   >   
   >   * Textfeld mit Formatierung
   >   * Beschreibender Text.
   >   
   >   Informationen zu den benutzerdefinierten Feldtypen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).

1. Klicken Sie im Feld &quot;Berechnungs-Editor&quot;auf das große Textfeld, klicken Sie dann auf &quot;Suchen&quot;oder &quot;Erweitern&quot;und klicken Sie auf eine Option aus dem **Ausdruck** und **Felder** rechts neben dem Textfeld. Dadurch werden sie zur Berechnung hinzugefügt.

   Sie können auch mit der Eingabe eines Ausdrucks oder Felds in das große Textfeld beginnen und es dann auswählen, wenn es angezeigt wird. Jedes Element wird mit einem &quot;F&quot;für das Feld oder einem &quot;E&quot;für den Ausdruck angezeigt.

   Wenn Sie eine öffnende Klammer eingeben, wird die schließende Klammer automatisch hinzugefügt.

   >[!TIP]
   >
   >Sie können eine der folgenden Aktionen ausführen, um Hilfe bei der Berechnung zu erhalten:
   > 
   >* Bewegen Sie den Mauszeiger über einen Ausdruck in Ihrer Berechnung, um eine Beschreibung, ein Beispiel, in dem gezeigt wird, wie er verwendet werden kann, und einen Link &quot;Mehr erfahren&quot;zu weiteren Informationen in diesem Artikel anzuzeigen. [Übersicht über berechnete Datenausdrücke](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* Verwenden Sie die Farbcodierung, um die hinzugefügten Komponenten zu identifizieren. Die Ausdrücke werden blau und die Felder grün angezeigt.
   >  ![](assets/colors-fields-expressions.jpg)
   >* Suchen Sie nach Berechnungsfehlern, die bei der Durchführung hervorgehoben sind. Sie können den Mauszeiger über einen hervorgehobenen Fehler bewegen, um eine kurze Beschreibung seiner Ursache anzuzeigen.
   >  ![](assets/error-help.png)
   >* Im **Vorschau auf vorhandenes Objekt** Bereich unterhalb Ihrer Berechnung, beginnen Sie mit der Eingabe des Namens eines Workfront-Objekts und wählen Sie es aus, wenn es in der Liste angezeigt wird. Dadurch erhalten Sie eine Vorschau des Felds, wie es aussieht, wenn das Formular an das Objekt angehängt wird.
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* Referenzausdrücke in einer langen Berechnung unter Verwendung der auf der linken Seite angezeigten Zeilennummern.

1. Klicks **Minimieren** wenn Sie mit der Erstellung der Berechnung für das berechnete benutzerdefinierte Feld fertig sind.

   >[!NOTE]
   >
   >Im Anzeigebereich auf der rechten Seite zeigt das Feld den Füllwert 12345 an. Dies ist ein Hinweis, der Sie daran erinnert, dass es sich bei dem Feld um ein berechnetes benutzerdefiniertes Feld handelt, während Sie das benutzerdefinierte Formular erstellen oder bearbeiten. Wenn das Formular an ein Objekt angehängt ist und Benutzer es ausfüllen, sehen sie das Ergebnis der Berechnung im Feld und nicht den Wert 12345.

1. (Optional) Verwenden Sie eine der folgenden Optionen, um Ihr berechnetes benutzerdefiniertes Feld weiter zu konfigurieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Logik hinzufügen</td> 
      <td>Sie können die Anzeigelogik hinzufügen, um zu bestimmen, ob das berechnete Feld angezeigt wird, basierend auf mindestens einer Auswahl, die ein Benutzer beim Ausfüllen des Formulars in einem vorherigen Multiple-Choice-Feld (Dropdown, Kontrollkästchen oder Optionsfelder) trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen</a>. <p>Dies ist nur verfügbar, wenn dem berechneten benutzerdefinierten Feld im Formular mindestens ein Kontrollkästchen, ein Optionsfeld oder ein Dropdown-Feld vorangeht. </p> <p>Die Logik für das Überspringen ist für berechnete benutzerdefinierte Felder nicht verfügbar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorherige Berechnungen aktualisieren</td> 
      <td>Wenn Sie ein vorhandenes berechnetes benutzerdefiniertes Feld bearbeiten, können Sie diese Option auswählen, um beim Speichern des benutzerdefinierten Formulars eine Aktualisierung der Berechnung Trigger. Dies geschieht nur einmal, wenn Sie das benutzerdefinierte Formular speichern. Die Option wechselt in den deaktivierten Status zurück, nachdem Sie dies getan haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formel in Anleitungen anzeigen</td> 
      <td>Lassen Sie diese Option aktiviert, wenn Benutzer, die das benutzerdefinierte Formular ausfüllen, die Formel des Felds sehen sollen, wenn sie den Mauszeiger über das Feld bewegen. Weitere Informationen finden Sie in den Informationen zu <a href="#instructions" class="MCXref xref">Anweisungen</a> früher in dieser Tabelle.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Fertig** wenn alle Änderungen am berechneten benutzerdefinierten Feld abgeschlossen sind.

   Oder klicken Sie auf **Anwenden** , um Ihre Änderungen bis jetzt auf das Formular anzuwenden, wenn Sie dem Formular weiterhin benutzerdefinierte Felder hinzufügen möchten.

   Oder klicken Sie auf **Speichern und schließen** wenn alle Änderungen im benutzerdefinierten Formular abgeschlossen sind.
1. Um sicherzustellen, dass Ihr berechnetes benutzerdefiniertes Feld ordnungsgemäß funktioniert, hängen Sie das benutzerdefinierte Formular an ein Objekt an und überprüfen Sie dann das Ergebnis im berechneten benutzerdefinierten Feld.

   Anweisungen zum Anhängen eines benutzerdefinierten Formulars finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, können Sie mit einem der folgenden Artikel fortfahren:

   * [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Benutzerdefiniertes Formular in der Vorschau anzeigen und ausfüllen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Syntax in berechneten benutzerdefinierten Feldern erforderlich

Jedes Feld, das in einem benutzerdefinierten berechneten Feld verwendet wird, muss die unten erläuterte Syntax mit geschweiften Klammern um jeden Feldnamen verwenden. Wenn Sie mit der Eingabe des Namens eines Felds beginnen, unterbreitet das System Vorschläge und Sie können einen Vorschlag auswählen, um ihn in Ihre Berechnung einzufügen. Wenn Sie Daten in einer Berechnung fehlerhaft eingeben, werden Sie über eine Warnmeldung benachrichtigt. Sie können das Formular nur speichern, wenn Sie die Berechnung so bearbeiten, dass sie gültige Felder und einen gültigen berechneten Ausdruck enthält.

>[!NOTE]
>
>Derzeit unterbreitet das System Vorschläge nur, wenn Sie mit der Eingabe des Namens eines Felds beginnen, auf das Sie auf ein Objekt verweisen möchten, an das das benutzerdefinierte Formular angehängt wird, und nicht auf das übergeordnete Objekt des Objekts.

### Feldnamen in der Umgebung mit geschweiften Klammern

* Wenn die Berechnung auf ein integriertes Feld verweisen soll, muss der Feldname in geschweiften Klammern stehen und so formatiert sein, wie er in der Workfront-Datenbank erscheint. Sie können den Namen der Felder nicht so verwenden, wie er in der Benutzeroberfläche von Workfront angezeigt wird.

Beispiel: `{actualRevenue}`

Bei Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden und sie müssen im Binnenmajuskel-Format angezeigt werden, wie sie im Workfront-System angezeigt werden.

* Wenn die Berechnung auf ein benutzerdefiniertes Feld verweisen soll, muss der Name des Felds von geschweiften Klammern umgeben sein und von `DE:` innerhalb der Klammern. Bei benutzerdefinierten Feldern wird zwischen Groß- und Kleinschreibung unterschieden. Sie müssen so formatiert sein, wie sie in der Workfront-Benutzeroberfläche angezeigt werden.

Beispiel: `{DE:Profit}`

Das System listet alle benutzerdefinierten Felder auf, aus denen Sie bei der Eingabe auswählen können `DE:`.

* Wenn die Berechnung auf ein Feld verweisen soll, das Daten aus dem übergeordneten Objekt abruft, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird, müssen Sie dem Feldnamen den Objekttyp des übergeordneten Objekts voranstellen (auch in geschweiften Klammern).

  Wenn das benutzerdefinierte Formular beispielsweise für Aufgaben konfiguriert ist und Sie möchten, dass das Feld den tatsächlichen Umsatz des übergeordneten Objekts berechnet, wenn das Formular an eine Aufgabe angehängt wird, müssen Sie Folgendes angeben: `project` als Objekttyp des Felds:

  `{project}.{actualRevenue}`

  Oder, wenn es ein benutzerdefiniertes Feld ist:

  `{project}.{DE:profit}`

  Wenn Sie sich nicht sicher sind, welcher Objekttyp des übergeordneten Objekts lautet, weil das benutzerdefinierte Formular für mehrere Objekttypen konfiguriert ist, können Sie die Filtervariable &quot;Platzhalter&quot;verwenden `$$OBJCODE` , damit die Berechnung für jeden der möglichen Typen funktioniert. Weitere Informationen finden Sie unter [Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten](#calculated-custom-fields-in-multi-object-custom-forms) in diesem Artikel.

### Separate Elemente mit Zeiträumen

Wenn Sie in einem berechneten benutzerdefinierten Feld auf ein verwandtes Objekt verweisen, müssen Sie Objektnamen und -attribute durch Punkte trennen.

Wenn Sie beispielsweise in einem benutzerdefinierten Formular vom Typ Aufgabe den Namen des Eigentümers des Portfolios in einem berechneten benutzerdefinierten Feld anzeigen möchten, geben Sie Folgendes ein:

`{project}.{porfolio}.{owner}`

Dieses System ruft die Informationen in den folgenden Schritten ab (in dieser Reihenfolge):

1. Aus dem Objekt des benutzerdefinierten Formulars (einer Aufgabe) gefolgt von
1. Greifen Sie auf das übergeordnete Element der Aufgabe oder auf ein anderes verwandtes Objekt (Projekt) zu und
1. Greifen Sie auf das übergeordnete oder ein anderes verwandtes Objekt des Projekts zu (ein Portfolio) und
1. Greifen Sie auf das nächste verwandte Objekt auf das Portfolio zu (den Eigentümer des Portfolios).

### Namenssyntax für die Referenzierung eines benutzerdefinierten Felds

Wenn Sie in einem berechneten benutzerdefinierten Feld auf ein anderes benutzerdefiniertes Feld verweisen, müssen Sie den Feldnamen so eingeben, wie er in der Workfront-Benutzeroberfläche angezeigt wird.

Um beispielsweise auf die ausgewählte Option in einem benutzerdefinierten Feld mit der Bezeichnung Executive sponsor zu verweisen, geben Sie Folgendes ein:

`{DE:Executive sponsor}`

>[!NOTE]
>
>Die Syntax für ein Feld vom TypAhead unterscheidet sich von der für andere Feldtypen, da Sie `:name` am Ende.
>
>Um beispielsweise auf die ausgewählte Option in einem benutzerdefinierten Typenvorfeld mit dem Namen &quot;Executive sponsor&quot;zu verweisen, geben Sie Folgendes ein:
>
>`{DE:Executive sponsor:name}`

## Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten {#calculated-custom-fields-in-multi-object-custom-forms}

In einem benutzerdefinierten Formular mit mehreren Objekten müssen die ausgewählten Objektarten mit allen Feldern kompatibel sein, auf die in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Wenn eine Inkompatibilität vorliegt, werden Sie durch eine Meldung darauf hingewiesen, dass Sie Anpassungen vornehmen müssen.

>[!INFO]
>
>**Beispiel:**
>
>In einem benutzerdefinierten Formular, das für die Verwendung mit dem Task-Objekttyp konfiguriert wurde, erstellen Sie ein berechnetes benutzerdefiniertes Feld mit dem Namen In Charge. Sie konfigurieren es so, dass es auf das integrierte Feld verweist, sodass der Name des Hauptverantwortlichen angezeigt werden kann, sobald das Formular an eine Aufgabe angehängt wird:
>
>`{assignedTo}.{name}`
>
>Später fügen Sie dem benutzerdefinierten Formular den Projektobjekttyp hinzu. Eine Warnmeldung weist Sie darauf hin, dass der Projektobjekttyp nicht mit dem berechneten benutzerdefinierten Feld kompatibel ist.

In diesem Fall haben Sie folgende Möglichkeiten:

* Entfernen Sie eines der beiden inkompatiblen Elemente aus dem benutzerdefinierten Formular - entweder den Objekttyp oder das referenzierte berechnete benutzerdefinierte Feld.
* Beides beibehalten und die Platzhalterfiltervariable verwenden `$$OBJCODE` als Bedingung in einem IF-Ausdruck verwenden, um zwei verschiedene Versionen des Felds In Charge zu erstellen. Dadurch kann das Feld unabhängig vom Objekttyp, an den das Formular angehängt ist, erfolgreich funktionieren.

>[!INFO]
>
>**Beispiel:** Es gibt zwar kein Feld Zugeordneter Benutzer: Name in Projekten, es gibt jedoch ein integriertes Feld Inhaber (das automatisch mit dem Namen der Person ausgefüllt wird, die das Projekt erstellt hat, es sei denn, dies wird manuell geändert).
>
>In Ihrem benutzerdefinierten Feld &quot;In Charge&quot;können Sie also `$$OBJCODE` wie unten gezeigt, um auf das Feld Inhaber zu verweisen, wenn das benutzerdefinierte Formular an ein Projekt angehängt wird, und auf das Feld Zugeordneter Name , wenn das Formular an eine Aufgabe angehängt wird:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Weitere Informationen zu Variablen finden Sie unter `$$OBJCODE,` see [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Automatische Aktualisierung berechneter benutzerdefinierter Felder

Berechnete benutzerdefinierte Felder eines Objekts werden automatisch neu berechnet, wenn Folgendes geschieht:

* Es ändert sich etwas am Objekt, z. B. eine tägliche Timeline-Berechnung.
* Jemand bearbeitet ein anderes Feld, das durch ein berechnetes benutzerdefiniertes Feld im Objekt referenziert wird.
* Der berechnete Ausdruck ist leer und das Feld enthält einen Wert. Dadurch wird der Wert auf null gesetzt.

  >[!NOTE]
  >
  ><div>In einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, werden Datums- und Uhrzeitanweisungen in berechneten benutzerdefinierten Feldern gemäß der koordinierten UTC (Universal Time) berechnet und gespeichert, nicht gemäß den Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr Benutzerprofil festgelegt wurden. Berechnungen in einem benutzerdefinierten Formular werden basierend auf den individuellen Zeitzonen der einzelnen Benutzer generiert.</div>
