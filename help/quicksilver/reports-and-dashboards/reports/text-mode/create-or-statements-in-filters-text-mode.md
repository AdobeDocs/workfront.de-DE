---
product-area: reporting
navigation-topic: text-mode-reporting
title: Erstellen von „OR“-Anweisungen in Textmodusfiltern
description: Sie können mehrere -Anweisungen einfügen, wenn Sie einen Filter in Listen und Berichten erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Erstellen von „OR“-Anweisungen in Textmodusfiltern

Sie können mehrere -Anweisungen einfügen, wenn Sie einen Filter in Listen und Berichten erstellen.

Informationen zum Erstellen von Filtern finden Sie in den folgenden Artikeln:

* [Filter - Übersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Bearbeiten eines Filters im Textmodus](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## Textmodus-Filteroperatoren

Weitere Informationen zu Adobe Workfront-Filteroperatoren in der Standardfilterschnittstelle finden Sie unter [Filterübersicht](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront verfügt über zwei Filteroperatoren, die jede Filteranweisung verbinden:

* **AND**: Wenn Sie zwei Filteranweisungen durch den AND-Operator verbinden, geben Sie an, dass beide Filteranweisungen gleichzeitig erfüllt werden sollen.

  Standardmäßig werden die Anweisungen in einem Filter durch den AND-Operator verbunden.

  Beim Erstellen eines AND-Filters in der Textmodus-Benutzeroberfläche müssen Sie den AND-Operator nicht verwenden. Es wird angenommen.

  **Beispiel:** Um nach Aufgaben zu filtern, die ein geplantes Abschlussdatum von heute und einen Prozentsatz von Fertigstellungen unter 100 % haben, verwenden Sie den folgenden Textmodus-Code:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**: Wenn Sie zwei Filteranweisungen mit dem OR-Operator verbinden, geben Sie an, dass eine der beiden Anweisungen erfüllt sein soll.

  >[!TIP]
  >
  >Wenn Sie Ihre AND-Anweisungen in OR-Anweisungen ändern, sollte die Anzahl der Elemente in Ihrem Bericht steigen.

  Beim Erstellen eines OR-Filters mithilfe der Textmodus-Oberfläche müssen Sie den OR-Operator verwenden.

  **Beispiel:** Um nach Aufgaben zu filtern, deren geplantes Abschlussdatum auf heute oder weniger als 100 % fällt, verwenden Sie den folgenden Textmodus-Code:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## Textmodus-Syntax für OR-Filter

Die Textmodussyntax für einen OR-Filter muss Folgendes enthalten:

* Der OR-Operator, gefolgt von einem Doppelpunkt, einer Zahl und einem weiteren Doppelpunkt am Anfang jeder Filterzeile, die auf das Objekt in der OR-Anweisung verweist. Dazu gehören die Zeile, die auf das Filterfeld oder -attribut verweist, und die Zeile, die auf den Filtermodifikator verweist.

  Befolgen Sie dieses Muster beim Erstellen eines OR-Filters:

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >Beim OR-Operator wird zwischen Groß- und Kleinschreibung unterschieden.

  Ein Filter kann mehrere OR-Anweisungen enthalten. In diesem Fall erhält jede OR-Anweisung eine Nummer in der Reihenfolge, in der die Anweisungen angewendet werden sollen.

  **Beispiel:** Um nach Aufgaben zu filtern, deren geplantes Abschlussdatum weniger als 100 % oder aber weniger als das geplante Abschlussdatum beträgt, oder den Status Neu verwenden Sie den folgenden Textmodus-Code:

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* Der Name der Felder oder Attribute, auf die Sie in einem Filter verweisen, muss in Binnenmajuskel-Schreibweise geschrieben werden. Weitere Informationen zur Groß-/Kleinschreibung finden Sie unter [Übersicht über die Textmodus-Syntax](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* Wenn Sie auf benutzerdefinierte Felder in einem OR-Filter verweisen, müssen Sie zwischen der OR-Modifikatorsyntax und dem Namen des benutzerdefinierten Felds „DE:“ einfügen. Sie müssen den Namen des benutzerdefinierten Felds so buchstabieren, wie er in der Benutzeroberfläche von Workfront angezeigt wird.

  **Beispiel:** Verwenden Sie den folgenden Textmodus-Code, um nach Aufgaben zu filtern, deren Status „Neu“ oder „Prozent abgeschlossen“ weniger als 100 % beträgt, ODER nach einem benutzerdefinierten Feld namens „Kontotyp“ mit dem Wert „Gleich“:

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
