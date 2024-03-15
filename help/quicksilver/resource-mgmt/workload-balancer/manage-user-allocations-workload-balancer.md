---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Verwalten von Benutzerzuordnungen im Lastenausgleich
description: Als Ressourcen-Manager können Sie Benutzern Arbeit zuweisen und ihre täglichen, wöchentlichen oder monatlichen Zuordnungen über den Arbeitslastausgleich verwalten.
author: Lisa
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '2859'
ht-degree: 0%

---

# Verwalten von Benutzerzuordnungen im Lastenausgleich

<!-- Audited: 01/2024 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Als Ressourcen-Manager können Sie Benutzern Arbeit zuweisen und ihre täglichen, wöchentlichen oder monatlichen Zuordnungen über den Arbeitslastausgleich verwalten, um sicherzustellen, dass ihnen eine Anzahl von Stunden zugewiesen wird, die in ihre verfügbaren Zeitpläne passen.

## Zugriffsanforderungen {#access-requirements}

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Bei Verwendung des Lastenausgleichs im Bereich "Ressourcen"benötigen Sie:</p>
   <p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Plan</p>
   <p>Wenn Sie den Lastenausgleich eines Teams oder Projekts verwenden, benötigen Sie Folgendes:</p>
   <p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Arbeit</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Aufgaben</p> </li> 
     <li> <p>Probleme</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Fügen Sie Berechtigungen oder höher hinzu, die Zuweisen zu den Aufgaben und Problemen enthalten, für die Sie Zuordnungen verwalten möchten. </p> <p>Oder </p> <p>Verwalten Sie Berechtigungen für die Aufgaben, für die Sie zusätzlich zur Aktualisierung der Zuordnungen die geplanten Stunden aktualisieren möchten. Informationen zum Aktualisieren der geplanten Stunden im Arbeitslastausgleich finden Sie in der <a href="#update-task-planned-hours-when-managing-user-allocations">Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen</a> in diesem Artikel beschrieben.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Grundlegendes zu Benutzerzuordnungen

Benutzerzuweisungen sind Stunden, die die Zeit angeben, die ein Benutzer an einem bestimmten Tag, Wochentag, Woche oder Monat verbringen soll, um das Arbeitselement abzuschließen. Sie sind in den geplanten Stunden des Arbeitselements enthalten.

In diesem Artikel wird beschrieben, wie Sie die tägliche, wöchentliche oder monatliche stündliche Zuordnung für Benutzer aktualisieren, die Aufgaben oder Problemen zugewiesen sind. Informationen zum Verwalten der Gesamtzuweisungen für Benutzer und Auftragsrollen für Aufgaben finden Sie unter [Verwalten von Benutzer- und Rollenzuordnungsstunden für Aufgaben](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

### Übersicht über die Benutzerzuordnung {#user-allocation-overview}

Sie können die Benutzerzuordnung als Stunden oder als Prozentwert im Lastenausgleich anzeigen. Sie können Stunden oder Prozentsätze anpassen.

Benutzerzuweisungen sind in der Anzahl der geplanten Stunden eines Arbeitselements enthalten. Weitere Informationen zu geplanten Stunden finden Sie unter [Übersicht über geplante Stunden](../../manage-work/tasks/task-information/planned-hours.md).

Die geplante Aufgabe wird gleichmäßig auf alle Tage innerhalb der Aufgabendauer des der Aufgabe zugewiesenen Benutzers verteilt. Wenn eine Aufgabe beispielsweise eine Dauer von 5 Tagen und insgesamt 10 geplante Stunden hat, beträgt die Anzahl der täglichen Zuweisungen für die Aufgabe 2 Stunden. Die wöchentliche Zuordnung beträgt 10 Stunden. Das bedeutet, dass ein Benutzer für die Arbeit an der Aufgabe für 2 Stunden pro Tag zugewiesen wird. Sie können die tägliche Zuordnung für den Benutzer jedoch mithilfe des Lastenausgleichs manuell ändern.

>[!CAUTION]
>
>Der Lastenausgleich zeigt nur bis zu 1000 geplante Stunden pro Arbeitselement pro Benutzer und bis zu 1000 Tage von der Dauer eines Artikels an. Die Zuordnungen im Lastenausgleich werden nach Erreichen der Beschränkung von 1000 Stunden oder 1000 Tagen als null angezeigt. Es wird empfohlen, Aufgaben in kleinere Unteraufgaben zu unterteilen, um eine größere Anzahl von geplanten Stunden oder für längeren Aufenthalt von mehr als 1000 Tagen aufzunehmen.

Beachten Sie Folgendes bei der Suche nach täglichen, wöchentlichen oder monatlichen Zuweisungen für Aufgaben oder Probleme im Arbeitslastausgleich:

* Sie können die täglichen, wöchentlichen und monatlichen Zuordnungen der Benutzer zu ihren Arbeitselementen anzeigen. Aktivieren Sie die Wochen- oder Monatsansicht, um wöchentliche oder monatliche Zuordnungen anzuzeigen.
* Sie können den Lastenausgleich verwenden, um die tägliche, wöchentliche oder monatliche Zuordnung der Benutzer zu den Aufgaben oder Problemen zu ändern. Informationen zum Anpassen der Ansicht des Lastenausgleichs finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  >[!NOTE]
  >
  >Es wird empfohlen, bei der Verwaltung von Benutzerzuordnungen immer zu entscheiden, welchen Zeitraum (täglich, wöchentlich oder monatlich) Sie verwenden möchten, und nicht für dieselben Arbeitselemente zwischen ihnen zu wechseln. Durch die Aktualisierung der wöchentlichen Zuordnungen für denselben Benutzer, für den Sie zuvor die tägliche Zuordnung aktualisiert haben, wird die tägliche Zuordnung für den Benutzer geändert.

* Sie können die Zuordnungen für Arbeits- und Nichtarbeitstage aktualisieren.
* Die Zeitstempel für die geplanten Start- und Abschlussdaten der Arbeitselemente sowie der Zeitplan des Projekts sind wichtig, wenn Workfront die tägliche Zuweisung für die Aufgabe automatisch berechnet.

  >[!INFO]
  >
  > Eine Aufgabe kann beispielsweise eine Dauer von 2 Tagen und 2 geplanten Stunden haben und eine geplante Startzeit von 22:00 Uhr am ersten Tag der Dauer mit einem Benutzer und einen Projektplan, der um 17:00 Uhr endet, hat. Die Kapazität des Benutzers für den ersten Tag beträgt 5 Stunden. Die Kapazität des Benutzers für den zweiten Tag beträgt 8 Stunden (wenn der Zeitplan um 9 Uhr beginnt).
  >
  >Workfront berechnet die Zuweisung der 2 Stunden über die 2 Tage der Laufzeit mithilfe der folgenden Formel:
  >
  >`Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours`
  >
  >Die täglichen Zuordnungszeiten für jeden Tag in unserem Beispiel lauten:
  >   
  >(2 / 13) * 5 = 0,77 Zuordnungsstunden für den ersten Tag
  >
  >(2 / 13) * 8 = 1,23 Zuordnungsstunden für den zweiten Tag
  >
  >In den obigen Berechnungen ist 13 die Gesamtanzahl der für die Aufgabe verfügbaren Stunden: 5 + 8 = 13

* Zwei Benutzer in unterschiedlichen Zeitzonen oder Zeitplänen in unterschiedlichen Zeitzonen als die der zugewiesenen Benutzer können dazu führen, dass die Zuordnungsmengen für zwei Benutzer, die dieselben Arbeitselemente anzeigen, unterschiedlich angezeigt werden.

* Wenn ein Benutzer eine geplante Zeitüberschreitung festgelegt hat, wird der Tag oder der Teil des Tages in einem grauen Hintergrund angezeigt. Wenn der Workfront-Administrator die Einstellung Benutzerzeit deaktivieren im Bereich Einrichtung aktiviert hat, um die Zeitüberschreitung des Benutzers zu berücksichtigen, werden die zugewiesenen Stunden zum nächsten verfügbaren Tag in der Timeline verschoben. Wenn die Einstellung deaktiviert ist, bleiben die zugewiesenen Stunden am Tag, der für eine Zeitverzögerung markiert ist, und der Benutzer wird als übergeordnet angezeigt. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!TIP]
  >
  >Wenn die Zeit nach der Zuweisung des Benutzers zu einem Arbeitselement markiert wurde, müssen Sie die Timeline des Projekts neu berechnen, um die verschobene Zuordnung anzuzeigen. Weitere Informationen finden Sie unter [Projektzeitpläne neu berechnen](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* Wenn der Aufgabe mehrere Benutzer zugewiesen sind, wird die Anzahl der geplanten Stunden zunächst gleichmäßig an jeden Benutzer verteilt und dann gleichmäßig auf jeden Tag innerhalb der Dauer der Aufgabe. Diese Verteilung wird zur Zuordnung jedes Benutzers zur Aufgabe.

  Die folgenden Szenarien können beispielsweise existieren:

   * Für eine Aufgabe mit einer Dauer von 2 Tagen und 10 geplanten Stunden, die einem Benutzer zugewiesen ist, beträgt die tägliche Zuweisung für den Benutzer standardmäßig 5 Stunden pro Tag.
   * Für eine Aufgabe mit einer Dauer von 2 Tagen und 10 geplanten Stunden, die zwei Benutzern zugewiesen ist, beträgt die tägliche Zuweisung für jeden Benutzer standardmäßig 2,5 Stunden pro Tag.

* Wenn eine Aufgabe oder ein Problem vor dem geplanten Abschlussdatum abgeschlossen wurde, wird die Anzahl der zugewiesenen Stunden für die verbleibenden Tage erreicht und nicht in die Gesamtzuordnung des Benutzers einbezogen. Dies wird nur angezeigt, wenn sowohl das Symbol Zuordnungen anzeigen als auch die Einstellung Vorgeschlagene Daten anzeigen aktiviert sind. Weitere Informationen zum Aktivieren von Einstellungen im Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Zugewiesene Stunden](assets/allocations-struck-through-highlighted.png)

* Wenn ein Benutzer übergeordnet ist, werden die zugewiesenen Stunden im Benutzerfeld mit einem roten Hintergrund angezeigt.
* Wenn der Benutzer die geplante verfügbare Zeit nicht oder nicht über die gleiche Anzahl von Stunden verfügt, werden die Stunden mit blauem Hintergrund angezeigt.
* Sie können die Zuordnung der Benutzer in einer Diagrammansicht in der Benutzerzeile anzeigen. Informationen zum Aktivieren der Diagrammansicht für Benutzerzuordnungen finden Sie im Abschnitt &quot;Navigieren im Arbeitslastausgleich&quot;im Artikel [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Benutzerzuordnungsdiagramm](assets/user-allocation-chart.png)

### Kriterien für das Zurücksetzen der Benutzerzuordnungen {#criteria-that-reset-user-allocations}

Nicht alle Aufgaben ändern den Trigger der geänderten Zuordnungen zur Neuverteilung. Es gibt jedoch bestimmte Aktionen, die die bereits angepassten Zuweisungen für Ihre Ressourcen zurücksetzen und gleichmäßig auf alle Tage während der Dauer des Arbeitselements für jeden der Verantwortlichen verteilen könnten.

>[!NOTE]
>
>Wenn Sie die automatische Verteilung der Zuweisungen für Arbeitselemente nicht geändert haben, verteilen sich die Stunden gleichmäßig auf alle zugewiesenen Benutzer, wenn sich die Anzahl der Bevollmächtigten, die Dauer einer Aufgabe oder die Anzahl der geplanten Stunden für das Arbeitselement ändern.

#### Aktionen, die angepasste Zuordnungen zurücksetzen {#actions-that-reset-adjusted-allocations}

Die folgenden Aktionen setzen die täglichen, wöchentlichen oder monatlichen Zuordnungen für Benutzer zurück oder ändern sie, nachdem Sie sie manuell angepasst haben, wie im Abschnitt [Ändern der Benutzerzuordnungen](#modify-user-allocations) in diesem Artikel:

* Wenn Sie die Länge eines Arbeitselements verkürzen, das die Anzahl der Tage in seiner Dauer verkürzt, werden die angepassten zugewiesenen Stunden aus den verlorenen Tagen zum Zuordnungsbetrag des letzten Tages des Arbeitselements hinzugefügt.
* Wenn Sie die Anzahl der geplanten Stunden für einen Auftrag oder das Arbeitselement ändern, verteilt sich die neue Anzahl geplanter Stunden gleichmäßig für die gesamte Dauer des Arbeitselements.
* Wenn Sie einen Verantwortlichen zu einem Arbeitselement hinzufügen oder entfernen und dies dazu führt, dass sich die geplanten Stunden der Aufgabe ändern, werden die angepassten Werte gleichmäßig verteilt.

#### Aktionen, die die angepassten Zuweisungen nicht zurücksetzen {#actions-that-do-not-reset-adjusted-allocations}

Die folgenden Änderungen an einem Arbeitselement haben keinen Trigger auf die angepassten Zuordnungen zum Zurücksetzen oder Ändern:

* Wenn Sie die Tage eines Arbeitselements verschieben, sich die Anzahl der Tage in der Dauer jedoch nicht ändert, bleiben die angepassten zugewiesenen Werte unverändert und wechseln zu den neuen Daten.
* Wenn Sie die Dauer eines Arbeitselements erhöhen, durch das die Anzahl der Tage in seiner Dauer erhöht wird, bleiben die angepassten zugewiesenen Stunden für die angepassten Tage unverändert. Dem Arbeitselement werden zusätzliche Tage mit 0 zugewiesenen Stunden hinzugefügt.
* Wenn Sie einen Verantwortlichen zu einem Arbeitselement hinzufügen oder entfernen und dies nicht dazu führt, dass sich die geplanten Stunden des Elements ändern, bleiben die angepassten Werte gleich.

## Suchen Sie geplante Stunden im Arbeitslastausgleich.

Sie können die Benutzerzuordnungen zu Aufgaben oder Problemen mithilfe des Workload Balancer ändern, indem Sie die geplanten Stunden der Aufgaben oder Probleme suchen, die Benutzern zugewiesen sind.

Beachten Sie Folgendes bei der Anzeige der geplanten Stunden im Arbeitslastausgleich:

* Die Gesamtanzahl der geplanten Stunden für eine Aufgabe oder ein Problem wird links neben dem Aufgaben- oder Problemnamen auf dem Arbeitslastverteiler angezeigt.

* Die Gesamtanzahl der geplanten Stunden für ein Projekt wird neben dem Projektnamen auf der linken Seite des Workload Balancer angezeigt. Dies entspricht der Gesamtzahl der geplanten Stunden für alle Aufgaben und Probleme, die im Projekt im Lastenausgleich aufgeführt sind, und nicht für alle geplanten Stunden des Projekts.
* Die tägliche oder wöchentliche Zeitdauer für alle Aufgaben und für alle Projekte wird nur angezeigt, wenn Sie die Einstellung Zuordnungen anzeigen manuell aktivieren. Informationen zum Aktivieren von Einstellungen im Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ändern der Benutzerzuordnungen {#modify-user-allocations}

Im Rahmen der Zuweisung von Arbeit an Benutzer können Sie die Benutzerzuweisungen im Arbeitslasten-Balancer ändern, um sicherzustellen, dass sie nie überverteilt werden, oder um einen präzisen Zeitausgleich zwischen Ihren Ressourcen sicherzustellen. Informationen dazu, wie Sie erkennen, ob ein Benutzer übergeordnet ist, finden Sie im Abschnitt . [Übersicht über die Benutzerzuordnung](#user-allocation-overview) in diesem Artikel.

1. Stellen Sie sicher, dass Benutzern Aufgaben und Probleme zugewiesen sind. Informationen zum Zuweisen von Arbeit zu Benutzern im Lastenausgleich finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Wechseln Sie zum Lastenausgleich.
1. (Optional) Klicken Sie auf **Woche** oder **Monat** um wöchentliche oder monatliche Zuordnungen für Benutzer zu verwalten.

   ![Woche oder Monat auswählen](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. Im **Zugewiesene Arbeit** suchen Sie den Benutzer, für den Sie die Zuordnung manuell ändern möchten, und klicken Sie auf den Pfeil nach rechts neben dem Benutzernamen, um den Benutzer zu erweitern.

   ![Benutzer erweitern](assets/wb-highlight-on-name-caret2.png)

1. Klicken Sie auf den Rechtspfeil links neben dem Projektnamen, um das Projekt zu erweitern und die Arbeitselemente anzuzeigen, denen der Benutzer zugewiesen ist.

   >[!TIP]
   >
   >Sie können die Benutzerzuordnungen nur für Aufgaben und Probleme ändern. Sie können die Benutzerzuordnungen für Projekte nicht ändern.

1. (Optional) Klicken Sie auf die **Zuordnungen anzeigen** icon ![](assets/show-allocations-icon-small.png) , um Zuordnungen für alle Arbeitselemente anzuzeigen.

   Der Name der Aufgaben und der Projekte wird durch die Zuordnung des Benutzers für die Aufgabe oder das Projekt ersetzt.

1. (Optional) Klicken Sie auf die **Einstellungen** icon ![](assets/gear-icon-settings.png) und eine der folgenden Optionen auswählen:

   1. **Stunden aus Problemen einschließen**. Auf diese Weise können Sie neben der Aufgabenzuordnung auch Problemzuweisungen verwalten.
   1. **Fertige Arbeiten anzeigen**. Auf diese Weise werden Elemente angezeigt, die abgeschlossen und während der Zeitleiste geplant wurden, für die Sie Zuordnungen verwalten.
   1. **Restzeit anzeigen**. Die Gesamtanzahl der Stunden für jeden Benutzer (in der Benutzerzeile) ändert sich. Wenn diese Einstellung aktiviert ist, zeigt der Lastenausgleich die Stunden an, die jeder Benutzer für die Arbeit zur Verfügung hat, anstatt die Anzahl der Stunden, für die er zugewiesen ist.

      >[!TIP]
      >
      >Wenn Sie Zuordnungen ändern, wenn diese Einstellung aktiviert ist, wird die Gesamtanzahl der Benutzer verringert.

   1. **Projekt** im **Farbschema auswählen** Abschnitt. Dadurch werden jedes Projekt und seine jeweiligen Arbeitselemente in einzigartigen Farben angezeigt und es wird leichter zu verstehen, welche Elemente zu welchem Projekt gehören.
   1. **Prozentsatz** im **Anzeigen der Benutzerzuordnung in** Abschnitt. Dadurch werden Zuordnungen als Prozentwert angezeigt. Die Kapazität des Benutzers gemäß der Planung wird als 100 % betrachtet. Wenn beispielsweise ein Benutzer mit einem Zeitplan von 8 Stunden pro Tag verknüpft ist, entspricht 8 Stunden einer Kapazität von 100 %. Wenn Sie den Benutzer 4 Stunden am Tag für die Arbeit freigeben möchten, aktualisieren Sie seine Zuordnung auf 50 %.

      >[!NOTE]
      >
      >Der Workfront-Administrator entscheidet, welcher Zeitplan in Ihrem gesamten System zur Berechnung der Benutzerkapazität im Bereich &quot;Ressourcenverwaltung&quot;der Einrichtung verwendet werden soll. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-menu.png) für ein Arbeitselement klicken Sie dann auf **Zuordnungen bearbeiten**.

   ![Mehr Menü für Arbeitselemente](assets/more-menu-on-task-wb-nwe.png)

   Oder

   Doppelklicken Sie auf den Tag, die Woche oder den Monat in der Leiste einer Aufgabe oder eines Problems.

   Die Zuordnungsfelder werden bearbeitbar.

1. Klicken Sie in das Feld jeder täglichen, wöchentlichen oder monatlichen Zuordnung, um die Anzahl der Stunden oder den Prozentwert, denen der Benutzer pro Tag, Woche oder Monat zugewiesen werden soll, manuell zu aktualisieren, und klicken Sie dann auf die **Speichern** icon ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Klicken Sie auf **Abbrechen** icon ![](assets/cancel-allocations-wb.png) um die von Ihnen angepassten Zuordnungen zu entfernen.

   ![Angepasste Zuteilungen speichern oder abbrechen](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   Die Zuordnungen für die Benutzeraktualisierung.

   >[!TIP]
   >
   >Wenn eine Aufgabe oder ein Problem vor dem geplanten Abschlussdatum abgeschlossen wurde, wird die Anzahl der zugewiesenen Stunden für die verbleibenden Tage erreicht und nicht in die Gesamtzuordnung des Benutzers einbezogen. Dies wird nur angezeigt, wenn beide **Zuordnungen anzeigen** und dem **Vorgeschlagene Daten anzeigen** -Einstellung aktiviert ist.

   Die folgenden Szenarien existieren:

   * Bei Aufgaben mit nicht einfachen Typen für die Dauer oder bei Problemen muss die Gesamtanzahl der Zuweisungen mit der Aufgabe Geplante Stunden übereinstimmen, bevor Sie auf das Häkchen klicken können.
   * Bei Aufgaben mit dem Typ Einfache Dauer kann die Gesamtanzahl der Zuweisungen höher oder niedriger als die geplanten Stunden sein. Sie können auch dann auf das Häkchen klicken, wenn sie nicht übereinstimmen. Dadurch wird auch die Anzahl der geplanten Stunden für die Aufgabe aktualisiert. Sie müssen über die richtigen Berechtigungen und Zugriffsrechte verfügen, um geplante Stunden für Aufgaben über den Workload Balancer zu aktualisieren.

     >[!TIP]
     >
     >Ein Sperrsymbol wird rechts neben dem Aufgabennamen angezeigt, wenn Sie mit der Anpassung Ihrer Zuordnungen beginnen, um anzugeben, dass die Aufgabe über einen einfachen Dauerhaltungstyp verfügt.

     ![Sperrsymbol](assets/lock-icon-on-simple-task-in-the-balancer.png)

   Weitere Informationen zu den Bedingungen, die für die Aktualisierung der geplanten Stunden im Arbeitslastausgleich erfüllt werden müssen, finden Sie im Abschnitt [Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen](#update-task-planned-hours-when-managing-user-allocations) in diesem Artikel beschrieben. Weitere Informationen zu Aufgabendauer finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Bedingt) Wenn die Aufgabe mehr als einem Benutzer zugewiesen ist, wiederholen Sie diese Schritte für jeden Benutzer, der der Aufgabe zugewiesen ist, um die Zuordnungen für jeden Benutzer zu aktualisieren.

   Jeder, der Zugriff auf den Lastenausgleich hat und dieselben Benutzer und Projekte anzeigt, die Sie verwaltet haben, sieht nun die aktualisierte Zuordnung für die von Ihnen verwalteten Benutzer.

>[!TIP]
>
><span class="preview">Rechts neben dem Namen des Arbeitselements wird ein Stiftsymbol angezeigt, um anzugeben, dass es manuell angepasst wurde.</span>

![Symbol &quot;Manuell angepasste Stunden&quot;](assets/icon-for-manually-adjusted-hours.png)

## Aktualisierung der geplanten Aufgaben bei der Verwaltung der Benutzerzuordnungen {#update-task-planned-hours-when-managing-user-allocations}

Sie können die geplanten Stunden einer Aufgabe aktualisieren, wenn Sie die Benutzerzuweisungen im Arbeitslastausgleich für die Aufgabe verwalten. Dies geschieht, wenn die Summe der aktualisierten zugewiesenen Stunden nicht mit der ursprünglichen Gesamtsumme der geplanten Stunden für eine Aufgabe übereinstimmt.

>[!IMPORTANT]
>
>* Das Aktualisieren der geplanten Stunden für Aufgaben kann sich auf den Fortschritt Ihres Projekts auswirken.
>* Eine manuelle Aktualisierung der geplanten Stunden durch Änderung der täglichen Zuordnung kann sich auf die geplanten Stunden auswirken, wenn Zuweisungen aus den Aufgaben in der Zukunft entfernt werden. Weitere Informationen finden Sie unter [Übersicht über geplante Stunden](../../manage-work/tasks/task-information/planned-hours.md).
>
>* Es ist nicht möglich, geplante Stunden für Probleme zu aktualisieren, indem die Zuordnungen im Arbeitslastausgleich aktualisiert werden.

Dies ist möglich, wenn die folgenden Bedingungen erfüllt sind:

* Sie verfügen über die richtigen Berechtigungen und Zugriffsrechte, um geplante Stunden über den Lastenausgleich zu verwalten. Dazu gehören die folgenden:

   * Verwalten Sie Berechtigungen für die Aufgaben.
   * Aktualisieren Sie die geplanten Stunden im Zugriff auf den Lastenausgleich im Bereich Ressourcenverwaltung Ihrer Zugriffsebene.

  Weitere Informationen zum Zugriff, der für die Verwendung des Workload-Balancers erforderlich ist, finden Sie unter [Zugriffsanforderungen](#access-requirements) in diesem Artikel beschrieben.

* Die Aufgabe verfügt über den Typ Einfache Dauer .

