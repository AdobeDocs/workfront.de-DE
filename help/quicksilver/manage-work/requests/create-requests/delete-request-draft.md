---
product-area: requests
navigation-topic: create-requests
title: Löschen einer gesendeten Anfrage oder eines Anforderungsentwurfs
description: Sie können gesendete Anfragen oder Anfrageentwürfe in Adobe Workfront löschen.
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 9%

---

# Löschen einer gesendeten Anfrage oder eines Anfrageentwurfs

Sie können von Adobe Workfront oder Adobe Workfront Planning gesendete Anfragen oder Anfrageentwürfe löschen, für die Sie erstellt haben oder für die Sie Verwaltungsberechtigungen besitzen.

Workfront-Administratoren und Workfront Planning Workspace-Manager können auch Anfragen und Anfrageentwürfe löschen, die sie nicht erstellt haben.

Sie können keine Planungsanfragen in der Legacy-Anfrageerfahrung anzeigen.

In diesem Artikel wird beschrieben, wie Sie Anfrageentwürfe in der neuen Anfrageerfahrung löschen können. Das Löschen von Workfront- und Planungsanfragen oder deren Entwürfen ist identisch.

Weitere Informationen finden Sie unter:

* [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [Erstellen von Anfragen aus Entwürfen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Senden von Anfragen zum Erstellen von Einträgen in Adobe Workfront-Planung](/help/quicksilver/planning/requests/submit-requests.md)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebiges Workfront- oder Workflow-Paket</p>

<p>Beliebiges Workfront-Planungspaket zum Verwalten von Planungsanfragen </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator oder Planning Workspace-Manager sein, um nicht erstellte Anfragen löschen zu können.</p><p>Sie müssen Bearbeitungszugriff auf Anfragen haben.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie müssen die Anfrage oder den Entwurf erstellt haben, um sie bzw. ihn in der neuen anfragenden Version zu löschen, oder Workfront-Administrator bzw. Planning Workspace-Manager sein, um Entwürfe von Anfragen zu löschen, die Sie nicht gesendet haben.
   </p><p>Sie müssen über Bearbeitungsberechtigungen für die Probleme verfügen, die Sie löschen möchten.</p>  </td> 
  </tr>

</tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Löschen von Anfragen oder Anfrageentwürfen in der neuen anfragenden -Version

Sie können Anfragen und Entwürfe in den folgenden Bereichen löschen:

* Im Bereich Anfragen von Workfront
* Im Widget Meine Anfragen auf der Startseite
* Von einer Anfrageseite aus

Die folgenden Benutzer können Anfrageentwürfe löschen:

* Workfront-Administratoren können von ihnen oder anderen übermittelte Anfragen und Entwürfe löschen.
* Workfront Planning Workspace-Manager können Anfragen und Entwürfe im Planning Workspace löschen, den sie verwalten.
* Benutzer können von ihnen gesendete Anfragen und Entwürfe löschen.

### Löschen einer Anfrage oder eines Entwurfs aus dem Bereich Anfragen oder dem Widget „Meine Anfragen“ auf der Startseite

{{step1-to-requests}}

1. So greifen Sie auf das **Meine Anfragen**-Widget in **Startseite** zu:

   {{step1-to-home}}

   1. Suchen Sie das **Meine Anfragen**-Widget.

      Weitere Informationen über das Widget **Meine Anfragen** finden Sie unter [Verwenden des Widgets Meine Anfragen](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Bewegen Sie in **Anfragen** Liste oder dem **Meine Anfragen**-Widget in **Startseite** den Mauszeiger über die Anfrage oder den Entwurf, die bzw. den Sie löschen möchten, und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png)

1. Klicken Sie auf **Löschen**

   ODER

   Klicken Sie mit der rechten Maustaste auf die ausgewählte Anfrage und dann auf **Löschen**.

   >[!TIP]
   >
   >Wenn Sie keinen Zugriff haben, um Probleme zu erstellen, erhalten Sie eine Warnung, dass Ihr Administrator Sie daran gehindert hat, Anfragen zu erstellen.

1. Klicken Sie im daraufhin angezeigten Dialogfeld auf **Löschen**.

   Anfrage oder Entwurf wird gelöscht.

   Gelöschte Anfragen werden im Papierkorb gespeichert und ein Workfront-Administrator kann sie bis zu 30 Tage lang wiederherstellen. Entwürfe können nicht wiederhergestellt werden.

### Massenlöschanfragen aus einer Liste

{{step1-to-requests}}

1. So greifen Sie auf das **Meine Anfragen**-Widget in **Startseite** zu:

   {{step1-to-home}}

   1. Suchen Sie das **Meine Anfragen**-Widget.

      Weitere Informationen zum Widget „Meine Anfragen“ finden Sie unter [Verwenden des Widgets „Meine Anfragen“](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Klicken Sie in **Anfragen** Liste oder dem **Meine Anfragen**-Widget links neben jeder Anfrage, die Sie löschen möchten, auf das Kästchen.
1. Klicken Sie in der blauen Leiste unten auf der Seite auf **Löschen**.

   >[!NOTE]
   >
   >Wenn die Option **Löschen** in der blauen Leiste nicht sichtbar ist, haben Sie keine Berechtigung zum Löschen einer oder mehrerer der ausgewählten Anfragen.

### Voraussetzungen für das Löschen von Anfrageentwürfen

Sie müssen Folgendes tun, bevor Sie einen Anfrageentwurf löschen können:

* Erstellen Sie eine Anfrage. Dadurch wird die Anfrage automatisch im Abschnitt Entwürfe als Entwurf gespeichert.

  Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Löschen von Anfrageentwürfen im alten anfordernden Erlebnis

Entworfene Anfragen können gelöscht werden, nachdem sie als Entwürfe gespeichert wurden, falls sie für Sie nicht mehr relevant sind. Gelöschte Entwurfsanfragen können nicht wiederhergestellt werden.

Sie können nicht auf Planungsanfragen oder deren Entwürfe aus dem alten anfordernden Erlebnis zugreifen.

{{step1-to-requests}}

1. Klicken **im linken** auf „Entwürfe“.

   In dieser Liste werden alle Entwürfe für alle Anforderungswarteschlangen angezeigt.

1. Wählen Sie einen Entwurf in der Liste aus und klicken **oben in** Liste auf „Löschen“.
1. Klicken Sie **Ja, löschen**.

   Der Entwurf wird gelöscht und kann nicht wiederhergestellt werden.






