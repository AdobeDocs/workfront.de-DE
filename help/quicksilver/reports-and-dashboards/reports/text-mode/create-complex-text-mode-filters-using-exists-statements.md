---
product-area: reporting
navigation-topic: text-mode-reporting
title: Erstellen komplexer Textmodusfilter mithilfe von EXISTS-Anweisungen
description: Erstellen komplexer Textmodusfilter mithilfe von EXISTS-Anweisungen
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Erstellen komplexer Textmodusfilter mithilfe von EXISTS-Anweisungen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Dieser Artikel erfordert ein grundlegendes Verständnis der Adobe Workfront-API und der Benutzeroberfläche für die Textmodus-Berichterstellung. Informationen zur Workfront-API finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).\
>Informationen zur Verwendung des Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Übersicht über Objektbeziehungen in Workfront

Alle Objekte sind mit anderen Objekten in der Workfront-Datenbank verknüpft.

Anhand der Hierarchie und Interdependenz von Objekten können Sie feststellen, auf welche Objekte in Berichten verwiesen werden kann.

Informationen darüber, welche Objekte sich in Workfront befinden, sowie zu ihrer Hierarchie und Interdependenz finden Sie unter [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Beim Erstellen von Filtern können Sie mithilfe der standardmäßigen Berichterstellungsoberfläche auf bis zu zwei Beziehungsebenen auf andere Objekte verweisen, die mit dem Objekt des Filters verbunden sind.

Beispielsweise können Sie die Portfolio-ID in einem Ausgabeffilter referenzieren, um nur Probleme zu Projekten anzuzeigen, die mit einem bestimmten Portfolio verknüpft sind, indem Sie die Standardoberfläche verwenden. In diesem Fall ist das Portfolio 2 Stufen von den Emissionen entfernt.

Sie können jedoch nicht den Eigentümer des Portfolios in einem Problemfilter mithilfe der Standardschnittstelle referenzieren, um nur Probleme aus Projekten anzuzeigen, die mit Portfolios verknüpft sind, bei denen der Eigentümer ein bestimmter Benutzer ist. Sie müssen den Textmodus verwenden, um auf das Feld &quot;Portfolio Owner Name&quot;zuzugreifen, das sich drei Ebenen von Problemen entfernt befindet.

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Eine vollständige Liste der Objekte in Workfront finden Sie in der [API-Explorer](../../../wf-api/general/api-explorer.md).

Informationen zum Navigieren im API Explorer und Suchen von Objekten finden Sie unter [API Explorer verwenden](../../../wf-api/general/using-api-explorer.md).

Beim Erstellen von Filtern müssen Sie komplexe Anweisungen in der Textmodus-Oberfläche erstellen, um auf diese Objekttypen zu verweisen.

Informationen zum Erstellen komplexer Filter finden Sie in der [Übersicht über komplexe Textmodusfilter, die vorhandene Anweisungen verwenden](#overview-of-complex-text-mode-filters-that-use-exists-statements) Abschnitt.

## Übersicht über komplexe Textmodusfilter, die EXISTS-Anweisungen verwenden {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Beachten Sie beim Erstellen von Filtern, die sich über mehrere Ebenen in der Objekthierarchie erstrecken oder nach fehlenden Objekten filtern:

* Sie müssen komplexe Filter erstellen, wenn Sie auf Objekte verweisen möchten, die nicht direkt mit dem Filterobjekt verbunden sind.
* Sie müssen eine EXISTS-Anweisung verwenden, um Folgendes zu tun:

   * Erstellen Sie Filter, die mehrere Ebenen umfassen.
   * Erstellen Sie Filter, die nach fehlenden Objekten suchen.\
      Beim Erstellen eines Benutzerberichts können Sie beispielsweise nach Benutzern filtern, die für einen bestimmten Zeitraum keine Zeit protokolliert haben.

Beachten Sie bei der Verwendung von EXISTS-Anweisungen in einem Filter die folgenden Regeln:

* Es gibt drei Objekte, die Sie in einem EXISTS-Filter referenzieren können:

   * Das Objekt des Filters (Originalobjekt).
   * Das Objekt, dessen Feld Sie referenzieren möchten (Target-Objekt).
   * Das Objekt, das das Original mit den Zielobjekten verbindet, falls diese nicht direkt miteinander verbunden sind (Verknüpfungsobjekt).

* Filter, die EXISTS verwenden, enthalten zwei separate Anweisungen, die durch ein Gleichheitszeichen verknüpft sind:

   * Die Anweisung vor dem Gleichheitszeichen bezieht sich auf das Objekt, auf das Sie verweisen (die Verknüpfung oder das Zielobjekt).
   * Die Anweisung nach dem Gleichheitszeichen bezieht sich auf das Objekt, von dem Sie verweisen (das Originalobjekt).

* Sie müssen den Objektcode des Linkobjekts verwenden, um Ihre Anweisungen zu verbinden.\
   Den Objektcode aller Objekte finden Sie im API Explorer.\
   Weitere Informationen zum API Explorer finden Sie in der [API-Explorer](https://one.workfront.com/s/api-explorer).

* Wenn ein Verknüpfungsobjekt fehlt, weil das Original und die Zielobjekte direkt miteinander verbunden sind, können Sie den Objektcode des Zielobjekts anstelle des Verknüpfungsobjekts verwenden.
* Sie können mehrere Felder (Zielfelder) für dasselbe Objekt (Zielobjekt) referenzieren. In diesem Fall müssen Sie die Zeilen, die auf die Felder verweisen, durch UND verbinden.\
   Ein Beispiel für die Filterung nach mehr als einem Feld, das zum Target-Objekt gehört, finden Sie unter [Beispiel 4: Filtern nach mehreren Feldern: Aufgaben nach Portfolio Owner Name und Portfolio Alignment Scorecard ID](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) in diesem Artikel.

* Der einzige Modifikator, der für eine EXISTS-Anweisung unterstützt wird, ist NOTEXISTS.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Filter in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Filtern in einem Bericht verwalten</p> <p>Berechtigungen für einen Filter verwalten und ihn bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen komplexer Textmodusfilter, die mehrere Ebenen in der Objekthierarchie umfassen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Sie können einen Filter erstellen, der Objekte über mehrere Ebenen der Objekthierarchie hinweg referenziert, in der sich das Filterobjekt befindet. Beispielsweise können Sie einen Problemfilter für Probleme erstellen, die sich auf Projekte beziehen, die nicht mit einem bestimmten Portfolio-Eigentümer verknüpft sind.

Sie müssen immer eine EXISTS-Anweisung und die Textmodus-Oberfläche verwenden, um diesen Filter zu erstellen.

Beispiele für Filter finden Sie unter [Beispiel 1: Filtern nach Problemen nach Portfolio Owner Name](#example-1-filter-for-issues-by-portfolio-owner-name) in diesem Artikel.

So erstellen Sie einen Filter, der sich über mehrere Ebenen in der Objekthierarchie erstreckt:

1. Identifizieren Sie das Objekt Ihres Filters. Dieses Objekt wird als Originalobjekt bezeichnet.\
   Beispiel: Problem.
1. Identifizieren Sie das Feld, nach dem Sie filtern möchten. Wir bezeichnen dieses Objekt als Zielfeld, das zu einem Target-Objekt gehört.\
   Beispielsweise das Feld ownerID (Target-Feld), das zu Portfolio gehört (Target-Objekt).
1. (Bedingt) Wenn das Originalobjekt (Problem) und das Zielfeld (ownerID) nicht direkt miteinander verbunden sind, müssen Sie ein drittes Objekt finden, ein Verknüpfungsobjekt (Projekt), das diese verbindet. Das Verknüpfungsobjekt muss über mindestens ein Feld verfügen, das auf den Registerkarten &quot;Felder&quot;oder &quot;Verweise&quot;des ursprünglichen Objekts (im Originalobjekt angezeigtes Verknüpfungsfeld) referenziert wird, und außerdem muss es über ein Verknüpfungsfeld mit dem Zielobjekt verfügen, das auf den Registerkarten &quot;Felder&quot;oder &quot;Verweise&quot;des Verknüpfungsobjekts angezeigt wird. Das Verknüpfungsfeld mit dem Zielobjekt, das auf dem Verknüpfungsobjekt (oder dem Verknüpfungsfeld auf dem Verknüpfungsobjekt) angezeigt wird, muss mit dem Zielfeld übereinstimmen.\
   Beispielsweise wird aus &quot;Issues&quot;(Originalobjekt) auf die (Projekt-)ID (Verknüpfungsfeld, das auf dem Originalobjekt angezeigt wird) verwiesen. (Portfolio) ownerID (Verknüpfungsfeld mit Zielobjekt) wird auf der Registerkarte &quot;Felder&quot;des Projekts (Verknüpfungsobjekt) angezeigt. Portfolio ownerID ist auch ein Feld im Target-Objekt (Portfolio). Das Verknüpfungsfeld im Verknüpfungsobjekt entspricht dem Zielfeld.\
   ![Portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Identifizieren Sie mithilfe des API Explorers die **Objektcode** des Verknüpfungsobjekts (Projekt).\
   Beispielsweise ist der Objektcode für das Projekt PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Erstellen Sie einen Filter für das Originalobjekt.\
   Erstellen Sie beispielsweise einen Filter Problem .\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. Fügen Sie das folgende Formelbeispiel in die Textmodusschnittstelle des neuen Filters ein und ersetzen Sie den vorgeschlagenen Text durch die richtigen Objekte und Felder:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Ein Beispiel für die Verwendung der oben identifizierten Felder finden Sie im Abschnitt [Beispiel 1: Filtern nach Problemen nach Portfolio Owner Name](#example-1-filter-for-issues-by-portfolio-owner-name) in diesem Artikel.

1. Klicken **Filter speichern**.

## Erstellen komplexer Textmodusfilter für fehlende Objekte

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Sie können einen Filter erstellen, der auf fehlende Objekte verweist. Sie können beispielsweise einen Benutzerfilter erstellen, der anzeigt, welche Benutzer keine Stunden in Workfront angemeldet haben.

Sie müssen immer eine *VORHANDEN* -Anweisung und der Textmodus-Oberfläche, um diesen Filter zu erstellen.

Beispiele für Filter für fehlende Objekte finden Sie in den folgenden Abschnitten in diesem Artikel:

* [Beispiel 2: Nach fehlenden Objekten filtern: benutzerdefinierte Felder, die nicht in benutzerdefinierten Formularen angezeigt werden](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Beispiel 3: Nach fehlenden Objekten filtern: Benutzer, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

So erstellen Sie einen Filter, der auf fehlende Objekte verweist:

1. Identifizieren Sie das Objekt Ihres Filters. Dieses Objekt wird als Originalobjekt bezeichnet.\
   Beispiel: Parameter oder benutzerdefiniertes Feld.
1. Identifizieren Sie das Feld, nach dem Sie filtern möchten. Wir bezeichnen dieses Objekt als Zielfeld, das zu einem Target-Objekt gehört.\
   Beispielsweise das Feld categoryID (Target-Feld), das zur Kategorie (Target-Objekt) gehört.
1. Da das Originalobjekt (Parameter) und das Zielfeld (categoryID) nicht direkt miteinander verbunden sind, müssen Sie ein drittes Objekt finden, ein Verknüpfungsobjekt (ein Kategorieparameter), das diese verbindet. Das Verknüpfungsobjekt muss über mindestens ein Feld verfügen, das auf den Registerkarten &quot;Felder&quot;oder &quot;Verweise&quot;des ursprünglichen Objekts (im Originalobjekt angezeigtes Verknüpfungsfeld) referenziert wird, und außerdem muss es über ein Verknüpfungsfeld mit dem Zielobjekt verfügen, das auf den Registerkarten &quot;Felder&quot;oder &quot;Verweise&quot;des Verknüpfungsobjekts angezeigt wird. Das Verknüpfungsfeld mit dem Zielobjekt, das auf dem Verknüpfungsobjekt (oder dem Verknüpfungsfeld auf dem Verknüpfungsobjekt) angezeigt wird, muss mit dem Zielfeld übereinstimmen.\
   Beispielsweise wird die ID des Kategorieparameters (Verknüpfungsfeld, das auf dem Originalobjekt angezeigt wird) aus Parameter(Originalobjekt) referenziert. parameterID (Verknüpfungsfeld mit Zielobjekt) wird auf der Registerkarte &quot;Felder&quot;des Kategorieparameters (Verknüpfungsobjekt) angezeigt. Das Verknüpfungsfeld mit dem Zielobjekt, das auf dem Verknüpfungsobjekt angezeigt wird, stimmt mit dem Zielfeld überein.
1. Identifizieren Sie mithilfe des API Explorers die **Objektcode** des Verknüpfungsobjekts (Kategorieparameter).\
   Beispielsweise ist der Objektcode für den Kategorieparameter CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Erstellen Sie einen Filter für das Originalobjekt.\
   Erstellen Sie beispielsweise einen Parameterfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. (Bedingt) Wenn Sie nach fehlenden Objekten filtern, fügen Sie das folgende Formelbeispiel in die Textmodusschnittstelle des neuen Filters ein und ersetzen Sie den vorgeschlagenen Text durch die richtigen Objekte und Felder:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Ein Beispiel für die Berichterstellung über benutzerdefinierte Felder, die nicht mit benutzerdefiniertem Forms verknüpft sind, finden Sie unter [Beispiel 2: Nach fehlenden Objekten filtern: benutzerdefinierte Felder, die nicht in benutzerdefinierten Formularen angezeigt werden](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) in diesem Artikel.

1. Klicken **Filter speichern**.

## Beispiele für Textmodusfilter, die mehrere Ebenen in der Objekthierarchie umfassen

* [Beispiel 1: Filtern nach Problemen nach Portfolio Owner Name](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Beispiel 2: Nach fehlenden Objekten filtern: benutzerdefinierte Felder, die nicht in benutzerdefinierten Formularen angezeigt werden](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Beispiel 3: Nach fehlenden Objekten filtern: Benutzer, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Beispiel 4: Filtern nach mehreren Feldern: Aufgaben nach Portfolio Owner Name und Portfolio Alignment Scorecard ID](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Beispiel 1: Filtern nach Problemen nach Portfolio Owner Name {#example-1-filter-for-issues-by-portfolio-owner-name}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter für eine Liste von Problemen erstellen, um nur Probleme anzuzeigen, die sich auf Projekte beziehen, die mit einem Portfolio verknüpft sind, dessen Eigentümer ein bestimmter Benutzer ist.

So filtern Sie Probleme nach dem Namen des Portfolios-Eigentümers:

1. Erstellen Sie einen Filter Problem .\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. Siehe folgenden allgemeinen Code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Fügen Sie den folgenden Code in die **Festlegen von Filterregeln für Ihren Bericht** -Bereich, der den oben genannten generischen Code ersetzen soll:

   <pre>VORHANDEN:A:$$OBJCODE=PROJ<br>VORHANDEN:A:ID=FIELD:projectID<br>VORHANDEN:A:portfolio:ownerID=4d94d7da001699b19edf50de1568221</pre>

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Problem
   >* Das Target-Objekt ist Portfolio.
   >* Das Verknüpfungsobjekt ist &quot;Projekt&quot;.
   >* Das Zielfeld und das Verknüpfungsfeld mit dem vom Verknüpfungsobjekt referenzierten Zielobjekt ist ownerID.
   >* Der Objektcode des Linkobjekts hier ist PROJ.
   >* Das auf dem Originalobjekt angezeigte Verknüpfungsfeld ist projectID und das Verknüpfungsfeld ist ID.


1. Ersetzen Sie den Wert des Zielfelds (ownerID) in der letzten Anweisung durch eine Benutzer-ID aus Ihrer Umgebung.
1. Klicken **Filter speichern**.

### Beispiel 2: Nach fehlenden Objekten filtern: benutzerdefinierte Felder, die nicht in benutzerdefinierten Formularen angezeigt werden {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter erstellen, um benutzerdefinierte Felder (Parameter) anzuzeigen, die nicht mit benutzerdefiniertem Forms (Kategorien) verknüpft sind. Dieser Filter verknüpft Parameter mit Kategorien, die über ein anderes Objekt, den Kategorieparameter, verbunden sind. Da die beiden Felder nicht direkt miteinander verbunden sind und Sie nach fehlenden Informationen filtern, müssen Sie eine EXISTS-Anweisung verwenden.

>[!IMPORTANT]
>
>Ein Parameter ist ein Feld, da es in der in einem benutzerdefinierten Formular referenzierten Feldbibliothek vorhanden ist. Ein Kategorieparameter ist die Version eines Felds, das in einem bestimmten Formular angezeigt wird. Wenn beispielsweise dasselbe Feld in 5 Formularen angezeigt wird, befinden sich 1 Parameter und 5 Kategorieparameter in der Workfront-Datenbank.

So filtern Sie nach benutzerdefinierten Feldern, die nicht mit einem benutzerdefinierten Formular verknüpft sind:

1. Erstellen Sie einen Parameter oder einen Filter für benutzerdefinierte Felder .\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. Siehe folgenden allgemeinen Code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Fügen Sie den folgenden Code in die **Festlegen von Filterregeln für Ihren Bericht** -Bereich, der den oben genannten generischen Code ersetzen soll:

   <pre>VORHANDEN:A:$$OBJCODE=CTGYPA<br>VORHANDEN:A:parameterID=FIELD:ID<br>VORHANDEN:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Parameter.
   >* Das Target-Objekt ist Kategorie.
   >* Das Verknüpfungsobjekt ist der Kategorieparameter.
   >* Der Objektcode des Verknüpfungsobjekts ist CTGYPA.
   >* Das Verknüpfungsfeld mit dem Target-Objekt ist parameterID, da parameterID sowohl in der Tabelle &quot;Verknüpfungsobjekt&quot;als auch in der Tabelle &quot;Zielobjekt&quot;vorhanden ist.
   >* Das auf dem Originalobjekt angezeigte Verknüpfungsfeld ist die ID (des Kategorieparameters).


1. Klicken **Filter speichern**.

### Beispiel 3: Nach fehlenden Objekten filtern: Benutzer, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter erstellen, um Benutzer anzuzeigen, die die Zeit für einen bestimmten Zeitraum nicht protokolliert haben. Dieser Filter verknüpft Benutzer mit Stunden, die direkt miteinander verbunden sind. Sie müssen jedoch eine EXISTS-Anweisung und die Textmodus-Oberfläche verwenden, um nach fehlenden Informationen filtern zu können.

So filtern Sie nach Benutzern, die die Zeit in der letzten Woche nicht protokolliert haben:

1. Erstellen Sie einen Benutzerfilter.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. Siehe folgenden allgemeinen Code:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Fügen Sie den folgenden Code in die **Festlegen von Filterregeln für Ihren Bericht** -Bereich, der den oben genannten generischen Code ersetzen soll:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* Das ursprüngliche Objekt ist das Objekt des Berichts: Benutzer.
   >* Das Target-Objekt ist Stunde.
   >* In diesem Beispiel benötigen Sie kein Verknüpfungsobjekt, da Benutzer und Stunden direkt mit der Workfront-Datenbank verbunden sind.
   >* Da es kein Verknüpfungsobjekt gibt, müssen Sie den Objektcode des Target-Objekts verwenden: STUNDE.
   >* Das Verknüpfungsfeld mit dem Target-Objekt ist ownerID (das im Originalobjekt angezeigt wird). das Verknüpfungsobjekt fehlt).
   >* Das im Originalobjekt angezeigte Verknüpfungsfeld ist die ID (der Stunde) (die im Zielobjekt angezeigt wird). das Verknüpfungsobjekt fehlt.)
   >* VORHANDEN:A:entryDate -Anweisung bezieht sich auf Felder, die das Target-Objekt (Stunde) definieren und dieselbe Syntax wie in einer regulären Filteranweisung verwenden. Dadurch wird sichergestellt, dass Sie nur die Benutzer anzeigen, die die Zeit für einen bestimmten Zeitraum (in diesem Fall die vorherige Woche) nicht protokolliert haben.
   >* Der NOTEXISTS-Modifikator zeigt an, dass wir nach Elementen (Stunden) suchen, die für das Objekt des Berichts (Benutzer) nicht vorhanden sind.


1. Klicken **Filter speichern**.

### Beispiel 4: Filtern nach mehreren Feldern: Aufgaben nach Portfolio Owner Name und Portfolio Alignment Scorecard ID {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Mithilfe der Textmodus-Benutzeroberfläche können Sie einen Filter erstellen, der auf mehr als ein Feld im Target-Objekt verweist. In diesem Fall müssen die Filteranweisungen, die auf die Zielfelder verweisen, durch AND verbunden werden.

Sie können beispielsweise eine Liste von Aufgaben filtern, um nur Aufgaben anzuzeigen, die die folgenden Kriterien erfüllen:

* Sie befinden sich in einem Projekt, das mit einem Portfolio verknüpft ist, dessen Eigentümer ein bestimmter Benutzer ist.
* Sie befinden sich in einem Projekt, das mit einem Portfolio verknüpft ist, dessen Projekte nicht mit einer bestimmten Alignment-Scorecard verbunden sind.

So filtern Sie Aufgaben nach dem Portfolio Owner Name und der Scorecard-ID der Portfolio-Ausrichtung:

1. Erstellen Sie einen Filter &quot;Aufgabe&quot;.\
   Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken **In den Textmodus wechseln**.
1. Fügen Sie den folgenden Code in die **Festlegen von Filterregeln für Ihren Bericht** Bereich:
   <pre>VORHANDEN:A:$$OBJCODE=PROJ<br>VORHANDEN:A:ID=FIELD:projectID<br>VORHANDEN:A:portfolio:ownerID=4d80ce520000528787d57807732a33f<br>UND:A:VORHANDEN:A:$$EXISTSMOD=NOTEXISTS<br>UND:A:VORHANDEN:A:$$OBJCODE=PROJ<br>UND:A:VORHANDEN:A:ID=FIELD:projectID<br>UND:A:VORHANDEN:A:Portfolio:alignScoreCardID=4da387b0001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* Das Originalobjekt ist das Objekt des Filters: Aufgabe.
   >* Das Target-Objekt ist Portfolio.
   >* Das erste Zielfeld ist ownerID.
   >* Das zweite Zielfeld ist die Kennung der Alignment-Scorecard.
   >* Das Verknüpfungsobjekt ist &quot;Projekt&quot;.
   >* Der Objektcode des Verknüpfungsobjekts ist PROJ.
   >* Das Verknüpfungsfeld mit dem Zielobjekt ist die ID (des Portfolios).
   >* Das auf dem Originalobjekt angezeigte Verknüpfungsfeld ist projectID.
   >* Ersetzen Sie die ownerID durch eine Benutzer-ID aus Ihrer Umgebung.


1. Klicken **Filter speichern**.
