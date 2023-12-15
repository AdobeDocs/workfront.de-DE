---
content-type: overview;reference
navigation-topic: workfront-navigation
title: "[!DNL Adobe Workfront] Objektübersicht"
description: "Die Informationen, die Sie unter [!DNL Adobe Workfront] wird durch Objekte dargestellt, die in der [!DNL Workfront] Datenbank. Die Objekte sind das, was die Informationen in [!DNL Workfront]. Weitere Informationen zu diesen Objekten finden Sie in diesem Artikel."
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '2306'
ht-degree: 1%

---

# [!DNL Adobe Workfront] Objektübersicht

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Die Informationen, die Sie in [!DNL Adobe Workfront] wird durch Objekte dargestellt, die in der [!DNL Workfront] Datenbank. Die Objekte sind das, was die Informationen in [!DNL Workfront].

Grundlegendes zur Definition der Objekte unter [!DNL Workfront] ist wichtig, damit Sie das richtige Objekt für die Anforderungen in Ihrer Organisation verwenden können.

Wenn Sie beispielsweise eine große Menge an Arbeit planen, müssen Sie die [!UICONTROL Projekt] -Objekt, um diese Arbeit zu definieren. Um diese Arbeit in kleinere geplante Inkremente zu unterteilen, können Sie die [!UICONTROL Aufgabe] -Objekt. Für einen kleineren Arbeitsaufwand, der nicht geplant ist und unerwartet auftreten kann, können Sie das Objekt Problem verwenden. Wenn Sie den Fortschritt und die Einhaltung des Budgets und der Zeitleiste einer Projektgruppe verfolgen möchten, können Sie diese in [!UICONTROL Portfolios] und [!UICONTROL Programme]. Um andere Elemente zu definieren, die Ihnen bei der Auflösung Ihrer Arbeit helfen, möchten Sie andere Objekte verwenden, die unter gespeichert sind [!UICONTROL Projekte], [!UICONTROL Aufgaben], [!UICONTROL Probleme]oder [!UICONTROL Portfolios], wie [!UICONTROL Dokumente], [!UICONTROL Updates], [!UICONTROL Stunden], [!UICONTROL Benutzer]oder [!UICONTROL Vorgangsrollen].

[!UICONTROL Berichte] und [!UICONTROL Dashboards] sind ein weiteres Beispiel für Objekte, mit denen Sie die Datenmenge organisieren können, in der Sie [!DNL Workfront] visuell, damit sie für alle Benutzer leicht zugänglich ist.

Eine vollständige Liste der Objekte in [!DNL Workfront], siehe [API-Explorer](../../../wf-api/general/api-explorer.md).

## Abhängigkeit und Hierarchie von Objekten

Objekte sind miteinander verknüpft in [!UICONTROL Workfront]. Beispielsweise kann eine Aufgabe oder ein Problem nie unabhängig von einem Projekt existieren. [!UICONTROL Aufgaben] und [!UICONTROL issues] sind Beispiele für Objekte, die im [!UICONTROL Projekt] -Objekt. [!UICONTROL Aufgaben] und [!UICONTROL issues] werden als untergeordnete Objekte zu Projekten betrachtet.

Im Folgenden finden Sie einige der am häufigsten verwendeten Objekte in [!DNL Workfront] und die entsprechenden übergeordneten und untergeordneten Objekte:

| **Objekt** | **Übergeordnete Objekte** | **Untergeordnete Objekte** |
|---|---|---|
| [!UICONTROL Portfolios] |  | [!UICONTROL Programme], [!UICONTROL Projekte], [!UICONTROL Dokumente], [!DNL Notes], [!UICONTROL Benutzer] |
| [!UICONTROL Programme] | [!UICONTROL Portfolios] | [!UICONTROL Projekte], [!UICONTROL Dokumente], [!UICONTROL Hinweise], [!UICONTROL Benutzer] |
| [!UICONTROL Projekte] | [!UICONTROL Portfolios], [!UICONTROL Programme] | [!UICONTROL Aufgaben], [!UICONTROL Probleme], [!UICONTROL Dokumente], [!UICONTROL Hinweise], [!UICONTROL Stunden], [!UICONTROL Benutzer] |
| [!UICONTROL Aufgaben] | [!UICONTROL Projekte] | [!UICONTROL Probleme], [!UICONTROL Untergeordnete Aufgaben], [!UICONTROL Dokumente], [!UICONTROL Hinweise], [!UICONTROL Stunden], [!UICONTROL Benutzer] |
| [!UICONTROL Probleme] | [!UICONTROL Aufgaben], [!UICONTROL Projekte] | [!UICONTROL Dokumente], [!UICONTROL Hinweise], [!UICONTROL Stunden], [!UICONTROL Benutzer] |
| [!UICONTROL Dashboards] |  | [!UICONTROL Berichte], externe Seiten |
| [!UICONTROL Berichte] | [!UICONTROL Dashboards] |  |
| [!UICONTROL Gruppen] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Teams] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Benutzende] | [!UICONTROL Gruppen], [!UICONTROL Teams], [!UICONTROL Unternehmen] | [!UICONTROL Vorgangsrollen] |
| [!UICONTROL Unternehmen] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Dokumente] | [!UICONTROL Aufgaben], [!UICONTROL Probleme], [!UICONTROL Projekte], [!UICONTROL Portfolios], [!UICONTROL Programme], [!UICONTROL Benutzer] |  |
| [!UICONTROL Pläne]* |  | [!UICONTROL Initiativen] |
| [!DNL Goals]* |  | [!UICONTROL Ergebnisse], [!UICONTROL Tätigkeiten] |

Eine vollständige Liste der Objekte in [!DNL Workfront], siehe [API-Explorer](../../../wf-api/general/api-explorer.md).

*Pläne sind die Objekte der [!DNL Adobe Workfront Scenario Planner]. Informationen zum [!DNL Scenario Planner], siehe [Die [!UICONTROL Szenario-Planer] Übersicht](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Ziele] sind die Objekte von [!DNL Adobe Workfront Goals]. Informationen zu [!DNL Workfront Goals], siehe [[!DNL Adobe Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Objektnamen anpassen

Als [!DNL Workfront] Administratoren können die Objektnamen in [!DNL Workfront] durch Verwendung von [!UICONTROL Layout-Vorlage].

Weitere Informationen zum Anpassen von Objektnamen mithilfe eines  [!UICONTROL Layout-Vorlage], siehe [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Nachdem Sie eine Layoutvorlage angepasst und sie Benutzern zugewiesen haben, sehen diese Benutzer die benutzerdefinierten Namen für die Objekte. Die Benutzer, die der Layoutvorlage zugewiesen wurden, sehen die Standardnamen für die Objekte nirgendwo in der Webanwendung mehr.

Wenn beispielsweise der größere Arbeitsaufwand in Ihrer Organisation als &quot;Interaktion&quot;bezeichnet wird, können Sie den Namen &quot;Interaktion&quot;ersetzen[!UICONTROL Projekt]&quot; mit &quot;Interaktion&quot;ein. Ihre [!DNL Workfront] -Benutzeroberfläche zeigt &quot;Interaktion&quot;anstelle von &quot;[!UICONTROL Projekt]&quot; überall, wo der Name &quot;[!UICONTROL Projekt]&quot; angezeigt.

>[!NOTE]
>
>Damit die neuen Namen der Objekte für Ihre Benutzer sichtbar sind, müssen sie sich ab- und wieder bei anmelden [!DNL Workfront] nach dem Speichern der  [!UICONTROL Layout-Vorlage].

>[!IMPORTANT]
>
>Die [!DNL Workfront] -Dokumentation bezieht sich immer auf die Standardnamen der Objekte. Als [!DNL Workfront] müssen Sie sicherstellen, dass Sie Benutzer über die Änderungen an Objektnamen informieren, damit sie verstehen können, wie die [!DNL Workfront] -Dokumentation sowie die Bereiche der Anwendungen, die nicht die Namensänderungen der Objekte widerspiegeln.

* [Objektnamen, die mithilfe einer  [!UICONTROL Layout-Vorlage]](#object-names-that-can-be-customized-using-a-layout-template)
* [Gebiete von [!DNL Workfront] , die die benutzerdefinierten Objektnamen widerspiegeln](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Gebiete von [!DNL Workfront] die nicht die benutzerdefinierten Objektnamen widerspiegeln](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Objektnamen, die mithilfe einer [!UICONTROL Layout-Vorlage]

Als [!DNL Workfront] -Administrator können Sie die Namen der folgenden Objekte so anpassen, dass sie mit der Terminologie in Ihrer Organisation übereinstimmen:

* [!UICONTROL Portfolio]
* [!UICONTROL Programm]
* [!UICONTROL Projekt]
* [!UICONTROL Aufgabe]
* [!UICONTROL Problem]
* [!UICONTROL Ziel]*
* [!UICONTROL Ergebnis]*
* [!UICONTROL Aktivität]*

  *[!UICONTROL Ziele], [!UICONTROL Ergebnisse], und [!UICONTROL activities] nur verfügbar sind, wenn Ihr Unternehmen [!DNL Workfront Goals]. Informationen zu [!DNL Workfront Goals], siehe [[!DNL Adobe Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Szenario]**
* [!UICONTROL Plan]**

  **[!UICONTROL Initiativen], [!UICONTROL Szenarien], und [!UICONTROL Pläne] sind nur verfügbar, wenn Ihr Unternehmen [!DNL Workfront Scenario Planner]. Informationen zum [!DNL Scenario Planner], siehe [Erste Schritte mit [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Weitere Informationen zum Anpassen von Objektnamen finden Sie unter  [!UICONTROL Layout-Vorlagen], siehe [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Sie können die Namen anderer Objekte in Workfront nicht anpassen. Eine vollständige Liste der Objekte in [!DNL Workfront], siehe [API-Explorer](../../../wf-api/general/api-explorer.md).

Wenn Sie den Namen eines Objekts anpassen, wird der neue Name für dieses Objekt in den meisten Bereichen der [!DNL Workfront] -Anwendung, in der dieser Objektname angezeigt wird.

### Gebiete von [!DNL Workfront] , die die benutzerdefinierten Objektnamen widerspiegeln

Die folgenden Bereiche zeigen den aktualisierten Namen der Objekte:

* Navigation oben
* Alle Abschnitte in der linken Bedienfeldnavigation
* Alle Menüs
* In-App-Benachrichtigungen
* Berichterstellung und Berichterstellungselemente (Ansichten, Filter und Gruppierungen)
* [!UICONTROL Speichern] Schaltflächen
* Exportierte Dateien
* E-Mails
* Mobile Apps

### Gebiete von [!DNL Workfront] die nicht die benutzerdefinierten Objektnamen widerspiegeln

In den folgenden Bereichen wird der aktualisierte Name der Objekte nicht angezeigt:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Add-in

### Auswirkungen der Anpassung von Objektnamen

Beachten Sie Folgendes beim Anpassen von Objektnamen in [!DNL Workfront]:

* Sie können stilistische oder grammatikalische Fehler in Systemanzeigen feststellen. Wenn Sie beispielsweise &quot;[!UICONTROL Problem]&#39; auf &#39;Request&#39; und Sie sehen irgendwo im System die Phrase &#39;An request&#39;, dies funktioniert wie beabsichtigt und sollte nicht als Fehler betrachtet werden.
* Ihre benutzerdefinierten Namen für die Objekte können nicht übersetzt werden. Nur die [!DNL Workfront] Standardnamen können in die unterstützten Sprachen übersetzt werden. Weitere Informationen zu Sprachen, die in unterstützt werden [!DNL Workfront], siehe [Unterstützte Sprachen in [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Die benutzerdefinierten Objektnamenfelder unterstützen Fremdzeichen, sodass Sie Terminologie in jeder Sprache eingeben können.
* Beim Anpassen von Objektnamen mithilfe einer  [!UICONTROL Layout-Vorlage], empfehlen wir Ihnen, Ihre  [!UICONTROL Layout-Vorlagen] basierend auf Ihren Geschäftseinheiten (Teams oder Gruppen).\
   Es wird empfohlen, Namen zu verwenden, die von den Benutzern dieser Geschäftsbereiche deutlich verstanden werden, um Verwirrung zu vermeiden.
* E-Mail-Benachrichtigungen und zugestellte Berichte enthalten immer Objektnamen, die durch die  [!UICONTROL Layout-Vorlage] des Benutzers, der die E-Mail generiert. Ihre Benutzer sollten darauf vorbereitet sein, in ihren E-Mails Objektnamen anzuzeigen, die nicht mit ihrer Gruppe oder ihrem Team verbunden sind, wenn sie E-Mail-Benachrichtigungen von Benutzern in anderen Teams und Gruppen erhalten.\
   Als [!DNL Workfront] Administratoren sollten die Benutzer auf die Symbole hinweisen, die mit den einzelnen Objekten verknüpft sind. Die Symbole bleiben zwischen verschiedenen Objektnamen konsistent und entsprechen dem Standardobjekt, wie es in der Datenbank angezeigt wird. Für eine Liste aller [!DNL Workfront] mit Objekten verknüpfte Symbole, siehe [Objektsymbole](#object-icons).

  >[!TIP]
  >
  >Für häufige Aufgaben in Ihrem Unternehmen sollten Sie eine benutzerdefinierte Dokumentation erstellen, die Ihre Terminologie widerspiegelt.

## Objektsymbole

Die [!DNL Workfront] -Dokumentation bezieht sich immer auf die Standardnamen von Objekten. Wenn die Namen Ihrer Objekte angepasst wurden, können Sie sich auf das ihnen zugeordnete Symbol verlassen, um zu verstehen, welches angepasste Objekt welcher entspricht [!DNL Workfront] Standardobjekt

Weitere Informationen darüber, welche Objekte benutzerdefinierte Namen haben können in [!DNL Workfront], siehe [Objektnamen, die mithilfe einer  [!UICONTROL Layout-Vorlage]](#object-names-that-can-be-customized-using-a-layout-template).

Im Folgenden finden Sie eine Liste der Objekte und der zugehörigen Symbole in Workfront.

| **Objekt** | **Symbol** | **Anpassbarer Objektname** |
|---|---|---|
| [!UICONTROL Firma] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Ziel] | ![](assets/nwe-goal-icon.png) | ms |
| [!UICONTROL Gruppe] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Problem] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ms |
| [!UICONTROL Auftragsrolle] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ms |
| [!UICONTROL Programm] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ms |
| [!UICONTROL Projekt] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ms |
| [!UICONTROL Bericht] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Aufgabe] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ms |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Vorlage] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Referenzanzahl von Objekten

Jedes Objekt, das in [!DNL Workfront] wird eine eindeutige Referenznummer zugewiesen. Referenznummern sind nützlich, um zwischen zwei ansonsten ähnlichen Objekten zu unterscheiden (z. B. Aufgaben mit demselben Namen). Sie können anhand der Referenznummern nach Objekten suchen und Referenznummern in Berichte aufnehmen.

Informationen zum Suchen nach Objekten anhand der Referenznummer finden Sie unter [Referenzanzahl von Objekten verwenden](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Objektspezifische Suchvorgänge

Sie können alle Objekte durchsuchen, die in [!DNL Workfront]oder Sie können ein bestimmtes Objekt auswählen, nach dem Sie in Ihren einfachen und erweiterten Suchvorgängen suchen möchten.

Es sind nicht alle Objekte durchsuchbar in [!DNL Workfront]. Sie können grundlegende und erweiterte Suchen nach den folgenden Objekten in [!DNL Workfront]:

| **Objekt** | **Grundlegende Suche** | **Erweiterte Suche** |
|---|---|---|
| [!UICONTROL Projekte] | ✓ | ✓ |
| [!UICONTROL Aufgaben] | ✓ | ✓ |
| [!UICONTROL Probleme] | ✓ | ✓ |
| [!UICONTROL Berichte] | ✓ | ✓ |
| [!UICONTROL Benutzende] | ✓ | ✓ |
| [!UICONTROL Vorlagen] | ✓ | ✓ |
| [!UICONTROL Dokumente] | ✓ | ✓ |
| [!UICONTROL Portfolios] | ✓ | ✓ |
| [!UICONTROL Programme] | ✓ | ✓ |
| [!UICONTROL Dashboards] | ✓ | ✓ |
| [!UICONTROL Unternehmen] | ✓ | ✓ |
| [!UICONTROL Hinweise] (oder [!UICONTROL Updates]) | ✓ |  |

Weitere Informationen zum Ausführen grundlegender und erweiterter Suchvorgänge finden Sie unter [!DNL Workfront], siehe [Suche [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Berichte zu Objekten

Das Verständnis der Hierarchie und Interdependenz von Objekten ist äußerst wichtig, bevor Sie mit der Erstellung von Berichten in [!DNL Workfront]. Berichte sind objektspezifisch. Sie müssen das richtige Objekt für Ihren Bericht auswählen, bevor Sie die gewünschten Daten anzeigen können.

>[!IMPORTANT]
>
>Sie können nur Berichte zu dem ausgewählten Objekt und den übergeordneten Objekten im selben Bericht erstellen. Informationen zu den untergeordneten Objekten können nicht in einem übergeordneten Objektbericht enthalten sein. Beispielsweise können Sie Projektinformationen in einem Aufgabenbericht anzeigen, aber keine Aufgabeninformationen in einem Projektbericht.

Über unsere offene API können Sie Berichte zu allen Objekten in der Datenbank erstellen. Eine vollständige Liste aller Objekte in der Datenbank finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Wenn Sie die Namen Ihrer Objekte mithilfe einer Layoutvorlage angepasst haben, wurden auch die Namen des Objekts in ReportBuilder angepasst. Stellen Sie sicher, dass Sie wissen, welche Objekte angepasst wurden, und suchen Sie im ReportBuilder nach dem angepassten Namen. Weitere Informationen darüber, welche Objekte benutzerdefinierte Namen haben können in [!DNL Workfront], siehe [Objektnamen, die mithilfe einer  [!UICONTROL Layout-Vorlage]](#object-names-that-can-be-customized-using-a-layout-template) in diesem Artikel.
> * Bei der Verwendung des Textmodus in Ihren Berichten sind die Namen der Objekte in Textmodusausdrücken die Standardnamen in [!DNL Workfront]und nicht die angepassten Objektnamen. Weitere Informationen zur Verwendung des Textmodus in Berichten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Weitere Informationen über unsere API finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

### Für Berichte verfügbare Objekte

Sie können Berichte zu den folgenden Objekten erstellen, wenn Sie die Berichterstellung im [!DNL Workfront] Webanwendung. Eingezogene Aufzählungspunkte geben weitere Informationen zum Objekt und stellen keine zusätzlichen Objekte dar.

* [!UICONTROL Projekt]
* [!UICONTROL Aufgabe]
* [!UICONTROL Stunde]
* [!UICONTROL Problem]
* [!UICONTROL Benutzer]
* [!UICONTROL Zugriff] Ebene
* [!UICONTROL Validierung]
* [!UICONTROL Validierungsprozess]
* [!UICONTROL Zuweisung]
* [!UICONTROL Grundlinie]
* [!UICONTROL Baseline-Aufgabe]
* [!UICONTROL Rechnungsdatensatz]
* [!UICONTROL Budgetierte Stunde]
   * Dies ist die [!UICONTROL Budgetierte Stunden], wie sie in älteren, veralteten Tools zur Ressourcenverwaltung angezeigt werden.
   * Der &quot;Bud. Stundenfeld im Feld [!UICONTROL Budgetierte Stunde] Der Bericht bezieht sich auf die Stunden, die für Stellenrollen in der [!UICONTROL Ressourcenplaner]. Weitere Informationen finden Sie unter [Grundlegendes [!UICONTROL Geplante Arbeitskosten] und [!UICONTROL Budgetierte Stunden] für Projekte](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Kalenderereignis]
* [!UICONTROL Firma]
* [!UICONTROL Benutzerdefiniertes Formular]
* [!UICONTROL Dashboard]
* [!UICONTROL Dokument]
* [!UICONTROL Dokumentvalidierung]
* [!UICONTROL Dokumentversion]
   * Sie können Informationen zur Version des Dokuments, zum Dokument, mit dem die Version verknüpft ist, zum Ersteller der Version und zum Benutzer, der den Testversand in der Dokumentversion erstellt hat, sofern vorhanden (Testversand-Ersteller) anzeigen.
* [!UICONTROL E-Mail-Vorlage]
* [!UICONTROL Ausgaben]
* [!UICONTROL Ausgabentyp]
* [!UICONTROL Externe Seite]
* [!UICONTROL Favorit]
* [!UICONTROL Filter]
* [!UICONTROL Ziel]
   * Sie können einen Bericht für strategische Ziele erstellen oder zielbezogene Informationen in einem Projektbericht anzeigen, wenn Projekte mit Zielen als Zielaktivitäten verknüpft sind. Sie können strategische Ziele erstellen und Projekte nur dann verbinden, wenn Ihr Unternehmen eine [!DNL Workfront Goals] -Lizenz. Informationen zu [!DNL Workfront Goals], siehe [[!DNL Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md). Weitere Informationen zur Verbindung von Projekten mit strategischen Zielen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Sie können keine Berichte zu Projektzielen erstellen, die mit einem [!UICONTROL Geschäftsfall]. Weitere Informationen zu Projektzielen und strategischen Zielen finden Sie unter [Glossar [!DNL Adobe Workfront] Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Gruppe]
* [!UICONTROL Gruppierung]
* [!UICONTROL Stündentyp]
* [!UICONTROL Initiative]
   * Sie können nur dann einen Bericht für Initiativen erstellen, die die untergeordneten Objekte eines Plans sind, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz. Weitere Informationen zu Initiativen finden Sie unter [Übersicht über Initiativen im [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Aufgabengebiet für Initiative
   * Sie können nur dann einen Bericht über die mit den Initiativen in einem Plan verbundenen Arbeitsplatzrollen erstellen, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz. Informationen zum Erstellen von Initiativen und deren Zuordnung zu Berufsrollen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteration]
* [!UICONTROL Auftragsrolle]
* [!UICONTROL Journaleintrag]
   * Sie können Berichte zu getrackten Systemaktualisierungen im Abschnitt [!UICONTROL Updates] Objektbereich wie Aufgaben, Projekte, Probleme usw. Weitere Informationen finden Sie unter [Bericht über [!UICONTROL Updates] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout-Vorlage]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone-Pfad]
* [!UICONTROL Hinweis] oder [!UICONTROL Updates]
   * Sie können Berichte zu Kommentaren erstellen, die von einzelnen Benutzern hinzugefügt wurden.

* [!UICONTROL Parameter] (oder [!UICONTROL Benutzerdefiniertes Feld])
* [!UICONTROL Parametergruppe] (oder [!UICONTROL Abschnittsumbruch])
* [!UICONTROL Portfolio]
* [!UICONTROL Programm]
* [!UICONTROL Projekt] ([!UICONTROL Finanzdaten])

  >[!NOTE]
  >
  >Finanzinformationen werden in [!UICONTROL Projekt] ([!UICONTROL Finanzdaten]) werden nur dann gemeldet, wenn die damit verbundenen Daten weniger als 5 Jahre alt sind. Wenn beispielsweise im Januar 2015 einer Aufgabe eine berufliche Rolle zugewiesen wurde und heute September 2021 ist, wird ein Finanzfeld wie der [!UICONTROL Zuordnungsdatum] für die Stellenrolle nicht in der [!UICONTROL Projekt (Finanzdaten)] Bericht.

* [!UICONTROL Validierung des Testversands]
   * Sie können verschiedene Informationen über die Validierung des Testversands einsehen, einschließlich des Testversands, der zur Validierung unterbreitet wurde, Informationen über die [!UICONTROL Genehmiger], Informationen zum Antragsteller (wenn der Antragsteller lizenziert ist) [!DNL Workfront] Benutzer), Versionsinformationen, Testversand-ID und Erstellungsdatum des Testversands.\
      [!UICONTROL Validierung des Testversands] Berichte enthalten nur Testsendungen, die in den Arbeitsbereichen der Benutzer verfügbar sind, in denen noch keine Entscheidungen getroffen wurden.\
   * Die Befähigungsnachweise werden unter [!DNL Workfront] wie beschrieben [Benutzer zu Testversand hinzufügen](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Freigeben eines Testversands in [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Warteschlange]
* [!UICONTROL Warteschlangenthema]
* [!UICONTROL Rate] (zeigt die Vorgangsrolle an. [!UICONTROL Abrechnungsrate] information)
* [!UICONTROL Erinnerungsbenachrichtigung]
* [!UICONTROL Bericht]
* [!UICONTROL Ressourcenpool]
* [!UICONTROL Risiko]
* [!UICONTROL Risikotyp]
* [!UICONTROL Zeitplan]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Vorlage]
* [!UICONTROL Vorlagenaufgabe]
* [!UICONTROL Zeitlimit]
   * Sie können Berichte zur Zeitüberschreitung eines Benutzers erstellen, wie vom Benutzer in seinem Profil angegeben.

* [!UICONTROL Datenblatt]
* [!UICONTROL Datenblatt-Profil]
* [!UICONTROL Themengruppe]
* [!UICONTROL Benutzervalidierung]
* [!UICONTROL Benutzerdelegierung]

   * Sie können Berichte zu Benutzern erstellen, die beauftragt wurden, Aufgaben und Probleme anderer Benutzer auszuführen, während sie nicht im Büro sind. Dieser Bericht zeigt den Abwesenheitsbenutzer sowie den Benutzer an, der während seiner Abwesenheit seinen Verpflichtungen nachkommt.

* [!UICONTROL Benutzerentscheidungen]

   * Sie können berichten, wie viele Entscheidungen Benutzer im aktuellen Monat bezüglich Testsendungen und Dokumenten getroffen haben.

* [!UICONTROL Ansicht]
* [!UICONTROL Arbeitselement] (Dadurch wird ein Bericht für Aufgaben und Probleme erstellt)
