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
source-git-commit: b6731b9877237916259a862863b30c8ef65ad343
workflow-type: tm+mt
source-wordcount: '1318'
ht-degree: 2%

---

# Geschäftsregeln erstellen und bearbeiten

Mit einer Geschäftsregel können Sie Validierungen auf Workfront-Objekte anwenden und Benutzer daran hindern, ein Objekt zu erstellen, zu bearbeiten oder zu löschen, wenn bestimmte Bedingungen erfüllt sind. Geschäftsregeln tragen dazu bei, die Datenqualität und die betriebliche Effizienz zu verbessern, indem sie Maßnahmen verhindern, die die Datenintegrität beeinträchtigen könnten.

Eine einzelne Geschäftsregel kann nur einem Objekt zugewiesen werden. Wenn Sie beispielsweise eine Geschäftsregel erstellen, um Projekte unter bestimmten Bedingungen nicht zu bearbeiten, können Sie dieselbe Regel nicht auf Aufgaben anwenden. Sie müssten eine separate Geschäftsregel mit denselben Bedingungen für Aufgaben erstellen.

Zugriffsebenen und Objektfreigabe haben eine höhere Priorität als Geschäftsregeln, wenn ein Benutzer mit einem Objekt interagiert. Wenn ein Benutzer beispielsweise über eine Zugriffsebene oder Berechtigung verfügt, die die Bearbeitung eines Projekts nicht zulässt, haben diese Vorrang vor einer Geschäftsregel, die die Bearbeitung eines Projekts unter bestimmten Bedingungen zulässt.

Wenn mehr als eine Geschäftsregel auf ein Objekt angewendet wird, werden die Regeln alle befolgt, aber nicht in einer bestimmten Reihenfolge angewendet. Sie haben beispielsweise zwei Geschäftsregeln. Eine Option schränkt die Erstellung von Ausgaben im Monat Februar ein. Die zweite Option verhindert, dass ein Projekt bearbeitet wird, wenn der Projektstatus „abgeschlossen“ ist. Wenn ein(e) Benutzende(r) versucht, einem abgeschlossenen Projekt im Juni eine Ausgabe hinzuzufügen, kann die Ausgabe nicht hinzugefügt werden, da dadurch die zweite Regel ausgelöst wurde.

Geschäftsregeln gelten für das Erstellen, Bearbeiten und Löschen von Objekten sowohl über die API als auch in der Workfront-Oberfläche.

>[!NOTE]
>
>Da Geschäftsregeln bestimmte Aktionen blockieren, sollten Sie Ihre Geschäftsregeln immer zuerst in einer Sandbox- oder Vorschau-Umgebung konfigurieren und gründlich testen, bevor Sie sie in der Produktion aktivieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Ultimate</p>
    <p>Workflow Ultimate</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Szenarien für Geschäftsregeln

Das Format einer Geschäftsregel lautet: „Wenn die definierte Bedingung erfüllt ist, kann der Benutzer die Aktion für das Objekt nicht ausführen, und die Nachricht wird angezeigt.“

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

## Neue Geschäftsregel hinzufügen

{{step-1-to-setup}}

1. Klicken Sie **linken** auf „Geschäftsregeln“.
1. Klicken Sie **Neue Geschäftsregel**.
1. Wählen Sie den Objekttyp aus, dem die Geschäftsregel zugewiesen werden soll, und klicken Sie dann auf **Weiter**.

   ![Objekt auswählen](assets/object-for-business-rule3.png)

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

1. Geben Sie **Name** für die Geschäftsregel im Dialogfeld „Regel-Builder“ ein.
1. Wählen Sie im Feld **Ist aktiv** aus, ob die Regel beim Speichern aktiv sein soll.

   Wenn Sie **Nein** auswählen, wird die Regel als inaktiv gespeichert und kann später aktiviert werden.

1. Wählen Sie einen **Trigger** für die Geschäftsregel aus. Die Optionen sind:

   * **Bei der Objekterstellung:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu erstellen.
   * **Bei Objektbearbeitung:** Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu bearbeiten.
   * **Beim Löschen eines Objekts:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu löschen.

1. (Optional) Geben Sie eine **Beschreibung** der Geschäftsregel ein und erfahren Sie, was bei ihrer Anwendung passiert.
1. Erstellen Sie die Formel im Formeleditor in der Mitte des Dialogfelds „Geschäftsregel“.

   Das Format einer Geschäftsregel lautet: „Wenn die definierte Bedingung erfüllt ist, kann der Benutzer die Aktion für das Objekt nicht ausführen, und die Nachricht wird angezeigt.“

   Im Bereich Formel sind die Teile der von Ihnen erstellten Geschäftsregel die Bedingung und die Meldung, die in Workfront angezeigt wird, wenn die Bedingung erfüllt ist.

   * Das „Objekt“ ist der Objekttyp, den Sie beim Erstellen der Geschäftsregel ausgewählt haben. Er wird in der Überschrift des Dialogfelds angezeigt.
   * Die „Aktion“ ist der Trigger, den Sie für die Regel ausgewählt haben: Erstellen, Bearbeiten oder Löschen des Objekts.
   * Da das -Objekt und die Aktion bereits definiert sind, schließen Sie sie nicht in die Formel ein.
   * Die benutzerdefinierte Fehlermeldung wird Benutzenden beim Trigger der Geschäftsregel angezeigt. Es sollte klare Anweisungen dazu geben, was schiefgelaufen ist und wie das Problem behoben werden kann.

     Sie können der Fehlermeldung eine statische URL hinzufügen, um eine Verknüpfung zu Dokumentationen oder anderen hilfreichen Seiten herzustellen, die Benutzern dabei helfen, ihre Aktion innerhalb der Beschränkung der Regel zu ändern.

     In diesem Beispiel wird „Weitere Informationen“ mit der URL verknüpft. `"You are not allowed to add a new project in November.[Learn more](http://url)"` Die URL muss in Klammern stehen, aber Link-Text in Klammern ist nicht erforderlich. Sie können die vollständige URL anzeigen. Dabei handelt es sich um einen anklickbaren Link.

   ![Dialogfeld „Geschäftsregel hinzufügen“](assets/add-business-rule-dialog-no-ai-button.png)

   Dieses Beispiel ist eine Geschäftsregel für Projekte. Wenn der aktuelle Monat November ist, dürfen Benutzer keine neuen Projekte erstellen. Die Meldung erklärt dies.

   Weitere Beispiele für Geschäftsregeln finden Sie unter [Szenarien für &#x200B;](#scenarios-for-business-rules) in diesem Artikel.

1. (Optional) Verwenden Sie die Formel **Ausdrücke** und **Felder** im rechten Bedienfeld, um beim Erstellen der Regel zu helfen.

   Suchen Sie nach einem Ausdruck oder Feld, um die Liste der verfügbaren Elemente einzugrenzen.

   Die Liste der verfügbaren Felder ist auf Felder beschränkt, die sich auf den Objekttyp der Geschäftsregel beziehen.

1. Klicken Sie **Speichern** wenn Sie mit dem Erstellen der Geschäftsregel fertig sind.

>[!NOTE]
>
>Nachdem Sie eine Geschäftsregel hinzugefügt haben, sollten Sie sie testen, indem Sie das zugehörige Objekt hinzufügen, bearbeiten oder löschen, um sicherzustellen, dass die Regel ordnungsgemäß angewendet wird.

## Aktivieren einer Geschäftsregel

Wenn eine Geschäftsregel inaktiv ist, wird im Feld Ist Aktiv in der Liste der Geschäftsregeln False angezeigt. Sie können den Status der Regel in der Listenansicht nicht aktualisieren.

So aktivieren Sie eine Geschäftsregel:

1. Wählen Sie die Geschäftsregel in der Regelliste aus und klicken Sie auf das Symbol Bearbeiten .
1. Wählen Sie **Ja** für **Ist Aktiv** im Dialogfeld „Geschäftsregel“ aus.
1. Klicken Sie auf **Speichern**.
