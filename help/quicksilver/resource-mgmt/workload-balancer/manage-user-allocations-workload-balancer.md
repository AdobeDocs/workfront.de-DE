---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Verwalten von Benutzerzuweisungen im Workload Balancer
description: Als Ressourcen-Manager können Sie Benutzern Arbeit zuweisen und ihre täglichen, wöchentlichen oder monatlichen Zuweisungen über den Workload-Balancer verwalten.
author: Lisa
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '2898'
ht-degree: 0%

---

# Verwalten von Benutzerzuweisungen im Workload Balancer

<!-- Audited: 01/2024 -->

Als Ressourcen-Manager können Sie Benutzern Arbeit zuweisen und ihre täglichen, wöchentlichen oder monatlichen Zuweisungen über den Workload-Balancer verwalten, um sicherzustellen, dass sie eine Stundenmenge zugewiesen bekommen, die zu ihren verfügbaren Zeitplänen passt.

## Zugriffsanforderungen {#access-requirements}

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan, wenn der Workload Balancer im Bereich „Ressourcen“ verwendet wird</br>
       Arbeit bei Verwendung des Workload Balancer eines Teams oder Projekts</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes bearbeiten:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen oder höher, die Zuweisungen an die Aufgaben und Probleme enthalten, für die Sie Zuweisungen verwalten möchten. </p> <p>Oder </p> <p>Verwalten Sie zusätzlich zur Aktualisierung der Zuweisungen Berechtigungen für die Aufgaben, für die Sie die geplanten Stunden aktualisieren möchten. Informationen zum Aktualisieren der geplanten Stunden im Workload Balancer finden Sie im Abschnitt <a href="#update-task-planned-hours-when-managing-user-allocations">Aktualisieren der geplanten Stunden bei der Verwaltung </a> Benutzerzuweisungen) in diesem Artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerzuweisungen verstehen

Benutzerzuweisungen sind Stundenbeträge, die die Zeit angeben, die ein Benutzer an einem bestimmten Tag oder Wochentag, einer bestimmten Woche oder einem bestimmten Monat verbringen soll, um das Arbeitselement abzuschließen. Sie sind in den geplanten Stunden des Arbeitselements enthalten.

In diesem Artikel wird beschrieben, wie Sie die täglichen, wöchentlichen oder monatlichen stündlichen Zuweisungen für Benutzende aktualisieren, die Aufgaben oder Problemen zugewiesen sind. Informationen zum Verwalten der Gesamtzuweisungen für Benutzer und Aufgabengebiete für Aufgaben finden Sie unter [Verwalten der Stunden für die Zuordnung von Benutzern und Rollen für Aufgaben](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

### Übersicht über die Benutzerzuordnung {#user-allocation-overview}

Sie können die Benutzerzuordnung im Workload-Balancer als Stunden oder als Prozentwert anzeigen. Sie können Stunden oder Prozentsätze anpassen.

Benutzerzuweisungen sind in der Anzahl der geplanten Stunden eines Arbeitselements enthalten. Informationen zu den geplanten Stunden finden Sie unter [Übersicht über die geplanten Stunden](../../manage-work/tasks/task-information/planned-hours.md).

Die für die Aufgabe geplanten Stunden werden für den Benutzer, der der Aufgabe zugewiesen ist, gleichmäßig auf alle Tage innerhalb der Aufgabendauer verteilt. Wenn eine Aufgabe beispielsweise eine Dauer von 5 Tagen und insgesamt 10 geplanten Stunden hat, beträgt die Anzahl der täglichen Zuweisungen für die Aufgabe 2 Stunden. Die wöchentliche Zuteilung beträgt 10 Stunden. Das bedeutet, dass ein(e) Benutzende(r) zwei Stunden pro Tag für die Arbeit an der Aufgabe zugewiesen ist. Sie können jedoch die tägliche Zuordnung für den Benutzer manuell über den Workload-Balancer ändern.

>[!CAUTION]
>
>Der Workload Balancer zeigt nur bis zu 1.000 geplante Stunden pro Arbeitselement und bis zu 1.000 Tage der Dauer eines Elements an. Die Zuordnungen im Workload Balancer werden als Null angezeigt, nachdem das Limit von 1.000 Stunden oder 1.000 Tagen erreicht wurde. Es wird empfohlen, Aufgaben in kleinere Teilaufgaben zu unterteilen, um eine größere Anzahl geplanter Stunden oder für eine Dauer von mehr als 1000 Tagen aufzunehmen.

Beachten Sie Folgendes, wenn Sie im Workload Balancer tägliche, wöchentliche oder monatliche Zuweisungen für Aufgaben oder Probleme finden:

* Sie können die tägliche, wöchentliche und monatliche Zuordnung der Benutzer zu ihren Arbeitselementen anzeigen. Aktivieren Sie die Wochen- oder Monatsansicht, um die wöchentlichen oder monatlichen Zuweisungen anzuzeigen.
* Mit dem Workload Balancer können Sie die tägliche, wöchentliche oder monatliche Zuordnung der Benutzer zu den Aufgaben oder Problemen ändern. Informationen zum Anpassen der Ansicht des Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  >[!NOTE]
  >
  >Es wird empfohlen, zu entscheiden, welchen Zeitrahmen (täglich, wöchentlich oder monatlich) Sie bei der Verwaltung von Benutzerzuweisungen immer verwenden möchten, und nicht zwischen ihnen für dieselben Arbeitselemente zu wechseln. Durch die Aktualisierung der wöchentlichen Zuweisungen für denselben Benutzer, für den Sie zuvor die täglichen Zuweisungen aktualisiert haben, wird die tägliche Zuordnung für den Benutzer geändert.

* Sie können Zuordnungen für Arbeits- und arbeitsfreie Tage aktualisieren.
* Die Zeitstempel für das geplante Start- und Abschlussdatum der Arbeitselemente sowie der Zeitplan des Projekts sind wichtig, wenn Workfront die tägliche Zuordnung für die Aufgabe automatisch berechnet.

  >[!INFO]
  >
  > Eine Aufgabe kann beispielsweise eine Dauer von 2 Tagen und 2 geplanten Stunden haben und sie hat eine geplante Startzeit von 12:00 Uhr am ersten Tag der Dauer mit einem Benutzer und einem Projektplan, der um 17 Uhr endet. Die Kapazität des Benutzers für den ersten Tag beträgt 5 Stunden. Die Kapazität des Benutzers für den zweiten Tag beträgt 8 Stunden (wenn der Zeitplan um 9 Uhr morgens beginnt).
  >
  >Workfront berechnet die Zuordnung der 2 Stunden für die 2 Tage der Dauer anhand der folgenden Formel:
  >
  >`Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours`
  >
  >In unserem Beispiel sind die täglichen Zuordnungsstunden für jeden Tag:
  >   
  >(2 / 13) * 5 = 0,77 Stunden für den ersten Tag
  >
  >(2 / 13) * 8 = 1,23 Zuteilungsstunden für den zweiten Tag
  >
  >In den obigen Berechnungen entspricht 13 der insgesamt verfügbaren Stunden für die Aufgabe: 5 + 8 = 13

* Zwei Benutzer in unterschiedlichen Zeitzonen oder Zeitplänen in unterschiedlichen Zeitzonen als die der zugewiesenen Benutzer können dazu führen, dass die Zuordnungsbeträge für zwei Benutzer, die dieselben Arbeitselemente anzeigen, unterschiedlich aussehen.

* Wenn ein(e) Benutzende(r) eine Ausfallzeit eingeplant hat, wird der Tag oder der Teil des Tages in einem grauen Hintergrund angezeigt und ein Flugzeugsymbol zeigt die Ausfallzeit an. Wenn der Workfront-Administrator bzw. die Benutzerin die Einstellung „Ausfallzeit“ im Bereich „Setup“ aktiviert hat, um die Ausfallzeit des/der Benutzenden zu berücksichtigen, werden die zugewiesenen Stunden auf den nächsten verfügbaren Tag in der Timeline verschoben. Wenn die Einstellung deaktiviert ist, bleiben die zugewiesenen Stunden an dem Tag, der als Ausfallzeit markiert ist, und der Benutzer wird als überlastet angezeigt. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!TIP]
  >
  >Wenn die Ausfallzeit markiert wurde, nachdem der Benutzer einem Arbeitselement zugewiesen wurde, müssen Sie die Timeline des Projekts neu berechnen, um die verschobene Zuordnung anzuzeigen. Weitere Informationen finden Sie unter [Neuberechnen von Projektzeitleisten](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   * Wenn einer Aufgabe mehrere Benutzer zugewiesen sind und der primäre Zugewiesene Ausfallzeiten geplant hat, wird die Zeitleiste verschoben (wenn die Daten nicht fest sind) und die geplanten Stunden aller Zugewiesenen werden über die neue Dauer der Aufgabe neu verteilt. Wenn die Aufgabe feste Termine hat, wird die Zeitleiste aufgrund der Ausfallzeit nicht geändert und die Stunden werden den verbleibenden Tagen neu zugewiesen.
   * Wenn Zuweisungen manuell vorgenommen werden, werden die geplanten Stunden nach der Ausfallzeit nicht neu zugewiesen.

* Wenn der Aufgabe mehrere Benutzer zugewiesen sind, wird der Betrag der geplanten Stunden zuerst gleichmäßig auf jeden Benutzer und dann gleichmäßig auf jeden Tag innerhalb der Aufgabendauer verteilt. Diese Verteilung wird zur Zuordnung jedes Benutzers zur Aufgabe.

  Beispielsweise können die folgenden Szenarien vorhanden sein:

   * Für eine Aufgabe mit einer Dauer von 2 Tagen und mit 10 geplanten Stunden, die einem Benutzer zugewiesen sind, beträgt die tägliche Zuweisung für den Benutzer standardmäßig 5 Stunden für jeden Tag.
   * Für eine Aufgabe mit einer Dauer von 2 Tagen und mit zwei Benutzern zugewiesenen 10 geplanten Stunden beträgt die tägliche Zuweisung für jeden Benutzer standardmäßig 2,5 Stunden für jeden Tag.

* Wenn eine Aufgabe oder ein Problem vor dem geplanten Abschlussdatum abgeschlossen wurde, wird die Anzahl der zugewiesenen Stunden für die verbleibenden Tage durchgestrichen und nicht auf die Gesamtzuweisung des Benutzers angerechnet. Dies wird nur angezeigt, wenn sowohl das Symbol Zuteilungen anzeigen als auch die Einstellung Prognostiziertes Datum anzeigen aktiviert sind. Weitere Informationen zum Aktivieren der Einstellungen im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Zugeordnete Stunden durchgestrichen](assets/allocations-struck-through-highlighted.png)

* Wenn eine Benutzerin oder ein Benutzer überlastet ist, werden die zugewiesenen Stunden mit einem roten Hintergrund im Benutzerfeld angezeigt.
* Wenn der/die Benutzende nicht ausgelastet ist oder der geplanten verfügbaren Zeit gleich viele Stunden zugewiesen sind, werden die Stunden mit blauem Hintergrund angezeigt.
* Sie können die Zuordnung der Benutzer in einer Diagrammansicht in der Benutzerzeile anzeigen. Informationen zum Aktivieren der Diagrammansicht für Benutzerzuweisungen finden Sie im Abschnitt „Navigieren im Workload Balancer“ im Artikel [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Benutzerzuordnungsdiagramm](assets/user-allocation-chart.png)

### Kriterien zum Zurücksetzen von Benutzerzuweisungen {#criteria-that-reset-user-allocations}

Nicht alle Aufgabenänderungen ändern den Trigger der geänderten Zuteilungen, die umverteilt werden sollen. Es gibt jedoch bestimmte Aktionen, die die bereits angepassten Zuweisungen für Ihre Ressourcen zurücksetzen und sie gleichmäßig auf alle Tage während der Dauer des Arbeitselements für jeden der Zugewiesenen verteilen können.

>[!NOTE]
>
>Wenn Sie die automatische Verteilung der Zuweisungen für Arbeitselemente nicht geändert haben, werden die Stunden gleichmäßig auf alle Bevollmächtigten verteilt, wenn sich die Anzahl der Bevollmächtigten, die Dauer einer Aufgabe oder die Anzahl der für das Arbeitselement geplanten Stunden ändert.

#### Aktionen zum Zurücksetzen angepasster Zuweisungen {#actions-that-reset-adjusted-allocations}

Die folgenden Aktionen setzen die täglichen, wöchentlichen oder monatlichen Zuweisungen für Benutzer zurück oder ändern sie, nachdem Sie sie manuell angepasst haben, wie im Abschnitt [Ändern von Benutzerzuweisungen](#modify-user-allocations) in diesem Artikel beschrieben:

* Wenn Sie die Länge eines Arbeitselements verkürzen, was die Anzahl der Tage in seiner Dauer verkürzt, werden die angepassten zugeordneten Stunden aus den verlorenen Tagen zum Zuordnungsbetrag des letzten Tages des Arbeitselements hinzugefügt.
* Wenn Sie die Anzahl der geplanten Stunden für eine Zuordnung oder für ein Arbeitselement ändern, wird die neue Anzahl der geplanten Stunden gleichmäßig über die gesamte Dauer des Arbeitselements neu verteilt.
* Wenn Sie einen Verantwortlichen zu einem Arbeitselement hinzufügen oder daraus entfernen und dies dazu führt, dass sich die geplanten Stunden der Aufgabe ändern, werden die angepassten Werte gleichmäßig verteilt.

#### Aktionen, die die angepassten Zuweisungen nicht zurücksetzen {#actions-that-do-not-reset-adjusted-allocations}

Die folgenden Änderungen an einem Arbeitselement führen nicht zum Trigger der angepassten Zuordnungen, die zurückgesetzt oder geändert werden sollen:

* Wenn Sie die Tage eines Arbeitselements verschieben, die Anzahl der Tage in der Dauer sich jedoch nicht ändert, bleiben die angepassten zugeordneten Werte unverändert und wechseln zu den neuen Datumsangaben.
* Wenn Sie die Dauer eines Arbeitselements erhöhen, was die Anzahl der Tage in seiner Dauer erhöht, bleiben die angepassten zugeordneten Stunden für die angepassten Tage gleich. Zusätzliche Tage werden dem Arbeitselement mit 0 zugewiesenen Stunden hinzugefügt.
* Wenn Sie einen Verantwortlichen zu einem Arbeitselement hinzufügen oder entfernen und dies nicht dazu führt, dass sich die geplanten Stunden des Elements ändern, bleiben die angepassten Werte unverändert.

## Suchen nach „Geplante Stunden“ im Workload Balancer

Sie können mithilfe des Workload-Balancers die Zuordnung von Benutzern zu Aufgaben oder Problemen ändern, indem Sie nach den geplanten Stunden der Aufgaben oder Probleme suchen, die Benutzern zugewiesen wurden.

Beachten Sie beim Anzeigen geplanter Stunden im Workload Balancer Folgendes:

* Die Gesamtzahl der geplanten Stunden für eine Aufgabe oder ein Problem wird neben dem Namen der Aufgabe oder des Problems auf der linken Seite des Workload-Balancer angezeigt.

* Die Gesamtzahl der geplanten Stunden für ein Projekt wird neben dem Projektnamen links im Workload Balancer angezeigt. Dies stellt die Gesamtzahl der geplanten Stunden für alle Aufgaben und Probleme dar, die unter dem Projekt im Workload Balancer aufgelistet sind, und nicht alle geplanten Stunden des Projekts.
* Die Zeit, die täglich oder wöchentlich für alle Aufgaben und für alle Projekte zugewiesen wurde, wird nur angezeigt, wenn Sie die Einstellung „Zuteilungen anzeigen“ manuell aktivieren. Informationen zum Aktivieren der Einstellungen im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Benutzerzuweisungen ändern {#modify-user-allocations}

Im Rahmen der Zuweisung von Arbeit zu Benutzenden können Sie Benutzerzuweisungen im Workload Balancer ändern, um sicherzustellen, dass sie nie überlastet werden, oder um einen genauen Ausgleich der Stunden zwischen Ihren Ressourcen sicherzustellen. Informationen dazu, wie Sie feststellen können, ob eine Benutzerzuordnung überlastet ist, finden Sie im Abschnitt [Übersicht über die Benutzerzuordnung](#user-allocation-overview) in diesem Artikel.

1. Stellen Sie sicher, dass den Benutzern Aufgaben und Probleme zugewiesen sind. Informationen zum Zuweisen von Arbeit zu Benutzern im Workload Balancer finden Sie unter [Übersicht über das Zuweisen von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Navigieren Sie zum Workload Balancer.
1. (Optional) Klicken Sie auf **Woche** oder **Monat**, um die wöchentlichen oder monatlichen Zuweisungen für Benutzer zu verwalten.

   ![Woche oder Monat auswählen](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. Suchen Sie im Bereich **Zugewiesene Arbeit** den Benutzer, für den Sie die Zuordnung manuell ändern möchten, und klicken Sie auf den nach rechts zeigenden Pfeil links neben dem Benutzernamen, um den Benutzer zu erweitern.

   ![Benutzer erweitern](assets/wb-highlight-on-name-caret2.png)

1. Klicken Sie auf den nach rechts zeigenden Pfeil links neben dem Projektnamen, um das Projekt zu erweitern und die Arbeitselemente anzuzeigen, denen der Benutzer zugewiesen ist.

   >[!TIP]
   >
   >Benutzerzuweisungen können nur für Aufgaben und Probleme geändert werden. Benutzerzuweisungen für Projekte können nicht geändert werden.

1. (Optional) Klicken Sie auf das Symbol **Zuordnungen anzeigen**, ![](assets/show-allocations-icon-small.png) Zuordnungen für alle Arbeitselemente anzuzeigen.

   Der Name der Aufgaben und der Projekte wird durch die Zuordnung des Benutzers für die Aufgabe oder das Projekt ersetzt.

1. (Optional) Klicken Sie auf **Symbol** Einstellungen![](assets/gear-icon-settings.png) und wählen Sie eine der folgenden Optionen aus:

   1. **Stunden aus Problemen einbeziehen**. Auf diese Weise können Sie zusätzlich zur Aufgabenzuweisung auch Problemzuweisungen verwalten.
   1. **Abgeschlossene Arbeiten anzeigen**. Hier werden Elemente angezeigt, die abgeschlossen wurden und während der Zeitleiste geplant sind, für die Sie Zuweisungen verwalten.
   1. **Verbleibende Zeit anzeigen**. Die Gesamtstundenzahl für jeden Benutzer (in der Benutzerzeile) ändert sich. Wenn diese Einstellung aktiviert ist, zeigt der Workload Balancer die Stunden an, die den einzelnen Benutzenden für Arbeit zur Verfügung stehen, anstatt die Anzahl der Stunden, für die sie zugewiesen sind.

      >[!TIP]
      >
      >Wenn Zuteilungen geändert werden, wenn diese Einstellung aktiviert ist, verringert sich die Gesamtzahl in der Benutzerzeile.

   1. **Projekt** im Abschnitt **Farbschema auswählen**. Dadurch werden jedes Projekt und die entsprechenden Arbeitselemente in eindeutigen Farben angezeigt und es wird leichter zu verstehen, welche Elemente zu welchem Projekt gehören.
   1. **Prozentsatz** im Abschnitt **Benutzerzuordnung anzeigen in**. Dadurch werden die Zuteilungen als Prozentwert angezeigt. Die Kapazität des Benutzers gemäß dem Zeitplan wird als 100 % betrachtet. Wenn beispielsweise ein Benutzer einem Zeitplan von 8 Stunden pro Tag zugeordnet ist, entspricht 8 Stunden 100 % Kapazität. Wenn Sie dem Benutzer die Arbeit von 4 Stunden pro Tag zuweisen möchten, aktualisieren Sie seine Zuordnung auf 50 %.

      >[!NOTE]
      >
      >Der Workfront-Administrator entscheidet, welcher Zeitplan für die Berechnung der Benutzerkapazität im gesamten System im Bereich Ressourcenverwaltung unter „Setup“ verwendet werden soll. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Klicken Sie auf **Mehr**-![](assets/qs-more-menu.png) für ein Arbeitselement und dann auf **Zuweisungen bearbeiten**.

   ![Mehr Menü für Arbeitselement](assets/more-menu-on-task-wb-nwe.png)

   Oder

   Doppelklicken Sie auf den Tag, die Woche oder den Monat in der Leiste einer Aufgabe oder eines Problems.

   Die Zuordnungsfelder können nun bearbeitet werden.

1. Klicken Sie in das Feld jeder täglichen, wöchentlichen oder monatlichen Zuordnung, um die Anzahl der Stunden oder den Prozentwert, für die der Benutzer pro Tag, Woche oder Monat zugewiesen werden soll, manuell zu aktualisieren, und klicken Sie dann auf das Symbol **Speichern** ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Klicken Sie auf das **Abbrechen**-Symbol ![](assets/cancel-allocations-wb.png), um die angepassten Zuordnungen zu entfernen.

   ![Speichern oder Abbrechen angepasster Zuweisungen](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   Die Zuweisungen für die Benutzeraktualisierung.

   >[!TIP]
   >
   >Wenn eine Aufgabe oder ein Problem vor dem geplanten Abschlussdatum abgeschlossen wurde, wird die Anzahl der zugewiesenen Stunden für die verbleibenden Tage durchgestrichen und nicht auf die Gesamtzuweisung des Benutzers angerechnet. Dies wird nur angezeigt, wenn sowohl das **Zuteilungen anzeigen** als auch die Einstellung **Prognostiziertes Datum anzeigen** aktiviert sind.

   Die folgenden Szenarien sind vorhanden:

   * Bei Aufgaben mit nicht einfachen Dauertypen oder bei Problemen muss die Gesamtzuordnung den geplanten Stunden für die Aufgabe entsprechen, bevor Sie auf das Häkchen klicken können.
   * Bei Aufgaben mit dem Typ Einfache Dauer kann die Summe der Zuordnungen höher oder niedriger als die geplanten Stunden sein, und Sie können auf das Häkchen klicken, selbst wenn sie nicht übereinstimmen. Dadurch wird auch die Anzahl der geplanten Stunden für die Aufgabe aktualisiert. Sie müssen über die richtigen Berechtigungen und Zugriffsrechte verfügen, um die geplanten Stunden für Aufgaben über den Workload-Balancer zu aktualisieren.

     >[!TIP]
     >
     >Rechts neben dem Aufgabennamen wird ein Sperrsymbol angezeigt, wenn Sie mit der Anpassung Ihrer Zuordnungen beginnen, um anzugeben, dass die Aufgabe einen einfachen Dauertyp aufweist.

     ![Sperrsymbol](assets/lock-icon-on-simple-task-in-the-balancer.png)

   Weitere Informationen zu den Bedingungen, die erfüllt sein müssen, um die geplanten Stunden im Workload Balancer zu aktualisieren, finden Sie im Abschnitt [Aktualisieren der geplanten Stunden bei der Verwaltung ](#update-task-planned-hours-when-managing-user-allocations) Benutzerzuweisungen) in diesem Artikel. Informationen zu den Aufgabendauer-Typen finden Sie [Übersicht über die Aufgabendauer und den ](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)).

1. (Bedingt) Wenn die Aufgabe mehr als einem Benutzer zugewiesen ist, wiederholen Sie diese Schritte für jeden Benutzer, der der Aufgabe zugewiesen ist, um die Zuordnungen für jeden Benutzer zu aktualisieren.

   Jeder, der Zugriff auf den Workload Balancer hat und dieselben Benutzer und dieselben Projekte anzeigt, die Sie verwaltet haben, zeigt jetzt die aktualisierte Zuordnung für die von Ihnen verwalteten Benutzer an.

>[!TIP]
>
>Rechts neben dem Namen des Arbeitselements wird ein Stiftsymbol angezeigt, das angibt, dass es manuell angepasst wurde.

![Symbol für manuell angepasste Stunden](assets/icon-for-manually-adjusted-hours.png)

## Geplante Stunden für Aufgabe bei der Verwaltung von Benutzerzuweisungen aktualisieren {#update-task-planned-hours-when-managing-user-allocations}

Sie können die geplanten Stunden einer Aufgabe aktualisieren, wenn Sie die Benutzerzuweisungen im Workload-Balancer für die Aufgabe verwalten. Dies geschieht, wenn die Summe der aktualisierten zugeordneten Stunden nicht mit der ursprünglichen Summe der geplanten Stunden für eine Aufgabe übereinstimmt.

>[!IMPORTANT]
>
>* Die Aktualisierung der geplanten Stunden für Aufgaben kann sich auf den Fortschritt Ihres Projekts auswirken.
>* Die manuelle Aktualisierung der geplanten Stunden durch Änderung der täglichen Zuweisungen kann sich auf die geplanten Stunden auswirken, wenn Zuweisungen künftig aus den Aufgaben entfernt werden. Weitere Informationen finden Sie unter [Übersicht über geplante Stunden](../../manage-work/tasks/task-information/planned-hours.md).
>
>* Es ist nicht möglich, die geplanten Stunden für Probleme zu aktualisieren, indem Zuteilungen im Workload-Balancer aktualisiert werden.

Dies ist möglich, wenn die folgenden Bedingungen vorliegen:

* Sie verfügen über die richtigen Berechtigungen und Zugriffsrechte, um geplante Stunden über den Workload-Balancer zu verwalten. Dazu gehören die folgenden:

   * Verwalten Sie die Berechtigungen für die Aufgaben.
   * Aktualisieren Sie die geplanten Stunden im Zugriff auf den Workload Balancer im Bereich „Ressourcenverwaltung“ Ihrer Zugriffsebene.

  Weitere Informationen zum Zugriff, der für die Verwendung des Workload Balancer erforderlich ist, finden Sie [ Abschnitt &quot;](#access-requirements)&quot; in diesem Artikel.

* Die Aufgabe hat den Dauertyp „Einfach“.

