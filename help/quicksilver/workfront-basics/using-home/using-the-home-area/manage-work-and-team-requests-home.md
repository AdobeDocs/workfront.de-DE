---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Verwalten von Arbeits- und Teamanfragen im Startbereich
description: Wenn Ihnen Arbeitsaufgaben und Probleme zugewiesen werden, werden sie im [!UICONTROL Arbeitsliste] im [!UICONTROL Startseite] Bereich. Sie können eine Anforderung anzeigen, neu zuweisen, beantworten, bearbeiten oder entfernen. Arbeitsanforderungen in [!UICONTROL Startseite] -Bereich ist nicht auf Probleme im Zusammenhang mit Anforderungswarteschlangen beschränkt.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Verwalten von Arbeits- und Team-Anforderungen in [!UICONTROL Startseite] area

Wenn Ihnen Arbeitsaufgaben und Probleme zugewiesen werden, werden sie im [!UICONTROL Arbeitsliste] im [!UICONTROL Startseite] Bereich. Sie können eine Anforderung anzeigen, neu zuweisen, beantworten, bearbeiten oder entfernen. Arbeitsanforderungen in [!UICONTROL Startseite] -Bereich ist nicht auf Probleme im Zusammenhang mit Anforderungswarteschlangen beschränkt.

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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf Aufgaben und Probleme bearbeiten</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Aufgaben und Problemen, an denen Sie arbeiten müssen.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Anzeigen einer Arbeitsanforderung

Arbeitsanforderungen, die Ihnen zugewiesen sind, werden im linken Bereich in [!UICONTROL Startseite]. Sie können konfigurieren, welche Anforderungen in [!UICONTROL Startseite] Verwenden des Filters oben im [!UICONTROL Arbeitsliste].

Sie können Filter auswählen, die Elemente anzeigen, die für die Arbeit bereit sind, oder Elemente, an denen Sie derzeit arbeiten.

In diesem Artikel wird beschrieben, wie Sie die Filter im [!UICONTROL Startseite] -Bereich, um Elemente anzuzeigen, an denen Sie derzeit arbeiten oder die Sie in Erwägung ziehen könnten, mit der Arbeit zu beginnen. Informationen zu allen Filtern in der [!UICONTROL Startseite] -Bereich, siehe [Anzeigen von Elementen in der Arbeitsliste im [!UICONTROL Startseite] area](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Klicken Sie auf **[!UICONTROL Filter]** Dropdown-Menü.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Klicken Sie auf eine oder beide der folgenden Optionen für Aufgaben:

   **[!UICONTROL Bereit zum Start]:** Zeigt nur Aufgaben und Probleme an, die startbereit sind. Beide der folgenden Anweisungen müssen wahr sein:

   * Die Aufgaben und ihre Eltern haben keine Vorgänger oder Aufgabeneinschränkungen, die sie daran hindern, daran gearbeitet zu werden.
   * Die [!UICONTROL Geplantes Startdatum] der Aufgaben oder Probleme in der Vergangenheit oder bis zu zwei Wochen in der Zukunft.

   **[!UICONTROL Nicht bereit]**: Zeigt nur Aufgaben und Probleme an, die noch nicht startbereit sind. Jede der folgenden Anweisungen muss &quot;true&quot;lauten:

   * Die Aufgaben und ihre Eltern haben möglicherweise Vorgänger oder Aufgabeneinschränkungen, die deren Bearbeitung verhindern.
   * Die Aufgaben oder Probleme haben eine [!UICONTROL Geplantes Startdatum] Das sind mehr als zwei Wochen in der Zukunft.



1. Klicken **[!UICONTROL Arbeiten an]** under [!UICONTROL Aufgaben] oder [!UICONTROL Probleme] , um Aufgaben und Probleme anzuzeigen, an denen Sie derzeit arbeiten.
1. Klicken **[!UICONTROL Angefordert]** under [!UICONTROL Probleme] , um Probleme anzuzeigen, die von Ihnen angefordert wurden (Ihnen zugewiesen sind), aber noch nicht zur Bearbeitung akzeptiert wurden.

## Zugriff auf Teamanfragen

Sie können direkt über die [!UICONTROL Startseite] Bereich. Weitere Informationen zu Team-Anfragen finden Sie unter [Übersicht über Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Im **[!UICONTROL Arbeitsliste]** Bereich, klicken Sie auf , um die **[!UICONTROL Team-Anforderungen]** Gruppierung.

   Wenn Ihrem Team keine Anforderungen zugewiesen sind, wird die Gruppierung nicht angezeigt.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Klicken Sie auf den Teamnamen.\
   Die **[!UICONTROL Team-Anforderungen]** angezeigt und zeigt alle Anforderungen an, die Ihrem Team zugewiesen sind. Weitere Informationen zum Arbeiten mit Teamanfragen finden Sie unter [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Anforderung erneut zuweisen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Im **[!UICONTROL Arbeitsliste]** Bereich, wählen Sie die Anforderung aus, die Sie neu zuweisen möchten.

1. Klicken Sie auf **[!UICONTROL Zuweisungen]** Widget aus der Anforderung entfernen, und geben Sie dann den Namen des Benutzers ein, dem Sie die Anforderung neu zuweisen möchten.

   >[!TIP]
   >
   >Wenn sich die Arbeitanforderung noch im Status &quot;Bereit zum Start&quot;oder &quot;Nicht bereit&quot;befindet, können Sie die **[!UICONTROL Neu zuweisen]** im **[!UICONTROL Mehr]** im Menü [!UICONTROL Arbeitsliste].\
   >![Schaltfläche &quot;Neu zuweisen&quot;](assets/reassign-in-left-panel-350x204.png)

1. Wenn der Status einer Aufgabe geändert wird in [!UICONTROL Neu] oder [!UICONTROL In Bearbeitung] Nachdem die Aufgabe abgeschlossen wurde, müssen Sie die Zuweisung des Benutzers aufheben, die Aufgabe speichern und den Benutzer neu zuweisen, damit die Aufgabe wieder in der Arbeitsliste für die Startseite angezeigt wird.

## Antwort auf eine Anfrage

Sie können auf eine Anfrage antworten, um die Anfrage weiter zu klären oder ein neues Datum vorzuschlagen.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Im **[!UICONTROL Arbeitsliste]** -Bereich, wählen Sie die Anforderung aus, auf die Sie antworten möchten.
1. Suchen Sie die Person, die Ihnen die Anfrage zugewiesen hat.

   Diese Informationen finden Sie im [!UICONTROL Updates] Registerkarte der Aufgabe. Stellen Sie sicher, dass die Option **[!UICONTROL Systemaktualisierungen anzeigen]** aktiviert ist.

1. Klicken **[!UICONTROL Neue Aktualisierung starten]** und beginnen Sie mit der Eingabe Ihrer Antwort.
1. Geben Sie den Namen des Empfängers im **[!UICONTROL Benachrichtigen]** und klicken Sie auf **[!UICONTROL Aktualisieren]**.

   >[!TIP]
   >
   >Wenn sich die Arbeitsanforderung noch im Bereich &quot;Bereit zum Start&quot;befindet, oder [!UICONTROL Nicht bereit] -Status, können Sie die **[!UICONTROL Antwort]** im **[!UICONTROL Mehr]** im Menü [!UICONTROL Arbeitsliste].\
   >![[!UICONTROL Schaltfläche &quot;Antwort&quot;]](assets/reassign-in-left-panel-350x204.png)   >

## Bearbeitung einer Anforderung

Wenn Sie auf die [!UICONTROL Arbeiten daran] -Schaltfläche verwenden, geben Sie dem Benutzer, der die Anfrage gesendet hat, und jedem anderen Benutzer, der der Anfrage zugewiesen wurde, an, dass Sie mit der Bearbeitung der Anfrage beginnen werden. Weitere Informationen zum Bearbeiten von Anforderungen finden Sie unter  [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Im **[!UICONTROL Arbeitsliste]** Bereich, wählen Sie die Anforderung aus, an der Sie arbeiten möchten, und klicken Sie dann auf **[!UICONTROL Arbeiten daran]**.\
   Informationen zum Problem werden im rechten Bereich angezeigt.

## Anforderung entfernen

Wenn Sie sich dafür entscheiden, die Anforderung nicht zu bearbeiten, können Sie die Aufgabe oder das Problem entweder zurück in eine Anforderung konvertieren oder aus Ihrer Liste entfernen.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Im **[!UICONTROL Arbeitsliste]**, verweisen Sie auf den Artikel, der darauf wartet, bearbeitet zu werden.
1. Klicken Sie auf **[!UICONTROL Zuweisungen]** Widget und entfernen Sie sich selbst. Dadurch wird das Arbeitselement aus der Arbeitsliste entfernt. Wenn die Anforderung keinem anderen Benutzer oder einer anderen Team- oder Jobrolle zugewiesen wird, bleibt die Zuweisung der Anforderung aufgehoben.

   Oder

   Klicken Sie auf **[!UICONTROL Mehr]** Menüsymbol ![](assets/more-icon.png) rechts neben dem Namen der Aufgabe oder des Problems im [!UICONTROL Hausarbeit] Liste.

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Wählen Sie aus den folgenden Optionen aus:

   * **[!UICONTROL In Arbeitsanforderung konvertieren]:** Wählen Sie diese Option aus, um das Arbeitselement zurück in eine Arbeitsanforderung zu konvertieren.\

      Das Arbeitselement wird zurück zu einer Anforderung übergeben und Sie bleiben der Anforderung zugewiesen.\
      Sie können die Anfrage zu einem späteren Zeitpunkt annehmen, indem Sie auf **[!UICONTROL Arbeiten daran]** erneut.

   * **[!UICONTROL Entfernen]:** Wählen Sie diese Option aus, um eine Anforderung aus dem [!UICONTROL Arbeitsliste].\

      Die Zuweisung der Anfrage wird aufgehoben und die Anfrage ist nicht mehr mit Ihrem Namen in [!DNL Adobe Workfront].\
      Wenn die Anforderung keinem anderen Benutzer oder einer anderen Team- oder Jobrolle zugewiesen wird, bleibt die Zuweisung der Anforderung aufgehoben.
