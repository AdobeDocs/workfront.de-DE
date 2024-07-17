---
product-area: projects
navigation-topic: issue-information
title: Verwenden Sie "opTask"und "issue", wenn Sie auf Probleme verweisen
description: Der Name eines Problems wird als opTask in der Adobe Workfront-Datenbank angezeigt. Obwohl Sie manchmal den Namen des Problemfelds verwenden müssen, um auf Probleme zu verweisen, müssen Sie in den meisten Fällen den Feldnamen opTask anstelle des Problems verwenden, wenn Sie auf Probleme verweisen.
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Verwenden Sie &quot;opTask&quot;und &quot;issue&quot;, wenn Sie auf Probleme verweisen

Der Name eines Problems wird als `opTask` in der Adobe Workfront-Datenbank angezeigt. Es gibt zwar Fälle, in denen Sie den Feldnamen `issue` verwenden müssen, um auf Probleme zu verweisen, aber in den meisten Fällen müssen Sie beim Referenzieren von Problemen den Feldnamen `opTask` anstelle von `issue` verwenden.

Weitere Informationen dazu, wie Objekte in der Workfront-Datenbank angezeigt werden, finden Sie im [API-Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Verwenden Sie den Feldnamen `opTask` , wenn Sie in den folgenden Kontexten auf Probleme verweisen:

* Wenn Sie einen benutzerspezifischen Textmodus-Bericht für Probleme erstellen und Probleme in Ansichten, Filtern, Gruppierungen oder Eingabeaufforderungen referenzieren möchten.

  Weitere Informationen zur Verwendung des Textmodus in einem Bericht finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Beim Aktualisieren von Problemfeldern in einem Kick-Start-Daten-Importer-Blatt.

  Weitere Informationen zum Importieren von Daten in Workfront mit einem Kick-Start finden Sie unter [Importieren von Daten in Adobe Workfront mit einer Kick-Start-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` Feldname

Verwenden Sie den Feldnamen `issue` , um Probleme in den folgenden Kontexten zu referenzieren:

* Wenn Sie in einem Bericht im Textmodus auf Probleme in einer Sammlung verweisen.
* Wenn Sie eine Problemkollektion mithilfe der Workfront-API referenzieren.

Informationen zum Reporting über Sammlungen finden Sie unter [Verweisen auf Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
