---
product-area: reporting
navigation-topic: text-mode-reporting
title: Erstellen von "OR"-Anweisungen in Textmodusfiltern
description: Sie können beim Erstellen eines Filters in Listen und Berichten mehrere Anweisungen hinzufügen.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Erstellen von &quot;OR&quot;-Anweisungen in Textmodusfiltern

Sie können beim Erstellen eines Filters in Listen und Berichten mehrere Anweisungen hinzufügen.

Informationen zum Erstellen von Filtern finden Sie in den folgenden Artikeln:

* [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Filter im Textmodus bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Textmodus-Filteroperatoren

Informationen zu Adobe Workfront-Filteroperatoren in der Standardfilteroberfläche finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront verfügt über zwei Filteroperatoren, die jede Filteranweisung miteinander verbinden:

* **UND**: Wenn Sie zwei Filteranweisungen durch den UND -Operator verknüpfen, geben Sie an, dass beide Filteranweisungen gleichzeitig erfüllt werden sollen.

  Standardmäßig werden die Anweisungen in einem Filter durch den UND -Operator verbunden.

  Beim Erstellen eines UND-Filters in der Textmodus-Benutzeroberfläche müssen Sie den UND-Operator nicht verwenden. Es wird angenommen.

  **Beispiel:** Um nach Aufgaben zu filtern, die ein geplantes Abschlussdatum von heute und einen Prozentwert von weniger als 100 % aufweisen, verwenden Sie den folgenden Textmodus-Code:

  <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **ODER**: Wenn Sie zwei Filteranweisungen des ODER-Operators verknüpfen, geben Sie an, dass beide Anweisungen erfüllt werden sollen.

  >[!TIP]
  >
  >Wenn Sie Ihre AND-Anweisungen in OR-Anweisungen ändern, sollte die Anzahl der Elemente in Ihrem Bericht erhöht werden.

  Beim Erstellen eines ODER-Filters mit der Textmodus-Benutzeroberfläche müssen Sie den ODER-Operator verwenden.

  **Beispiel:** Verwenden Sie den folgenden Textmodus-Code, um nach Aufgaben zu filtern, die das geplante Abschlussdatum Heute oder den Prozentwert Complete unter 100 % aufweisen:

  <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>ODER:1:percentComplete=100</pre><pre>ODER:1:percentComplete_Mod=lt</pre>

## Textmodussyntax für OR-Filter

Die Textmodussyntax für einen ODER-Filter muss Folgendes enthalten:

* Der ODER -Operator gefolgt von einem Doppelpunkt, einer Zahl und einem weiteren Doppelpunkt am Anfang jeder Filterzeile, die auf das Objekt in der OR-Anweisung verweist. Dazu gehören die Zeile, die auf das Filterfeld oder Attribut verweist, und die Zeile, die auf den Filtermodifikator verweist.

  Gehen Sie beim Erstellen eines ODER-Filters wie folgt vor:

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>ODER:1:<field name in camel case>=<value></pre><pre>ODER:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >Beim ODER-Operator wird zwischen Groß- und Kleinschreibung unterschieden.

  Ein Filter kann mehrere OR-Anweisungen enthalten. In diesem Fall erhält jede OR-Anweisung eine Zahl in der Reihenfolge, in der die Anweisungen angewendet werden sollen.

  **Beispiel:**  Um nach Aufgaben zu filtern, die das geplante Abschlussdatum Heute ODER einen Prozentsatz abgeschlossen haben, der unter 100 % liegt, ODER den Status Neu , verwenden Sie den folgenden Textmoduscode:

  <pre>scheduledCompletionDate=$$TODAY</pre><pre>scheduledCompletionDate_Mod=eq</pre><pre>ODER:1:status=NEW</pre><pre>ODER:1:status_Mod=in</pre><pre>ODER:2:percentComplete=100</pre><pre>ODER:2:percentComplete_Mod=lt</pre>

* Der Name der Felder oder Attribute, auf die Sie in einem Filter verweisen, muss in Binnenmajuskel-Schreibweise geschrieben sein. Weitere Informationen zum Kamelfall finden Sie unter [Übersicht über die Syntax der Textmodi](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Wenn Sie in einem ODER-Filter auf benutzerdefinierte Felder verweisen, müssen Sie DE: zwischen der ODER-Modifikatorsyntax und dem Namen des benutzerdefinierten Felds einfügen. Sie müssen den Namen des benutzerdefinierten Felds so buchstabieren, wie er in der Benutzeroberfläche von Workfront angezeigt wird.

  **Beispiel:** Verwenden Sie den folgenden Textmoduscode, um nach Aufgaben zu filtern, die den Status Neu ODER einen Prozentwert Complete unter 100 % ODER ein benutzerdefiniertes Feld namens &quot;Kontotyp&quot;mit dem Wert &quot;Equal&quot;aufweisen:

  <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>ODER:1:percentComplete=100</pre><pre>ODER:1:percentComplete_Mod=lt</pre><pre>ODER:2:DE:Account type=Capital</pre><pre>ODER:2:DE:Account Type_Mod=in</pre>
