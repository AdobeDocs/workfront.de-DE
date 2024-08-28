---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Hinzufügen von Meldungen zu einer vorhandenen Iteration
description: Sie können einer Iteration auf vielerlei Weise Geschichten hinzufügen.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# Hinzufügen von Meldungen zu einer vorhandenen Iteration

Sie können einer Iteration auf eine der folgenden Arten Meldungen hinzufügen:

* Aus dem Rückprotokoll nach der Erstellung der Iteration, wie im Abschnitt [Meldungen aus dem Rückstadium in eine Iteration verschieben oder [!UICONTROL Kanban]-Pinnwand](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) in [Verwalten des agilen Backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) beschrieben

* Auf der Seite [!UICONTROL Details] der einzelnen Aufgabe oder des Problems
* Von der Aufgaben- oder Problemliste
* Berichte
* Über ein Dashboard

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erfahren Sie, wie sich das Hinzufügen von Meldungen auf Aufgabendaten auswirkt

Wenn Sie einer Iteration eine vorhandene Aufgabe hinzufügen, werden das [!UICONTROL geplante Startdatum] und das [!UICONTROL geplante Abschlussdatum] der Aufgabe standardmäßig wie folgt festgelegt:

### Aufgabe [!UICONTROL Vorgesehenes Startdatum]

* Die Aufgabe verwendet das Startdatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL Geplantes Startdatum] festgelegt.
   * Das [!UICONTROL geplante Startdatum des Projekts] ist *vor* oder *auf* das Startdatum der Iteration.

* Die Aufgabe verwendet das [!UICONTROL geplante Startdatum] des Projekts, wenn:

   * Das geplante Startdatum des Projekts [!UICONTROL  ist ] nach dem Startdatum der Iteration *.*

### Aufgabe [!UICONTROL Geplantes Abschlussdatum]

* Die Aufgabe verwendet das Enddatum der Iteration, wenn:

   * Für das Projekt ist kein [!UICONTROL geplantes Abschlussdatum] festgelegt.
   * Das [!UICONTROL geplante Startdatum des Projekts] ist *vor oder am* dem Startdatum der Iteration oder das geplante Abschlussdatum des Projekts [!UICONTROL 5} ist *vor oder am* dem Enddatum der Iteration.]

* Die Aufgabe verwendet das [!UICONTROL geplante Abschlussdatum] des Projekts, wenn

   * Das geplante Startdatum des Projekts [!UICONTROL  ist ] *nach* dem Startdatum der Iteration und das geplante Abschlussdatum des Projekts [!UICONTROL 5} ist *nach* dem Enddatum der Iteration.]

Sie können einzelne Scrum-Teams so konfigurieren, dass die Projektdaten standardmäßig anstelle der Iterationsdaten verwendet werden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren, wie Daten angewendet werden, wenn Arbeitselemente zu einer Iteration hinzugefügt werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Hinzufügen einer Geschichte zu einer vorhandenen Iteration

Sie können jede Aufgabe oder jedes Problem zu jeder Iteration hinzufügen, wenn Sie Zugriff auf das Projekt verwalten haben. Beachten Sie beim Verschieben einer Aufgabe oder eines Problems in eine Iteration Folgendes:

* Wenn Sie mehrere Teams hinzufügen, kann die Aufgabe oder das Problem nur bei der Iteration eines Teams angezeigt werden. Dies ist die Iteration, die Sie in Schritt 3 unten auswählen.
* Wenn die Aufgabe oder das Problem einem agilen Team zugewiesen und in die Iteration eines anderen Teams verschoben wird, ändert sich die Teamzuweisung nicht.
* Wenn die Aufgabe oder das Problem nicht einem Team zugewiesen ist, wird die Aufgabe bzw. das Problem dem Team zugewiesen, dem die Iteration gehört.
* Sie können der Iteration keine übergeordneten Aufgaben hinzufügen. Wenn Sie untergeordnete Aufgaben hinzufügen, wird die übergeordnete Aufgabe auf der Scrum-Pinnwand als Swimlane angezeigt.

>[!IMPORTANT]
>
>Nachdem die Aufgabe in die Iteration verschoben wurde, können Sie die [!UICONTROL Dauer Typ] oder [!UICONTROL Aufgabenbegrenzung] nicht aktualisieren. Der [!UICONTROL Dauer-Typ] ist auf [!UICONTROL Einfach] und die [!UICONTROL Aufgabenbegrenzung] auf [!UICONTROL Feste Datumswerte] eingestellt, damit die Zeitleiste der Aufgabe mit der Timeline der Iteration konsistent bleibt.

1. Öffnen Sie die Aufgabe oder das Problem, das Sie einer Iteration hinzufügen möchten.
Oder
Gehen Sie zum Projekt, Bericht oder Dashboard, das die Aufgabe oder das Problem enthält, die/das Sie einer Iteration hinzufügen möchten. Wählen Sie dann eine oder mehrere Aufgaben oder Probleme aus.

1. Klicken Sie auf **[!UICONTROL Mehr]** ![](assets/more-icon.png) > **[!UICONTROL Zu Iteration hinzufügen]**.
Nicht agilen Teams können keine Aufgaben oder Probleme zugewiesen werden.

1. Geben Sie im Feld **[!UICONTROL Hinzufügen zu]** den Namen der Iteration ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können eine Geschichte von einer vorhandenen Iteration in eine neue Iteration verschieben.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.
