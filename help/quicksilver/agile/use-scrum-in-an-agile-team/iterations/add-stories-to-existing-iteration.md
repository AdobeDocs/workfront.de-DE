---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Hinzufügen von Meldungen zu einer vorhandenen Iteration
description: Sie können einer Iteration auf vielerlei Weise Geschichten hinzufügen.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Hinzufügen von Meldungen zu einer vorhandenen Iteration

Sie können einer Iteration auf eine der folgenden Arten Meldungen hinzufügen:

* Aus dem Rückprotokoll nach der Erstellung der Iteration, wie im Abschnitt [Meldungen aus dem Rückstadium in eine Iteration verschieben oder [!UICONTROL Kanban]-Pinnwand](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) in [Verwalten des agilen Backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) beschrieben

* Auf der Seite [!UICONTROL Details] der einzelnen Aufgabe oder des Problems
* Von der Aufgaben- oder Problemliste
* Berichte
* Über ein Dashboard

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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

Sie können einzelne Scrum-Teams so konfigurieren, dass die Projektdaten standardmäßig anstelle der Iterationsdaten verwendet werden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren, wie Daten angewendet werden, wenn Arbeitselemente zu einer Iteration hinzugefügt werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Hinzufügen einer Geschichte zu einer vorhandenen Iteration

So fügen Sie einer Iteration direkt über die Aufgabe oder das Problem Meldungen hinzu:

>[!IMPORTANT]
>
>Nachdem die Aufgabe in die Iteration verschoben wurde, können Sie die [!UICONTROL Dauer Typ] oder [!UICONTROL Aufgabenbegrenzung] nicht aktualisieren. Der [!UICONTROL Dauer-Typ] ist auf [!UICONTROL Einfach] und die [!UICONTROL Aufgabenbegrenzung] auf [!UICONTROL Feste Datumswerte] eingestellt, damit die Zeitleiste der Aufgabe mit der Timeline der Iteration konsistent bleibt.

### Registerkarte Aufgaben oder Probleme

Sie können jede Aufgabe oder jedes Problem zu jeder Iteration hinzufügen, wenn Sie Zugriff auf das Projekt verwalten haben. Beachten Sie beim Verschieben einer Aufgabe oder eines Problems in eine Iteration Folgendes:

* Wenn Sie mehrere Teams hinzufügen, kann die Aufgabe oder das Problem nur bei der Iteration eines Teams angezeigt werden. Dies ist die Iteration, die Sie in Schritt 3 unten auswählen.
* Wenn die Aufgabe oder das Problem einem agilen Team zugewiesen und in die Iteration eines anderen Teams verschoben wird, ändert sich die Teamzuweisung nicht.
* Wenn die Aufgabe oder das Problem nicht einem Team zugewiesen ist, wird die Aufgabe bzw. das Problem dem Team zugewiesen, dem die Iteration gehört.
* Sie können der Iteration keine übergeordneten Aufgaben hinzufügen. Wenn Sie untergeordnete Aufgaben hinzufügen, wird die übergeordnete Aufgabe auf der Scrum-Pinnwand als Swimlane angezeigt.

1. Gehen Sie zum Projekt, Bericht oder Dashboard, das die Aufgabe oder das Problem enthält, die/das Sie einer Iteration hinzufügen möchten.
1. Wählen Sie eine oder mehrere Aufgaben oder Probleme aus.
1. Klicken Sie auf **[!UICONTROL Mehr]** ![](assets/more-icon.png) > **[!UICONTROL Zu Iteration hinzufügen]**.\
   Nicht agilen Teams können keine Aufgaben oder Probleme zugewiesen werden.

1. Geben Sie in das Feld **[!UICONTROL Meldungen hinzufügen]** den Namen der Iteration ein.

   >[!NOTE]
   >
   >Sie können eine Geschichte von einer vorhandenen Iteration in eine neue Iteration verschieben.

1. Wenn Sie Aufgaben hinzufügen, klicken Sie auf **[!UICONTROL Meldungen hinzufügen]**.\
   Oder\
   Wenn Sie Probleme hinzufügen, klicken Sie auf **[!UICONTROL Probleme hinzufügen]**.
