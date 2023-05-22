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
source-wordcount: '252'
ht-degree: 0%

---

# Verwenden Sie &quot;opTask&quot;und &quot;issue&quot;, wenn Sie auf Probleme verweisen

Der Name eines Problems wird als `opTask` in der Adobe Workfront-Datenbank. Auch wenn es Zeiten gibt, in denen Sie die `issue` Feldname, um auf Probleme zu verweisen, meistens müssen Sie die `opTask` Feldname anstelle von `issue` beim Referenzieren von Problemen.

Weitere Informationen dazu, wie Objekte in der Workfront-Datenbank angezeigt werden, finden Sie im Abschnitt [API-Explorer](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

Verwenden Sie die `opTask` Feldname beim Referenzieren von Problemen in den folgenden Kontexten:

* Wenn Sie einen benutzerspezifischen Textmodus-Bericht für Probleme erstellen und Probleme in Ansichten, Filtern, Gruppierungen oder Eingabeaufforderungen referenzieren möchten.

   Weitere Informationen zur Verwendung des Textmodus in einem Bericht finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* Beim Aktualisieren von Problemfeldern in einem Kick-Start-Daten-Importer-Blatt.

   Weitere Informationen zum Importieren von Daten in Workfront mithilfe eines Kick-Start finden Sie unter [Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` Feldname

Verwenden Sie die `issue` Feldname, um Probleme in den folgenden Kontexten zu referenzieren:

* Wenn Sie in einem Bericht im Textmodus auf Probleme in einer Sammlung verweisen.
* Wenn Sie eine Problemkollektion mithilfe der Workfront-API referenzieren.

Informationen zum Reporting zu Sammlungen finden Sie unter [Referenzieren von Sammlungen in einem Bericht](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
