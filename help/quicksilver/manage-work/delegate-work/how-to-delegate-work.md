---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegieren von Aufgaben und Problemen
description: Sie können die Arbeit, der Sie zugewiesen sind, während Sie nicht im Büro sind, vorübergehend delegieren. In diesem Artikel wird beschrieben, wie Aufgaben und Problemzuweisungen delegiert werden.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 0%

---

# Verwalten der Zuweisung von Aufgaben und Ausgaben

<!-- Audited: 1/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Sie können die Arbeit, der Sie zugewiesen sind, während Sie nicht im Büro sind, vorübergehend delegieren.

Sie können Aufgaben- und Problemzuweisungen delegieren oder Genehmigungen delegieren. In diesem Artikel wird beschrieben, wie Aufgaben und Problemzuweisungen delegiert werden.

Allgemeine Informationen zum Delegieren von Arbeit finden Sie unter [Übersicht über die Delegierung von Arbeiten ](../../manage-work/delegate-work/delegate-work-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

>[!IMPORTANT]
>
>* Die Benutzer, die Sie als Delegierte auswählen, erhalten dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihnen zuweisen.
>* Die Berechtigungen müssen innerhalb ihrer Zugriffsstufen funktionieren, und manchmal können ihre Zugriffsebenen niedriger sein als Ihre.
>
>   
>   Wenn ein Benutzer beispielsweise nur Zugriff auf Aufgaben in ihrer Zugriffsebene anzeigen hat und Sie über Verwaltungsberechtigungen für die Aufgaben verfügen, die Sie ihm zuweisen, erhält er Verwaltungsberechtigungen für die Aufgaben, die Sie ihm zuweisen. Sie können jedoch nicht dieselben Aktionen wie Sie für die delegierten Aufgaben durchführen. Damit Aufgaben in Ihrer Abwesenheit aktualisiert werden können, müssen sie vom Systemadministrator die Option Zugriff auf Aufgaben bearbeiten anfordern.
>
>   
>   Informationen dazu, wie ein Systemadministrator Ihre Zugriffsebene ändern kann, finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Bei Elementen, die zugewiesen werden, nachdem die Zuweisung bereits begonnen hat, kann es bis zu eine Stunde dauern, bis das Element für [!DNL Workfront] zugewiesen wurde, um die neu zugewiesenen Elemente für den Delegaten freizugeben.


Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Mitarbeiter oder höher</p><p>Oder</p><p>Aktuell: Überprüfen oder höher</p>

>[!NOTE]
>
>Obwohl Sie mit einer Lizenz für einen Antrag zugewiesen werden können, können Sie Ihre Arbeit nicht an andere delegieren. [!DNL Workfront] rät davon ab, Benutzern von Review-, Anforderungs- oder Mitwirkenden Aufgaben zuzuweisen.

</tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Aufgaben oder Probleme, denen Sie zugewiesen sind</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Voraussetzungen

Bevor Sie die in diesem Artikel beschriebenen Aktivitäten durchführen können, müssen Sie Folgendes sicherstellen:

* Ihr [!DNL Workfront]- oder Gruppenadministrator hat die Einstellung [!UICONTROL Benutzern erlauben, Aufgaben und Probleme mit protokollierten Stunden zu löschen] im Bereich [!UICONTROL Einrichtung] Ihrer [!DNL Workfront]-Instanz aktiviert.

  Weitere Informationen finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegieren von Aufgaben und Problemen an einen anderen Benutzer

Bevor Sie die Arbeit an andere delegieren, empfehlen wir Ihnen, sich an diese zu wenden und sie darüber zu informieren, dass sie zu Ihren Arbeitselementen als Delegierte ernannt werden. Bitten Sie um ihre verbale Genehmigung, bevor Sie die Arbeit delegieren, um sicherzustellen, dass sie die Zeit haben, die zum Abschluss der Arbeit benötigt wird, während Sie abwesend sind.

Allgemeine Informationen zum Delegieren von Aufgaben und Problemen finden Sie unter [Delegieren von Aufgaben und Problemen - Übersicht](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

So delegieren Sie Ihre Aufgaben und Probleme an andere:

1. Wechseln Sie zum Bereich [!UICONTROL **Home**] und klicken Sie dann oben in der [!UICONTROL **Arbeitsliste**] auf [!UICONTROL **Delegieren**] .

   ![](assets/delegate-button-in-home.png)

1. Aktualisieren Sie auf der Registerkarte [!UICONTROL **Aufgaben und Probleme delegieren**] Folgendes:

   * [!UICONTROL **Delegieren Sie Ihre Aufgaben und Probleme an**]: Beginnen Sie mit der Eingabe des Namens eines Benutzers, dem Ihre Aufgaben und Probleme zugewiesen werden sollen, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Sie können nur einen Benutzer auswählen.

     Der Benutzer, den Sie als Delegierter auswählen, erhält dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihm zuweisen.

   * [!UICONTROL **Startdatum**]: Wählen Sie ein Datum aus dem Kalender aus, an dem die Zuweisung Ihrer Arbeitselemente beginnen soll.

     >[!TIP]
     >
     >Das Startdatum kann nicht in der Vergangenheit liegen.

   * [!UICONTROL **Kein Enddatum**]: Wählen Sie diese Option, wenn Sie das Enddatum für Ihre Delegation nicht angeben möchten.

   * [!UICONTROL **Enddatum**]: Wählen Sie ein Datum aus dem Kalender aus, an dem die Zuweisung beendet werden soll.

     >[!TIP]
     >
     >Wenn Sie das Feld Enddatum leer lassen und die Option Kein Enddatum nicht ausgewählt ist, wird die Zuweisung nur für den aktuellen Tag festgelegt.

     ![](assets/delegate-box-expanded-in-home.png)

1. Klicken Sie auf [!UICONTROL **Speichern**].

   Folgendes geschieht:

   * Ihre Arbeit wird an den angegebenen Benutzer delegiert. Alle unvollständigen Aufgaben oder Probleme, die innerhalb des ausgewählten Zeitrahmens liegen (einschließlich neu zugewiesener Aufgaben, nachdem die Zuweisung aktiviert wurde), werden delegiert.

     >[!TIP]
     >
     >   Abgeschlossene Arbeitselemente, die Daten innerhalb des Zeitrahmens der Zuweisung enthalten, werden nicht delegiert.


   * Sie erhalten eine Meldung in der rechten oberen Ecke des Bildschirms, um zu bestätigen, dass Sie die Zuweisung Ihrer Arbeit an einen anderen Benutzer aktiviert haben. Der Name des Delegate-Benutzers wird in der Bestätigungsmeldung angezeigt.

   * Ein Hinweis darauf, dass Ihre Aufgaben und Probleme an andere Benutzer delegiert wurden, wird in den meisten Bereichen angezeigt, in denen Zuweisungen in [!DNL Workfront] angezeigt werden. Weitere Informationen darüber, welche Bereiche keine Delegationsnamen enthalten, finden Sie unter [Übersicht über die Arbeit delegieren](delegate-work-overview.md).

   * Die Schaltfläche [!UICONTROL **Delegieren**] im Bereich [!UICONTROL Home] ändert sich in [!UICONTROL **Delegation bearbeiten**], um anzugeben, dass eine Delegation vorhanden ist.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Wenn Ihre Ereignisbenachrichtigungen und Ihre persönlichen Benachrichtigungen aktiviert sind, erhalten Sie auch eine E-Mail-Bestätigung Ihrer Delegation.

   * Der Benutzer, den Sie als Ihr Delegat ausgewählt haben, erhält eine E-Mail über die Zuweisung, wenn seine Ereignisbenachrichtigungen aktiviert sind.

     Informationen zum Aktivieren von persönlichen E-Mail-Benachrichtigungen finden Sie unter [Ändern eigener E-Mail-Benachrichtigungen](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Bearbeiten oder Anhalten der Zuweisung

Sie können eine Zuweisung ablaufen lassen, wenn Sie ein Enddatum ausgewählt haben, oder Sie können es manuell anhalten. Sie können auch den Zeitrahmen für die Delegation ändern, wenn sich die Daten für die Delegation geändert haben.

1. Wechseln Sie zum Bereich [!UICONTROL Startseite] und klicken Sie dann oben rechts in der Arbeitsliste auf [!UICONTROL Zuweisung bearbeiten] .
1. Führen Sie auf der Registerkarte [!UICONTROL Aufgaben und Probleme delegieren] einen der folgenden Schritte aus:
   * Ändern Sie das [!UICONTROL **Startdatum**] oder das [!UICONTROL **Enddatum**]
   * Klicken Sie auf [!UICONTROL **Delegation stoppen**]

   >[!TIP]
   >
   >    Sie können nur das Enddatum einer Delegation bearbeiten, wenn diese bereits begonnen hat.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Bedingt) Klicken Sie auf [!UICONTROL **Speichern**] , um die neuen Delegationsdaten zu speichern.

   Oder

   Klicken Sie im Bestätigungsfeld auf [!UICONTROL **Delegation stoppen**] , um das Beenden der Delegation zu bestätigen.

   Die Delegation aktualisierte entweder die Daten oder stoppte sie und die delegierten Benutzer wurden aus Ihren Aufgaben und Problemen entfernt. Ihre Berechtigungen für die Aufgaben und Probleme bleiben erhalten.


## Delegierte Arbeit lokalisieren und Informationen delegieren

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Wenn Aufgaben und Probleme delegiert werden, gibt es in [!DNL Workfront] mehrere Bereiche, in denen die delegierte Arbeit angezeigt wird oder wer die Delegierten sind.

* [Delegates im Feld &quot;Zuweisungen&quot;suchen](#locate-delegates-in-the-assignments-box)
* [Suchen Sie delegierte Arbeit in [!UICONTROL Home]](#locate-delegated-work-in-home)


### Suchen Sie Delegates im Feld [!UICONTROL Zuweisungen] .

Wenn Ihr System- oder Gruppenadministrator die Arbeitsdelegierung in Ihrem System aktiviert, werden im Feld [!UICONTROL Zuweisungen] die folgenden Registerkarten angezeigt, auf die Sie zugreifen können:

* [!UICONTROL **Zuweisungen**]: Benutzer, die der Aufgabe oder dem Problem zugewiesen sind, werden hier angezeigt.
* [!UICONTROL **Delegationen**]: Hier werden Benutzer angezeigt, die von den Verantwortlichen für die Aufgabe oder das Problem als Delegierte benannt wurden.

Sie können in den folgenden Bereichen auf das Feld [!UICONTROL Zuweisungen] zugreifen:

* Aufgaben- oder Problemkopfzeile

  Das Feld [!UICONTROL Zuweisungen] in der Aufgaben- oder Problemüberschrift ändert sich in [!UICONTROL Zuweisungen und Delegationen].

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* Der [!UICONTROL Lastenausgleich] beim manuellen Zuweisen von Aufgaben oder Problemen

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Sie können Delegaten nicht im Abschnitt [!UICONTROL Zuweisungen] einer Aufgabe oder im Feld &quot;Problembearbeitung&quot;anzeigen.

Wenn eine Aufgabe oder ein Problem delegiert wird und die Unterregisterkarte [!UICONTROL Delegations] leer ist, kann eines der folgenden Szenarien vorliegen:

* Sie sind der Aufgabe oder dem Problem nicht zugewiesen.
* Die Aufgaben- oder Ausgabedaten liegen außerhalb des Zeitrahmens der Delegierung.

>[!TIP]
>
>Die geplanten oder tatsächlichen Stunden für delegierte Aufgaben und Probleme werden in den Tools für die Ressourcenverwaltung nicht berücksichtigt, wie z. B. der [!UICONTROL Lastenausgleich] oder der [!DNL Resource Planner] für die delegierten Benutzer. Die Stunden bleiben nur mit dem zugewiesenen Benutzer verknüpft.

### Suchen Sie delegierte Arbeit in [!UICONTROL Home]

1. Wechseln Sie zum Bereich [!UICONTROL **Home**] , klicken Sie auf das Dropdown-Menü &quot;Filter&quot;und wählen Sie eine oder mehrere der folgenden Optionen aus:
   * [!UICONTROL **Delegiert**]: zum Anzeigen von Aufgaben und Problemen, die Ihnen oder Ihnen zugewiesen wurden.
   * [!UICONTROL **Delegiert an mich**]: zum Anzeigen von Aufgaben und Problemen, die Ihnen von einem anderen Benutzer zugewiesen wurden.
   * [!UICONTROL **Von mir delegiert**]: zum Anzeigen von Aufgaben und Problemen, die von Ihnen an andere Benutzer delegiert wurden.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Klicken Sie auf das Dropdown-Menü [!UICONTROL Sortieren] , um die Liste nach folgenden Kriterien zu sortieren:
   * [!UICONTROL Geplanter Abschluss]. Dies ist die standardmäßige Sortieroption.
   * [!UICONTROL Geplanter Start]
   * [!UICONTROL Datum der Übermittlung]
   * [!UICONTROL Projekt]
   * [!UICONTROL Meine Priorität]
1. Erweitern Sie die Gruppierungen in der [!UICONTROL **Arbeitsliste**], um zugewiesene Arbeitselemente anzuzeigen. Die folgenden Szenarien existieren:
   * Bei Elementen, die Sie an andere delegiert haben, wird der Name des Delegaten in der [!UICONTROL **Arbeitsliste**] sowie im Feld [!UICONTROL **Zuweisungen und Delegationen**] auf der rechten Seite angezeigt.

   * Für Elemente, die Ihnen zugewiesen wurden, wird der Name des Verantwortlichen in der [!UICONTROL **Arbeitsliste**] sowie im Feld **[!UICONTROL Zuweisungen und Delegationen]** auf der rechten Seite angezeigt.

   >[!TIP]
   >
   >    Wenn die Zuweisung so eingestellt ist, dass sie zu einem Datum nach dem heutigen Datum beginnt, wird das Startdatum der Zuweisung auch in der [!UICONTROL Arbeitsliste] angezeigt. Die zugewiesenen Elemente werden in der Gruppierung angezeigt, die Sie für die [!UICONTROL Arbeitsliste] auswählen, je nach Gruppierungstyp. Wenn Sie beispielsweise nach dem geplanten Abschlussdatum ] gruppieren, werden die zugewiesenen Elemente in der Gruppierung angezeigt, die mit den geplanten Abschlussdaten übereinstimmt.[!UICONTROL 
