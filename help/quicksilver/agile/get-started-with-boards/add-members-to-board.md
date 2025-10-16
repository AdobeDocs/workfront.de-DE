---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Mitglieder zu einer Pinnwand hinzufügen oder daraus entfernen
description: Personen müssen der Pinnwand als Mitglieder hinzugefügt werden, bevor sie die Pinnwand anzeigen und Karten zugewiesen werden können.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Mitglieder zu einer Pinnwand hinzufügen oder daraus entfernen

Personen und Teams müssen dem Board als Mitglieder hinzugefügt werden, bevor sie das Board anzeigen können.

Der Ersteller einer Pinnwand ist standardmäßig der Besitzer. Der Board-Besitzer ist die einzige Person, die diese Pinnwand löschen oder ihre Filter im Bedienfeld „Konfigurieren“ aktualisieren kann. Nur ein Systemadministrator oder der aktuelle Board-Eigentümer kann den Board-Eigentümer ändern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mitglieder zu einer Pinnwand hinzufügen

{{step1-to-boards}}

1. Eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf **[!UICONTROL Symbol]** Mitglied hinzufügen![ (Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png).
1. Beginnen Sie im Feld **[!UICONTROL Mitglieder hinzufügen]** mit der Eingabe eines Namens und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   Sie können ein einzelnes Mitglied oder ein Team auswählen. Wenn Sie ein Team auswählen, wird das Team selbst der Pinnwand hinzugefügt.

   >[!NOTE]
   >
   >Für einen einzelnen Benutzer muss die Option **[!UICONTROL Anzeigen]** oder **[!UICONTROL Bearbeiten]** in der Zugriffsebene für Teams festgelegt sein, da er sonst das Board nicht anzeigen kann.


   ![Mitglieder zu Pinnwand hinzufügen](assets/boards-add-members.png)

## Mitglieder aus einer Pinnwand entfernen

{{step1-to-boards}}

1. Eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf **[!UICONTROL Symbol]** Mitglied hinzufügen![ (Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png).
1. Klicken Sie im Feld **[!UICONTROL Mitglieder hinzufügen]** auf das X neben dem Namen einer Person oder eines Teams, um sie aus der Pinnwand zu entfernen.

   ![Mitglied aus der Pinnwand entfernen](assets/boards-remove-member-from-board-350x367.png)

   Wenn Sie ein Mitglied aus einer Pinnwand entfernen, wird es nicht aus den Karten entfernt, denen es zugewiesen ist. Bei verbundenen Karten werden die Zuweisungen auch bei der [!DNL Workfront] Aufgabe oder dem Problem aktualisiert.

   Mitglieder werden nur aus dieser Pinnwand entfernt. Sie werden nicht von anderen Boards entfernt, denen sie angehören.

   >[!NOTE]
   >
   >Sie können den Board-Besitzer nicht entfernen.

## Pinnwand-Besitzer ändern

>[!NOTE]
>
>Nur ein Systemadministrator oder der aktuelle Board-Eigentümer kann den Board-Eigentümer ändern. Ein Board kann nur einen Besitzer haben.
>
>Die Möglichkeit, den Boardbesitzer zu ändern, ist auf grundlegenden, retrospektiven und Kanban-Boards verfügbar, nicht aber auf dynamischen Boards.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das **[!UICONTROL Mehr]** Menü ![Mehr](assets/more-icon-spectrum.png) neben dem Board-Namen und wählen Sie dann **[!UICONTROL Board-Inhaber ändern]**.
1. Suchen Sie im Dialogfeld Pinnwand-Inhaber ändern nach dem Benutzer, den Sie zum Besitzer machen möchten, und wählen Sie ihn aus.

   Sie können nicht nach Benutzern suchen, die bereits Mitglieder im Board sind. Um ein vorhandenes Mitglied zum Besitzer zu machen, müssen Sie es zunächst aus dem Board entfernen. Wenn Sie einen Benutzer zum Besitzer des Boards machen, wird dieser dem Board hinzugefügt.

   Nur ein Benutzer kann Besitzer des Boards sein. Ein Team kann kein Besitzer sein.

1. Klicken Sie auf [!UICONTROL **Aktualisieren**].
