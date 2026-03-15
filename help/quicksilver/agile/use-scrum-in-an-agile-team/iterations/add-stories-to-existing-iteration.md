---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Textabschnitte zu einer vorhandenen Iteration hinzufügen
description: Sie haben verschiedene Möglichkeiten, um einer Iteration Stories hinzuzufügen.
author: Courtney
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 7%

---

# Hinzufügen von Storys zu einer bestehenden Iteration

Sie können einer Iteration auf eine der folgenden Arten Stories hinzufügen:

* Aus dem Rückstand nach der Erstellung der Iteration, wie im Abschnitt [Verschieben von Storys aus dem Rückstand in eine Iteration oder [!UICONTROL Kanban] Board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) in [Verwalten des agilen Rückstands](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Von der Seite [!UICONTROL Details] des jeweiligen Vorgangs oder Problems
* Von einer Task- oder Problemliste
* Aus einem Bericht
* Von einem Dashboard aus

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf das Projekt verwalten, in dem sich die Story befindet </td> 
  </tr>
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erfahren Sie, wie sich das Hinzufügen von Storys auf die Aufgabendaten auswirkt

Wenn Sie einer Iteration eine vorhandene Aufgabe hinzufügen, werden das [!UICONTROL geplante Startdatum] und das [!UICONTROL geplante Abschlussdatum] der Aufgabe standardmäßig wie folgt festgelegt:

### Vorgang [!UICONTROL Geplantes Startdatum]

* Die Aufgabe verwendet das Startdatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL Geplantes Startdatum] festgelegt.
   * Das Projekt [!UICONTROL Geplantes Startdatum] ist *vor* oder *am* Startdatum der Iteration.

* Die Aufgabe verwendet das geplante [!UICONTROL  des Projekts] wenn:

   * Das Projekt [!UICONTROL Geplantes Startdatum] ist *nach* dem Startdatum der Iteration.

### Vorgang [!UICONTROL Geplantes Abschlussdatum]

* Die Aufgabe verwendet das Enddatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL Geplantes Abschlussdatum] festgelegt.
   * Das [!UICONTROL geplante Startdatum des Projekts] ist *vor oder am* das Startdatum der Iteration oder das [!UICONTROL geplante Abschlussdatum des Projekts] ist *vor oder am* Enddatum der Iteration.

* Der Task verwendet das [!UICONTROL geplante Abschlussdatum des Projekts], wenn:

   * Das [!UICONTROL geplante Startdatum des Projekts] ist *nach* das Startdatum der Iteration und das [!UICONTROL geplante Abschlussdatum des Projekts] ist *nach* das Enddatum der Iteration.

Sie können einzelne Scrum-Teams so konfigurieren, dass sie standardmäßig die Projektdaten und nicht die Iterationsdaten verwenden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitsaufgaben zu einer Iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) im Artikel [Scrum konfigurieren](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Hinzufügen einer Story zu einer vorhandenen Iteration

Sie können jeder Iteration eine beliebige Aufgabe oder ein beliebiges Problem hinzufügen, wenn Sie über Verwaltungszugriff auf das Projekt verfügen. Beachten Sie beim Verschieben einer Aufgabe oder eines Problems in eine Iteration Folgendes:

* Wenn Sie mehrere Teams hinzufügen, kann die Aufgabe oder das Problem nur in der Iteration eines Teams angezeigt werden. Dies ist die Iteration, die Sie in Schritt 3 unten auswählen.
* Wenn die Aufgabe oder das Problem einem agilen Team zugewiesen und in die Iteration eines anderen Teams verschoben wurde, ändert sich die Teamzuweisung nicht.
* Wenn die Aufgabe oder das Problem nicht einem Team zugewiesen ist, wird die Aufgabe oder das Problem dem Team zugewiesen, das Eigentümer der Iteration ist.
* Sie können der Iteration keine übergeordneten Aufgaben hinzufügen. Wenn Sie untergeordnete Aufgaben hinzufügen, wird die übergeordnete Aufgabe auf dem Scrum-Board als Übersichtshilfe angezeigt.

>[!IMPORTANT]
>
>Nachdem die Aufgabe in die Iteration verschoben wurde, können Sie die [!UICONTROL Dauerart] oder die [!UICONTROL Aufgabenbeschränkung] nicht aktualisieren. [!UICONTROL Der Typ der Dauer] ist auf [!UICONTROL Einfach] und [!UICONTROL Die Aufgabeneinschränkung] auf [!UICONTROL Feste Termine] festgelegt, um die Zeitleiste der Aufgabe mit der Zeitleiste der Iteration konsistent zu halten.

1. Öffnen Sie die Aufgabe oder das Problem, die bzw. das Sie einer Iteration hinzufügen möchten.
oder
Wechseln Sie zum Projekt, Bericht oder Dashboard, das die Aufgabe oder das Problem enthält, die bzw. das Sie einer Iteration hinzufügen möchten. Wählen Sie dann eine oder mehrere Aufgaben oder Probleme aus.

1. Klicken Sie auf **[!UICONTROL Mehr]** ![Mehr-Symbol](assets/more-icon.png) > **[!UICONTROL Zu Iteration hinzufügen]**.
Nicht-agilen Teams können keine Aufgaben oder Probleme zugewiesen werden.

1. Beginnen Sie im Feld **[!UICONTROL Hinzufügen zu]** mit der Eingabe des Namens der Iteration und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können eine Story von einer vorhandenen Iteration in eine neue Iteration verschieben.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.
