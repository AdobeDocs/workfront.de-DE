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
source-wordcount: '673'
ht-degree: 0%

---

# Hinzufügen von Meldungen zu einer vorhandenen Iteration

Sie können einer Iteration auf eine der folgenden Arten Meldungen hinzufügen:

* Aus dem Backlog nach der Erstellung der Iteration, wie im Abschnitt [Verschieben von Meldungen aus dem Rückstand in eine Iteration oder [!UICONTROL Kanban] Pinnwand](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) Abschnitt in [Verwalten des agilen Rückprotokolls](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* Aus dem [!UICONTROL Details] Seite der einzelnen Aufgabe oder des Problems
* Von der Aufgaben- oder Problemliste
* Aus einem Bericht
* Über ein Dashboard

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Erfahren Sie, wie sich das Hinzufügen von Meldungen auf Aufgabendaten auswirkt

Wenn Sie einer Iteration eine vorhandene Aufgabe hinzufügen, wird die Aufgabe standardmäßig von [!UICONTROL Geplantes Startdatum] und [!UICONTROL Geplantes Abschlussdatum] werden wie folgt festgelegt:

### Aufgabe [!UICONTROL Geplantes Startdatum]

* Die Aufgabe verwendet das Startdatum der Iteration, wenn:

   * Das Projekt verfügt über keine [!UICONTROL Geplantes Startdatum] gesetzt.
   * Das Projekt [!UICONTROL Geplantes Startdatum] is *before* oder *on* das Startdatum der Iteration.

* Die Aufgabe verwendet die [!UICONTROL Geplantes Startdatum] wenn:

   * Das Projekt [!UICONTROL Geplantes Startdatum] is *after* das Startdatum der Iteration.

### Aufgabe [!UICONTROL Geplantes Abschlussdatum]

* Die Aufgabe verwendet das Enddatum der Iteration, wenn:

   * Das Projekt verfügt über keine [!UICONTROL Geplantes Abschlussdatum] gesetzt.
   * Das Projekt [!UICONTROL Geplantes Startdatum] is *vor oder auf* das Startdatum der Iteration oder das Projektdatum [!UICONTROL Geplantes Abschlussdatum] is *vor oder auf* das Enddatum der Iteration.

* Die Aufgabe verwendet die [!UICONTROL Geplantes Abschlussdatum] wenn:

   * Das Projekt [!UICONTROL Geplantes Startdatum] is *after* das Startdatum der Iteration und das Projektdatum [!UICONTROL Geplantes Abschlussdatum] is *after* das Enddatum der Iteration.

Sie können einzelne Scrum-Teams so konfigurieren, dass die Projektdaten standardmäßig anstelle der Iterationsdaten verwendet werden. Weitere Informationen finden Sie im Abschnitt . [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Hinzufügen einer Geschichte zu einer vorhandenen Iteration

So fügen Sie einer Iteration direkt über die Aufgabe oder das Problem Meldungen hinzu:

>[!IMPORTANT]
>
>Nachdem die Aufgabe in die Iteration verschoben wurde, können Sie die [!UICONTROL Dauer Typ] oder [!UICONTROL Aufgabenbegrenzung]. [!UICONTROL Dauer Typ] auf [!UICONTROL Einfach] und [!UICONTROL Aufgabenbegrenzung] auf [!UICONTROL Feste Datumswerte] um die Zeitleiste der Aufgabe mit der Zeitleiste der Iteration konsistent zu halten.

### Auf der Registerkarte Aufgaben oder Probleme

Sie können jede Aufgabe oder jedes Problem zu jeder Iteration hinzufügen, wenn Sie Zugriff auf das Projekt verwalten haben. Beachten Sie beim Verschieben einer Aufgabe oder eines Problems in eine Iteration Folgendes:

* Wenn Sie mehrere Teams hinzufügen, kann die Aufgabe oder das Problem nur bei der Iteration eines Teams angezeigt werden. Dies ist die Iteration, die Sie in Schritt 3 unten auswählen.
* Wenn die Aufgabe oder das Problem einem agilen Team zugewiesen und in die Iteration eines anderen Teams verschoben wird, ändert sich die Teamzuweisung nicht.
* Wenn die Aufgabe oder das Problem nicht einem Team zugewiesen ist, wird die Aufgabe oder das Problem dem Team zugewiesen, dem die Iteration gehört.
* Sie können der Iteration keine übergeordneten Aufgaben hinzufügen. Wenn Sie untergeordnete Aufgaben hinzufügen, wird die übergeordnete Aufgabe auf der Scrum-Pinnwand als Swimlane angezeigt.

1. Gehen Sie zum Projekt, Bericht oder Dashboard, das die Aufgabe oder das Problem enthält, die/das Sie einer Iteration hinzufügen möchten.
1. Wählen Sie eine oder mehrere Aufgaben oder Probleme aus.
1. Klicken **[!UICONTROL Mehr]** ![](assets/more-icon.png) > **[!UICONTROL Zu Iteration hinzufügen]**.\
   Nicht agilen Teams können keine Aufgaben oder Probleme zugewiesen werden.

1. Im **[!UICONTROL Meldungen hinzufügen]** den Namen der Iteration eingeben.

   >[!NOTE]
   >
   >Sie können eine Geschichte von einer vorhandenen Iteration in eine neue Iteration verschieben.

1. Wenn Sie Aufgaben hinzufügen, klicken Sie auf **[!UICONTROL Meldungen hinzufügen]**.\
   Oder\
   Wenn Sie Probleme hinzufügen, klicken Sie auf **[!UICONTROL Hinzufügen von Problemen]**.
