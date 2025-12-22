---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Hinzufügen von Storys zu einer vorhandenen Iteration
description: Sie haben verschiedene Möglichkeiten, um einer Iteration Stories hinzuzufügen.
author: Jenny
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 3%

---

# Hinzufügen von Storys zu einer vorhandenen Iteration

Sie können einer Iteration auf eine der folgenden Arten Stories hinzufügen:

* Aus dem Rückstand nach der Erstellung der Iteration, wie im Abschnitt [Verschieben von Storys aus dem Rückstand in eine Iteration oder [!UICONTROL Kanban] Board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) in [Verwalten des agilen Rückstands](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Auf der [!UICONTROL Details]-Seite der einzelnen Aufgabe oder Anfrage
* Aus einer Aufgaben- oder Problemliste
* Aus einem Bericht
* Aus einem Dashboard

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
   <td>Zugriff auf das Projekt verwalten, an dem sich die Story befindet </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## verstehen, wie sich das Hinzufügen von Storys auf Aufgabendaten auswirkt

Wenn Sie eine vorhandene Aufgabe zu einer Iteration hinzufügen, werden standardmäßig das [!UICONTROL Geplantes Startdatum] und [!UICONTROL Geplantes Abschlussdatum] der Aufgabe wie folgt festgelegt:

### Aufgabe [!UICONTROL geplantes Startdatum]

* Die Aufgabe verwendet das Startdatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL Geplantes Startdatum] festgelegt.
   * Das Projekt [!UICONTROL Geplantes Startdatum] ist *vor* oder *am* Startdatum der Iteration.

* Die Aufgabe verwendet das geplante [!UICONTROL &#x200B; des Projekts] wenn:

   * Das Projekt [!UICONTROL Geplantes Startdatum] ist *nach* dem Startdatum der Iteration.

### Aufgabe [!UICONTROL Geplantes Abschlussdatum]

* Die Aufgabe verwendet das Enddatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL Geplantes Abschlussdatum“ &#x200B;].
   * Das Projekt [!UICONTROL Geplantes Startdatum] liegt *vor oder am* dem Startdatum der Iteration oder das [!UICONTROL Geplantes Abschlussdatum] des Projekts liegt *vor oder* dem Enddatum der Iteration.

* Die Aufgabe verwendet das &quot;[!UICONTROL &#x200B; Abschlussdatum“ des Projekts] wenn:

   * Das Projekt [!UICONTROL Geplantes Startdatum] ist *nach* dem Startdatum der Iteration und das [!UICONTROL Geplantes Abschlussdatum] des Projekts ist *nach* Enddatum der Iteration.

Sie können einzelne Scrum-Teams so konfigurieren, dass sie standardmäßig die Projektdaten und nicht die Iterationsdaten verwenden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Hinzufügen einer Story zu einer vorhandenen Iteration

Sie können jeder Iteration eine beliebige Aufgabe oder ein beliebiges Problem hinzufügen, wenn Sie über Verwaltungszugriff auf das Projekt verfügen. Beachten Sie beim Verschieben einer Aufgabe oder eines Problems in eine Iteration Folgendes:

* Wenn Sie mehrere Teams hinzufügen, kann die Aufgabe oder das Problem nur in der Iteration eines Teams angezeigt werden. Dies ist die Iteration, die Sie in Schritt 3 unten auswählen.
* Wenn die Aufgabe oder das Problem einem agilen Team zugewiesen und in die Iteration eines anderen Teams verschoben wird, ändert sich die Team-Zuweisung nicht.
* Wenn die Aufgabe oder das Problem keinem Team zugewiesen ist, wird die Aufgabe oder das Problem dem Team zugewiesen, dem die Iteration gehört.
* Sie können der Iteration keine übergeordneten Aufgaben hinzufügen. Wenn Sie untergeordnete Aufgaben hinzufügen, wird die übergeordnete Aufgabe auf dem Scrum-Board als Verantwortlicher angezeigt.

>[!IMPORTANT]
>
>Nachdem die Aufgabe in die Iteration verschoben wurde, können Sie den [!UICONTROL Dauertyp] oder die [!UICONTROL Aufgabenbeschränkung] nicht aktualisieren. [!UICONTROL Dauertyp] wird auf [!UICONTROL Einfach] und [!UICONTROL Aufgabenbeschränkung] auf [!UICONTROL Feste Datumswerte] festgelegt, um die Zeitleiste der Aufgabe konsistent mit der Zeitleiste der Iteration zu halten.

1. Öffnen Sie die Aufgabe oder das Problem, das Sie einer Iteration hinzufügen möchten.
oder
Wechseln Sie zum Projekt, Bericht oder Dashboard, das die Aufgabe oder das Problem enthält, die bzw. das Sie einer Iteration hinzufügen möchten. Wählen Sie dann eine oder mehrere Aufgaben oder Probleme aus.

1. Klicken Sie auf **[!UICONTROL Mehr]** ![Mehr-Symbol](assets/more-icon.png) > **[!UICONTROL Zu Iteration hinzufügen]**.
Nicht-agilen Teams können keine Aufgaben oder Probleme zugewiesen werden.

1. Beginnen Sie im Feld **[!UICONTROL Hinzufügen zu]** mit der Eingabe des Namens der Iteration und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können eine Story von einer vorhandenen Iteration in eine neue Iteration verschieben.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.
