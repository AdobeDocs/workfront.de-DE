---
title: "Best Practices für die Adobe Workfront-Planung"
description: Als Leiter von Marketingvorgängen können Sie mit Adobe Workfront Planning die Arbeit über den gesamten Marketing-Lebenszyklus für alle Ihre Teams organisieren. Dies sind einige Best Practices, die wir für die ersten Schritte mit der Workfront-Planung empfehlen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Best Practices für die Planung von Adobe Workfront

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Als Leiter von Marketingvorgängen können Sie mit Adobe Workfront Planning die Arbeit über den gesamten Marketing-Lebenszyklus für alle Ihre Teams organisieren.

In diesem Artikel werden einige Best Practices beschrieben, die wir beim Einstieg in die Workfront-Planung empfehlen.

## Was ist Workfront-Planung?

Das Workfront-Planungsmodul ist eine von drei unterschiedlichen, aber miteinander verbundenen Workfront-Funktionen, die zusammen ein Marketing-Aufzeichnungssystem erstellen. Die drei Funktionen sind:

* **Planung**: Die neuen erweiterten Funktionen der Workfront-Planung.

* **Workflow**: Die kollaborativen Arbeitsverwaltungsfunktionen, die Sie heute in Workfront verwenden (Projektmanagement, Ressourcenverwaltung usw.)

* **Automatisierung und Integration**: Die umfassenden Integrations- und Automatisierungsfunktionen von Workfront Fusion.

Die Workfront-Planung ist in hohem Maße anpassbar. Weitere Informationen zur Terminologie und zum Schlüsselkonzept der Workfront-Planung finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md).

## Fragen vor der Einrichtung der Workfront-Planung

Nachdem Sie sich mit der Terminologie und Architektur der Workfront-Planung vertraut gemacht haben, können Sie mit der Einrichtung Ihrer neuen Umgebung beginnen.

Einige Fragen, die Sie sich möglicherweise bei der Einrichtung der Planung stellen:

* **Möchten Sie Arbeitsbereiche für größere Unternehmensgruppen verwenden? Oder sollte ich die Menschen dazu ermutigen, persönliche zu gründen?**

  Sie werden vielleicht feststellen, dass es einen guten Nutzen für beide gibt. Es wird empfohlen, nicht zu viele Arbeitsbereiche zu verwenden, da diese sich als schwierig erweisen könnten und Ihre Arbeitsabläufe zu fragmentiert sein könnten.

  >[!TIP]
  >
  >    Sie können in einer Workfront-Instanz über 1.000 Arbeitsbereiche verfügen.

* **Welche benutzerdefinierten Datensatztypen sollte ich in den einzelnen Arbeitsbereichen erstellen?**

  Datensatztypen ähneln den Objekttypen von Workfront. Denken Sie an Ihre Workflows und entscheiden Sie, welche Datensatztypen (Arbeitsobjekte, Personenobjekte, Taxonomien usw.) jeden Workflow benötigen.

  Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md)

* **Wie erstelle ich meine Datensätze? Gibt es eine externe Liste oder Tabelle, die bereits die Datensätze enthält, die ich zur Planung hinzufügen muss und die ich verwenden kann? Werden Datensätze nach und nach hinzugefügt, je nach Bedarf? Oder werden sie mithilfe einer Fusion- oder benutzerdefinierten API-Integration importiert?**

  Weitere Informationen finden Sie unter:

   * [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md)
   * [Adobe Workfront-Planungsmodule](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **Welche Felder muss ich für meine Datensätze erstellen?**

  Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

* **Welche Workfront- oder AEM Assets-Objekttypen benötige ich, um eine Verbindung zu Workfront Planning-Record-Typen herzustellen, damit Abhängigkeiten angezeigt und ein nahtloser Workflow für mein Unternehmen erstellt werden kann?**

  Weitere Informationen finden Sie unter [Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types.md)

* **Welche Marketingkalender und -ansichten benötige ich, um die Geschichte meiner Kampagnen zu erzählen? Und welche Stakeholder könnte ich diese Ansichten für eine nahtlose Zusammenarbeit zur Verfügung stellen?**

  Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).


## Best Practices für die Planung von Workfront

In diesem Abschnitt werden verschiedene Vorgehensweisen und Best Practices für die Einrichtung der Workfront-Planung aufgeführt.

Die Richtlinien sind je nach dem Objekt oder Gebiet, das Sie einrichten, angeordnet.

### Arbeitsbereiche

#### Die Aufgaben und Aufgaben der Arbeitsbereiche

* Erstellen Sie Designs für die kleinste Anzahl von Arbeitsbereichen auf Unternehmensebene.

  Versuchen Sie beispielsweise, eine einzelne Workspace für alle Marketingaktivitäten zu erstellen.

* Kuratieren Sie Ihre Arbeitsbereiche regelmäßig. Möglicherweise können Sie eine vorhandene ändern, anstatt eine neue zu erstellen.

* Erstellen Sie eine neue Workspace für ein Team, das eine völlig andere Betriebsbewegung hat.

  Der Arbeitsbereich &quot;Produktentwicklung&quot;sollte sich von dem Arbeitsbereich &quot;Marketing&quot;unterscheiden

* Erstellen Sie nicht für jede Kleinigkeit einen eigenen Arbeitsbereich. Stellen Sie sich Arbeitsbereiche eher als ein Aufzeichnungssystem vor, das einer ganzen Organisation zugute kommen kann und es jedem ermöglicht, Workflows zu kartieren und zusammenzuarbeiten, anstatt einen privaten Raum zur Verfolgung persönlicher Anforderungen zu schaffen.

* Erstellen Sie keine eindeutigen Arbeitsbereiche für jedes Team oder jeden Prozess innerhalb einer Organisation.

  Die Marketing-Organisation sollte sich bemühen, nur einen Arbeitsbereich zu verwalten, um die Sichtbarkeit zu wahren und eine Datenaggregation auf globaler Planungs-Ebene zu ermöglichen.

  Vermeiden Sie die Erstellung ähnlicher oder doppelter Arbeitsbereiche für Teams, die ähnlichen Prozessen folgen (z. B. EMEA Marketing VS APAC Marketing), insbesondere dort, wo diese Teams Arbeiten durchführen können, die zu einer gemeinsamen strategischen Kampagne zusammengeführt werden.

#### Wie sollte ich Workspace-Abschnitte verwenden?

* Erstellen und beschriften Sie Abschnitte, damit Ihre Benutzer verstehen können, wie Sie Ihren Betriebslebenszyklus organisieren.

  Sie können beispielsweise einen Abschnitt mit der Bezeichnung &quot;Core Records&quot;erstellen, in dem Sie Ihre Kampagnen, Taktiken und Lieferziele platzieren.

* Gruppieren Sie &quot;like&quot;-Datensatztypen zusammen.

  Sie können einen Abschnitt mit der Bezeichnung &quot;Geografien&quot;erstellen, der Datensatztypen wie Region, Land und Stadt enthält.

#### Wie soll ich Arbeitsbereichsberechtigungen verwalten?

* Beschränken Sie den Zugriff auf &quot;Verwalten&quot;auf eine ausgewählte Gruppe vertrauenswürdiger Personen, die einen Datensatztyp nicht versehentlich löschen oder anderweitig unnötige Datensatztypen und -felder erstellen.

  >[!TIP]
  >
  >Wir haben während unseres Betaprogramms herausgefunden, dass viele Kunden den Gruppenadministratoren den Zugriff &quot;Verwalten&quot;gewähren.

* Fügen Sie den Planungsbereich der Layoutvorlage von Benutzern mit einer Standardlizenz hinzu.

* Erlauben Sie Benutzern mit einer Standardlizenz, persönliche Arbeitsbereiche zu erstellen. Dadurch erhalten sie einen sicheren Raum, um das Tool zu erlernen und sich damit vertraut zu machen. Dies wird das Erlebnis für andere nicht stören und kann die persönliche Produktivität des Benutzers verbessern.

  >[!TIP]
  >
  >    Empfehlen Sie ihnen, ihre persönlichen Arbeitsbereiche nicht als Best Practice freizugeben.


### Datensatztypen

#### Ein einzelnes oder Mehrfachauswahlfeld im Vergleich zu einem verknüpften Datensatztyp

* Erstellen Sie einen neuen Datensatztyp, wenn das Objekt in mehreren anderen Datensatztypen verwendet wird.

  Eine Kampagne kann beispielsweise mit mehreren Target-Zielgruppen verbunden sein und eine Tactik kann über eine Verbindung zu einer einzelnen Target-Zielgruppe verfügen.

* Erstellen Sie einen neuen Datensatztyp, wenn das Objekt zusätzliche Metadatenwerte speichern muss, die bei Suchen nützlich sein könnten.

  Beispielsweise kann ein Kanal-Record-Typ wie &quot;E-Mail&quot;eine Liste unterstützender Lieferziele speichern, entweder als native Metadaten oder als Verbindung zum eigenständigen &quot;Lieferziele&quot;-Record-Typ.

* Fügen Sie keinen neuen Datensatztyp hinzu, wenn die Daten, die Sie speichern, nur auf einen einzigen Datensatztyp übertragen werden müssen. Verwenden Sie stattdessen ein Auswahlfeld.

  Beispielsweise kann ein Kampagnentyp ein Feld mit einer Auswahl namens Kampagnengröße enthalten, das nur relevant ist, wenn er einer bestimmten Kampagne direkt zugeordnet ist.

#### Wie sollte ich meine Datensatztypen beschriften?

Erstellen und beschriften Sie Datensatztypen, die ein einzelnes Konstrukt oder Substantiv darstellen, z. B. &quot;Kampagnen&quot;

:no_entry_sign: Erstellen Sie keinen Datensatztyp, der besser als Ansichtsebene dargestellt wird. Beispielsweise ist &quot;Kalender&quot;eine schlechte Wahl für einen Datensatztyp, da es sich nicht um den Datensatztyp selbst, sondern um eine Ansicht von Datensätzen handelt.

### Wie viele Hierarchieebenen sollte ich erstellen?

Ansichten

...

Workflow

...

### Feldverwaltung

Primäres Feld

Verwenden Sie eindeutige Primärfeldwerte, um diese Datensätze beim Herstellen von Verbindungen leichter zu finden und zu &quot;wählen&quot;.

Bei der Herstellung einer Verbindung durchsuchen die Benutzer die Werte im Primären Feld. Wenn sie nicht eindeutig sind, wissen die Benutzer nicht, welche ausgewählt werden soll.

Vermeiden Sie die Verwendung nicht eindeutiger Werte als primäres Feld, da dies für Benutzer, die beim Verwenden des Verbindungsauswahl-Menüs im Primärfeld suchen müssen, Verwirrung verursachen kann.



Von Chris O&#39;Neal:

Ein weiterer Bereich, über den bzw. den nicht nachgedacht werden kann, sind Anwendungsfälle, die für die Planung am besten geeignet sind (oder sind). Zum Beispiel die Diskussion über die Ressourcenverwaltung, die wir heute hatten.



Alinas Notizen:

Beispiel für den Artikel &quot;Best Practices&quot;von ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Zusätzliche Informationen von Field Readiness von Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346