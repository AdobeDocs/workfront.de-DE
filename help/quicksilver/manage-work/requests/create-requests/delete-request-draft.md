---
product-area: requests
navigation-topic: create-requests
title: Löschen einer gesendeten Anfrage als Entwurf einer Anfrage
description: Sie können gesendete Anfragen oder Anfrageentwürfe löschen.
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 3%

---

# Löschen einer gesendeten Anfrage oder eines Anfrageentwurfs

Sie können gesendete Anfragen oder Anfrageentwürfe löschen, die Sie in der neuen Anfrageerfahrung erstellt haben. Workfront-Administratoren und Planning Workspace-Administratoren können Anfragen auch löschen.

Im alten anfordernden Erlebnis können Sie Anfrageentwürfe löschen. Gesendete Anfragen können nicht gelöscht werden.

Weitere Informationen finden Sie unter:

* [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [Anforderungen aus Entwürfen erstellen](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator oder Planning Workspace-Administrator sein, um nicht erstellte Anfragen löschen zu können.</p><p>Sie müssen Bearbeitungszugriff auf Anfragen haben, um Entwürfe aus der Legacy-Version zu löschen, die Anfragen stellt.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie müssen die Anfrage oder den Entwurf erstellt haben, um sie bzw. ihn in der neuen anfragenden -Version zu löschen.</p><p>Sie müssen Bearbeitungszugriff auf Anfragen haben, um Entwürfe aus der Legacy-Version zu löschen, die Anfragen stellt.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen von Anfragen oder Anfrageentwürfen in der neuen anfragenden -Version

Sie können Anfragen im Bereich Anfragen von Workfront oder im Widget Meine Anfragen auf der Startseite löschen.

* Workfront-Administratoren können Anfragen und Entwürfe in ihrer Organisation löschen.
* Workfront Planning Workspace-Administratoren können Anfragen und Entwürfe im Planning Workspace löschen, den sie verwalten.
* Benutzer können von ihnen gesendete Anfragen und Entwürfe löschen.

### Löschen einer Anforderung aus dem Dreipunkt-Menü

{{step1-to-requests}}

1. So greifen Sie auf die Startseite auf das Widget Meine Anfragen zu:

   {{step1-to-home}}

   1. Suchen Sie das Widget Meine Anfragen .

      Weitere Informationen zum Widget „Meine Anfragen“ finden Sie unter [Verwenden des Widgets „Meine Anfragen“](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Bewegen Sie in der **Anfragen** Liste oder dem **Meine Anfragen** Widget auf der Startseite den Mauszeiger über die Anfrage oder den Entwurf, die bzw. den Sie löschen möchten, und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png)

1. Klicken Sie auf **Löschen**

   ODER

   Klicken Sie mit der rechten Maustaste auf die ausgewählte Anfrage und dann auf **Löschen**.

   >[!TIP]
   >
   >Wenn Sie keinen Zugriff haben, um Probleme zu erstellen, erhalten Sie eine Warnung, dass Ihr Administrator Sie daran gehindert hat, Anfragen zu erstellen.

1. Klicken Sie im daraufhin angezeigten Dialogfeld auf **Löschen**.

   Anfrage oder Entwurf wird gelöscht.

### Massenlöschanfragen

{{step1-to-requests}}

1. So greifen Sie auf die Startseite auf das Widget Meine Anfragen zu:

   {{step1-to-home}}

   1. Suchen Sie das Widget Meine Anfragen .

      Weitere Informationen zum Widget „Meine Anfragen“ finden Sie unter [Verwenden des Widgets „Meine Anfragen“](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Klicken Sie in der Anfragenliste oder im Widget Meine Anfragen auf das Feld links neben jeder Anfrage, die Sie löschen möchten.
1. Klicken Sie in der blauen Leiste unten auf der Seite auf **Löschen**.

   >[!NOTE]
   >
   >Wenn die Option Löschen in der blauen Leiste nicht sichtbar ist, haben Sie nicht die Berechtigung, eine oder mehrere der ausgewählten Anfragen zu löschen.

</div>

## Löschen von Anfrageentwürfen im alten anfordernden Erlebnis

Entworfene Anfragen können gelöscht werden, nachdem sie als Entwürfe gespeichert wurden, falls sie für Sie nicht mehr relevant sind. Gelöschte Entwurfsanfragen können nicht wiederhergestellt werden.

### Voraussetzungen für das Löschen von Anfrageentwürfen

Sie müssen Folgendes tun, bevor Sie einen Anfrageentwurf löschen können:

* Erstellen Sie eine Anfrage. Dadurch wird die Anfrage automatisch im Abschnitt Entwürfe als Entwurf gespeichert.

  Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

### Löschen eines Anfrageentwurfs

{{step1-to-requests}}

1. Wählen **Entwürfe** im linken Bedienfeld aus.

   In dieser Liste werden alle Entwürfe für alle Anforderungswarteschlangen angezeigt.

1. (Optional) Klicken Sie **Nach Anfragetyp filtern** in der rechten oberen Ecke der Entwurfsliste und wählen Sie dann die Anfragewarteschlange aus, die die Entwürfe enthält, die Sie anzeigen möchten.
1. Wählen Sie einen Entwurf in der Liste aus und klicken **oben in** Liste auf „Löschen“.
1. Klicken Sie **Ja, löschen**.

   Der Entwurf wird gelöscht und kann nicht wiederhergestellt werden.
