---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegieren von Aufgaben und Problemen
description: Sie können die Arbeit, der Sie zugewiesen sind, während Sie nicht im Büro sind, vorübergehend delegieren. In diesem Artikel wird beschrieben, wie Aufgaben und Problemzuweisungen delegiert werden.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 1%

---

# Verwalten der Zuweisung von Aufgaben und Ausgaben

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Sie können die Arbeit, der Sie zugewiesen sind, während Sie nicht im Büro sind, vorübergehend delegieren.

Sie können Aufgaben- und Problemzuweisungen delegieren oder Genehmigungen delegieren. In diesem Artikel wird beschrieben, wie Aufgaben und Problemzuweisungen delegiert werden.

Allgemeine Informationen zur Delegierung von Arbeiten finden Sie unter [Delegieren von Arbeiten - Übersicht](../../manage-work/delegate-work/delegate-work-overview.md).

## Zugriffsanforderungen

>[!IMPORTANT]
>
>* Die Benutzer, die Sie als Delegierte auswählen, erhalten dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihnen zuweisen.
>* Die Berechtigungen müssen innerhalb ihrer Zugriffsstufen funktionieren, und manchmal können ihre Zugriffsebenen niedriger sein als Ihre.
>
>   
>   Wenn ein Benutzer beispielsweise nur Zugriff auf Aufgaben in ihrer Zugriffsebene anzeigen hat und Sie über Verwaltungsberechtigungen für die Aufgaben verfügen, die Sie ihm zuweisen, erhält er Verwaltungsberechtigungen für die Aufgaben, die Sie ihm zuweisen. Sie können jedoch nicht dieselben Aktionen wie Sie für die delegierten Aufgaben durchführen. Sie müssen vom Systemadministrator Zugriff auf Aufgaben bearbeiten anfordern, um in Ihrer Abwesenheit Aufgaben aktualisieren zu können.
>
>   
>   Informationen dazu, wie Sie Ihre Zugriffsebene ändern können, finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Bei Elementen, die zugewiesen werden, nachdem die Zuweisung der Zuweisung bereits begonnen hat, kann es bis zu eine Stunde dauern, bis das Element für [!DNL Workfront] , um die neu zugewiesenen Elemente für den Delegaten freizugeben.


Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>Überprüfen oder höher</p>

>[!NOTE]
>
>Obwohl Sie mit einer Lizenz für einen Antrag zugewiesen werden können, können Sie Ihre Arbeit nicht an andere delegieren. [!DNL Workfront] empfiehlt nicht, Benutzern von Review oder Anforderung Aufgaben zuzuweisen.

</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Aufgaben oder Probleme, denen Sie zugewiesen sind</p> 
    <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Voraussetzungen

Bevor Sie die in diesem Artikel beschriebenen Aktivitäten durchführen können, müssen Sie Folgendes sicherstellen:

* Ihre [!DNL Workfront] oder der Gruppenadministrator die [!UICONTROL Löschen von Aufgaben und Problemen in angemeldeten Stunden durch Benutzer zulassen] -Einstellung in [!UICONTROL Einrichtung] Ihres [!DNL Workfront] -Instanz.

  Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegieren von Aufgaben und Problemen an einen anderen Benutzer

Bevor Sie die Arbeit an andere delegieren, empfehlen wir Ihnen, sich an diese zu wenden und sie darüber zu informieren, dass sie zu Ihren Arbeitselementen als Delegierte ernannt werden. Bitten Sie um ihre verbale Genehmigung, bevor Sie die Arbeit delegieren, um sicherzustellen, dass sie die Zeit haben, die zum Abschluss der Arbeit benötigt wird, während Sie abwesend sind.

Allgemeine Informationen zum Delegieren von Aufgaben und Problemen finden Sie unter [Delegieren von Aufgaben und Problemen - Übersicht](delegate-work.md).

So delegieren Sie Ihre Aufgaben und Probleme an andere:

1. Navigieren Sie zu [!UICONTROL **Startseite**] Bereich und klicken Sie dann auf [!UICONTROL **Delegieren**] oben im [!UICONTROL **Arbeitsliste**].

   ![](assets/delegate-button-in-home.png)

1. Im [!UICONTROL **Aufgaben und Probleme delegieren**] aktualisieren Sie Folgendes:

   * [!UICONTROL **Delegieren Sie Ihre Aufgaben und Probleme an**]: Beginnen Sie mit der Eingabe des Namens eines Benutzers, dem Ihre Aufgaben und Probleme zugewiesen werden sollen, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können nur einen Benutzer auswählen.\

     Der Benutzer, den Sie als Delegierter auswählen, erhält dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihm zuweisen. Weitere Informationen finden Sie unter [Delegieren von Aufgaben und Problemübersicht](delegate-work-overview.md).

   * [!UICONTROL **Startdatum**]: Wählen Sie ein Datum aus dem Kalender aus, an dem die Zuweisung Ihrer Arbeitselemente beginnen soll.

     >[!TIP]
     >
     >Das Startdatum kann nicht in der Vergangenheit liegen.

   * [!UICONTROL **Kein Enddatum**]: Wählen Sie diese Option aus, wenn Sie das Enddatum für Ihre Delegation nicht angeben möchten.

   * [!UICONTROL **Enddatum**]: Wählen Sie ein Datum aus dem Kalender aus, an dem die Zuweisung gestoppt werden soll.

     >[!TIP]
     >
     >Wenn Sie kein Enddatum auswählen, wird die Zuweisung nur für den aktuellen Tag aktiviert.

     ![](assets/delegate-box-expanded-in-home.png)

1. Klicken Sie auf [!UICONTROL **Speichern**].

   Folgendes geschieht:

   * Ihre Arbeit wird an den angegebenen Benutzer delegiert. Alle unvollständigen Aufgaben oder Probleme, die innerhalb des ausgewählten Zeitrahmens liegen (einschließlich neu zugewiesener Aufgaben, nachdem die Zuweisung aktiviert wurde), werden delegiert.

   >[!TIP]
   >
   >   Abgeschlossene Arbeitselemente, die Daten innerhalb des Zeitrahmens der Zuweisung enthalten, werden nicht delegiert.


   * Sie erhalten eine Meldung in der rechten oberen Ecke des Bildschirms, um zu bestätigen, dass Sie die Zuweisung Ihrer Arbeit an einen anderen Benutzer aktiviert haben. Der Name des Delegate-Benutzers wird in der Bestätigungsmeldung angezeigt.

   * Ein Hinweis darauf, dass Ihre Aufgaben und Probleme an andere Benutzer delegiert wurden, wird in den meisten Bereichen angezeigt, in denen Sie Zuweisungen in [!DNL Workfront]. Weitere Informationen darüber, welche Bereiche keine Delegationsnamen enthalten, finden Sie unter [Delegieren von Aufgaben und Problemübersicht](delegate-work-overview.md).

   * Die [!UICONTROL **Delegieren**] im [!UICONTROL Startseite] Bereichsänderungen in [!UICONTROL **Delegation bearbeiten**] um anzugeben, dass eine Delegation eingerichtet ist.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Wenn Ihre Ereignisbenachrichtigungen und Ihre persönlichen Benachrichtigungen aktiviert sind, erhalten Sie auch eine E-Mail-Bestätigung Ihrer Delegation.

   * Der Benutzer, den Sie als Ihr Delegat ausgewählt haben, erhält eine E-Mail über die Zuweisung, wenn seine Ereignisbenachrichtigungen aktiviert sind.

     Informationen zum Aktivieren von persönlichen E-Mail-Benachrichtigungen finden Sie unter [Aktivieren oder Deaktivieren Ihrer eigenen Ereignisbenachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).




## Bearbeiten oder Anhalten der Zuweisung

Sie können eine Zuweisung ablaufen lassen, wenn Sie ein Enddatum ausgewählt haben, oder Sie können es manuell anhalten. Sie können auch den Zeitrahmen für die Delegation ändern, wenn sich die Daten für die Delegation geändert haben.

1. Navigieren Sie zu [!UICONTROL Startseite] Bereich und klicken Sie dann auf [!UICONTROL Delegation bearbeiten] in der oberen rechten Ecke der Arbeitsliste.
1. Im [!UICONTROL Aufgaben und Probleme delegieren] führen Sie einen der folgenden Schritte aus:
   * Ändern Sie die [!UICONTROL **Startdatum**] oder [!UICONTROL **Enddatum**]
   * Klicks [!UICONTROL **Zuweisung beenden**]

   >[!TIP]
   >
   >    Sie können nur das Enddatum einer Delegation bearbeiten, wenn diese bereits begonnen hat.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Bedingt) Klicken Sie auf [!UICONTROL **Speichern**] Speichern der neuen Delegationsdaten

   Oder

   Klicks [!UICONTROL **Zuweisung beenden**] in das Bestätigungsfeld ein, um das Beenden der Delegation zu bestätigen.

   Die Delegation aktualisierte entweder die Daten oder stoppte sie und die delegierten Benutzer wurden aus Ihren Aufgaben und Problemen entfernt. Ihre Berechtigungen für die Aufgaben und Probleme bleiben erhalten.


## Delegierte Arbeit lokalisieren und Informationen delegieren

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Wenn Aufgaben und Probleme delegiert werden, gibt es mehrere Bereiche in [!DNL Workfront] wo Sie die delegierte Arbeit sehen können oder wer die Delegierten sind.

* [Delegates im Feld &quot;Zuweisungen&quot;suchen](#locate-delegates-in-the-assignments-box)
* [Suchen Sie delegierte Arbeit in [!UICONTROL Startseite]](#locate-delegated-work-in-home)


### Suchen Sie Delegates in der [!UICONTROL Zuweisungen] box

Wenn Ihr System- oder Gruppenadministrator die Arbeitszuweisung in Ihrem System aktiviert, wird die [!UICONTROL Zuweisungen] zeigt die folgenden Registerkarten an, auf die Sie zugreifen können:

* [!UICONTROL **Zuweisungen**]: Benutzer, die der Aufgabe oder dem Problem zugewiesen sind, werden hier angezeigt.
* [!UICONTROL **Delegationen**]: Hier werden Benutzer angezeigt, die von den Verantwortlichen für die Aufgabe oder das Problem als Delegierte benannt wurden.

Sie können auf die [!UICONTROL Zuweisungen] in den folgenden Bereichen:

* Aufgaben- oder Problemkopfzeile

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

  Die [!UICONTROL Zuweisungen] -Feld in der Aufgabe oder in der Problemüberschrift ändern sich zu [!UICONTROL Zuweisung und Delegationen].

* Die [!UICONTROL Lastenausgleich] beim manuellen Zuweisen von Aufgaben oder Problemen

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Sie können Delegates nicht im [!UICONTROL Zuweisungen] Abschnitt einer Aufgabe oder eines Problems bearbeiten -Felds.

Wenn eine Aufgabe oder ein Problem delegiert wird und die [!UICONTROL Delegationen] subtab leer ist, kann eines der folgenden Szenarien vorliegen:

* Sie sind der Aufgabe oder dem Problem nicht zugewiesen.
* Die Aufgaben- oder Ausgabedaten liegen außerhalb des Zeitrahmens der Delegierung.

>[!TIP]
>
>Die geplanten oder tatsächlichen Stunden für delegierte Aufgaben und Probleme werden in den Tools für die Ressourcenverwaltung nicht berücksichtigt, z. B. bei der [!UICONTROL Lastenausgleich] oder [!DNL Resource Planner] für die delegierten Benutzer. Die Stunden bleiben nur mit dem zugewiesenen Benutzer verknüpft.

### Suchen Sie delegierte Arbeit in [!UICONTROL Startseite]

1. Navigieren Sie zu [!UICONTROL **Startseite**] auf das Dropdown-Menü &quot;Filter&quot;klicken und eine oder mehrere der folgenden Optionen auswählen:
   * [!UICONTROL **Delegiert**]: um Aufgaben und Probleme anzuzeigen, die Ihnen oder Ihnen zugewiesen wurden.
   * [!UICONTROL **Delegiert an mich**]: um Aufgaben und Probleme anzuzeigen, die Ihnen von einem anderen Benutzer zugewiesen wurden.
   * [!UICONTROL **Delegiert von mir**]: um Aufgaben und Probleme anzuzeigen, die von Ihnen an andere Benutzer delegiert wurden.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Klicken Sie auf [!UICONTROL Sortierung] Dropdown-Menü, um die Liste nach folgenden Kriterien zu sortieren:
   * [!UICONTROL Geplanter Abschluss]. Dies ist die standardmäßige Sortieroption.
   * [!UICONTROL Geplanter Start]
   * [!UICONTROL Verpflichtungsdatum]
   * [!UICONTROL Projekt]
   * [!UICONTROL Meine Priorität]
1. Erweitern Sie die Gruppierungen im [!UICONTROL **Arbeitsliste**] , um delegierte Arbeitselemente anzuzeigen. Die folgenden Szenarien existieren:
   * Für Elemente, die Sie anderen zugewiesen haben, wird der Name des Delegaten im [!UICONTROL **Arbeitsliste**] sowie [!UICONTROL **Zuweisung und Delegationen**] auf der rechten Seite.

   * Für Elemente, die Ihnen zugewiesen wurden, wird der Name des Bevollmächtigten im [!UICONTROL **Arbeitsliste**] sowie **[!UICONTROL Zuweisung und Delegationen]** auf der rechten Seite.

   >[!TIP]
   >
   >    Wenn die Delegation zu einem Datum nach dem heutigen Datum beginnen soll, wird das Beginndatum der Delegation auch im [!UICONTROL Arbeitsliste]. Die zugewiesenen Elemente werden in der Gruppierung angezeigt, die Sie für die [!UICONTROL Arbeitsliste], je nach Gruppierungstyp. Wenn Sie beispielsweise nach [!UICONTROL Geplantes Abschlussdatum], werden die delegierten Elemente in der Gruppierung angezeigt, die mit den geplanten Abschlussdaten übereinstimmt.
