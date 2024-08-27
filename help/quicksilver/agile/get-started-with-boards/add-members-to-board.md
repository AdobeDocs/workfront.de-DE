---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand
description: Personen müssen als Mitglieder zur Pinnwand hinzugefügt werden, bevor sie die Pinnwand anzeigen und Karten zugewiesen werden können.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand

Personen und Teams müssen als Mitglieder in die Pinnwand aufgenommen werden, bevor sie die Pinnwand anzeigen können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL Anforderung] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mitglieder zu einer Pinnwand hinzufügen

{{step1-to-boards}}

1. Erstellen Sie eine neue Pinnwand oder bearbeiten Sie eine vorhandene Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf das Symbol **[!UICONTROL Mitglied hinzufügen]** ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png).
1. Geben Sie im Feld **[!UICONTROL Mitglieder hinzufügen]** einen Namen ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   Sie können ein einzelnes Mitglied oder ein Team auswählen. Wenn Sie ein Team auswählen, wird das Team selbst zum Forum hinzugefügt.

   >[!NOTE]
   >
   >Einem einzelnen Benutzer muss die Option **[!UICONTROL Ansicht]** oder **[!UICONTROL Bearbeiten]** in seiner Zugriffsebene für Teams festgelegt sein, andernfalls kann er die Pinnwand nicht anzeigen.


   ![Mitglieder zur Pinnwand hinzufügen](assets/boards-add-members.png)

## Entfernen von Elementen aus einer Pinnwand

{{step1-to-boards}}

1. Erstellen Sie eine neue Pinnwand oder bearbeiten Sie eine vorhandene Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf das Symbol **[!UICONTROL Mitglied hinzufügen]** ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png).
1. Klicken Sie im Feld **[!UICONTROL Mitglieder hinzufügen]** auf das X neben einem Personen- oder Teamnamen, um sie aus der Pinnwand zu entfernen.

   ![Mitglied aus Pinnwand entfernen](assets/boards-remove-member-from-board-350x367.png)

   Wenn Sie ein Mitglied aus einer Pinnwand entfernen, werden diese nicht aus den Karten entfernt, denen es zugewiesen ist. Bei verbundenen Karten werden die Zuweisungen auch bei der Aufgabe bzw. dem Problem [!DNL Workfront] aktualisiert.

   Mitglieder werden nur aus diesem Gremium entfernt. Sie werden nicht aus anderen Pinnwänden entfernt, denen sie angehören.

   >[!NOTE]
   >
   >Sie können den Pinnwandbesitzer nicht entfernen.
