---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Erstellen und Bearbeiten von Geschäftsregeln
description: Sie können auswählen, ob Sie monatlich oder vierteljährlich neue Workfront-Funktionen erhalten möchten.
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d96ddcc2f514d9f79e94a3437a3b66e07a270abc
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Geschäftsregeln

Mit einer Geschäftsregel können Sie eine Validierung auf Workfront-Objekte anwenden und verhindern, dass Benutzer ein Objekt erstellen, bearbeiten oder löschen, wenn bestimmte Bedingungen erfüllt sind. Geschäftsregeln helfen bei der Verbesserung der Datenqualität und der betrieblichen Effizienz, indem sie Aktionen verhindern, die die Datenintegrität beeinträchtigen könnten.

Eine einzelne Geschäftsregel kann nur einem Objekt zugewiesen werden. Wenn Sie beispielsweise eine Geschäftsregel erstellen, die unter bestimmten Bedingungen keine Projekte bearbeitet, können Sie nicht dieselbe Regel auf Aufgaben anwenden. Sie müssten eine separate Geschäftsregel mit denselben Bedingungen für Aufgaben erstellen.

Zugriffsebenen und die Objektfreigabe haben eine höhere Priorität als Geschäftsregeln, wenn ein Benutzer mit einem Objekt interagiert. Wenn ein Benutzer beispielsweise über eine Zugriffsebene oder -berechtigung verfügt, die die Bearbeitung eines Projekts nicht zulässt, haben diese Vorrang vor einer Geschäftsregel, die die Bearbeitung eines Projekts unter bestimmten Bedingungen zulässt.

Eine Hierarchie existiert auch, wenn mehrere Geschäftsregeln auf ein Objekt angewendet werden. Sie haben beispielsweise zwei Geschäftsregeln. Man beschränkt die Erstellung von Ausgaben im Februar. Das zweite verhindert die Bearbeitung eines Projekts, wenn der Projektstatus Abgeschlossen ist. Wenn ein Benutzer versucht, einem im Juni abgeschlossenen Projekt eine Ausgabe hinzuzufügen, kann die Ausgabe nicht hinzugefügt werden, da sie die zweite Regel ausgelöst hat.

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Szenarien für Geschäftsregeln

Einige einfache Geschäftsregelszenarien sind:

* Benutzer können in der letzten Februar-Woche keine neuen Ausgaben hinzufügen. Diese Formel könnte wie folgt lauten: `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* Benutzer können kein Projekt bearbeiten, das sich im Status Abgeschlossen befindet. Diese Formel könnte wie folgt lauten: `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

Die Syntax zum Erstellen einer Geschäftsregel entspricht der Erstellung eines berechneten Felds in einem benutzerdefinierten Formular. Weitere Informationen zur Syntax finden Sie unter [Berechnete Felder mit dem Formularentwickler hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Weitere Informationen zu IF-Anweisungen finden Sie unter [Übersicht über &quot;IF&quot;-Anweisungen](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) und [Bedingungsoperatoren in berechneten benutzerdefinierten Feldern](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Weitere Informationen zu nutzerbasierten Platzhaltern finden Sie unter [Verwenden benutzerbasierter Platzhalter zum Generalisieren von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Informationen zu datumsbasierten Platzhaltern finden Sie unter [Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## Neue Geschäftsregel hinzufügen

{{step-1-to-setup}}

1. Klicks **Geschäftsregeln** im linken Bereich.
1. Klicks **Neue Geschäftsregel**.
1. Wählen Sie den Objekttyp aus, dem die Geschäftsregel zugewiesen werden soll, und klicken Sie dann auf **Weiter**.

   ![Auswählen eines Objekts](assets/object-for-business-rule2.png)

1. Geben Sie die **Name** für die Geschäftsregel.
1. Im **Ist aktiv** auswählen, ob die Regel beim Speichern aktiv sein soll.

   Wenn Sie **Nein**, wird die Regel als inaktiv gespeichert und Sie können sie später aktivieren.

1. Wählen Sie eine **Trigger** für die Geschäftsregel. Die Optionen sind:

   * **Bei der Objekterstellung:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu erstellen.
   * **Bei der Objektbearbeitung:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu bearbeiten.
   * **Beim Löschen eines Objekts:** Die Regel wird angewendet, wenn ein Benutzer versucht, ein Objekt zu löschen.

1. (Optional) Geben Sie einen **Beschreibung** der Geschäftsregel und was passiert, wenn sie angewendet wird.
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

1. (Optional) Die Formel verwenden **Ausdruck** und **Felder** im rechten Bereich, um beim Erstellen der Regel zu helfen.

   Suchen Sie nach einem Ausdruck oder Feld, um die Liste der verfügbaren Elemente einzuschränken.

   Die Liste der verfügbaren Felder ist auf Felder beschränkt, die sich auf den Objekttyp für die Geschäftsregel beziehen.

1. Klicks **Speichern** wenn Sie mit der Erstellung der Geschäftsregel fertig sind.

>[!NOTE]
>
>Nachdem Sie eine Geschäftsregel hinzugefügt haben, sollten Sie sie testen, indem Sie das zugehörige Objekt hinzufügen, bearbeiten oder löschen, um sicherzustellen, dass die Regel ordnungsgemäß angewendet wird.

## Geschäftsregel aktivieren

Wenn eine Geschäftsregel inaktiv ist, zeigt das Feld Ist aktiv in der Liste der Geschäftsregeln den Wert False an. Der Status der Regel kann nicht in der Listenansicht aktualisiert werden.

So aktivieren Sie eine Geschäftsregel:

1. Wählen Sie die Geschäftsregel in der Regelliste aus und klicken Sie auf das Symbol Bearbeiten .
1. Auswählen **Ja** für **Ist aktiv** im Dialog mit Geschäftsregeln.
1. Klicken Sie auf **Speichern**.
