---
product-area: reporting
navigation-topic: text-mode-reporting
title: Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen
description: Mit EXISTS-Anweisungen können Sie komplexe Textmodusfilter erstellen. Dieser Artikel erfordert ein gründliches Verständnis der Adobe Workfront-API und der Textmodus-Berichterstellungsoberfläche.
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '2660'
ht-degree: 0%

---

# Erstellen komplexer Textmodusfilter mit EXISTS-Anweisungen

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Dieser Artikel erfordert ein gründliches Verständnis der Adobe Workfront-API und der Textmodus-Berichterstellungsoberfläche. Weitere Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).\
>Weitere Informationen zur Verwendung des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Übersicht über Objektbeziehungen in Workfront

Alle Objekte sind mit anderen Objekten in der Workfront-Datenbank verknüpft.

Wenn Sie die Hierarchie und Interdependenz von Objekten verstehen, können Sie herausfinden, auf welche Objekte in Berichten verwiesen werden kann.

Informationen darüber, welche Objekte sich in Workfront befinden, sowie über ihre Hierarchie und Interdependenz finden Sie unter [Übersicht über Adobe Workfront-Objekte](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Beim Erstellen von Filtern können Sie mithilfe der standardmäßigen Berichtsschnittstelle innerhalb von bis zu zwei Beziehungsebenen auf andere Objekte verweisen, die mit dem Objekt des Filters verbunden sind.

Sie können beispielsweise in einem Problemfilter auf die Portfolio-ID verweisen, um mithilfe der Standardschnittstelle nur Probleme in Projekten anzuzeigen, die mit einem bestimmten Portfolio verknüpft sind. In diesem Fall ist das Portfolio zwei Ebenen von Problemen entfernt.

Sie können jedoch nicht in einem Problemfilter mithilfe der Standardschnittstelle auf den Eigentümer des Portfolios verweisen, um nur Probleme aus Projekten anzuzeigen, die mit Portfolios verknüpft sind, in denen der Eigentümer ein bestimmter Benutzer ist. Sie müssen den Textmodus verwenden, um auf das Feld Name des Portfolio-Inhabers zuzugreifen, das drei Ebenen von Problemen entfernt ist.

![Problem mit Symbolen für Portfoliobesitzer](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Eine vollständige Liste der Objekte in Workfront finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

Informationen zum Navigieren im API Explorer und Suchen von Objekten finden Sie unter [Verwenden des API Explorers](../../../wf-api/general/using-api-explorer.md).

Beim Erstellen von Filtern müssen Sie in der Textmodusschnittstelle komplexe Anweisungen erstellen, um auf diese Objekttypen zu verweisen.

Informationen zum Erstellen komplexer Filter finden Sie im Abschnitt [Übersicht über Filter für den komplexen Textmodus, die EXISTS-Anweisungen verwenden](#overview-of-complex-text-mode-filters-that-use-exists-statements) dieses Artikels.

## Übersicht über komplexe Textmodusfilter, die EXISTS-Anweisungen verwenden {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Beachten Sie Folgendes beim Erstellen von Filtern, die sich über mehrere Ebenen in der Objekthierarchie erstrecken oder nach fehlenden Objekten filtern:

* Sie müssen komplexe Filter erstellen, wenn Sie auf Objekte verweisen möchten, die nicht direkt mit dem Filterobjekt verbunden sind.
* Sie müssen eine EXISTS-Anweisung verwenden, um Folgendes auszuführen:

   * Erstellen Sie Filter, die mehrere Ebenen umfassen.
   * Erstellen Sie Filter, die nach fehlenden Objekten suchen.\
     Wenn Sie beispielsweise einen Benutzerbericht erstellen, können Sie nach Benutzern filtern, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben.

Beachten Sie die folgenden Regeln, wenn Sie EXISTS-Anweisungen in einem Filter verwenden:

* Es gibt drei Objekte, auf die Sie in einem EXISTS-Filter verweisen können:

   * Das -Objekt des Filters (Original-Objekt).
   * Das Objekt, auf dessen Feld Sie verweisen möchten (Zielobjekt).
   * Das -Objekt, das das Original- und das Zielobjekt verbindet, falls sie nicht direkt miteinander verbunden sind (Verknüpfungsobjekt).

* Filter, die EXISTS verwenden, enthalten zwei separate Anweisungen, die durch ein Gleichheitszeichen verknüpft sind:

   * Die Anweisung vor dem Gleichheitszeichen bezieht sich auf das Objekt, auf das Sie verweisen (das Verknüpfungsobjekt oder das Zielobjekt).
   * Die Anweisung nach dem Gleichheitszeichen bezieht sich auf das Objekt, von dem aus Sie verweisen (das Original-Objekt).

* Sie müssen den Objektcode des Verknüpfungsobjekts verwenden, um Ihre Anweisungen zu verbinden.\
  Den Objektcode aller Objekte finden Sie im API Explorer.\
  Weitere Informationen zum API-Explorer finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

* Wenn ein Verknüpfungsobjekt fehlt, weil das Original- und das Zielobjekt direkt miteinander verbunden sind, können Sie den Objektcode des Zielobjekts anstelle des Verknüpfungsobjekts verwenden.
* Sie können auf mehrere Felder (Zielfelder) desselben Objekts (Zielobjekt) verweisen. In diesem Fall müssen Sie die Zeilen verbinden, die auf die Felder durch UND verweisen.\
  Portfolio Ein Beispiel für das Filtern nach mehr als einem Feld, das zum Zielobjekt gehört, finden Sie im Abschnitt [Beispiel 4: Filtern nach mehreren Feldern: Aufgaben nach Namen des Aufgabenbesitzers und ID der Scorecard für die Ausrichtung des Portfolios ](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) in diesem Artikel.

* Der einzige für eine EXISTS-Anweisung unterstützte Modifikator ist NOTEXISTS.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Filter in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berichtsberechtigungen zum Bearbeiten von Filtern in einem Bericht</p> <p>Verwalten von Berechtigungen für einen Filter, um ihn zu bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen komplexer Textmodusfilter, die sich über mehrere Ebenen in der Objekthierarchie erstrecken

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Sie können einen Filter erstellen, der auf Objekte über mehrere Ebenen der Objekthierarchie hinweg verweist, in der das Filterobjekt vorhanden ist. Sie können beispielsweise einen Problemfilter für Probleme erstellen, die sich in Projekten befinden, die nicht mit einem bestimmten Portfolio-Inhaber verknüpft sind.

Sie müssen immer eine EXISTS-Anweisung und die Textmodus-Schnittstelle verwenden, um diesen Filter zu erstellen.

Beispiele für Filter finden Sie im Abschnitt [Beispiel 1: Nach Namen des Portfolios nach ](#example-1-filter-for-issues-by-portfolio-owner-name) filtern) in diesem Artikel.

So erstellen Sie einen Filter, der sich über mehrere Ebenen in der Objekthierarchie erstreckt:

1. Identifizieren Sie das Objekt Ihres Filters. Dieses Objekt wird als „Original“-Objekt bezeichnet.\
   Beispiel: Problem.

1. Identifizieren Sie das Feld, nach dem Sie filtern möchten. Dieses Objekt wird als Zielfeld bezeichnet, das zu einem Zielobjekt gehört.\
   Beispiel: das Feld ownerID (Zielfeld), das zum Portfolio (Zielobjekt) gehört.

1. (Bedingt) Wenn das ursprüngliche Objekt (Problem) und das Zielfeld (ownerID) nicht direkt miteinander verbunden sind, müssen Sie ein drittes Objekt, ein Verknüpfungsobjekt (Projekt) finden, das sie verbindet. Das Verknüpfungsobjekt muss über mindestens ein Feld verfügen, das von den Registerkarten Felder oder Verweise des ursprünglichen Objekts referenziert wird (auf dem ursprünglichen Objekt angezeigtes Verknüpfungsfeld), und es muss auch über ein Verknüpfungsfeld zum Zielobjekt verfügen, das auf den Registerkarten Felder oder Verweise des Verknüpfungsobjekts angezeigt wird. Das Verknüpfungsfeld mit dem Zielobjekt, das im Verknüpfungsobjekt angezeigt wird (oder das Verknüpfungsfeld, das im Verknüpfungsobjekt angezeigt wird), muss mit dem Zielfeld übereinstimmen.

   Beispielsweise wird die (Projekt-)ID (Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird) von „Anfragen“ referenziert (Originalobjekt). (Portfolio) ownerID (Feld wird mit dem Zielobjekt verknüpft) wird auf der Registerkarte Felder des Projekts (Objekt wird verknüpft) angezeigt. Portfolio ownerID ist auch ein Feld im Zielobjekt (Portfolio). Das Verknüpfungsfeld im Verknüpfungsobjekt entspricht dem Zielfeld.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Identifizieren Sie mithilfe des API-Explorers den **Objekt-Code** des Verknüpfungsobjekts (Projekt).\
   Der Objekt-Code für das Projekt lautet beispielsweise PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Erstellen Sie einen Filter für das ursprüngliche Objekt.\
   Erstellen Sie beispielsweise einen Problemfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. Fügen Sie das folgende Formelbeispiel in die Textmodusschnittstelle des neuen Filters ein und ersetzen Sie den Beispieltext durch die richtigen Objekte und Felder:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>`

   `EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

   Ein Beispiel für die Verwendung der oben genannten Felder finden Sie im Abschnitt [Beispiel 1: Filtern nach Portfolio-Inhabername](#example-1-filter-for-issues-by-portfolio-owner-name) in diesem Artikel.

1. Klicken Sie auf **Filter speichern**.

## Erstellen komplexer Textmodusfilter für fehlende Objekte

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Sie können einen Filter erstellen, der auf fehlende Objekte verweist. Sie können beispielsweise einen Benutzerfilter erstellen, der anzeigt, welche Benutzenden keine Stunden in Workfront protokolliert haben.

Sie müssen immer eine *EXISTS*-Anweisung und die Textmodus-Schnittstelle verwenden, um diesen Filter zu erstellen.

Beispiele für Filter für fehlende Objekte finden Sie in den folgenden Abschnitten in diesem Artikel:

* [Beispiel 2: Filtern nach fehlenden Objekten: benutzerdefinierte Felder, die in keinem benutzerdefinierten Formular angezeigt werden](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Beispiel 3: Filtern nach fehlenden Objekten: Benutzer, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

So erstellen Sie einen Filter, der auf fehlende Objekte verweist:

1. Identifizieren Sie das Objekt Ihres Filters. Dieses Objekt wird als „Original“-Objekt bezeichnet.\
   Beispiel: Parameter oder benutzerdefiniertes Feld.

1. Identifizieren Sie das Feld, nach dem Sie filtern möchten. Dieses Objekt wird als Zielfeld bezeichnet, das zu einem Zielobjekt gehört.\
   Zum Beispiel das Feld categoryID (Zielfeld), das zur Kategorie (Zielobjekt) gehört.

1. Da das ursprüngliche Objekt (Parameter) und das Zielfeld (categoryID) nicht direkt miteinander verbunden sind, müssen Sie ein drittes Objekt, ein Verknüpfungsobjekt (einen Kategorieparameter) finden, das sie verbindet. Das Verknüpfungsobjekt muss über mindestens ein Feld verfügen, das von den Registerkarten Felder oder Verweise des ursprünglichen Objekts referenziert wird (auf dem ursprünglichen Objekt angezeigtes Verknüpfungsfeld), und es muss auch über ein Verknüpfungsfeld zum Zielobjekt verfügen, das auf den Registerkarten Felder oder Verweise des Verknüpfungsobjekts angezeigt wird. Das Verknüpfungsfeld mit dem Zielobjekt, das im Verknüpfungsobjekt angezeigt wird (oder das Verknüpfungsfeld, das im Verknüpfungsobjekt angezeigt wird), muss mit dem Zielfeld übereinstimmen.

   Beispielsweise wird die ID des Kategorieparameters (Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird) von Parameter (Original-Objekt) referenziert. parameterID (Linking Field to the Target Object) wird auf der Registerkarte Felder des Kategorieparameters (Linking Object) angezeigt. Das Verknüpfungsfeld mit dem Zielobjekt, das auf dem Verknüpfungsobjekt angezeigt wird, stimmt mit dem Zielfeld überein.

1. Identifizieren Sie mithilfe des API-Explorers den **Objekt-Code** des Verknüpfungsobjekts (Kategorieparameter).\
   Beispielsweise ist der Objektcode für den Kategorieparameter CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Erstellen Sie einen Filter für das ursprüngliche Objekt.\
   Erstellen Sie beispielsweise einen Parameterfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. (Bedingt) Wenn Sie nach fehlenden Objekten filtern, fügen Sie das folgende Formelbeispiel in die Textmodusschnittstelle des neuen Filters ein und ersetzen Sie den Beispieltext durch die richtigen Objekte und Felder:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   Ein Beispiel für das Reporting zu benutzerdefinierten Feldern, die nicht mit benutzerdefinierter Forms verknüpft sind, finden Sie im Abschnitt [Beispiel 2: Filtern nach fehlenden Objekten: Benutzerdefinierte Felder, die in keinem benutzerdefinierten Formular ](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) werden in diesem Artikel.

1. Klicken Sie auf **Filter speichern**.

## Beispiele für Textmodusfilter, die sich über mehrere Ebenen in der Objekthierarchie erstrecken

Verwenden Sie diese Beispiele, um Textmodusfilter mit EXISTS-Anweisungen zu erstellen.

### Beispiel 1: Filtern von Problemen nach Portfolio-Inhabername {#example-1-filter-for-issues-by-portfolio-owner-name}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter für eine Liste von Problemen erstellen, um nur Probleme anzuzeigen, die zu Projekten gehören, die mit einem Portfolio verknüpft sind, dessen Besitzer ein bestimmter Benutzer ist.

So filtern Sie Probleme nach dem Namen des Portfolio-Inhabers:

1. Erstellen Sie einen Problemfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. Siehe folgenden generischen Code:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>`

   `EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

1. Fügen Sie den folgenden Code in den Bereich **Filterregeln für Ihren Bericht festlegen** ein, um den obigen generischen Code zu ersetzen:

   `EXISTS:A:$$OBJCODE=PROJ`

   `EXISTS:A:ID=FIELD:projectID`

   `EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221`

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Problem
   >* Das Zielobjekt ist Portfolio.
   >* Das Verknüpfungsobjekt ist Projekt.
   >* Das Zielfeld und das Verknüpfungsfeld mit dem Zielobjekt, auf das vom Verknüpfungsobjekt verwiesen wird, ist „ownerID“.
   >* Der Objektcode des Verknüpfungsobjekts ist hier PROJ.
   >* Das Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird, ist projectID, und das Verknüpfungsfeld ist ID.

1. Ersetzen Sie den Wert des Zielfelds (ownerID) in der letzten Anweisung durch eine Benutzer-ID aus Ihrer Umgebung.
1. Klicken Sie auf **Filter speichern**.

### Beispiel 2: Filtern nach fehlenden Objekten: benutzerdefinierte Felder, die in keinem benutzerdefinierten Formular angezeigt werden {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Mithilfe der Textmodusschnittstelle können Sie einen Filter erstellen, um benutzerdefinierte Felder (Parameter) anzuzeigen, die nicht mit benutzerdefiniertem Forms (Kategorien) verknüpft sind. Dieser Filter verknüpft Parameter mit Kategorien, die über ein anderes Objekt, den Kategorieparameter, verbunden sind. Da die beiden Felder nicht direkt miteinander verbunden sind und Sie nach fehlenden Informationen filtern, müssen Sie eine EXISTS-Anweisung verwenden.

>[!IMPORTANT]
>
>Ein Parameter ist ein Feld, das in der Feldbibliothek vorhanden ist, auf die in einem benutzerdefinierten Formular verwiesen wird. Ein Kategorieparameter ist die Version eines Felds, das in einem bestimmten Formular angezeigt wird. Wenn dasselbe Feld beispielsweise in 5 Formularen angezeigt wird, enthält die Workfront-Datenbank 1 Parameter und 5 Kategorieparameter.

So filtern Sie nach benutzerdefinierten Feldern, die nicht mit einem benutzerdefinierten Formular verknüpft sind:

1. Erstellen Sie einen Parameter oder einen benutzerdefinierten Feldfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. Siehe folgenden generischen Code:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Fügen Sie den folgenden Code in den Bereich **Filterregeln für Ihren Bericht festlegen** ein, um den obigen generischen Code zu ersetzen:

   `EXISTS:A:$$OBJCODE=CTGYPA`

   `EXISTS:A:parameterID=FIELD:ID`

   `EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Parameter.
   >* Das Zielobjekt ist Kategorie .
   >* Das Verknüpfungsobjekt ist ein Kategorieparameter.
   >* Der Objektcode des Verknüpfungsobjekts ist CTGYPA.
   >* Das Verknüpfungsfeld mit dem Zielobjekt ist parameterID, da parameterID sowohl in der Tabelle des Verknüpfungsobjekts als auch in der Tabelle des Zielobjekts vorhanden ist.
   >* Das Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird, ist die ID (des Kategorieparameters).

1. Klicken Sie auf **Filter speichern**.

### Beispiel 3: Filtern nach fehlenden Objekten: Benutzer, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter erstellen, um Benutzer anzuzeigen, die in einem bestimmten Zeitraum keine Zeit protokolliert haben. Dieser Filter verknüpft Benutzer mit Stunden, die direkt miteinander verbunden sind. Sie müssen jedoch eine EXISTS-Anweisung und die Textmodus-Schnittstelle verwenden, um nach fehlenden Informationen filtern zu können.

So filtern Sie nach Benutzern, die die Zeit der letzten Woche nicht protokolliert haben:

1. Erstellen Sie einen Benutzerfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. Siehe folgenden generischen Code:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Fügen Sie den folgenden Code in den Bereich **Filterregeln für Ihren Bericht festlegen** ein, um den obigen generischen Code zu ersetzen:

   `EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Benutzer.
   >* Das Zielobjekt ist Stunde.
   >* Sie benötigen in diesem Beispiel kein Verknüpfungsobjekt, da Benutzende und Stunden direkt in der Workfront-Datenbank verbunden sind.
   >* Da es kein Verknüpfungsobjekt gibt, müssen Sie den Objektcode des Zielobjekts verwenden: STUNDE.
   >* Das Verknüpfungsfeld zum Zielobjekt ist ownerID (das im ursprünglichen Objekt angezeigt wird, da das Verknüpfungsobjekt fehlt).
   >* Das Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird, ist die ID (der Stunde) (die auf dem Zielobjekt angezeigt wird; das Verknüpfungsobjekt fehlt).
   >* Die EXISTS:A:entryDate-Anweisung bezieht sich auf Felder, die das Zielobjekt (Stunde) definieren, und verwendet dieselbe Syntax wie in einer regulären Filteranweisung. Dadurch wird sichergestellt, dass nur die Benutzer angezeigt werden, die die Zeit für einen bestimmten Zeitraum, in diesem Fall die Vorwoche, nicht protokolliert haben.
   >* Der NOTEXISTS-Modifikator gibt an, dass Elemente (Stunden) gesucht werden, die für das Berichtsobjekt (Benutzer) nicht vorhanden sind.

1. Klicken Sie auf **Filter speichern**.

### Beispiel 4: Filtern nach mehreren Feldern: Aufgaben nach Name des Portfolio-Inhabers und Scorecard-ID für die Portfolio-Ausrichtung {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Mithilfe der Textmodusschnittstelle können Sie einen Filter erstellen, der auf mehr als ein Feld des Zielobjekts verweist. In diesem Fall müssen die Filteranweisungen, die sich auf die Zielfelder beziehen, über UND verbunden werden.

Sie können beispielsweise eine Liste von Aufgaben so filtern, dass nur Aufgaben angezeigt werden, die die folgenden Kriterien erfüllen:

* Sie befinden sich in einem Projekt, das mit einem Portfolio verknüpft ist, dessen Besitzer ein bestimmter Benutzer ist.
* Sie befinden sich in einem Projekt, das mit einem Portfolio verknüpft ist, dessen Projekte nicht mit einer bestimmten Alignment-Scorecard verknüpft sind.

So filtern Sie Aufgaben nach dem Namen des Portfolio-Verantwortlichen und der Scorecard-ID für die Portfolio-Ausrichtung:

1. Erstellen Sie einen Aufgabenfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie **In Textmodus wechseln**.
1. Fügen Sie den folgenden Code in den Bereich **Filterregeln für Ihren Bericht festlegen** ein:

   `EXISTS:A:$$OBJCODE=PROJ`
   `EXISTS:A:ID=FIELD:projectID`
   `EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f`
   `AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS`
   `AND:A:EXISTS:A:$$OBJCODE=PROJ`
   `AND:A:EXISTS:A:ID=FIELD:projectID`
   `AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad`

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Filters: Aufgabe.
   >* Das Zielobjekt ist Portfolio.
   >* Das erste Zielfeld ist Besitzer-ID.
   >* Das zweite Zielfeld ist die Ausrichtungs-Scorecard-ID.
   >* Das Verknüpfungsobjekt ist Projekt.
   >* Der Objektcode des Verknüpfungsobjekts ist PROJ.
   >* Das Verknüpfungsfeld mit dem Zielobjekt ist die ID (des Portfolios).
   >* Das Verknüpfungsfeld, das auf dem ursprünglichen Objekt angezeigt wird, ist projectID.
   >* Ersetzen Sie die Besitzer-ID durch eine Benutzer-ID aus Ihrer Umgebung.

1. Klicken Sie auf **Filter speichern**.
