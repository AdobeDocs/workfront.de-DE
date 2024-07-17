---
content-type: overview;reference
navigation-topic: workfront-navigation
title: "[!DNL Adobe Workfront] Objektübersicht"
description: "Die Informationen, die Sie in [!DNL Adobe Workfront] anzeigen, werden durch Objekte dargestellt, die in der [!DNL Workfront] Datenbank gespeichert sind. Die Objekte sind das, was die Informationen in [!DNL Workfront] antreibt. Weitere Informationen zu diesen Objekten finden Sie in diesem Artikel."
feature: Get Started with Workfront
author: Alina
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 25939493f6ffed31ae1bdaf26d417ce4e5e5c004
workflow-type: tm+mt
source-wordcount: '2419'
ht-degree: 1%

---

# Überblick über [!DNL Adobe Workfront] Objekte

<!--Audited: 12/2023-->

<!--
<***Linked to several articles, do not remove/ change. 
-->

Die Informationen, die Sie in [!DNL Adobe Workfront] anzeigen, werden durch Objekte dargestellt, die in der [!DNL Workfront] -Datenbank gespeichert sind. Die Objekte sind das, was die Informationen in [!DNL Workfront] antreibt.

Es ist wichtig zu verstehen, wie die Objekte in [!DNL Workfront] definiert sind, damit Sie das richtige Objekt für die in Ihrer Organisation erforderlichen Anforderungen verwenden können.

Wenn Sie beispielsweise eine große Arbeitsmenge planen, müssen Sie das Objekt [!UICONTROL Projekt] verwenden, um diese Arbeit zu definieren. Um diese Arbeit in kleinere geplante Inkremente zu unterteilen, können Sie das Objekt [!UICONTROL Aufgabe] verwenden. Für einen kleineren Arbeitsaufwand, der nicht geplant ist und unerwartet auftreten kann, können Sie das Objekt Problem verwenden. Wenn Sie den Fortschritt und die Einhaltung des Budgets und der Zeitleiste einer Projektgruppe verfolgen möchten, können Sie diese in [!UICONTROL Portfolios] und [!UICONTROL Programme] organisieren. Um weitere Elemente zu definieren, die Sie bei der Auflösung Ihrer Arbeit unterstützen, möchten Sie andere Objekte verwenden, die unter [!UICONTROL Projekte], [!UICONTROL Aufgaben], [!UICONTROL Probleme] oder [!UICONTROL Portfolios] gespeichert sind, wie [!UICONTROL Dokumente], [!UICONTROL Aktualisierungen], [!UICONTROL Stunden], [!UICONTROL Benutzer]}, oder [!UICONTROL Auftragsrollen].

[!UICONTROL Berichte] und [!UICONTROL Dashboards] sind ein weiteres Beispiel für Objekte, mit denen Sie die Datenmenge, die Sie in [!DNL Workfront] haben, visuell organisieren können, damit sie für alle Benutzer leicht zugänglich ist.

Eine vollständige Liste der Objekte in [!DNL Workfront] finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

## Abhängigkeit und Hierarchie von Objekten

Objekte sind in [!UICONTROL Workfront] miteinander verknüpft. Beispielsweise kann eine Aufgabe oder ein Problem nie unabhängig von einem Projekt existieren. [!UICONTROL Aufgaben] und [!UICONTROL Probleme] sind Beispiele für Objekte, die im Objekt [!UICONTROL Projekt] gespeichert sind. [!UICONTROL Aufgaben] und [!UICONTROL Probleme] werden als untergeordnete Objekte von Projekten betrachtet.

Im Folgenden finden Sie einige der am häufigsten verwendeten Objekte in [!DNL Workfront] und die zugehörigen übergeordneten und untergeordneten Objekte:

| **Objekt** | **Übergeordnete Objekte** | **Untergeordnete Objekte** |
|---|---|---|
| [!UICONTROL Portfolios] |  | [!UICONTROL Programme], [!UICONTROL Projekte], [!UICONTROL Dokumente], [!DNL Notes], [!UICONTROL Benutzer] |
| [!UICONTROL Programme] | [!UICONTROL Portfolios] | [!UICONTROL Projekte], [!UICONTROL Dokumente], [!UICONTROL Notizen], [!UICONTROL Benutzer] |
| [!UICONTROL Projekte] | [!UICONTROL Portfolios], [!UICONTROL Programme] | [!UICONTROL Aufgaben], [!UICONTROL Probleme], [!UICONTROL Dokumente], [!UICONTROL Notizen], [!UICONTROL Stunden], [!UICONTROL Benutzer] |
| [!UICONTROL Aufgaben] | [!UICONTROL Projekte] | [!UICONTROL Issues], [!UICONTROL Children Tasks], [!UICONTROL Documents], [!UICONTROL notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Probleme] | [!UICONTROL Aufgaben], [!UICONTROL Projekte] | [!UICONTROL Dokumente], [!UICONTROL Notizen], [!UICONTROL Stunden], [!UICONTROL Benutzer] |
| [!UICONTROL Dashboards] |  | [!UICONTROL Berichte], externe Seiten |
| [!UICONTROL Berichte] | [!UICONTROL Dashboards] |  |
| [!UICONTROL Gruppen] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Teams] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Benutzende] | [!UICONTROL Gruppen], [!UICONTROL Teams], [!UICONTROL Unternehmen] | [!UICONTROL Vorgangsrollen] |
| [!UICONTROL Unternehmen] |  | [!UICONTROL Benutzende] |
| [!UICONTROL Dokumente] | [!UICONTROL Aufgaben], [!UICONTROL Probleme], [!UICONTROL Projekte], [!UICONTROL Portfolios], [!UICONTROL Programme], [!UICONTROL Benutzer] |  |
| [!UICONTROL Pläne]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Ergebnisse], [!UICONTROL Aktivitäten] |

Eine vollständige Liste der Objekte in [!DNL Workfront] finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

*Pläne sind die Objekte von [!DNL Adobe Workfront Scenario Planner]. Weitere Informationen zum [!DNL Scenario Planner] finden Sie unter [Überblick über den [!UICONTROL Szenario-Planer]](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Ziele] sind die Objekte von [!DNL Adobe Workfront Goals]. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter [[!DNL Adobe Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Objektnamen anpassen

Als [!DNL Workfront] -Administrator können Sie die Objektnamen in [!DNL Workfront] anpassen, indem Sie eine [!UICONTROL Layout-Vorlage] verwenden.

Weitere Informationen zum Anpassen von Objektnamen mit einer [!UICONTROL Layout-Vorlage] finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Nachdem Sie eine Layoutvorlage angepasst und sie Benutzern zugewiesen haben, sehen diese Benutzer die benutzerdefinierten Namen für die Objekte. Die Benutzer, die der Layoutvorlage zugewiesen wurden, sehen die Standardnamen für die Objekte nirgendwo in der Webanwendung mehr.

Wenn beispielsweise der größere Arbeitsaufwand in Ihrer Organisation als &quot;Interaktion&quot;bezeichnet wird, können Sie den Namen &quot;[!UICONTROL Projekt]&quot;durch &quot;Interaktion&quot;ersetzen. Ihre [!DNL Workfront] -Oberfläche zeigt überall &quot;Interaktion&quot;anstelle von &quot;[!UICONTROL Projekt]&quot;an, wo der Name &quot;[!UICONTROL Projekt]&quot;angezeigt wird.

>[!NOTE]
>
>Damit die neuen Namen der Objekte für Ihre Benutzer sichtbar sind, müssen sie sich ab- und wieder bei [!DNL Workfront] anmelden, nachdem Sie die [!UICONTROL Layout-Vorlage] gespeichert haben.

>[!IMPORTANT]
>
>Die Dokumentation [!DNL Workfront] bezieht sich immer auf die Standardnamen der Objekte. Stellen Sie als Administrator von [!DNL Workfront] sicher, dass Sie Benutzer über Änderungen an Objektnamen informieren, damit sie verstehen können, wie die [!DNL Workfront] -Dokumentation verwendet wird, sowie über die Bereiche der Anwendungen, die nicht die Änderungen an den Namen der Objekte widerspiegeln.

* [Objektnamen, die mit einer [!UICONTROL Layout-Vorlage] angepasst werden können](#object-names-that-can-be-customized-using-a-layout-template)
* [Bereiche von  [!DNL Workfront] , die die benutzerdefinierten Objektnamen widerspiegeln](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Bereiche von  [!DNL Workfront] , die nicht die benutzerdefinierten Objektnamen widerspiegeln](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Objektnamen, die mit einer [!UICONTROL Layout-Vorlage] angepasst werden können

Als [!DNL Workfront] -Administrator können Sie die Namen der folgenden Objekte an die Terminologie in Ihrer Organisation anpassen:

* [!UICONTROL Portfolio]
* [!UICONTROL Programm]
* [!UICONTROL Projekt]
* [!UICONTROL Aufgabe]
* [!UICONTROL Probleme]
* [!UICONTROL Ziel]*
* [!UICONTROL Ergebnis]*
* [!UICONTROL Aktivität]*

  *[!UICONTROL Ziele], [!UICONTROL Ergebnisse] und [!UICONTROL Aktivitäten] sind nur verfügbar, wenn Ihr Unternehmen [!DNL Workfront Goals] erworben hat. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter [[!DNL Adobe Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Szenario]**
* [!UICONTROL Plan]**

  **[!UICONTROL Initiativen], [!UICONTROL Szenarien] und [!UICONTROL Pläne] sind nur verfügbar, wenn Ihr Unternehmen die [!DNL Workfront Scenario Planner] erworben hat. Weitere Informationen zum [!DNL Scenario Planner] finden Sie unter [Erste Schritte mit dem  [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).



Weitere Informationen dazu, wie Sie Objektnamen mit [!UICONTROL Layout-Vorlagen] anpassen können, finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Sie können die Namen anderer Objekte in Workfront nicht anpassen. Eine vollständige Liste der Objekte in [!DNL Workfront] finden Sie im [API-Explorer](../../../wf-api/general/api-explorer.md).

Wenn Sie den Namen eines Objekts anpassen, wird der neue Name für dieses Objekt in den meisten Bereichen der [!DNL Workfront]-Anwendung angezeigt, in denen dieser Objektname angezeigt wird.

### Bereiche von [!DNL Workfront], die die benutzerdefinierten Objektnamen widerspiegeln

Die folgenden Bereiche zeigen den aktualisierten Namen der Objekte:

* Navigation oben
* Alle Abschnitte in der linken Bedienfeldnavigation
* Alle Menüs
* In-App-Benachrichtigungen
* Berichterstellung und Berichterstellungselemente (Ansichten, Filter und Gruppierungen)
* Schaltflächen [!UICONTROL Speichern]
* Exportierte Dateien
* E-Mails
* Mobile Apps

### Bereiche von [!DNL Workfront], die nicht die benutzerdefinierten Objektnamen widerspiegeln

In den folgenden Bereichen wird der aktualisierte Name der Objekte nicht angezeigt:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Add-in

### Auswirkungen der Anpassung von Objektnamen

Beachten Sie beim Anpassen der Objektnamen in [!DNL Workfront] Folgendes:

* Sie können stilistische oder grammatikalische Fehler in Systemanzeigen feststellen. Wenn Sie beispielsweise &quot;[!UICONTROL Problem]&quot;in &quot;Anfrage&quot;umbenennen und irgendwo im System die Wortgruppe &quot;Eine Anfrage&quot;sehen, funktioniert dies wie beabsichtigt und sollte nicht als Fehler betrachtet werden.
* Ihre benutzerdefinierten Namen für die Objekte können nicht übersetzt werden. Nur die Standardnamen [!DNL Workfront] können in die unterstützten Sprachen übersetzt werden. Weitere Informationen zu Sprachen, die in [!DNL Workfront] unterstützt werden, finden Sie unter [Unterstützte Sprachen in  [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). Die benutzerdefinierten Objektnamenfelder unterstützen Fremdzeichen, sodass Sie Terminologie in jeder Sprache eingeben können.
* Wenn Sie Objektnamen mithilfe einer [!UICONTROL Layout-Vorlage] anpassen, empfehlen wir, Ihre [!UICONTROL Layout-Vorlagen] basierend auf Ihren Geschäftseinheiten (Teams oder Gruppen) zuzuweisen.\
   Es wird empfohlen, Namen zu verwenden, die von den Benutzern dieser Geschäftsbereiche deutlich verstanden werden, um Verwirrung zu vermeiden.
* E-Mail-Benachrichtigungen und zugestellte Berichte enthalten immer Objektnamen, die in der [!UICONTROL Layout-Vorlage] des Benutzers definiert sind, der die E-Mail generiert. Ihre Benutzer sollten darauf vorbereitet sein, in ihren E-Mails Objektnamen anzuzeigen, die nicht mit ihrer Gruppe oder ihrem Team verbunden sind, wenn sie E-Mail-Benachrichtigungen von Benutzern in anderen Teams und Gruppen erhalten.\
   Als [!DNL Workfront] -Administrator empfehlen Sie Benutzern, die mit jedem Objekt verknüpften Symbole zu bemerken. Die Symbole bleiben zwischen verschiedenen Objektnamen konsistent und entsprechen dem Standardobjekt, wie es in der Datenbank angezeigt wird. Eine Liste aller mit Objekten verknüpften [!DNL Workfront] Symbole finden Sie unter [Objektsymbole](#object-icons).

  >[!TIP]
  >
  >Für häufige Aufgaben in Ihrem Unternehmen sollten Sie eine benutzerdefinierte Dokumentation erstellen, die Ihre Terminologie widerspiegelt.

## Objektsymbole

Die Dokumentation [!DNL Workfront] bezieht sich immer auf die Standardnamen der Objekte. Wenn die Namen Ihrer Objekte angepasst wurden, können Sie sich auf das ihnen zugeordnete Symbol verlassen, um zu verstehen, welches angepasste Objekt mit welchem [!DNL Workfront] Standardobjekt übereinstimmt.

Weitere Informationen dazu, welche Objekte in [!DNL Workfront] benutzerdefinierte Namen haben können, finden Sie unter [Objektnamen, die mit einer [!UICONTROL Layout-Vorlage]](#object-names-that-can-be-customized-using-a-layout-template) angepasst werden können.

Im Folgenden finden Sie eine Liste der Objekte und der zugehörigen Symbole in Workfront.

| **Objekt** | **Symbol** | **Anpassbarer Objektname** |
|---|---|---|
| [!UICONTROL Firma] | ![](assets/company-icon-nwe.png) , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png) , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Ziel] | ![](assets/nwe-goal-icon.png) | ms |
| [!UICONTROL Gruppe] | ![](assets/groups-icon-nwe.png) , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Probleme] | ![](assets/issue-icon-nwe.png) , ![](assets/nwe-issues-icon.png) | ms |
| [!UICONTROL Auftragsrolle] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png) , ![](assets/nwe-portfolios-icon.png) | ms |
| [!UICONTROL Programm] | ![](assets/program-icon-nwe.png) , ![](assets/nwe-programs-icon.png) | ms |
| [!UICONTROL Projekt] | ![](assets/project-icon-nwe.png) , ![](assets/nwe-projects-icon.png) | ms |
| [!UICONTROL Bericht] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Aufgabe] | ![](assets/task-icon-new.png) , ![](assets/nwe-tasks-icon.png) | ms |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png), ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Vorlage] | ![](assets/template-icon-nwe.png) , ![](assets/nwe-templates-icon.png) |  |
| [!UICONTROL Benutzer] | ![](assets/users-icon-gray.png) , ![](assets/user-icon-blue.png) , ![](assets/user-icon-initials.png), ![](assets/user-avatar.png), ![](assets/user-main-menu-area.png) |  |

## Referenzanzahl von Objekten

Jedem in [!DNL Workfront] erstellten Objekt wird eine eindeutige Referenznummer zugewiesen. Referenznummern sind nützlich, um zwischen zwei ansonsten ähnlichen Objekten zu unterscheiden (z. B. Aufgaben mit demselben Namen). Sie können anhand der Referenznummern nach Objekten suchen und Referenznummern in Berichte aufnehmen.

Weitere Informationen zum Suchen nach Objekten anhand der Referenznummer finden Sie unter [Verwenden der Referenznummer von Objekten](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Objektspezifische Suchvorgänge

Sie können alle Objekte durchsuchen, die in [!DNL Workfront] durchsucht werden können, oder Sie können ein bestimmtes Objekt auswählen, nach dem in Ihren einfachen und erweiterten Suchen gesucht werden soll.

Nicht alle Objekte können in [!DNL Workfront] durchsucht werden. Sie können grundlegende und erweiterte Suchen nach den folgenden Objekten in [!DNL Workfront] ausführen:

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
| [!UICONTROL Notizen] (oder [!UICONTROL Aktualisierungen]) | ✓ |  |

Weitere Informationen zum Ausführen einfacher und erweiterter Suchvorgänge in [!DNL Workfront] finden Sie unter [Suchen [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).


## Eingeschränkter Zugriff auf Objekte

Wenn ein Benutzer keinen Zugriff auf ein Objekt hat, wird ihm an einer beliebigen Stelle in Workfront der Objektname &quot;Kein Zugriff&quot;angezeigt.

Der Zugriff auf Objekte kann auf Zugriffsebene oder in den Berechtigungen eines bestimmten Objekts eingeschränkt werden.

Dies gilt für alle Objekte und untergeordneten Objekte, die im Abschnitt [Interdependenz und Hierarchie von Objekten](#interdependency-and-hierarchy-of-objects) in diesem Artikel aufgeführt sind. Dies gilt nicht für Team- und User-Objekte.

## Berichte zu Objekten

Das Verständnis der Hierarchie und Interdependenz von Objekten ist äußerst wichtig, bevor Sie mit dem Erstellen von Berichten in [!DNL Workfront] beginnen. Berichte sind objektspezifisch. Sie müssen das richtige Objekt für Ihren Bericht auswählen, bevor Sie die gewünschten Daten anzeigen können.

>[!IMPORTANT]
>
>Sie können nur Berichte zu dem ausgewählten Objekt und den übergeordneten Objekten im selben Bericht erstellen. Informationen zu den untergeordneten Objekten können nicht in einem übergeordneten Objektbericht enthalten sein. Beispielsweise können Sie Projektinformationen in einem Aufgabenbericht anzeigen, aber keine Aufgabeninformationen in einem Projektbericht.

Über unsere offene API können Sie Berichte zu allen Objekten in der Datenbank erstellen. Eine vollständige Liste aller Objekte in der Datenbank finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
> * Wenn Sie die Namen Ihrer Objekte mithilfe einer Layoutvorlage angepasst haben, wurden auch die Namen des Objekts in ReportBuilder angepasst. Stellen Sie sicher, dass Sie wissen, welche Objekte angepasst wurden, und suchen Sie im ReportBuilder nach dem angepassten Namen. Weitere Informationen dazu, welche Objekte in [!DNL Workfront] benutzerdefinierte Namen haben können, finden Sie unter [Objektnamen, die mit einer [!UICONTROL Layout-Vorlage]](#object-names-that-can-be-customized-using-a-layout-template) angepasst werden können.
> * Bei der Verwendung des Textmodus in Ihren Berichten sind die Namen der Objekte in Textmodusausdrücken die Standardnamen in [!DNL Workfront] und nicht die benutzerdefinierten Objektnamen. Weitere Informationen zur Verwendung des Textmodus in Berichten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
Weitere Informationen zu unserer API finden Sie unter [API-Explorer](../../../wf-api/general/api-explorer.md).

### Für Berichte verfügbare Objekte

Sie können Berichte zu den folgenden Objekten erstellen, wenn Sie ReportBuilder in der [!DNL Workfront] -Webanwendung verwenden. Eingezogene Aufzählungspunkte geben weitere Informationen zum Objekt und stellen keine zusätzlichen Objekte dar.

* [!UICONTROL Projekt]
* [!UICONTROL Aufgabe]
* [!UICONTROL Stunde]
* [!UICONTROL Probleme]
* [!UICONTROL Benutzer]
* [!UICONTROL Zugriffsebene]
* [!UICONTROL Genehmigung]
* [!UICONTROL Genehmigungsprozess]
* [!UICONTROL Zuweisung]
* [!UICONTROL Grundlinie]
* [!UICONTROL  Baseline-Aufgabe]
* [!UICONTROL Abrechnungsdatensatz]
* [!UICONTROL Budgetierte Stunde]
   * Dies sind die [!UICONTROL budgeted Hours], wie sie in älteren, veralteten Tools zur Ressourcenverwaltung angezeigt werden.
   * Der &quot;Bud. Das Feld &quot;Stunden&quot;im Bericht [!UICONTROL Budgetierte Stunde] bezieht sich auf die Stunden, die im [!UICONTROL Ressourcenplaner] für Stellenrollen vorgesehen sind. Weitere Informationen finden Sie unter [Verstehen der [!UICONTROL budgetierten Arbeitskosten] und der [!UICONTROL budgetierten Arbeitsstunden] für Projekte](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Kalenderereignis]
* [!UICONTROL Firma]
* [!UICONTROL Benutzerdefiniertes Formular]
* [!UICONTROL Dashboard]
* [!UICONTROL Document]
* [!UICONTROL Dokumentgenehmigung]
* [!UICONTROL Dokumentversion]
   * Sie können Informationen zur Version des Dokuments, zum Dokument, mit dem die Version verknüpft ist, zum Ersteller der Version und zum Benutzer, der den Testversand in der Dokumentversion erstellt hat, sofern vorhanden (Testversand-Ersteller) anzeigen.
* [!UICONTROL E-Mail-Vorlage]
* [!UICONTROL Kosten]
* [!UICONTROL Ausgabentyp]
* [!UICONTROL Externe Seite]
* [!UICONTROL Favorit]
* [!UICONTROL Filter]
* [!UICONTROL Ziel]
   * Sie können einen Bericht für strategische Ziele erstellen oder zielbezogene Informationen in einem Projektbericht anzeigen, wenn Projekte mit Zielen als Zielaktivitäten verknüpft sind. Sie können strategische Ziele erstellen und Projekte nur dann verknüpfen, wenn Ihr Unternehmen eine [!DNL Workfront Goals] -Lizenz erworben hat. Weitere Informationen zu [!DNL Workfront Goals] finden Sie unter [[!DNL Workfront Goals] Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md). Informationen zum Verbinden von Projekten mit strategischen Zielen finden Sie unter [Projekte zu Zielen in Adobe Workfront hinzufügen](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
*Sie können keine Berichte zu Projektzielen erstellen, die mit einem [!UICONTROL Geschäftsszenario] verknüpft sind. Weitere Informationen zu Projektzielen und strategischen Zielen finden Sie unter [Glossar zur  [!DNL Adobe Workfront] Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Gruppe]
* [!UICONTROL Grouping]
* [!UICONTROL Stundentyp]
* [!UICONTROL Initiative]
   * Sie können nur dann einen Bericht für Initiativen erstellen, die die untergeordneten Objekte eines Plans sind, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat. Weitere Informationen zu Initiativen finden Sie unter [Übersicht über Initiativen in der [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).

* Aufgabengebiet für Initiative
   * Sie können nur dann einen Bericht für die mit den Initiativen in einem Plan verbundenen Arbeitsplatzrollen erstellen, wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat. Weitere Informationen zum Erstellen von Initiativen und zum Verknüpfen dieser Initiativen mit Arbeitsplatzrollen finden Sie unter [Erstellen und Bearbeiten von Initiativen im Abschnitt [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).

* [!UICONTROL Iteration]
* [!UICONTROL Auftragsrolle]
* [!UICONTROL Journaleintrag]
   * Sie können über getrackte Systemaktualisierungen im Bereich [!UICONTROL Aktualisierungen] von Objekten wie Aufgaben, Projekten, Problemen usw. berichten. Weitere Informationen finden Sie unter [Bericht über den Bereich [!UICONTROL Aktualisierungen]](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout-Vorlage]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone-Pfad]
* [!UICONTROL Hinweis] oder [!UICONTROL Aktualisierungen]
   * Sie können Berichte zu Kommentaren erstellen, die von einzelnen Benutzern hinzugefügt wurden.

* [!UICONTROL Parameter] (oder [!UICONTROL Benutzerdefiniertes Feld])
* [!UICONTROL Parametergruppe] (oder [!UICONTROL Abschnittsumbruch])
* [!UICONTROL Portfolio]
* [!UICONTROL Programm]
* [!UICONTROL Projekt (Finanzdaten)]
   * Finanzinformationen werden in [!UICONTROL Projekt (Finanzdaten)] -Berichten nur angezeigt, wenn die damit verbundenen Daten weniger als 5 Jahre alt sind. Wenn beispielsweise im Januar 2015 einer Aufgabe eine Stellenrolle zugewiesen wurde und heute der September 2021 ist, wird ein Finanzfeld wie das [!UICONTROL Zuordnungsdatum] für die Stellenrolle nicht im Bericht [!UICONTROL Projekt (Finanzdaten)] ausgefüllt.

  >[!CAUTION]
  >
  >Die Ausführung des Berichts Projekt (Finanzdaten) führt eine Neuberechnung Ihrer Finanzdaten durch, die frühere Finanzdaten überschreiben können und viel Zeit in Anspruch nehmen können. Weitere Informationen zu den Auswirkungen der Neuberechnung finanzieller Daten finden Sie unter [Neuberechnung der Projektfinanzen vornehmen](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

* [!UICONTROL Korrekturabzug-Genehmigung]
   * Ermöglicht die Anzeige verschiedener Informationen zur Testversand-Validierung, darunter der zur Validierung eingereichte Testversand, Informationen zum [!UICONTROL Genehmiger], Informationen zum Antragsteller (wenn der Antragsteller ein lizenzierter [!DNL Workfront] Benutzer ist), Versionsinformationen, die Kennung des Testversands und das Erstellungsdatum des Testversands.\
      Die Berichte [!UICONTROL Validierungsnachweis] enthalten nur Testsendungen, die in den Arbeitsbereichen der Benutzer verfügbar sind, in denen noch keine Entscheidungen getroffen wurden.\
   * Testversand-Genehmigungen werden in [!DNL Workfront] wie im Abschnitt [Hinzufügen von Benutzern zu einem Testversand](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Freigeben eines Testversands innerhalb von  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) beschrieben zugewiesen.

* [!UICONTROL Queue]
* [!UICONTROL Warteschlangenthema]
* [!UICONTROL Rate] (Zeigt Informationen zur Auftragsrolle [!UICONTROL Abrechnungsrate] an)
* [!UICONTROL Erinnerungsbenachrichtigung]
* [!UICONTROL Bericht]
* [!UICONTROL Ressourcen-Pool]
* [!UICONTROL Risiko]
* [!UICONTROL Risikotyp]
* [!UICONTROL Zeitplan]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Vorlage]
* [!UICONTROL Vorlagenaufgabe]
* [!UICONTROL Ausschaltzeit]
   * Sie können Berichte zur Zeitüberschreitung eines Benutzers erstellen, wie vom Benutzer in seinem Profil angegeben.

* [!UICONTROL Zeitblatt]
* [!UICONTROL Timesheet-Profil]
* [!UICONTROL Themengruppe]
* [!UICONTROL Benutzergenehmigung]
* [!UICONTROL Benutzerdelegierung]

   * Sie können Berichte zu Benutzern erstellen, die beauftragt wurden, Aufgaben und Probleme anderer Benutzer auszuführen, während sie nicht im Büro sind. Dieser Bericht zeigt den Abwesenheitsbenutzer sowie den Benutzer an, der während seiner Abwesenheit seinen Verpflichtungen nachkommt.

* [!UICONTROL Benutzerentscheidungen]

   * Sie können berichten, wie viele Entscheidungen Benutzer im aktuellen Monat bezüglich Testsendungen und Dokumenten getroffen haben.

* [!UICONTROL Anzeigen]
* [!UICONTROL Arbeitselement] (dadurch wird ein Bericht für Aufgaben und Probleme erstellt)
