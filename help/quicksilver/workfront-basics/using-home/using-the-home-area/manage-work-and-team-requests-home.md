---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Verwalten von Arbeits- und Teamanfragen im Startbereich
description: Wenn Ihnen Arbeitsaufgaben und -probleme zugewiesen sind, werden sie auf der [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] aufgelistet. Sie können eine Anforderung anzeigen, neu zuweisen, beantworten, bearbeiten oder entfernen. Arbeitsanforderungen im Bereich [!UICONTROL Startseite] sind nicht auf Probleme beschränkt, die mit Anforderungswarteschlangen verbunden sind.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Verwalten von Arbeits- und Teamanfragen im Bereich [!UICONTROL Home]

Wenn Ihnen Arbeitsaufgaben und -probleme zugewiesen sind, werden sie auf der [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] aufgelistet. Sie können eine Anforderung anzeigen, neu zuweisen, beantworten, bearbeiten oder entfernen. Arbeitsanforderungen im Bereich [!UICONTROL Startseite] sind nicht auf Probleme beschränkt, die mit Anforderungswarteschlangen verbunden sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf Aufgaben und Probleme bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Contribute-Berechtigungen oder höher für die Aufgaben und Probleme, an denen Sie arbeiten müssen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen einer Arbeitsanforderung

Arbeitsanforderungen, die Ihnen zugewiesen sind, werden im linken Bereich in [!UICONTROL Startseite] angezeigt. Sie können konfigurieren, welche Anforderungen in [!UICONTROL Startseite] angezeigt werden, indem Sie den Filter oben in der [!UICONTROL Arbeitsliste] verwenden.

Sie können Filter auswählen, die Elemente anzeigen, die für die Arbeit bereit sind, oder Elemente, an denen Sie derzeit arbeiten.

In diesem Artikel wird beschrieben, wie Sie die Filter im Bereich [!UICONTROL Startseite] verwenden, um Elemente anzuzeigen, an denen Sie derzeit arbeiten oder die Sie in Erwägung ziehen könnten, mit der Arbeit zu beginnen. Informationen zu allen Filtern im Bereich [!UICONTROL Home] finden Sie unter [Elemente in der Arbeitsliste im Bereich [!UICONTROL Home] anzeigen](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Filter]** .

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Klicken Sie auf eine oder beide der folgenden Optionen für Aufgaben:

   **[!UICONTROL Bereit zum Start]:** Zeigt nur Aufgaben und Probleme an, die startbereit sind. Beide der folgenden Anweisungen müssen wahr sein:

   * Die Aufgaben und ihre Eltern haben keine Vorgänger oder Aufgabeneinschränkungen, die sie daran hindern, daran gearbeitet zu werden.
   * Das [!UICONTROL geplante Startdatum] der Aufgaben oder Probleme liegt in der Vergangenheit oder bis zu zwei Wochen in der Zukunft.

   **[!UICONTROL Nicht bereit]**: Zeigt nur Aufgaben und Probleme an, die noch nicht startbereit sind. Jede der folgenden Anweisungen muss &quot;true&quot;lauten:

   * Die Aufgaben und ihre Eltern haben möglicherweise Vorgänger oder Aufgabeneinschränkungen, die deren Bearbeitung verhindern.
   * Die Aufgaben oder Probleme haben ein [!UICONTROL geplantes Startdatum], das mehr als zwei Wochen in der Zukunft beträgt.


1. Klicken Sie unter [!UICONTROL Aufgaben] oder [!UICONTROL Probleme] auf **[!UICONTROL Arbeiten an]** , um Aufgaben und Probleme anzuzeigen, an denen Sie derzeit arbeiten.
1. Klicken Sie unter [!UICONTROL Probleme] auf **[!UICONTROL Angefordert]** , um Probleme anzuzeigen, die von Ihnen angefordert wurden (Ihnen wurden zugewiesen), für die Sie sich jedoch noch nicht zur Arbeit bereit erklärt haben.

## Zugriff auf eine Teamanfrage

Sie können direkt über den Bereich [!UICONTROL Home] auf eine Ihrem Team zugewiesene Anforderung zugreifen. Weitere Informationen zu Team-Anforderungen finden Sie unter [Übersicht über Team-Anforderungen](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Klicken Sie im Bereich **[!UICONTROL Arbeitsliste]** auf , um die Gruppe **[!UICONTROL Team-Anforderungen]** zu erweitern.

   Wenn Ihrem Team keine Anforderungen zugewiesen sind, wird die Gruppierung nicht angezeigt.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Klicken Sie auf den Teamnamen.\
   Im Abschnitt **[!UICONTROL Team-Anforderungen]** werden alle Anforderungen angezeigt, die Ihrem Team zugewiesen sind. Weitere Informationen zum Arbeiten mit Teamanfragen finden Sie unter [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Anforderung erneut zuweisen

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Wählen Sie im Bereich **[!UICONTROL Arbeitsliste]** die Anforderung aus, die Sie neu zuweisen möchten.

1. Klicken Sie auf das Widget **[!UICONTROL Zuweisungen]** , entfernen Sie sich aus der Anforderung und geben Sie dann den Namen des Benutzers ein, dem Sie die Anforderung neu zuweisen möchten.

   >[!TIP]
   >
   >Wenn sich die Arbeitanforderung noch im Status &quot;Bereit zum Start&quot;oder &quot;Nicht bereit&quot;befindet, können Sie die Schaltfläche **[!UICONTROL Neu zuweisen]** im Menü **[!UICONTROL Mehr]** in der [!UICONTROL Arbeitsliste] verwenden.\
   >![Schaltfläche &quot;Neu zuweisen&quot;](assets/reassign-in-left-panel-350x204.png)

1. Wenn der Status einer Aufgabe nach Abschluss in [!UICONTROL Neu] oder [!UICONTROL In Bearbeitung] geändert wird, müssen Sie die Zuweisung des Benutzers aufheben, die Aufgabe speichern und den Benutzer neu zuweisen, damit die Aufgabe wieder in der Arbeitsliste der Startseite angezeigt wird.

## Antwort auf eine Anfrage

Sie können auf eine Anfrage antworten, um die Anfrage weiter zu klären oder ein neues Datum vorzuschlagen.

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Wählen Sie im Bereich **[!UICONTROL Arbeitsliste]** die Anforderung aus, auf die Sie antworten möchten.
1. Suchen Sie die Person, die Ihnen die Anfrage zugewiesen hat.

   Sie finden diese Informationen auf der Registerkarte [!UICONTROL Aktualisierungen] der Aufgabe. Stellen Sie sicher, dass die Option &quot;**[!UICONTROL Systemaktualisierungen anzeigen]**&quot;aktiviert ist.

1. Klicken Sie auf **[!UICONTROL Neues Update starten]** und beginnen Sie mit der Eingabe Ihrer Antwort.
1. Geben Sie den Namen des Empfängers in das Feld **[!UICONTROL Benachrichtigen]** ein und klicken Sie dann auf **[!UICONTROL Aktualisieren]**.

   >[!TIP]
   >
   >Wenn sich die Arbeitanforderung noch im Status &quot;Bereit zum Start&quot;oder &quot;[!UICONTROL Nicht bereit]&quot;befindet, können Sie die Schaltfläche &quot;**[!UICONTROL Antwort]**&quot;im Menü &quot;**[!UICONTROL Mehr]**&quot;in der [!UICONTROL Arbeitsliste]&quot;verwenden.\
   >![[!UICONTROL Schaltfläche &quot;Antworten&quot;]](assets/reassign-in-left-panel-350x204.png)   >

## Bearbeitung einer Anforderung

Wenn Sie auf die Schaltfläche [!UICONTROL Bearbeiten] klicken, geben Sie an den Benutzer, der die Anforderung gesendet hat, und an jeden anderen Benutzer, der der Anforderung möglicherweise zugewiesen ist, dass Sie mit der Bearbeitung der Anforderung beginnen werden. Weitere Informationen zum Bearbeiten von Anforderungen finden Sie unter [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Wählen Sie im Bereich **[!UICONTROL Arbeitsliste]** die Anforderung aus, an der Sie arbeiten möchten, und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.\
   Informationen zum Problem werden im rechten Bereich angezeigt.

## Anforderung entfernen

Wenn Sie sich dafür entscheiden, die Anforderung nicht zu bearbeiten, können Sie die Aufgabe oder das Problem entweder zurück in eine Anforderung konvertieren oder aus Ihrer Liste entfernen.

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. Zeigen Sie in der **[!UICONTROL Arbeitsliste]** auf das Element, auf das gewartet wird.
1. Klicken Sie auf das Widget **[!UICONTROL Zuweisungen]** und entfernen Sie sich selbst. Dadurch wird das Arbeitselement aus der Arbeitsliste entfernt. Wenn die Anforderung keinem anderen Benutzer oder einer anderen Team- oder Jobrolle zugewiesen wird, bleibt die Zuweisung der Anforderung aufgehoben.

   Oder

   Klicken Sie auf das Menüsymbol **[!UICONTROL Mehr]** rechts neben dem Namen der Aufgabe oder des Problems in der Liste [!UICONTROL Home Work].![](assets/more-icon.png)

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Wählen Sie aus den folgenden Optionen aus:

   * **[!UICONTROL In Arbeitsanforderung konvertieren]:** Wählen Sie diese Option, um das Arbeitselement wieder in eine Arbeitsanforderung zu konvertieren.\

     Das Arbeitselement wird zurück zu einer Anforderung übergeben und Sie bleiben der Anforderung zugewiesen.\
      Sie können die Anforderung zu einem späteren Zeitpunkt annehmen, indem Sie erneut auf **[!UICONTROL Bearbeiten]** klicken.

   * **[!UICONTROL Entfernen]:** Wählen Sie diese Option aus, um eine Anforderung aus Ihrer [!UICONTROL Arbeitsliste] zu entfernen.\

     Sie werden aus der Anfrage nicht zugewiesen und die Anfrage ist nicht mehr mit Ihrem Namen in [!DNL Adobe Workfront] verknüpft.\
      Wenn die Anforderung keinem anderen Benutzer oder einer anderen Team- oder Jobrolle zugewiesen wird, bleibt die Zuweisung der Anforderung aufgehoben.
