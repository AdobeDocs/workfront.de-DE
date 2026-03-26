---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Erstellen und Bearbeiten von Geschäftsregeln
description: Mit einer Geschäftsregel können Sie Validierungen auf Workfront-Objekte anwenden und Benutzer daran hindern, ein Objekt zu erstellen, zu bearbeiten oder zu löschen, wenn bestimmte Bedingungen erfüllt sind. Geschäftsregeln tragen dazu bei, die Datenqualität und die betriebliche Effizienz zu verbessern, indem sie Maßnahmen verhindern, die die Datenintegrität beeinträchtigen könnten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: c16d107d8162f77436337d0b08ea5826d5c25d83
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 5%

---

# Geschäftsregeln erstellen und bearbeiten

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

-->

Mit einer Geschäftsregel können Sie Validierungen auf Workfront-Objekte anwenden und Benutzer daran hindern, ein Objekt zu erstellen, zu bearbeiten oder zu löschen, wenn bestimmte Bedingungen erfüllt sind. Die Validierung von Geschäftsregeln hilft, die Datenqualität und die betriebliche Effizienz zu verbessern, indem Aktionen verhindert werden, die die Datenintegrität beeinträchtigen könnten.

<!--

<div class="preview">

Organizations that have the Workflow Ultimate package can also configure business rules to automate actions for the created, edited, or modified object when certain conditions are met. Available actions include sharing the object, notifying a user, or attaching a custom form to the object.  

</div>

-->

Eine einzelne Geschäftsregel kann nur einem Objekt zugewiesen werden. Wenn Sie beispielsweise eine Geschäftsregel erstellen, um Projekte unter bestimmten Bedingungen nicht zu bearbeiten, können Sie dieselbe Regel nicht auf Aufgaben anwenden. Sie müssten eine separate Geschäftsregel mit denselben Bedingungen für Aufgaben erstellen.

Zugriffsebenen und Objektfreigabe haben eine höhere Priorität als Geschäftsregeln, wenn ein Benutzer mit einem Objekt interagiert. Wenn ein Benutzer beispielsweise über eine Zugriffsebene oder Berechtigung verfügt, die die Bearbeitung eines Projekts nicht zulässt, haben diese Vorrang vor einer Geschäftsregel, die die Bearbeitung eines Projekts unter bestimmten Bedingungen zulässt.

Wenn mehr als eine Geschäftsregel auf ein Objekt angewendet wird, werden die Regeln alle befolgt, aber nicht in einer bestimmten Reihenfolge angewendet. Sie haben beispielsweise zwei Geschäftsregeln. Eine Option schränkt die Erstellung von Ausgaben im Monat Februar ein. Die zweite Option verhindert, dass ein Projekt bearbeitet wird, wenn der Projektstatus „abgeschlossen“ ist. Wenn ein(e) Benutzende(r) versucht, einem abgeschlossenen Projekt im Juni eine Ausgabe hinzuzufügen, kann die Ausgabe nicht hinzugefügt werden, da dadurch die zweite Regel ausgelöst wurde.

Geschäftsregeln gelten für das Erstellen, Bearbeiten und Löschen von Objekten sowohl über die API als auch in der Workfront-Oberfläche.

>[!NOTE]
>
>Da Geschäftsregeln bestimmte Aktionen blockieren, sollten Sie Ihre Geschäftsregeln immer zuerst in einer Sandbox- oder Vorschau-Umgebung konfigurieren und gründlich testen, bevor Sie sie in der Produktion aktivieren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Validierung der Geschäftsregel:<ul><li><p>Ultimate</p></li><li>
    <p>Workflow Ultimate</p></li></ul></p><p>Automatisierung von Geschäftsregeln:<ul><li>
    <p>Workflow Ultimate</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Szenarien für Geschäftsregeln

* [Szenarien für die Validierung von Geschäftsregeln](#scenarios-for-business-rule-validation)
* [Szenarien für die Automatisierung von Geschäftsregeln](#scenarios-for-business-rule-automation)

### Szenarien für die Validierung von Geschäftsregeln

Das Format einer Geschäftsregelvalidierung lautet: „Wenn die definierte Bedingung erfüllt ist, kann der Benutzer das Objekt nicht bearbeiten, und die Nachricht wird angezeigt.“

Die Syntax für die Eigenschaften und andere Funktionen in einer Geschäftsregel entspricht der Syntax für ein berechnetes Feld in einem benutzerdefinierten Formular. Weitere Informationen zur Syntax finden Sie unter [Hinzufügen berechneter Felder mit dem Formular-Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Weitere Informationen zu IF-Anweisungen finden Sie unter [&#x200B; „IF“-Anweisungen - &#x200B;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) und [Bedingungsoperatoren in berechneten benutzerdefinierten Feldern](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Informationen zu benutzerbasierten Platzhaltern finden Sie unter [Verwenden von benutzerbasierten Platzhaltern zum Verallgemeinern von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Weitere Informationen zu datumsbasierten Platzhaltern finden Sie unter [Verwenden von datumsbasierten Platzhaltern zum Verallgemeinern von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

Ein API-Platzhalter ist auch in Geschäftsregeln verfügbar. Verwenden Sie `$$ISAPI`, um die Regel nur in der API in Trigger zu setzen. Verwenden Sie `!$$ISAPI`, um die Regel nur in der Benutzeroberfläche durchzusetzen, und lassen Sie zu, dass Benutzer die Regel über die API umgehen.

* Beispielsweise verbietet diese Regel Benutzenden, abgeschlossene Projekte über die API zu bearbeiten. Wenn der Platzhalter nicht verwendet wurde, blockiert die Regel die Aktion sowohl in der Benutzeroberfläche als auch in der API.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

Die Platzhalter `$$BEFORE_STATE` und `$$AFTER_STATE` werden in Ausdrücken verwendet, um vor und nach jeder Bearbeitung auf die Feldwerte des Objekts zuzugreifen.

* Diese Platzhalter sind beide für den Trigger „Bearbeiten“ verfügbar. Der Standardstatus für den Bearbeitungsausdruck (wenn im Trigger kein Status enthalten ist) ist der `$$AFTER_STATE`.
* Der Trigger zur Objekterstellung lässt nur die `$$AFTER_STATE` zu, da der Status vor nicht vorhanden ist.
* Der Trigger zum Löschen von Objekten lässt nur die `$$BEFORE_STATE` zu, da der Status nach nicht vorhanden ist.

Einige einfache Szenarien für Geschäftsregeln sind:

* Benutzende können in der letzten Februarwoche keine neuen Ausgaben hinzufügen. Diese Formel könnte wie folgt angegeben werden:

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* Benutzende können den Projektnamen eines Projekts mit dem Status „Abgeschlossen“ nicht bearbeiten. Diese Formel könnte wie folgt angegeben werden:

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

Das System ermöglicht eine Geschäftsregel pro Objekt und Trigger. Beispielsweise ist eine Regel zum Bearbeiten von Triggern für Probleme zulässig. Sie können jedoch mehrere Regeln in eine Formel mit verschachtelten IF-Anweisungen aufnehmen.

Ein Szenario mit verschachtelten IF-Anweisungen ist:

Benutzende können keine abgeschlossenen Projekte bearbeiten und keine Projekte mit einem geplanten Abschlussdatum im März bearbeiten. Diese Formel könnte wie folgt angegeben werden:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```


<!--

## Scenarios for business rule automation

>[!NOTE]
>
>Your organization must have a Workflow Ultimate package to use business rule automation.

The format of a business rule automation is "IF the defined condition is met, then the selected automation is triggered."

Business rule automation formulas do not require an error message

To ensure that an automation runs whenever the selected object and action occurs, such as when a project is created, use the following formula:

```
IF(true, true)
```

To share a project only if that's project has been approved, use a formula like the following:

```
IF({status} = "APR", true)
```

You can use wildcards in business rule actions, as described in the section [Scenarios for business rule validation](#scenarios-for-business-rule-validation).

-->

## Neue Geschäftsregel hinzufügen

{{step-1-to-setup}}

1. Klicken Sie **linken** auf „Geschäftsregeln“.
1. Klicken Sie **Neue Geschäftsregel**.

1. Geben Sie **Name** für die Geschäftsregel im Dialogfeld „Regel-Builder“ ein.
1. Wählen Sie im Feld **Ist aktiv** aus, ob die Regel beim Speichern aktiv sein soll.

   Wenn Sie **Nein** auswählen, wird die Regel als inaktiv gespeichert und kann später aktiviert werden.

1. (Optional) Geben Sie eine **Beschreibung** der Geschäftsregel ein und erfahren Sie, was bei ihrer Anwendung passiert.


1. Wählen Sie den Objekttyp aus, dem die Geschäftsregel zugewiesen werden soll.

   ![Objekt auswählen](assets/object-for-business-rule4.png)

   Sie können Geschäftsregeln auf die folgenden Objekte anwenden:

   * Projekt
   * Aufgabe
   * Anfrage/Anfrage
   * Portfolio
   * Dokument
   * Programm
   * Ausgabe
   * Firma
   * Wiederholung
   * Abrechnungseintrag
   * Gruppe
   * Sonstige Ressource
   * Risiko
   * Tarifkarte
   * Zuweisung
   * Benutzerin oder Benutzer
   * Rolle
   * Stunde
   * Vorlage
   * Freizeit
   * Ressourcen-Pool
<!--
   * <span class="preview">Job role</span>
   * <span class="preview">Non-labor resource category</span>
   * <span class="preview">Resource Pool</span>
   * <span class="preview">Time Off</span>
   * <span class="preview">Hour</span>
   * <span class="preview">Staffing Plan</span>
   * <span class="preview">Template</span>
   * <span class="preview">Staffing Plan Resource</span>
   * <span class="preview">Team</span>
-->

1. Geben Sie **Name** für die Geschäftsregel im Dialogfeld „Regel-Builder“ ein.
1. Wählen Sie im Feld **Ist aktiv** aus, ob die Regel beim Speichern aktiv sein soll.

   Wenn Sie **Nein** auswählen, wird die Regel als inaktiv gespeichert und kann später aktiviert werden.

1. Wählen Sie einen **Trigger** für die Geschäftsregel aus. Die Optionen sind:

   * **Erstellt** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu erstellen.
   * **Bearbeitet** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu bearbeiten.
   * **Gelöscht** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu löschen.

1. Erstellen Sie die Formel im Formeleditor in der Mitte des Dialogfelds „Geschäftsregel“.

   Das Format einer Geschäftsregel lautet: „Wenn die definierte Bedingung erfüllt ist, kann der Benutzer die Aktion für das Objekt nicht ausführen, und die Nachricht wird angezeigt.“

   Im Bereich Formel sind die Teile der von Ihnen erstellten Geschäftsregel die Bedingung und die Meldung, die in Workfront angezeigt wird, wenn die Bedingung erfüllt ist.

   * Das „Objekt“ ist der Objekttyp, den Sie beim Erstellen der Geschäftsregel ausgewählt haben. Er wird in der Überschrift des Dialogfelds angezeigt.
   * Die „Aktion“ ist der Trigger, den Sie für die Regel ausgewählt haben: Erstellen, Bearbeiten oder Löschen des Objekts.
   * Da das -Objekt und die Aktion bereits definiert sind, schließen Sie sie nicht in die Formel ein.
   * Die benutzerdefinierte <!--<span class="preview">is included only if the rule is for validation, and </span>--> wird Benutzenden beim Trigger der Geschäftsregel angezeigt. Es sollte klare Anweisungen dazu geben, was schiefgelaufen ist und wie das Problem behoben werden kann.

     Sie können der Fehlermeldung eine statische URL hinzufügen, um eine Verknüpfung zu Dokumentationen oder anderen hilfreichen Seiten herzustellen, die Benutzern dabei helfen, ihre Aktion innerhalb der Beschränkung der Regel zu ändern.

     In diesem Beispiel wird „Weitere Informationen“ mit der URL verknüpft. `"You are not allowed to add a new project in November.[Learn more](http://url)"` Die URL muss in Klammern stehen, aber Link-Text in Klammern ist nicht erforderlich. Sie können die vollständige URL anzeigen. Dabei handelt es sich um einen anklickbaren Link.

   ![Dialogfeld „Geschäftsregel hinzufügen](assets/add-business-rule-dialog-no-ai-button.png) <!--UPDATE ME-->

   Dieses Beispiel ist eine Geschäftsregel für Projekte. Wenn der aktuelle Monat November ist, dürfen Benutzer keine neuen Projekte erstellen. Die Meldung erklärt dies.

   Weitere Beispiele für Geschäftsregeln finden Sie unter [Szenarien für &#x200B;](#scenarios-for-business-rules) in diesem Artikel.

1. (Optional) Verwenden Sie die Formel **Ausdrücke** und **Felder** im rechten Bedienfeld, um beim Erstellen der Regel zu helfen.

   Suchen Sie nach einem Ausdruck oder Feld, um die Liste der verfügbaren Elemente einzugrenzen.

   Die Liste der verfügbaren Felder ist auf Felder beschränkt, die sich auf den Objekttyp der Geschäftsregel beziehen.

1. (Bedingt) Wenn Sie die Aktion validieren möchten, wenn Ihr Unternehmen das Workfront Ultimate-Paket nutzt, wählen Sie im Bereich Dann **Objekt validieren** aus.

   Für andere Pakete ist diese Option vorausgewählt.

<!--

1. (Conditional) To automate another action,, select the action. 

   For details on these actions, see the section [Business rule automation options](#business-rule-automation-options) in this article.

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

   -->

1. Klicken Sie **Speichern** wenn Sie mit dem Erstellen der Geschäftsregel fertig sind.

>[!NOTE]
>
>Nachdem Sie eine Geschäftsregel hinzugefügt haben, sollten Sie sie testen, indem Sie das zugehörige Objekt hinzufügen, bearbeiten oder löschen, um sicherzustellen, dass die Regel ordnungsgemäß angewendet wird.

<!--

<div class="preview">

### Business rule automation options

   >[!NOTE]
   >
   >Your organization must be on the Workflow Ultimate package to use actions besides validation. If you do not see these other options, your organization is not on the Workflow Ultimate package.

You can set these actions to automate when the business rule is triggered. Available actions depend on the selected object type.

|Automation|Further configuration|
|---|---|
|Attach a custom form|Select the custom form that you want to add|
|Share the object|Select the people, roles, groups, companies, or access levels that you want to share the object with.|

-->

## Aktivieren einer Geschäftsregel

Wenn eine Geschäftsregel inaktiv ist, wird im Feld Ist Aktiv in der Liste der Geschäftsregeln False angezeigt. Sie können den Status der Regel in der Listenansicht nicht aktualisieren.

So aktivieren Sie eine Geschäftsregel:

1. Wählen Sie die Geschäftsregel in der Regelliste aus und klicken Sie auf das Symbol Bearbeiten .
1. Wählen Sie **Ja** für **Ist Aktiv** im Dialogfeld „Geschäftsregel“ aus.
1. Klicken Sie auf **Speichern**.
