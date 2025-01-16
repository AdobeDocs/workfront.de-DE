---
product-area: reporting
navigation-topic: text-mode-reporting
title: Übersicht über den Textmodus
description: Sie können einen Bericht oder eine Liste in Adobe Workfront erstellen, indem Sie entweder die Standardschnittstelle oder die Textmodusschnittstelle verwenden, wenn Sie die Elemente erstellen, aus denen der Bericht oder die Liste besteht.
author: Nolan
feature: Reports and Dashboards
exl-id: 8be8cbd0-da1b-4e90-a52e-dc352f646d18
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 0%

---

# Übersicht über den Textmodus

<!-- Audited: 1/2025 -->

<!--(NOTE: Linked to the UI (for the areas mentioned in the comments below and the new NWE filters as well))-->

<!--(NOTE: Alina: ***Linked to other articles. Do not move, rename or change url.Linked to the product, in the report builder, when using a field that is not recognized in standard mode.)-->

<!--(NOTE: This will be linked to the Ninja feature about adding a filter to the User typeahead field (which originally is open only for text mode filters). Update the Context Sensitive sheet at release time)-->

Sie können einen Bericht oder eine Liste in Adobe Workfront erstellen, indem Sie entweder die Standardschnittstelle oder die Textmodusschnittstelle verwenden, wenn Sie die Elemente erstellen, aus denen der Bericht oder die Liste besteht.

In der Standardschnittstelle können Sie auf Felder und ihre Attribute verweisen, die in der Workfront-Benutzeroberfläche verfügbar sind.

Mit dem Textmodus können Sie auf Felder und Attribute verweisen, die möglicherweise nicht im Standardmodus, aber in der Workfront-Datenbank verfügbar sind.

Weitere Informationen zum Erstellen von Berichten im Textmodus, einschließlich Klassen, Videos und Tutorials, finden Sie im Abschnitt Lernen auf der Adobe Experience League-Site.

## Überlegungen vor der Verwendung des Textmodus

>[!TIP]
>
>Sie können die Funktionen berechneter benutzerdefinierter Felder auch erweitern, indem Sie eine Version des Textmodus für benutzerdefinierte Felder verwenden. Die Syntax und die Regeln zum Erstellen eines berechneten benutzerdefinierten Felds unterscheiden sich von denen, die Sie in Berichten und Listen verwenden. Informationen zum Hinzufügen eines berechneten benutzerdefinierten Felds finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

* Bevor Sie mit der Verwendung des Textmodus in Ihren Berichten beginnen, empfehlen wir Ihnen dringend, unsere Kurse über erweiterte Berichte zu absolvieren, um ein tieferes Verständnis unserer Textmodussprache zu erhalten.
* Es wird empfohlen, den Standardmodus zu verwenden, um sicherzustellen, dass die von Ihnen erstellten Berichte auch nach der Aktualisierung der Workfront-Software intakt bleiben. Im Textmodus können Sie zwar komplexere Ansichten, Filter und Gruppierungen erstellen, die Verwaltung ist jedoch komplizierter und nicht garantiert, wenn die Workfront-Software aktualisiert wird.
* Es wird empfohlen, immer zu versuchen, alle Berichterstellungselemente in der Standardschnittstelle zu erstellen und nur für einige Anpassungen zum Textmodus-Builder zu wechseln.

  >[!TIP]
  >
  >Die Verwendung des Standard-Builders liefert wichtige Bausteine und Muster für Code, die Sie dann beim Ändern des Codes im Textmodus verwenden können.

* Es gibt einen Regelsatz und eine eindeutige Syntax, die Sie verwenden müssen, um Berichte und Listen im Textmodus erfolgreich zu erstellen. Vergewissern Sie sich, dass Sie mit der Workfront-Syntax für den Textmodus vertraut sind, bevor Sie beginnen.

  Weitere Informationen zur Syntax und den Regeln für die Verwendung des Textmodus finden Sie unter [Übersicht über die Textmodus-Syntax](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).

* Nachdem Sie ein Berichterstellungselement im Textmodus angepasst haben, können Sie entweder nicht zum Standardmodus (in einer Ansicht) zurückkehren oder der Code für das von Ihnen erstellte Element wird gelöscht (in Filtern und Gruppierungen). Dies liegt daran, dass nicht alle Felder, die im Textmodus unterstützt werden, im Standardmodus unterstützt werden.

## Standardmodus-Schnittstelle

In der Benutzeroberfläche Standardmodus werden Felder angezeigt, um die Anwendungselemente zuzuordnen, die Sie in einem Bericht oder einer Liste anzeigen möchten. Die Standardmodus-Benutzeroberfläche besteht aus einer Reihe von Dropdown-Menüs, aus denen Sie die Felder auswählen können, die Sie in Ihren Berichten oder Listen anzeigen möchten.

Weitere Informationen zum Standardmodus und zum Erstellen eines Berichts oder einer Liste finden Sie unter:

* [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
* [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)

## Textmodus-Oberfläche

Im Textmodus können Sie komplexere Ansichten, Filter, Gruppierungen und Eingabeaufforderungen erstellen, indem Sie Felder verwenden können, die in der Standardmodus-Benutzeroberfläche nicht verfügbar sind. Im Workfront-Textmodus handelt es sich um eine Sammlung von codierten Anweisungen, die angeben, welche Objekte Sie in einem Bericht oder einer Liste anzeigen möchten.

Eine vollständige Liste aller unserer berichtspflichtigen Felder finden Sie im [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Nicht alle über die API verfügbaren Felder sind über die Textmodusschnittstelle verfügbar. Wenn Sie das richtige Feld in Ihrem Textmodus-Code verwenden und nicht die erwarteten Ergebnisse anzeigen, ist das Feld möglicherweise nur über die API zu melden.

## Zugriff auf Berichtselemente und Textbearbeitungsmodus {#access-reporting-elements-and-edit-text-mode}

Der Zugriff auf die Textmodus-Oberfläche ist für Ansichten, Gruppierungen und Filter ähnlich, wenn über einen Bericht oder eine Liste darauf zugegriffen wird.

Informationen zur Verwendung des Textmodus in Ansichten, Filtern und Gruppierungen finden Sie unter:

* [Bearbeiten einer Ansicht im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
* [Bearbeiten eines Filters im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
* [Bearbeiten einer Gruppierung im Textmodus](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

Benutzerdefinierte Eingabeaufforderungen können nur im Textmodus bearbeitet werden. Sie können auf Eingabeaufforderungen nur über einen Bericht zugreifen.

Informationen zum Zugriff auf die Textmodusschnittstelle für benutzerdefinierte Eingabeaufforderungen finden Sie unter [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

## Häufige Gründe für die Verwendung des Textmodus {#common-reasons-to-use-text-mode}

Abgesehen von der Erstellung benutzerdefinierter Eingabeaufforderungen, die nur mithilfe des Textmodus konfiguriert werden können, empfehlen wir die Verwendung von Report Builder zum Erstellen Ihrer Ansichten, Filter und Gruppierungen. Es gibt jedoch einige Fälle, in denen Sie den Textmodus verwenden können, um Ihre Berichte und Listen zu verbessern.

Weitere Informationen zu häufigen Verwendungen für den Textmodus finden Sie unter [Übersicht über häufige Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
