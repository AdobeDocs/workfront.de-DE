---
product-area: projects
navigation-topic: issue-information
title: „OpTask“ und „Problem“ beim Referenzieren von Problemen verwenden
description: Der Name eines Problems wird in der Adobe Workfront-Datenbank als „opTask“ angezeigt. Es gibt zwar Fälle, in denen Sie den Problemfeldnamen verwenden müssen, um auf Probleme zu verweisen, aber in den meisten Fällen müssen Sie beim Verweisen auf Probleme den Feldnamen „opTask“ anstelle von „Problem“ verwenden.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# „OpTask“ und „Problem“ beim Referenzieren von Problemen verwenden

Der Name eines Problems wird in der Adobe Workfront-Datenbank als `opTask` angezeigt. Es gibt zwar Fälle, in denen Sie den `issue` Feldnamen verwenden müssen, um auf Probleme zu verweisen, aber in den meisten Fällen müssen Sie beim Verweisen auf Probleme den `opTask` Feldnamen anstelle von `issue` verwenden.

Weitere Informationen zum Aussehen von Objekten in der Workfront-Datenbank finden Sie im [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` Dateiname

Verwenden Sie den `opTask` Feldnamen beim Referenzieren von Problemen in den folgenden Kontexten:

* Wenn Sie einen benutzerdefinierten Bericht im Textmodus für Probleme erstellen und auf Probleme in Ansichten, Filtern, Gruppierungen oder Eingabeaufforderungen verweisen möchten.

  Weitere Informationen zur Verwendung des Textmodus in einem Bericht finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Beim Aktualisieren von Problemfeldern in einem Kickstart-Datenimportblatt.

  Weitere Informationen zum Importieren von Daten in Workfront mithilfe einer Kickstart-[ finden Sie unter „Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` Feldname

Verwenden Sie den `issue` Feldnamen, um auf Probleme in den folgenden Kontexten zu verweisen:

* Wenn Sie in einem Bericht im Textmodus auf Probleme in einer Sammlung verweisen.
* Wenn Sie mit der Workfront-API auf eine Problemsammlung verweisen.

Informationen zum Reporting über Sammlungen finden Sie unter [Referenzieren von Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
