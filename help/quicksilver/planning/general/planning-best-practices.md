---
title: Adobe Workfront-Planungsempfehlungen für die Implementierung
description: Als Leiter von Marketing-Abläufen können Sie mit Adobe Workfront Planning die Arbeit über den gesamten Marketing-Lebenszyklus hinweg für alle Ihre Teams organisieren. Dies sind einige Best Practices, die wir für den Einstieg in die Workfront-Planung empfehlen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '3362'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront Planungsempfehlungen für die Implementierung

<!-- this used to be called Adobe WFP best practices, but the best practice piece was replaced by this folder of articles: [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) -->

{{planning-important-intro}}

Als Leiter von Marketing-Abläufen können Sie mit Adobe Workfront Planning die Arbeit über den gesamten Marketing-Lebenszyklus hinweg für alle Ihre Teams organisieren.

In diesem Artikel werden einige häufig gestellte Fragen und Best Practices beschrieben, die wir für den Einstieg in Workfront Planning empfehlen.

Weitere Informationen finden Sie in den Artikeln in den [Best Practices für die Adobe Workfront-Planung: Artikelindex](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).


## Best Practices für die Konfiguration

### Arbeitsbereiche

Arbeitsbereiche sind zentrale Orte, an denen Teams ihre Arbeit planen können. Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen.

Im Folgenden finden Sie einige häufig gestellte Fragen zur Konfiguration von Workfront Planning.

#### Wie sollte ich beginnen?

* ✅ Wenn Sie sich zum ersten Mal bei Planning anmelden, folgen Sie unserem In-App-Onboarding-Prozess, der den Wert von Planning klar vermittelt und Sie bei der Navigation und der effektiven Verwendung des Produkts führt. Dadurch wird sichergestellt, dass Sie die Funktionen von verstehen und leicht mit Ihrer Arbeit beginnen können.
* ✅ erkunden Sie zunächst unsere vordefinierten Arbeitsbereich-Vorlagen, um Ideen für vorhandene ähnliche Anwendungsfälle zu erhalten. Sie können die vordefinierten Datensatztypen und Felder in einer Vorlage verwenden oder eigene hinzufügen.
* ✅ Identifizieren Sie die wichtigsten Anwendungsfälle, die Sie mit Workfront Planning lösen möchten. Die meisten Unternehmen möchten zum Beispiel den Überblick über strategische Aktivitäten verbessern, wozu auch die Erstellung eines besseren „Kampagnenkalenders“ gehören kann. Für diesen Anwendungsfall sollten Sie also zunächst einige Fragen beantworten:

   * Wer fragt danach?
   * Wie nennen sie die Dinge, die sie in den Kalender aufnehmen wollen?
Kampagnen? Taktik? Initiativen? Aktivitäten? Ereignisse?
   * Welche Fragen möchten sie mit diesem Kalender beantworten?
   * Gibt es überlappende Kampagnen für dieselbe Zielgruppe?
   * Wie hoch ist das Budget für diese Kampagne, Taktik, Aktivität oder dieses Ereignis?

  Die Antworten auf diese Fragen legen fest, was Sie in Workfront Planning erstellen müssen.

  Beachten Sie außerdem, dass es möglicherweise andere Planende gibt, die derzeit keine Workfront-Benutzer sind. Diese Planer können mit Excel-Tabellen, Word-Dokumenten, PowerPoint-Präsentationen usw. arbeiten. Überlegen Sie, wie sie in Workfront Planning auf Ihre Informationen zugreifen können.

* ✅ Um die Vorteile von Workfront Planning voll auszuschöpfen, sollten Sie in Workfront die Verwendung von Portfolios und Programmen durch eine andere Oberstufenstruktur in Workfront Planning ersetzen.

  Heute präsentieren Workfront-Kunden ihre strategische Arbeit durch Portfolios und Programme, in einigen Fällen als Projekte unterschiedlicher Art. Mit der Einführung von Planning sollte all diese strategische Arbeit durch benutzerdefinierte Datensatztypen in Workfront Planning abgewickelt werden, während Workfront sich auf die Ausführungsphase von Arbeit konzentriert, die als Projekte und Aufgaben dargestellt wird.

#### Wann sollte ich einen neuen Arbeitsbereich erstellen anstatt einen vorhandenen zu ändern?

* ✅ Design für die geringste Anzahl von Arbeitsbereichen auf Unternehmensebene. Sie können Arbeitsbereiche für bestimmte operative Organisationseinheiten entsprechend der individuellen Funktionsweise der einzelnen Einheiten erstellen.

  Informationen in einem einzigen Workspace zu haben, um sicherzustellen, dass Beziehungen zwischen allen Daten einfach verwaltet werden können.

  Versuchen Sie beispielsweise, einen einzigen Arbeitsbereich für die gesamte Marketing-Abteilung zu erstellen.

  Es ist in Ordnung, einen neuen Arbeitsbereich für ein Team zu erstellen, das eine völlig andere Betriebsstruktur hat:

  Beispielsweise sollte sich ein Arbeitsbereich **Produktentwicklung** von einem Arbeitsbereich **Marketing** unterscheiden.

* ⛔ Erstellen Sie keine eindeutigen Arbeitsbereiche für jedes Team oder jeden Prozess innerhalb einer Organisation.

  Die Marketing-Organisation sollte sich bemühen, nur einen Arbeitsbereich zu verwalten, um die Sichtbarkeit zu erhalten und Daten auf globaler Planungsebene aggregieren zu können.

  Vermeiden Sie die Erstellung ähnlicher oder doppelter Arbeitsbereiche für Teams, die ähnlichen Prozessen folgen (z. B. EMEA-Marketing oder APAC-Marketing), insbesondere wenn diese Teams Arbeiten erledigen können, die den üblichen strategischen Kampagnen entsprechen.

#### Wie sollte ich Workspace-Abschnitte verwenden?

* ✅ Erstellen und beschriften Sie die Abschnitte, um Ihren Benutzern zu zeigen, wie Sie Ihren Betriebslebenszyklus organisieren.

  Sie können beispielsweise einen Abschnitt mit dem Namen **Core-Datensätze** erstellen, in dem Sie Ihre Kampagnen, Taktiken und Ergebnisse in Ihrem Arbeitsbereich platzieren.
* ✅ Datensatztypen „like“ zusammen gruppieren.

  Sie können beispielsweise einen Abschnitt mit dem Namen &quot;**&quot; erstellen** der Datensatztypen wie „Region“, „Land“ und „Stadt“ enthält.

### Eintragstypen

Datensatztypen sind die Bausteine einer Workfront Planning-Workspace. Sie können festlegen, wie Datensatztypen miteinander verbunden werden.

#### Wie sollte ich Datensatztypen in meinem Arbeitsbereich definieren?

* ✅ Es kann einige Zeit dauern, bis Sie herausgefunden haben, welche Informationen Sie nachverfolgen müssen (welche Datensatztypen ich benötige) und wie diese Informationen verknüpft werden müssen. Sprechen Sie mit den Stakeholdern, die den Arbeitsbereich verwenden werden, um alle ihre Anforderungen zu berücksichtigen. Sie können auch benutzerdefinierte Abschnitte mit verschiedenen Datensatztypen erstellen, um die Informationen auf sehr benutzerfreundliche Weise darzustellen.

* ⛔ Duplizieren Sie keine Datensatztypen für einen anderen Zeitraum (erstellen Sie beispielsweise keine separaten Datensatztypen für **Kampagnen 2024“** &quot;**2025**).

  Wenn Sie verschiedene Datensatztypen erstellen, unterbricht dies den Datenfluss, wenn Sie Daten über mehrere Jahre hinweg vergleichen möchten. Die Ansichten heute sind pro Datensatztyp. Sobald das Jahr endet, zeigt die Ansicht dieses Datensatztyps nicht mehr die zukünftigen Elemente an. Es empfiehlt sich, für die Art der Arbeit einen einzigen Datensatztyp zu verwenden und die Daten mithilfe von Filtern zu segmentieren, die auf verschiedenen Feldern basieren, oder sie bei Bedarf zu archivieren.

#### Wann sollte ich ein einzelnes oder Mehrfachauswahlfeld gegenüber einem verknüpften Datensatztyp verwenden?

* ✅ Einen neuen Datensatztyp hinzufügen, wenn das Objekt in Verbindung mit mehreren anderen Datensatztypen verwendet wird

  Eine Kampagne kann beispielsweise eine Verbindung zu mehreren Target-Zielgruppen haben, und eine Taktik kann eine Verbindung zu einer einzelnen Target-Zielgruppe haben. Daher sollten Campaign, Taktik und Audience Datensatztypen und keine Felder mit Mehrfachauswahl sein.

* ✅ Fügen Sie einen neuen Datensatztyp hinzu, wenn das Objekt zusätzliche Metadatenwerte speichern muss, die bei der Suche nützlich sein können

  Beispielsweise kann ein Kanaldatensatztyp wie **E-Mail** eine Liste unterstützender Ergebnisse speichern, entweder als native Metadaten oder als Verbindung zu einem eigenständigen Datensatztyp **Ergebnisse**.
* ⛔ Fügen Sie keinen neuen Datensatztyp hinzu, wenn die Daten, die Sie speichern, nur für einen einzelnen Datensatztyp relevant sind.

  Ein Datensatztyp **Kampagne** kann beispielsweise über ein Einzelauswahlfeld namens „Kampagnengröße **verfügen,** nur relevant ist, wenn er direkt mit einer bestimmten Kampagne verknüpft ist. Erstellen Sie stattdessen ein Feld , um diese Informationen zu erfassen.

#### Wie sollte ich meine Datensatztypen beschriften?

* ✅ Datensatztypen, die ein einzelnes Konstrukt oder Substantiv darstellen, wie z. B. **Kampagnen“, erstellen und**.
* ⛔ Erstellen Sie keinen Datensatztyp, der besser als Ansicht dargestellt wird.

  Beispielsweise ist **Kalender** eine schlechte Wahl für einen Datensatztyp, da es nicht der Datensatztyp selbst ist, sondern eine Ansicht von Datensätzen.

### Außendienstverwaltung

Felder sind Attribute von Datensatztypen und werden in der Tabellenansicht als Spalten angezeigt. Sie können benutzerdefinierte Felder für Datensatztypen erstellen und diese Felder dann mit Workfront Planning-Datensätzen verknüpfen, um Datensatzinformationen zu verbessern.

#### Welches Feld sollte als Primäres Feld definiert werden?

* ✅ Verwenden Sie keine eindeutigen primären Feldwerte, um das Auffinden und „Auswählen“ dieser Datensätze bei Verbindungen zu erleichtern. 

  Beim Herstellen einer Verbindung suchen Benutzende nach den Werten im Primären Feld. Wenn die Werte nicht eindeutig sind, wissen die Benutzenden nicht, welche ausgewählt werden sollen. 
* ⛔ Verwenden Sie nicht eindeutige Werte nicht als primäres Feld, da dies zu Verwirrung bei Benutzenden führen kann, die beim Verwenden des Menüs „Verbindungsauswahl“ im primären Feld suchen müssen. 

#### Wie sollte ich Formeln verwenden?

* ✅ Verwenden Sie Formelfeldtypen, um manuelle Eingaben zu reduzieren. Wenn Sie Informationen eingeben, die auf Daten basieren, die sich bereits in Ihrer Tabellenansicht befinden, können Sie möglicherweise etwas Aufwand sparen, indem Sie diese Informationen automatisch mithilfe von Formeln berechnen.

#### Wie sollte ich die Daten in meinem Arbeitsbereich verbinden?

* ✅ Erstellen von Verbindungen ist eine der leistungsfähigsten Funktionen von Workfront Planning. Sie können Datensatztypen miteinander oder Datensatztypen mit Objekttypen aus anderen Programmen wie Adobe Workfront (Verbindung zu Projekten, Portfolios, Programmen, Unternehmen und Gruppen), Adobe Experience Manager Assets (Verbindung zu Assets und Ordnern) und Adobe GenStudio for Performance Marketing verbinden.

  Das Verbinden von Objekt- und Datensatztypen gibt Ihnen einen vollständigen Überblick darüber, wie alles in Ihrem Unternehmen verbunden ist.

  Sie haben beispielsweise einen Datensatztyp **Kampagne** und einen Datensatztyp **Taktik** und Sie können eine Verbindung zwischen diesen beiden Datensatztypen erstellen, um zu sehen, welche **Taktiken** einer bestimmten **Kampagne** zugeordnet sind.

  Nachdem Sie die Verbindung definiert haben, können alle Personen im Arbeitsbereich mit dem Hinzufügen von Werten für **Kampagnen** beginnen, indem sie in das Verbindungsfeld doppelklicken, wo eine Liste aller **Taktiken** verfügbar angezeigt wird. Auf diese Weise können Sie schnell herausfinden, welche Taktiken mit Ihren Kampagnen verknüpft werden müssen.

#### Wie sollte ich Suchfelder verwenden?

* ✅ Nachdem Sie die Verbindung zwischen Datensätzen oder Objekttypen hergestellt haben, können Sie einzelne Datensätze miteinander verbinden und Felder aus den verknüpften Datensatz- oder Objekttypen in einem Workfront Planning-Datensatz anzeigen. Sie werden die Anzahl der Stellen reduzieren, an denen Sie dieselbe Information aktualisieren müssen, und sicherstellen, dass sie perfekt übereinstimmen.

  Wenn Sie beispielsweise eine Verbindung zwischen einem Datensatztyp **Kampagne** und einem Datensatztyp **Taktik** haben, werden die primären Feldinformationen angezeigt. Wenn Sie jedoch Suchfelder hinzufügen, können Sie zusätzliche Informationen aus diesem Datensatztyp hinzufügen, z. B. das **Startdatum** für einen **Taktik**. Die Daten für diese Suchfelder werden automatisch ausgefüllt, nachdem die Datensätze hinzugefügt wurden.

#### Welcher Feldtyp wird für URLs empfohlen? 

* ✅ Verwenden Sie ein einzeiliges Textfeld, um einem Datensatz URL-Daten hinzuzufügen.

### Ansichten 

#### Wie entscheide ich zwischen einer Ansicht und einem Datensatztyp?

* ✅Erstellen Sie für Elemente, die ein einzelnes Konstrukt oder Substantiv darstellen (z **B** Kampagnen), einen Datensatztyp. 

* ⛔ Erstellen Sie keinen Datensatztyp, der besser als Ansicht dargestellt wird.

  Beispielsweise ist **Kalender** eine schlechte Wahl für einen Datensatztyp, da es nicht der Datensatztyp selbst ist, sondern eine Ansicht von Datensätzen. 

#### Sollte ich Felder ausblenden oder löschen, die für mich nicht relevant sind?

* ✅ Die Spalte ausblenden, anstatt sie zu löschen, wenn diese Informationen für eine andere Person mit demselben Datensatztyp relevant sein könnten. Wenn Sie das Feld in einer bestimmten Tabellenansicht löschen, wird dieses Feld auch in den übrigen Ansichten dieses Datensatzes sowie überall dort gelöscht, wo dieser Datensatztyp verknüpft ist.

#### Wie sollte ich Filter und Gruppierungen in den Tabellen- und Zeitleisten-Ansichten verwenden?

* ✅ Verwenden Sie Ansichten mit Filtern und Gruppierungen, um einen Schnappschuss dessen anzuzeigen, was Sie sehen müssen. Sie können die Daten filtern und gruppieren, um besser verstehen zu können, was geplant ist. Sie können die Datensätze nach Metadatenfeldern gruppieren.

  Sie können beispielsweise eine Zeitleisten -Ansicht für Ihren Datensatztyp **Kampagne** verwenden, die Sie nach „Zielgruppen **gruppieren** nach **Datum** filtern können, um nur das aktuelle Jahr anzuzeigen.

#### Warum sehe ich nicht alle Datensätze in meiner Zeitleisten-Ansicht?

* ✅ Denken Sie daran, zwei Datumsfelder für Ihre Datensätze zu definieren. Sie können eine Zeitleisten -Ansicht nur erstellen, wenn Sie mindestens zwei Datumsfelder mit einem Datensatztyp verknüpft haben. Einige Datensätze werden möglicherweise nicht in der Zeitleisten -Ansicht angezeigt, wenn entweder das Start- oder Enddatum oder beide keine Werte aufweisen oder wenn das Startdatum nach dem Enddatum liegt.

#### Wie sollte ich die Einstellungen für die Zeitleisten-Ansicht verwenden?

* ✅ Definieren Sie die Einstellungen Ihrer Zeitleistenansicht, z. B. den **Balkenstil** und die **Farbe**, um eine visuell ansprechendere Ansicht zu erhalten. Sie können den **Balkenstil** anpassen, indem Sie festlegen, ob eine Miniaturansicht mit einem aussagekräftigen Bild angezeigt werden soll, und weitere Felder hinzufügen, die auf der Leiste angezeigt werden sollen (z. B. **Inhaber** oder **Status**).

  Standardmäßig wird nur das primäre Feld angezeigt. Sie können die Farbe Ihres Balkens auch nach Feldwerten (Sie können beispielsweise die Farben Ihrer Balken anpassen, indem Sie sie mit dem Feld Status abgleichen) oder nach der angewendeten Gruppierung definieren. Standardmäßig entspricht die Farbe der Farbe des Datensatztyps.

  Nur Farben des Datensatztyps oder Felder mit Optionen, die mit Farben verknüpft sind, können sich auf die Farben der Datensatzleisten in der Zeitleiste auswirken.

### Berechtigungen und Freigabe

Verwenden Sie die Freigabefunktion, um anderen Benutzern die entsprechenden Berechtigungen für Ansichten und Arbeitsbereiche zu erteilen.

#### Wie sollte ich Berechtigungen für Arbeitsbereiche verwalten?

* ✅ Wenn Sie einen **Arbeitsbereich** erstellen, steht er nur Ihnen zur Verfügung. Alle anderen, die keine Systemadministratoren sind, können sie nicht finden. Sobald der Arbeitsbereich definiert ist und Sie bereit sind, Ihr Team für die Zusammenarbeit hinzuzuziehen, müssen Sie ihn für es freigeben und seine Berechtigungsstufe definieren.

  Sie können aus den folgenden Berechtigungsebenen auswählen:

   * **Verwalten**: Benutzer können den Arbeitsbereich bearbeiten, löschen und freigeben, Datensatztypen hinzufügen sowie Datensätze bearbeiten, löschen und erstellen.
   * **Beitragen**: Benutzer können Datensätze erstellen, bearbeiten und löschen.
   * **Anzeigen**: Benutzer können Datensätze anzeigen.

* ✅ Obwohl viele Kunden den Eindruck haben, dass sie Workspaces **Verwalten**-Berechtigungen für die meisten Benutzer erteilen würden, beschränken Sie die **Verwalten**-Berechtigungen auf eine ausgewählte Gruppe vertrauenswürdiger Personen, die keinen Datensatztyp versehentlich löschen oder anderweitig unnötige Datensatztypen und -felder erstellen. Sie können den Arbeitsbereich bearbeiten, freigeben und sogar löschen. Mit dieser Berechtigungsstufe erhalten sie vollständigen administrativen Zugriff auf die Workspace.

  Für die Verwaltung von Berechtigungen für einen Arbeitsbereich ist eine Standardbenutzerlizenz erforderlich.

* ✅ Erteilen Sie Benutzern **Beitragen** Berechtigungen, wenn Sie möchten, dass sie nur Datensätze erstellen, bearbeiten und löschen können, sie jedoch nicht die Struktur des Arbeitsbereichs ändern sollen. Mit **Contribute**-Berechtigungen können sie keine Datensatztypen erstellen oder die Felder in den vorhandenen Datensatztypen ändern.

  Eine Standardbenutzerlizenz ist erforderlich, damit eine Person über **Beitragen**-Berechtigungen für einen Arbeitsbereich verfügt.

* ✅ Erteilen Sie Benutzern **Anzeigen**-Berechtigungen, wenn sie nur Datensätze anzeigen sollen.

#### Wie sollte ich Berechtigungen für Datensatztypen verwalten?

* ✅ Denken Sie daran, dass die Berechtigungen von Benutzern mit den Verwaltungsberechtigungen für Arbeitsbereiche für den Datensatztyp nicht verringert werden können. Sie erben auch die Verwaltungsberechtigungen für den Datensatztyp. Sie können einem Benutzer keine Verwaltungsberechtigungen für den Arbeitsbereich erteilen, aber Beitragen- oder Anzeigeberechtigungen für den Datensatztyp erteilen.
* ✅ Wenn Sie möchten, dass Benutzende für den Datensatztyp eine niedrigere Berechtigungsstufe (z. B. Anzeigeberechtigungen) haben als für den Arbeitsbereich, empfehlen wir, ihnen Beitragsberechtigungen für den Arbeitsbereich zu erteilen. Anschließend können Sie ihnen Anzeigeberechtigungen für den Datensatztyp erteilen.
* Wenn Sie einen Benutzer aus den Berechtigungen des Datensatztyps entfernen, erhält er dennoch mindestens die Berechtigung zum Anzeigen des Arbeitsbereichs.

#### Wie sollte ich Berechtigungen für Ansichten verwalten?

* ✅ reservieren die **Verwalten**-Berechtigungen für Personen, die Sie bearbeiten, löschen und die Ansicht freigeben können möchten. Das bedeutet, dass sie die Filter, Gruppierungsfelder oder eine Konfiguration der Ansicht ändern können. Diese Änderungen wirken sich auf die Hauptkonfiguration der Ansicht für alle anderen aus, die ebenfalls die Ansicht verwenden.

  Für die Verwaltung von Berechtigungen für eine Ansicht ist eine Standardbenutzerlizenz erforderlich.

* ✅ Erteilen Sie Benutzern **Ansicht** Berechtigungen, um die Ansicht anwenden zu können. Sie können einige Filter oder Gruppierungen und die Sortierung ändern, diese Änderungen sind jedoch nur temporär. Die Änderungen werden nicht für alle anderen Benutzer gespeichert, die auf die Ansicht zugreifen. Diese Änderungen wirken sich nicht auf die Hauptkonfiguration der Ansicht für alle anderen aus, die ebenfalls die Ansicht verwenden.  Ihre Änderungen sind nur für den Benutzer sichtbar, der die geänderten Einstellungen anwendet. Nach Aktualisierung des Bildschirms werden die Änderungen auf den Standardwert zurückgesetzt.

* ✅ Erteilen Sie **Alle im Arbeitsbereich können anzeigen** Berechtigungen, wenn jeder, der den Arbeitsbereich anzeigen kann, die Datensätze und deren Felder in dieser spezifischen Ansicht sehen soll. Auf diese Weise müssen Sie für die Ansicht niemanden manuell zum Feld für die Freigabeberechtigung hinzufügen.

  >[!NOTE]
  >
  >Wenn eine Ansicht nicht freigegeben wurde und Sie einen Link dazu für andere Personen freigeben, können diese die Datensätze in der &quot;**Tabellenansicht“**. Wenn sie über eine Standard-Workfront-Lizenz verfügen, können sie ihre eigene Ansicht erstellen.

#### Wie unterscheidet sich die Freigabe von **Workspace** der **Ansichtsfreigabe**?

* **Workspace-Freigabe** Definiert den Zugriff von Personen auf den Arbeitsbereich, seine Datensatztypen, Datensätze und deren Felder.

* **Ansichtsfreigabe** legt fest, ob der/die Benutzende die von Ihnen erstellte Ansicht sehen kann und ob er/sie den Filter, die Gruppierungsfelder oder eine andere Konfiguration der Ansicht ändern kann. Die Sichtbarkeit der in der Ansicht angezeigten Datensätze wird durch die Freigabe von Workspace und nicht durch die Freigabe von Ansichten gesteuert.

#### Wie wirken sich Workfront-Lizenztypen auf Workfront Planning-Berechtigungen aus?

* Für die **Freigabe von Workspace**: Lizenzanwender von Light und Contribute können nur Ansichtszugriff auf einen Arbeitsbereich erhalten. Um jemandem die Berechtigung Beitragen oder Verwalten für einen Arbeitsbereich zu erteilen, muss er über eine Standardlizenz verfügen.

* **Ansichtsfreigabe**: Benutzer von Standardlizenzen, die über Verwaltungsberechtigungen für einen Arbeitsbereich verfügen, können eine Ansicht erstellen. Benutzer von Light and Contribute-Lizenzen können nur die Ansichten verwenden, die von Standardbenutzern erstellt und für sie freigegeben wurden. Andernfalls können Benutzende, wenn nichts freigegeben wurde, die &quot;**Tabellenansicht“**.

#### Was sollte ich tun, wenn ein Workspace-Besitzer wechselt?

* Workfront legt den Workspace-Ersteller als Eigentümer fest, der Eigentümer hat jedoch funktionell dieselben Berechtigungen wie jeder andere Benutzer mit der Berechtigung „Verwalten“.
* Wenn der Eigentümer deaktiviert ist, können andere Mitglieder ihre Arbeit im Arbeitsbereich ohne Unterbrechung fortsetzen.
* Systemadministratoren haben Zugriff auf jeden Arbeitsbereich. Wenn also der Eigentümer die einzige Person mit der Berechtigung „Verwalten“ ist, können Administratoren eine weitere Person hinzufügen und ihr die Berechtigung „Verwalten“ für die Verwaltung des Arbeitsbereichs erteilen.

### Übermitteln von Anfragen in Workfront Planning

Sie können für jeden Datensatztyp ein Anfrageformular erstellen, wenn Benutzer Datensätze außerhalb der Seite eines Datensatztyps hinzufügen sollen. Durch Senden des Formulars wird dem Datensatztyp ein neuer Datensatz hinzugefügt.

#### Wann sollte ich mit der Erstellung eines Anfrageformulars für einen Datensatztyp beginnen?

* ✅ Sie sollten sicherstellen, dass die Struktur des Datensatztyps zuerst eingerichtet wird, indem Sie die erforderlichen Felder zur Tabelle hinzufügen. Diese Felder beschreiben Ihre Datensätze und stehen im Formular-Builder zur Verfügung.

  Idealerweise sollten Sie das Anfrage- oder Aufnahmeformular erstellen, nachdem Ihre Datensatztypstruktur finalisiert wurde, um zu vermeiden, dass Schlüsselfelder fehlen.

#### Wer kann Anfrageformulare erstellen?

* ✅ Jeder Benutzer mit der Zugriffsberechtigung Verwalten auf den Arbeitsbereich kann ein Anfrageformular für einen Datensatztyp erstellen oder bearbeiten. Stellen Sie sicher, dass die Benutzerberechtigungen ordnungsgemäß zugewiesen sind, um diese Funktion zuzulassen.

#### Wie sollte ich ein Anfrageformular für einen Datensatztyp erstellen oder bearbeiten?

* ✅ Benutzer mit der Rolle „Zugriff auf den Arbeitsbereich verwalten“ können die Schritte ausführen, die im Artikel [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning“ beschrieben ](/help/quicksilver/planning/requests/create-request-form.md).


#### Wer kann neue Datensätze mithilfe des Anfrageformulars einreichen?

* ✅ Berechtigungen zum Senden hängen von den Einstellungen ab, die Sie für jedes Formular konfigurieren.

  Im Formular-Builder können Sie nach der Veröffentlichung des Formulars Berechtigungen verwalten, um zu steuern, wer Anfragen senden kann.

  Sie können aus den folgenden Freigabeoptionen wählen:

   * Für die interne Freigabe mit Personen in Workfront:

      * **Jeder mit Ansicht oder Zugriff auf den Arbeitsbereich:** Alle Benutzer mit Ansicht oder höheren Berechtigungen für den Arbeitsbereich können eine Anfrage senden, die einen Datensatz erstellt.
      * **Alle mit Zugriff auf den Arbeitsbereich, der Beiträge leistet oder darüber**: Beschränkt die Übermittlung auf Benutzer mit der Berechtigung „Beitragen“ oder einer höheren Berechtigung für den Arbeitsbereich.
      * **Nur eingeladene Personen können zugreifen**: Fügen Sie Personen, Teams, Rollen, Gruppen oder Unternehmen hinzu, die Anfragen an das Formular senden können.
   * Für die externe Freigabe für Personen ohne Workfront-Konto:
      * **Erstellen Sie einen öffentlichen Link** und kopieren Sie ihn dann und geben Sie ihn für alle frei, auch für Personen ohne Workfront-Konto: Ermöglicht es allen Benutzern, die den Formular-Link haben, eine Anfrage zu senden.
      * **Link-Ablaufdatum:** Stellen Sie sicher, dass Sie ein Ablaufdatum für den öffentlichen Link festlegen, um die Sicherheit zu erhöhen.

### Best Practices für die Verwaltung von Anfrageformularen

Im Folgenden finden Sie Empfehlungen für die Verwaltung von Anfrageformularen:

* Planen Sie im Voraus: Definieren Sie klar, welche Informationen von den Anfragenden benötigt oder benötigt werden, bevor Sie das Formular erstellen, um zu vermeiden, dass später übermäßige Revisionen vorgenommen werden.
* Klare Beschriftungen verwenden: Stellen Sie sicher, dass Feldbeschriftungen und Beschreibungen für alle Benutzer klar und verständlich sind.
* Testen von Formularen: Testen Sie Formulare vor dem Rollout neuer Formulare für eine breitere Zielgruppe mithilfe der Option Formular-Link und Formularvorschau , um sicherzustellen, dass alle Felder und Logiken wie erwartet funktionieren.
* Formulare auf dem neuesten Stand halten: Formulare werden regelmäßig überprüft und aktualisiert, damit sie etwaigen Änderungen in der Struktur des Datensatztyps oder in betrieblichen Prozessen entsprechen.

<!--do we need to add anything for the Configuration tab of a request form?? -->

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->