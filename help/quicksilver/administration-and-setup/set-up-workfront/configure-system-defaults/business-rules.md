---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Erstellen und Bearbeiten von Geschäftsregeln
description: Mit einer Geschäftsregel können Sie eine Validierung auf Workfront-Objekte anwenden und verhindern, dass Benutzer ein Objekt erstellen, bearbeiten oder löschen, wenn bestimmte Bedingungen erfüllt sind. Geschäftsregeln helfen bei der Verbesserung der Datenqualität und der betrieblichen Effizienz, indem sie Aktionen verhindern, die die Datenintegrität beeinträchtigen könnten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 0%

---

# Geschäftsregeln erstellen und bearbeiten

Mit einer Geschäftsregel können Sie eine Validierung auf Workfront-Objekte anwenden und verhindern, dass Benutzer ein Objekt erstellen, bearbeiten oder löschen, wenn bestimmte Bedingungen erfüllt sind. Geschäftsregeln helfen bei der Verbesserung der Datenqualität und der betrieblichen Effizienz, indem sie Aktionen verhindern, die die Datenintegrität beeinträchtigen könnten.

Eine einzelne Geschäftsregel kann nur einem Objekt zugewiesen werden. Wenn Sie beispielsweise eine Geschäftsregel erstellen, die unter bestimmten Bedingungen keine Projekte bearbeitet, können Sie nicht dieselbe Regel auf Aufgaben anwenden. Sie müssten eine separate Geschäftsregel mit denselben Bedingungen für Aufgaben erstellen.

Zugriffsebenen und die Objektfreigabe haben eine höhere Priorität als Geschäftsregeln, wenn ein Benutzer mit einem Objekt interagiert. Wenn ein Benutzer beispielsweise über eine Zugriffsebene oder -berechtigung verfügt, die die Bearbeitung eines Projekts nicht zulässt, haben diese Vorrang vor einer Geschäftsregel, die die Bearbeitung eines Projekts unter bestimmten Bedingungen zulässt.

Wenn mehr als eine Geschäftsregel auf ein Objekt angewendet wird, werden die Regeln alle befolgt, aber nicht in einer bestimmten Reihenfolge angewendet. Sie haben beispielsweise zwei Geschäftsregeln. Man beschränkt die Erstellung von Ausgaben im Februar. Das zweite verhindert die Bearbeitung eines Projekts, wenn der Projektstatus Abgeschlossen ist. Wenn ein Benutzer versucht, einem im Juni abgeschlossenen Projekt eine Ausgabe hinzuzufügen, kann die Ausgabe nicht hinzugefügt werden, da sie die zweite Regel ausgelöst hat.

Geschäftsregeln gelten für das Erstellen, Bearbeiten und Löschen von Objekten über die API sowie die Benutzeroberfläche von Workfront.

>[!NOTE]
>
>Da Geschäftsregeln bestimmte Aktionen blockieren, sollten Sie Ihre Geschäftsregeln immer zuerst in einer Sandbox- oder Vorschauumgebung konfigurieren und sie gründlich testen, bevor Sie sie in der Produktion aktivieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Abo</td> 
   <td>Ultimativ</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen auf Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Szenarien für Geschäftsregeln

Das Format einer Geschäftsregel lautet &quot;WENN die definierte Bedingung erfüllt ist, wird der Benutzer an der Aktion für das Objekt gehindert und die Nachricht wird angezeigt.&quot;

Die Syntax für die Eigenschaften und anderen Funktionen einer Geschäftsregel entspricht der Syntax für ein berechnetes Feld in einem benutzerdefinierten Formular. Weitere Informationen zur Syntax finden Sie unter [Berechnete Felder mit dem Formularentwickler hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Informationen zu IF-Anweisungen finden Sie unter [&quot;IF&quot;-Anweisungen - Übersicht](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) und [Bedingungsoperatoren in berechneten benutzerdefinierten Feldern](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Weitere Informationen zu nutzerbasierten Platzhaltern finden Sie unter [Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Informationen zu datumsbasierten Platzhaltern finden Sie unter [Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

In Geschäftsregeln ist auch ein API-Platzhalter verfügbar. Sie können `$$ISAPI` verwenden, um die Regel nur in der Benutzeroberfläche oder nur in der API Trigger.

Die Platzhalter `$$BEFORE_STATE` und `$$AFTER_STATE` werden in Ausdrücken verwendet, um vor und nach jeder Änderung auf die Feldwerte des Objekts zuzugreifen.

* Diese Platzhalter sind beide für den Trigger &quot;Bearbeiten&quot;verfügbar. Der Standardstatus für den Trigger &quot;Bearbeiten&quot;(wenn kein Status im Ausdruck enthalten ist) ist &quot;`$$AFTER_STATE`&quot;.
* Der Trigger zur Objekterstellung erlaubt nur den Wert `$$AFTER_STATE`, da der Status &quot;before&quot;nicht vorhanden ist.
* Der Trigger zum Löschen von Objekten lässt nur den Wert &quot;`$$BEFORE_STATE`&quot;zu, da der Nach-Status nicht vorhanden ist.

Einige einfache Geschäftsregelszenarien sind:

* Benutzer können in der letzten Februar-Woche keine neuen Ausgaben hinzufügen. Diese Formel könnte wie folgt lauten: `IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")`
* Benutzer können den Projektnamen eines Projekts nicht im Status Abgeschlossen bearbeiten. Diese Formel könnte wie folgt lauten: `IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")`

Ein Szenario mit verschachtelten IF-Anweisungen ist:

Benutzer können keine abgeschlossenen Projekte bearbeiten und keine Projekte mit dem geplanten Abschlussdatum im März bearbeiten. Diese Formel könnte wie folgt lauten:

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

1. Klicken Sie im linken Bereich auf **Geschäftsregeln** .
1. Klicken Sie auf **Neue Geschäftsregel**.
1. Wählen Sie den Objekttyp aus, dem die Geschäftsregel zugewiesen werden soll, und klicken Sie dann auf **Weiter**.

   ![Objekt auswählen](assets/object-for-business-rule2.png)

1. Geben Sie den **Namen** für die Geschäftsregel ein.
1. Wählen Sie im Feld **Ist aktiv** aus, ob die Regel beim Speichern aktiv sein soll.

   Wenn Sie **Nein** auswählen, wird die Regel als inaktiv gespeichert und Sie können sie später aktivieren.

1. Wählen Sie einen **Trigger** für die Geschäftsregel aus. Die Optionen sind:

   * **Bei der Objekterstellung:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu erstellen.
   * **Bei Objektbearbeitung:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu bearbeiten.
   * **Beim Löschen eines Objekts:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu löschen.

1. (Optional) Geben Sie eine **Beschreibung** der Geschäftsregel ein und geben Sie an, was passiert, wenn sie angewendet wird.
1. Erstellen Sie die Formel im Formeleditor in der Mitte des Dialogfelds &quot;Geschäftsregel&quot;.

   Das Format einer Geschäftsregel lautet &quot;WENN die definierte Bedingung erfüllt ist, wird der Benutzer an der Aktion für das Objekt gehindert und die Nachricht wird angezeigt.&quot;

   Im Formelbereich sind die von Ihnen erstellten Teile der Geschäftsregel die Bedingung und die Meldung, die in Workfront angezeigt wird, wenn die Bedingung erfüllt ist.

   * Das Objekt ist der Objekttyp, den Sie beim Erstellen der Geschäftsregel ausgewählt haben. Sie wird in der Überschrift des Dialogfelds angezeigt.
   * Die Aktion ist der Trigger, den Sie für die Regel ausgewählt haben: Erstellen, Bearbeiten oder Löschen des Objekts.
   * Da das Objekt und die Aktion bereits definiert sind, werden sie nicht in die Formel aufgenommen.
   * Die benutzerdefinierte Fehlermeldung wird dem Benutzer beim Trigger der Geschäftsregel angezeigt. Sie sollte klare Anweisungen dazu enthalten, was falsch gelaufen ist und wie das Problem zu beheben ist.

   ![Dialogfeld &quot;Geschäftsregel hinzufügen&quot;](assets/add-business-rule-dialog-no-ai-button.png)

   Dieses Beispiel ist eine Geschäftsregel für Ausgaben. Wenn der aktuelle Monat Juni ist, dürfen Benutzer keine neuen Ausgaben erstellen, was in der Nachricht erläutert wird.

   Weitere Beispiele für Geschäftsregeln finden Sie unter [Szenarien für Geschäftsregeln](#scenarios-for-business-rules) in diesem Artikel.

1. (Optional) Verwenden Sie die Formel **Ausdrücke** und **Felder** im rechten Bereich, um beim Erstellen der Regel behilflich zu sein.

   Suchen Sie nach einem Ausdruck oder Feld, um die Liste der verfügbaren Elemente einzuschränken.

   Die Liste der verfügbaren Felder ist auf Felder beschränkt, die sich auf den Objekttyp für die Geschäftsregel beziehen.

1. Klicken Sie auf **Speichern** , wenn Sie mit dem Erstellen der Geschäftsregel fertig sind.

>[!NOTE]
>
>Nachdem Sie eine Geschäftsregel hinzugefügt haben, sollten Sie sie testen, indem Sie das zugehörige Objekt hinzufügen, bearbeiten oder löschen, um sicherzustellen, dass die Regel ordnungsgemäß angewendet wird.

## Geschäftsregel aktivieren

Wenn eine Geschäftsregel inaktiv ist, zeigt das Feld Ist aktiv in der Liste der Geschäftsregeln den Wert False an. Der Status der Regel kann nicht in der Listenansicht aktualisiert werden.

So aktivieren Sie eine Geschäftsregel:

1. Wählen Sie die Geschäftsregel in der Regelliste aus und klicken Sie auf das Symbol Bearbeiten .
1. Wählen Sie **Ja** für **Ist aktiv** im Dialogfeld für Geschäftsregeln.
1. Klicken Sie auf **Speichern**.
