---
title: Hinzufügen berechneter Felder zu einem Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein berechnetes benutzerdefiniertes Feld hinzufügen, das vorhandene Daten verwendet, um neue Daten zu generieren, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '2412'
ht-degree: 0%

---

# Hinzufügen berechneter Felder zu einem Formular

<!-- Audited: 5/2025 -->

Sie können ein berechnetes benutzerdefiniertes Feld hinzufügen, das vorhandene Daten verwendet, um neue Daten zu generieren, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.

Ein berechnetes benutzerdefiniertes Feld kann Folgendes enthalten:

* Ein einfacher Verweis auf ein einzelnes integriertes Feld.

  >[!INFO]
  >
  >**Beispiel** Um den durch Projekte und Aufgaben generierten Umsatz zu berechnen, können Sie ein berechnetes benutzerdefiniertes Feld erstellen, das das integrierte Feld Tatsächlicher Umsatz enthält. Wenn jemand das benutzerdefinierte Formular an ein Projekt oder eine Aufgabe anhängt, wird der Umsatz für das Projekt oder die Aufgabe im Feld angezeigt.

* Ein Ausdruck, der auf ein oder mehrere Felder verweist. Dabei kann es sich um benutzerdefinierte Felder, andere berechnete benutzerdefinierte Felder und integrierte Felder handeln.

  >[!INFO]
  >
  >**Beispiel** Um den durch Projekte und Aufgaben generierten Gewinn zu berechnen, können Sie ein berechnetes benutzerdefiniertes Feld namens Gewinn erstellen, das einen mathematischen Ausdruck enthält, der Kosten vom Umsatz abzieht.
  >
  >Dazu können Sie den mathematischen Ausdruck SUB (subtrahieren) mit den integrierten Workfront-Feldern Istkosten und Istumsatz verwenden.
  >
  >In den folgenden Schritten können Sie sehen, wie Sie einen Ausdruck wie in diesem Beispiel erstellen.

>[!NOTE]
>
>Bei Änderungen an einem Direktfeld wird automatisch eine Aktualisierung des berechneten Feldwerts Trigger. (Direkte Felder sind Felder, die im Workfront-API-Explorer verfügbar sind, oder benutzerdefinierte Felder in einem benutzerdefinierten Formular, das an ein Objekt angehängt ist.) Änderungen an einer Referenz oder Formel erfordern eine manuelle Neuberechnung der Feldwerte.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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

## Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden

Sie können dasselbe berechnete benutzerdefinierte Feld für benutzerdefinierte Formulare verwenden, die zu verschiedenen Objekten gehören. Sie können beispielsweise das berechnete Feld Gewinn verwenden, das Sie für das benutzerdefinierte Formular Projekt in einem benutzerdefinierten Formular für eine Aufgabe erstellt haben.

Bei Verwendung eines vorhandenen berechneten benutzerdefinierten Felds wird die Berechnung nicht auf das neue Formular übertragen. Fügen Sie die Berechnung erneut für dasselbe Feld im neuen benutzerdefinierten Formular hinzu.

Sie können für dasselbe Feld auch auf dem neuen Formular eine andere Berechnung verwenden. Die Beibehaltung des gleichen Namens für das berechnete benutzerdefinierte Feld stellt die Kohärenz und Konsistenz Ihrer Namenskonvention sicher.

>[!IMPORTANT]
>
>Änderungen an berechneten Ausdrücken können dazu führen, dass der Feldwert in Objekten veraltet ist. Führen Sie einen der folgenden Schritte aus, um sicherzustellen, dass Sie in diesen Feldern immer die aktuelle Berechnung anzeigen:
>
>* Nachdem Sie ein Objekt gespeichert haben, bei dem Sie Daten in einem angehängten benutzerdefinierten Formular bearbeitet haben, klicken Sie auf der Hauptseite des Objekts auf das Symbol Mehr ![Mehr](assets/more-icon.png) und berechnen Sie dann benutzerdefinierte Ausdrücke neu.
>* Wählen Sie die Option Benutzerdefinierte Ausdrücke neu berechnen , wenn Sie Objekte stapelweise bearbeiten.
>* Wählen Sie beim Bearbeiten eines berechneten benutzerdefinierten Felds in einem benutzerdefinierten Formular die Option Vorherige Berechnungen aktualisieren .

So verwenden Sie ein vorhandenes berechnetes benutzerdefiniertes Feld wieder:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms** gefolgt von **Forms**.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Klicken Sie auf **Neues benutzerdefiniertes Formular**.

1. Wählen **Dialogfeld „Neues benutzerdefiniertes**&quot; aus, an welche Objekttypen das benutzerdefinierte Formular angehängt werden soll, und klicken Sie dann auf **Weiter**.
1. Klicken Sie oben links im Bildschirm auf &quot;**&quot;**.

   ![Feldbibliothek](assets/field-library.png)

1. Verwenden Sie das Suchfeld oder erweitern Sie den Abschnitt **Berechnet**, um das gewünschte berechnete Feld zu finden, und ziehen Sie das Feld dann an die Stelle, an der es im benutzerdefinierten Formular angezeigt werden soll.

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Felder hinzuzufügen.

   >[!NOTE]
   >
   >Sie können bis zu 500 Felder und Widgets in einem einzelnen benutzerdefinierten Formular hinzufügen. Je nach Komplexität eines Formulars kann es jedoch zu Leistungseinbußen kommen, wenn mehr als 100 auf dem Formular vorhanden sind.
   >
   >
   >Beispiele für komplexe Formulare sind Formulare mit kaskadierenden Parametern, berechneten benutzerdefinierten Datenfeldern und mehreren Wertoptionen in einem einzigen Feld.

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   oder

   Klicken Sie **Speichern und schließen**.

## Neues berechnetes Feld hinzufügen

>[!IMPORTANT]
>
>Bevor Sie ein neues berechnetes benutzerdefiniertes Feld erstellen, identifizieren Sie die vorhandenen Felder, die Sie einbeziehen möchten, damit Sie sicher sein können, dass die für die Berechnung erforderlichen Daten in Workfront vorhanden sind.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Benutzerdefinierte Forms** gefolgt von **Forms**.

1. Klicken Sie auf **Neues benutzerdefiniertes Formular**.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Wählen **Dialogfeld „Neues benutzerdefiniertes**&quot; aus, an welche Objekttypen das benutzerdefinierte Formular angehängt werden soll, und klicken Sie dann auf **Weiter**.

1. Suchen Sie auf der linken Seite des Bildschirms nach **Berechnet** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.

   ![Feld in Abschnitt ziehen](assets/drag-field-to-section.png)

1. Konfigurieren Sie auf der rechten Seite des Bildschirms die Optionen, die für den Typ des benutzerdefinierten Felds verfügbar sind, das Sie hinzufügen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td>Geben Sie einen Titel für das Feld ein. Dies wird Benutzern angezeigt, wenn sie das benutzerdefinierte Formular verwenden. Das Feld <b>Name</b> das automatisch ausgefüllt wird, wird von Workfront in Berichten referenziert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Anleitung</td> 
      <td> Standardmäßig wird die Formel, die Sie für das Feld erstellen, hier gespeichert. Sie können Text hinzufügen, um zusätzliche Informationen über das Feld und die darin enthaltene Formel bereitzustellen. Dies kann auf zwei Arten nützlich sein: 
       <ul> 
      <li><p>Als Erinnerung daran, was die Formel ist und wie sie funktioniert. Dies ist besonders hilfreich, wenn Sie dieses berechnete benutzerdefinierte Feld in mehreren Formularen verwenden möchten.</p> </li> 
      <li> <p>Als QuickInfo können Benutzer sehen, wenn sie den Mauszeiger über das Feld bewegen. Hier können Sie Text hinzufügen, der in der QuickInfo angezeigt werden soll.</p> <p>Wenn Sie nicht möchten, dass die Formel in der QuickInfo angezeigt wird, was für sie verwirrend sein könnte, können Sie sie ausblenden.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Format</td> 
      <td> <p>Das Format, in dem die Ergebnisse des Felds gespeichert und angezeigt werden sollen.</p> <p>Wenn das Feld in mathematischen Berechnungen verwendet wird, verwenden Sie immer das Format <strong>Zahl</strong> oder <strong>Währung</strong>. Wenn Sie <strong>Zahl</strong> oder <strong>Währung</strong> auswählen, kürzt das System automatisch Zahlen, die mit 0 beginnen.</p> 
      <p><b>WICHTIG</b>: Bevor Sie ein Format auswählen, überlegen Sie, welches Format für das neue Feld korrekt ist. Das Formatfeld kann nach dem Speichern des benutzerdefinierten Formulars nicht mehr bearbeitet werden. Die Auswahl des falschen Formats kann sich auf zukünftige Berechnungen und Aggregatwerte in Berichts- und Listengruppierungen auswirken.</p>
      <p><strong>HINWEIS</strong>: Berechnete Felder mit dem Format <strong>Währung</strong> sollten keine Anführungszeichen enthalten. (Verwenden Sie beispielsweise 800.00 und nicht „800.00.„) Die Verwendung von Anführungszeichen kann aufgrund von Nuancen bei der Sprachformatierung für Währungstypen unerwartete Folgen haben.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Beginnen Sie im Feld **Berechnung** mit der Erstellung Ihrer Berechnung:
   1. Klicken Sie **Maximieren**, um den Berechnungs-Editor zu öffnen und die Berechnung zu erstellen.</p>
Eine Berechnung beginnt normalerweise mit einem Ausdruck, gefolgt von Klammern mit den Feldern, auf die Sie verweisen möchten, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird.

      Jedes Feld muss von geschweiften Klammern umgeben sein. Wenn Sie mit der Eingabe eines Feldnamens beginnen, macht das System Vorschläge, und Sie können einen auswählen, um ihn in Ihre Berechnung einzufügen.

      +++ **Erweitern Sie , um die in berechneten benutzerdefinierten Feldern erforderliche Syntax anzuzeigen**

      Jedes Feld muss die unten beschriebene Syntax verwenden, wobei die einzelnen Feldnamen in geschweiften Klammern stehen müssen. Wenn Sie mit der Eingabe eines Feldnamens beginnen, macht das System Vorschläge, und Sie können einen auswählen, um ihn in Ihre Berechnung einzufügen. Wenn Sie Daten in eine Berechnung falsch eingeben, werden Sie durch eine Warnmeldung informiert. Das Formular kann erst gespeichert werden, wenn die Berechnung so bearbeitet wurde, dass sie gültige Felder und einen gültigen berechneten Ausdruck enthält.

      >[!NOTE]
      >
      >Derzeit macht das System Vorschläge nur, wenn Sie mit der Eingabe des Namens eines Felds beginnen, auf das Sie verweisen möchten, und zwar für ein Objekt, an das das benutzerdefinierte Formular angehängt wird. Felder aus dem übergeordneten Objekt werden nicht empfohlen.

      **Umschließen von Feldnamen mit geschweiften Klammern**

      * Wenn die Berechnung auf ein integriertes Feld verweisen soll, muss der Name des Felds von geschweiften Klammern umgeben sein.

        Beispiel: `{actualRevenue}`

        Bei Feldnamen wird zwischen Groß- und Kleinschreibung unterschieden und sie müssen in der Berechnung genau so angezeigt werden, wie sie im Workfront-System angezeigt werden.

        Navigieren Sie zum [Workfront-API-](https://developer.adobe.com/workfront/api-explorer/), um die Feldnamen zu identifizieren, die Sie für Berechnungen verwenden können.

      * Wenn die Berechnung auf ein benutzerdefiniertes Feld verweisen soll, muss der Name des Felds von geschweiften Klammern umgeben sein und vor den `DE:` in den Klammern stehen.

        Beispiel: `{DE:Profit}`

        Das System listet alle benutzerdefinierten Felder auf, aus denen Sie bei der Eingabe von `DE:` auswählen können.

         * Wenn die Berechnung auf ein Feld verweisen soll, das Daten aus dem *übergeordneten* Objekt abruft, wenn das benutzerdefinierte Formular an ein Objekt angehängt wird, müssen Sie dem Feldnamen den Objekttyp des übergeordneten Objekts voranstellen, auch in geschweiften Klammern.

        Wenn beispielsweise das benutzerdefinierte Formular für die Verwendung mit Aufgaben konfiguriert ist und Sie möchten, dass das Feld den tatsächlichen Umsatz des übergeordneten Objekts berechnet, wenn das Formular mit einer Aufgabe verknüpft ist, müssen Sie `Project` als Objekttyp des Felds angeben:

        `{project}.{actualRevenue}`

        Oder, wenn es ein benutzerdefiniertes Feld ist:

        `{project}.{DE:profit}`

        **Elemente durch Punkte trennen**

        Wenn Sie in einem berechneten benutzerdefinierten Feld auf ein verwandtes Objekt verweisen, müssen Sie Objektnamen und Attribute durch Punkte trennen.

        Um beispielsweise in einem benutzerdefinierten Formular vom Typ Aufgabe den Namen des Portfolio-Verantwortlichen in einem berechneten benutzerdefinierten Feld anzuzeigen, geben Sie Folgendes ein:

        `{project}.{porfolio}.{owner}`

        Dadurch würde Folgendes bestimmt: Über das Objekt des benutzerdefinierten Formulars (eine Aufgabe) können Sie auf das nächste Objekt zugreifen, das mit der Aufgabe verknüpft ist (ein Projekt). Dort können Sie auf das nächste mit dem Projekt verknüpfte Objekt (ein Portfolio) zugreifen und dann auf die Felder verweisen, die für das Portfolioobjekt (den Eigentümer) definiert sind

        **Namenssyntax für den Verweis auf ein benutzerdefiniertes Feld**

        Wenn Sie in einem berechneten benutzerdefinierten Feld auf ein anderes benutzerdefiniertes Feld verweisen, müssen Sie den Feldnamen so eingeben, wie er in der Benutzeroberfläche von Workfront angezeigt wird.

        Um beispielsweise auf die ausgewählte Option in einem benutzerdefinierten Feld mit der Bezeichnung „Executive Sponsor“ zu verweisen, geben Sie Folgendes ein:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >Die Syntax für ein Feld mit automatischer Textvervollständigung unterscheidet sich etwas von der für andere Feldtypen, da Sie am Ende `:name` hinzufügen müssen.
        >
        >Um beispielsweise auf die ausgewählte Option in einem benutzerdefinierten Feld mit automatischer Textvervollständigung mit dem Namen „Executive Sponsor“ zu verweisen, geben Sie Folgendes ein:
        >
        >`{DE:Executive sponsor:name}`


        **Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten**

        In einem benutzerdefinierten Formular mit mehreren Objekten müssen die ausgewählten Objekttypen mit mindestens einem Feld kompatibel sein, auf das in den berechneten benutzerdefinierten Feldern des Formulars verwiesen wird. Felder, die nicht mit dem Objekt kompatibel sind, werden im Formular nicht angezeigt.

        Um sicherzustellen, dass das berechnete Feld ein korrektes Ergebnis für alle Objekttypen anzeigt, müssen Sie `$$OBJCODE` verwenden, um eine Berechnung für jeden Objekttyp zu definieren.

        >[!INFO]
        >
        >**Beispiel:**
        >
        >In einem benutzerdefinierten Formular, das für die Arbeit mit Projekten, Aufgaben und Problemen konfiguriert wurde, können Sie die folgende Formel verwenden, um den Objekttyp anzuzeigen:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >Bei einem Projekt wird im Feld „Dies ist ein Projekt“ angezeigt, bei einer Aufgabe „Dies ist eine Aufgabe“ und bei einem Problem „Dies ist ein Problem“.


        >[!INFO]
        >
        >**Beispiel:** Obwohl es in Projekten kein Feld Zugewiesen an: Name gibt, gibt es ein integriertes Besitzerfeld (das automatisch mit dem Namen der Person ausgefüllt wird, die das Projekt erstellt hat, es sei denn, diese Person ändert dies manuell).
        >
        >In Ihrem benutzerdefinierten Feld „Verantwortlicher“ können Sie daher `$$OBJCODE` wie unten dargestellt verwenden, um auf das Feld „Verantwortlicher“ zu verweisen, wenn das benutzerdefinierte Formular an ein Projekt angehängt wird, und auf das Feld „Zugewiesen an: Name“, wenn das Formular an eine Aufgabe angehängt wird:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Weitere Informationen zu Variablen wie `$$OBJCODE,` finden Sie unter [Übersicht über Platzhalterfiltervariablen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Automatische Aktualisierungen berechneter benutzerdefinierter Felder**

        Berechnete benutzerdefinierte Felder eines Objekts werden automatisch neu berechnet, wenn Folgendes passiert:

         * Etwas im Objekt ändert sich, z. B. eine tägliche Zeitleistenberechnung.
         * Jemand bearbeitet ein anderes Feld, auf das ein berechnetes benutzerdefiniertes Feld im -Objekt verweist.
         * Der berechnete Ausdruck ist leer und das Feld enthält einen Wert. Dadurch wird der Wert auf null festgelegt.

           >[!NOTE]
           >
           ><div>In einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, werden Datums- und Zeitangaben in berechneten benutzerdefinierten Feldern durch die koordinierte Weltzeit (UTC) berechnet und gespeichert, nicht durch die Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr Benutzerprofil festgelegt sind. Berechnungen in einem benutzerdefinierten Formular, die auf der Grundlage der individuellen Zeitzonen der einzelnen Benutzenden erstellt werden.</div>

      +++

   1. Klicken Sie in das große Textfeld und dann auf **Ausdrücke** und **Felder**, die Sie Ihrer Berechnung hinzufügen können.

      Erweitern Sie einen Objektnamen unter **Felder**, um alle für dieses Objekt verfügbaren Felder anzuzeigen. Die Liste ist auf 200 Elemente beschränkt. Wenn Sie den Feldnamen kennen, können Sie danach suchen.

      Sie können auch beginnen, einen Ausdruck oder ein Feld in das große Textfeld einzugeben, und ihn dann bei der Anzeige auswählen. Jedes Element wird mit einem „F“ für Feld oder einem „E“ für Ausdruck angezeigt.

      Wenn Sie eine öffnende Klammer eingeben, wird die schließende Klammer automatisch hinzugefügt.

      +++ **Erweitern Sie , um hilfreiche Tipps anzuzeigen**

      >[!TIP]
      >
      >Sie können einen der folgenden Schritte ausführen, um Hilfe bei Ihrer Berechnung zu erhalten:
      > 
      >* Bewegen Sie den Mauszeiger über einen Ausdruck in Ihrer Berechnung, um eine Beschreibung, ein Beispiel, das zeigt, wie er verwendet werden kann, und einen **Weitere Informationen**-Link zu weiteren Informationen im Artikel [Übersicht über berechnete Datenausdrücke](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md) anzuzeigen.
      >  ![Hilfetext für Ausdruck](assets/hover-expression-help-text.jpg)
      >* Verwenden Sie die Farbcodierung, um die hinzugefügten Komponenten zu identifizieren. Ausdrücke werden in blauen und Felder in grün angezeigt.
      >  ![Farben für Feldausdrücke](assets/colors-fields-expressions.jpg)
      >* Suchen Sie nach Berechnungsfehlern, die Sie fortlaufend in Rosa markieren. Sie können den Mauszeiger über einen markierten Fehler bewegen, um eine kurze Beschreibung der Ursache anzuzeigen.
      >  ![Hilfe zu Fehlern](assets/error-help.png)
      >* Zeigen Sie im Bereich unterhalb Ihrer Berechnung die Ergebnisse eines vorhandenen Workfront-Objekts an.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![Vorschau der Berechnung](assets/preview-calc.jpg)
      >* Referenzausdrücke in einer langen Berechnung unter Verwendung der Zeilennummern, die links angezeigt werden.

      +++
   1. Klicken Sie **Minimieren** wenn Sie die Erstellung der Berechnung für das berechnete benutzerdefinierte Feld abgeschlossen haben.

   1. (Optional) Verwenden Sie eine der folgenden Optionen, um Ihr berechnetes benutzerdefiniertes Feld weiter zu konfigurieren:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Logik hinzufügen</td> 
      <td>Sie können eine Anzeigelogik hinzufügen, um zu bestimmen, ob das berechnete Feld angezeigt wird, basierend auf mindestens einer Auswahl, die ein Benutzer beim Ausfüllen des Formulars in einem vorangehenden Feld mit Mehrfachauswahl (Dropdown, Kontrollkästchen oder Optionsfelder) trifft. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Dies ist nur verfügbar, wenn dem berechneten benutzerdefinierten Feld im Formular mindestens ein Kontrollkästchen, ein Optionsfeld oder ein Dropdown-Feld vorangeht. </p> <p>Logik überspringen ist für berechnete benutzerdefinierte Felder nicht verfügbar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorherige Berechnungen aktualisieren</td> 
      <td>Wenn Sie ein bestehendes berechnetes benutzerdefiniertes Feld bearbeiten, können Sie diese Option auswählen, um beim Speichern des benutzerdefinierten Formulars eine Aktualisierung in der Berechnung Trigger. Dies geschieht nur einmal beim Speichern des benutzerdefinierten Formulars. Danach kehrt die Option in den deaktivierten Zustand zurück.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formel in Anleitungen anzeigen</td> 
      <td>Lassen Sie diese Option aktiviert, wenn die Benutzer, die das benutzerdefinierte Formular ausfüllen, die Formel des Felds sehen sollen, wenn sie den Mauszeiger über das Feld bewegen. Weitere Informationen finden Sie in den Informationen zu <a href="#instructions" class="MCXref xref">Anweisungen</a> weiter oben in dieser Tabelle.</td> 
     </tr> 
    </tbody> 
   </table>

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und gehen Sie zu einem anderen Abschnitt über, um mit der Erstellung Ihres Formulars fortzufahren.

   oder

   Klicken Sie **Speichern und schließen**.
