---
title: Erstellen von Briefs im Ideenraum
description: In diesem Artikel wird beschrieben, wie Sie im Ideationsbereich Ideen diskutieren und Strategien entwickeln können, um Briefs zu erstellen. Sie können fertige Ideenbeschreibungen in eine Datei oder in Workfront Planning exportieren, um Datensätze zu erstellen oder zu aktualisieren.
feature: Workfront Planning
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 2%

---


# Erstellen von Briefs im Ideationsbereich

<!-- add to TOC and miniTOC-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Es ist nur im Rahmen des Programms **Ideation Space Beta** verfügbar. </span>

<span class="preview">Weitere Informationen finden Sie unter [Erste Schritte mit dem Ideenraum für Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Mit der Ideation Space, einer neuen Funktion von Adobe Workfront Planning, können Sie Briefs in Planungsunterlagen umwandeln. Exportierte Briefs erstellen neue Datensätze oder aktualisieren vorhandene.

In diesem Artikel wird beschrieben, wie Sie im Ideationsbereich Ideen diskutieren und Strategien entwickeln können, um Briefs zu erstellen. Um Datensätze zu erstellen oder zu aktualisieren, exportieren Sie fertige Ideenbeschreibungen in eine -Datei oder in Workfront Planning.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Zusätzliche Produkte</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workflow-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> 
   <ul>
   <li><p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   </li>
   <li><p>Die Einstellung Ideenraum deaktivieren in Ihrer Zugriffsebene muss deaktiviert sein</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Arbeitsbereich und Datensatztyp bei, dem Sie Datensätze hinzufügen möchten </p>
      <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
      <p>Anzeigen von Berechtigungen für Workfront-Objekte, um sie zu Briefs hinzuzufügen <!--not sure if this is available--></p>
      <p>Editor-Berechtigungen für den Ideenraum zum Erstellen von Briefs</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-Benutzerrollen</p></td> 
   <td><p><ul><li>Jede GenStudio-Benutzerrolle für den Zugriff auf Kampagnen, Produkte und Personas</li>
   <li>GenStudio System Manager für den Zugriff auf Aktivierungen <!--and Events--></li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Erstellen von Ideen-Space-Briefs

1. Beginnen Sie in Workfront Planning und erstellen oder bearbeiten Sie einen Datensatz mithilfe des Ideationsbereichs.

   Weitere Informationen finden Sie unter [Erstellen von Planungsdatensätzen aus Ideation Space-Briefs](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).
1. Wenn **Ideationsbereich** geöffnet wird, verwenden Sie die Eingabeaufforderung, um die Art der Zusammenfassung zu beschreiben, die Sie erstellen möchten.

   Geben Sie zum Beispiel „Erstellen Sie eine Kampagne „Zurück zur Schule“ für Schüler der Klasse K-12, die durch den Monat August läuft, für Eltern und Lehrer in den USA ein“.  Um die Zusammenfassung so vollständig wie möglich zu gestalten, geben Sie so viele Informationen an, wie Sie für welche Art von Kampagne verfügbar haben, den Zeitplan, die Stakeholder und andere Details.

1. Klicken Sie **Ideating starten**.

   Nach dem Öffnen durchläuft der Ideation-Space-Agent die folgenden Schritte:

   1. **Datenaufnahme und -synthese**: Ruft relevante Informationen aus verbundenen Quellen ab. Beispiel:

      * Vorhandene Datensatztypen oder der vorhandene Datensatztyp, von dem aus Sie gestartet haben.
      * Letzte Dokumente, die Sie möglicherweise im Ideenbereich hochgeladen haben.
      * Web-Informationen, die Ihren Eingabeaufforderungskriterien entsprechen.

        >[!TIP]
        >
        >Die Web-Sucheinstellung muss aktiviert sein, damit KI im Web nach Informationen suchen kann.\
        >Weitere Informationen finden Sie im Abschnitt [Konfigurieren des Ideenraums](#configure-the-ideation-space) in diesem Artikel.
        >
   1. **Zielgruppendefinition**: Identifiziert oder empfiehlt Zielgruppenparameter basierend auf historischen Mustern.
   1. **Strategie-**: Strukturiert die strategische Erzählung für die Kampagne
   1. **Messaging und Konzeptidee**: Erzeugt Optionen für erste Nachrichten und kreative Konzeptrouten.
   1. **Kurze Erstellung und Übergabe der Planung**: Erstellt eine strukturierte Zusammenfassung, die in den Workfront Planning-Arbeitsbereich zurückeinfließt.

      Wenn der Ideationsagent den Prozess der Erfassung aller Informationen abschließt, treten folgende Dinge auf:

      * Fünf Karten werden erstellt und nach relevanten und ähnlichen Informationen geordnet.

        Die Karten werden mit verschiedenen Schritten bei der Erstellung des angeforderten Datensatzes benannt, um eine einfache Erkennung zu ermöglichen.

        Sie können beispielsweise folgendermaßen benannt werden:

        * Plan
        * Timeline
        * Segmente
        * Mechanik
        * Messaging

      Die Kartentitel sind für jede Karte in der Idee benutzerdefiniert.

      * Die Karten werden innerhalb desselben Rahmens platziert, was darauf hinweist, dass dies das Ergebnis einer Idee ist.

      * Eine Zusammenfassung wird erstellt und in einem Vorschaubild in der linken unteren Ecke des Ideenraums angezeigt. <!--add screen shot??-->

      Die Zusammenfassung enthält vorgeschlagene Felder, die das System für die zu untersuchenden Ideen für relevant hält.

1. (Optional) Klicken Sie auf das **Hilfe**-Symbol ![](assets/more-information-icon.png) oben rechts, um eine Liste der Tastaturbefehle anzuzeigen, die Ihnen bei der Navigation durch den Ideationsbereich helfen.

1. (Optional) Klicken Sie **Quellen** am unteren Rand jeder Karte, um zu verstehen, wo die Informationen erfasst wurden.

   Informationen können entweder aus Workfront Planning oder dem Web importiert werden.
1. (Optional) Verwenden Sie die Daumen-nach-oben- oder Daumen-nach-unten-Symbole auf einer Karte, um Feedback zu geben.<!--is this still available??-->
1. Klicken Sie auf eine Karte oder auf den Rahmen mit allen Karten und dann auf **Zu Zusammenfassung hinzufügen**, um ihre Informationen der Zusammenfassung hinzuzufügen.

   Workfront ordnet jedem Informationselement das Feld zu, in dem es am wahrscheinlichsten gespeichert wird.

   Beispielsweise werden Zeitleisten zu Datumsfeldern und Beschreibungen zu Absatzfeldern hinzugefügt.
   1. (Bedingt) Klicken Sie auf eine Karte und dann auf **KI bitten an …**, um Ideen für den nächsten Schritt zu erhalten, bevor Sie die Informationen zur Zusammenfassung hinzufügen. Die Antworten werden im Kontext der Informationen der einzelnen Karten angezeigt.
   1. Klicken Sie auf **Symbol** Dokumente hinzufügen![&#x200B; (Symbol &#x200B;](assets/add-documents-in-ideation-space.png) hinzufügen) in der linken oberen Ecke des Ideationsbereichs, um Dokumente in den Bereich hochzuladen. Sie können neue Dokumente oder Dokumente hinzufügen, die Sie bereits zu dem zuvor eingefügten Bereich hinzugefügt haben.

      >[!TIP]
      >
      >Die Einstellung Dokumente muss aktiviert sein, damit auf Dokumente zugegriffen und sie in den Bereich hochgeladen werden können.
      >Weitere Informationen finden Sie im Abschnitt [Konfigurieren des Ideenraums](#configure-the-ideation-space) in diesem Artikel.
      > 
   1. Klicken Sie auf das **WF-Taxonomiekarte hinzufügen**-Symbol ![Aus Workfront Planning hinzufügen](assets/add-from-wf-planning-on-ideations-space.png) <!--send this tooltip to be revised--> und wählen Sie einen verbundenen Datensatztyp und dann einen Datensatz aus jedem Typ aus, um die Informationen dieses Datensatztyps zum ausgewählten Datensatztyp hinzuzufügen.

      Es wird eine Karte für den Datensatz erstellt, den Sie der Platzierung hinzufügen möchten. Der Datensatztyp wird in der oberen linken Ecke der Datensatzkarte angezeigt.
   1. (Optional) Klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und klicken Sie auf **In Workfront anzeigen**.

      Die Detailseite des Datensatzes wird in Workfront Planning auf einer anderen Browser-Registerkarte geöffnet.
   1. (Optional) Wählen Sie den Ideenrahmen oder eine Karte aus und klicken Sie auf das Symbol Löschen und dann zur Bestätigung auf Löschen . Die Karte wird aus dem Ideationsraum entfernt.

      Wenn Sie Karten löschen, die einem gespeicherten Dokument oder Datensatz entsprechen, werden die Elemente aus dem Ideationsraum entfernt, bleiben aber in ihren jeweiligen Anwendungen.

1. (Optional) Verwenden Sie das **Alles fragen** Feld in der rechten unteren Ecke jederzeit, um Ihre Idee zu verfeinern.

   Geben Sie beispielsweise `regenerate` für eine bestimmte Karte ein, damit KI diese Karte unter Verwendung des aktualisierten Kontexts wiederholen kann. Der Ideenraum führt seine logischen Schritte (Suchen, Synthetisieren, Zitieren) erneut aus und aktualisiert die betroffenen Karten.

1. (Optional) Stellen Sie im Feld **Alles stellen** eine neue Frage, um eine neue Idee zu starten.

   Ein neuer Satz von Karten wird generiert, nachdem die Leerstelle ihre Schritte zur Argumentation wiederholt hat.

1. (Optional) Klicken Sie auf einen der lilafarbenen Anschlüsse in allen Ideenkartensätzen und klicken Sie dann auf das Symbol **In die Eingabeaufforderungsleiste kopieren**, um die Ideenbegründung erneut auszuführen.

   ![In Eingabeaufforderungsleiste kopieren](assets/copy-to-prompt-bar-icon-highlighted.png)

1. (Optional) Klicken Sie auf **Rückgängig** oder **Wiederholen** Symbole ![Rückgängig und Wiederholen](assets/undo-redo-icons.png) oben auf der Seite, um eine Aktion abzubrechen oder rückgängig zu machen.
1. Zoomen Sie heran, um das vollständige Bild zu sehen: Ihr ursprüngliches Kampagnenziel, alle KI-generierten Konzeptkarten mit Zitaten, zusätzliche Dokumente, die echten Workfront-Planungsdatensätze, die Sie eingezogen haben (Produkte, Personas usw.). Die **Brief** Zusammenfassungskarte in der linken unteren Ecke zieht alles zusammen.

1. Klicken Sie auf das Bild für die Kurzvorschau in der linken unteren Ecke, prüfen Sie die Kurzvorschau und klicken Sie dann auf eine der folgenden Optionen:

   * **In Datei exportieren**. Sie können die Zusammenfassung in die folgenden Dateitypen exportieren:

     * PDF
     * Wort
     * PowerPoint (mit oder ohne Vorlage)
   * **In Workfront Planning exportieren**. Der Export überschreibt alle vorhandenen Felddaten im Datensatz in Workfront Planning.

   Dadurch wird die Erstellung des Datensatzes mit den zusätzlichen Informationen abgeschlossen und dem ursprünglich ausgewählten Datensatztyp hinzugefügt.

   Weitere Informationen zur Aktualisierung von Planungsdatensätzen mithilfe von Briefs finden Sie im Abschnitt „Überlegungen zur Verwendung des Ideationsraums zur Erstellung von Datensätzen“ im Artikel [Erstellen von Planungsdatensätzen aus Ideationsraumbeschreibungen](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md).


## Ideationsbereich konfigurieren

Es gibt Steuerelemente für den Ideationsbereich, mit denen Sie konfigurieren können, was Sie auf dem Bildschirm sehen, und Ihnen beim Navigieren durch den Bereich helfen.

1. Klicken Sie auf das **Einstellungen**-Symbol ![Einstellungen](assets/setting-icon.png), um zu steuern, woher KI Informationen abruft, und wählen Sie dann einen der folgenden **Source-Typen**:

   * **Dokumente** - Dokumente, die in den ausgewählten Bereich hochgeladen wurden
   * **Web Search** — externe Web-Forschung
   * **CJA** — Adobe Customer Journey Analytics

1. Klicken Sie auf **Speichern**.

1. Klicken Sie auf **Hilfe**-Symbol ![Hilfe-Symbol](assets/more-information-icon.png), um die Tastaturbefehle anzuzeigen, mit denen Sie im Ideenraum navigieren oder einen anderen Zoom-Wert auswählen können.

   Wählen Sie aus den folgenden Zoomstufen:

   * Auf 100 % zoomen
   * Auf 200 % zoomen
   * An Fenstergröße anpassen

   Oder verwenden Sie einen der folgenden Tastaturbefehle, um auf der Seite zu navigieren:

   | Aktion | Tastenkombination |
   |---|---|
   | Vergrößern/Verkleinern | Strg/⌘ + / − |
   | An Auswahl anpassen/anpassen | – |
   | Zum Cursor zoomen | Strg/⌘ + Bildlauf |
   | Schwenken der Arbeitsfläche | Leertaste gedrückt halten + ziehen |
   | Punktraster ein-/ausblenden | G |

1. Klicken Sie auf das Suchsymbol, um im Ideenbereich nach Elementen zu suchen, und klicken Sie dann auf die -Anzeige in der Liste, um dorthin zu navigieren.








