---
content-type: reference
navigation-topic: boards
title: Agile-Team-Kanban-Karten zu Workfront-Boards migrieren
description: Sie können Ihre Arbeitselemente von einem Agile-Team-Kanban-Board auf ein neues oder vorhandenes Workfront-Board migrieren.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Migrieren von Agile-Team-Kanban-Karten zu Workfront-Boards

Sie können Ihre Arbeitselemente von einem Agile-Team-Kanban-Board auf ein neues oder vorhandenes Workfront-Board migrieren. Wenn Sie die Migration ausführen, werden alle Karten auf der Kanban-Pinnwand in die Workfront-Pinnwand kopiert. Es ist nicht erlaubt, bestimmte Karten auszuwählen.

Die Platzierung von Karten auf der Workfront-Pinnwand basiert auf Spaltenrichtlinien. (Eine Richtlinie kann beispielsweise alle Karten mit dem Status „In Bearbeitung“ in eine bestimmte Spalte verschieben. Weitere Informationen zu Spaltenrichtlinien finden Sie unter [Pinnwand-Spalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Wenn keine Richtlinien vorhanden sind oder die Karten nicht mit den Richtlinien übereinstimmen, werden die Karten in der Spalte ganz links auf der Pinnwand platziert. Derzeit werden die Karten in der Spalte „Rückstand“ auf der alten Pinnwand nicht zur Workfront-Pinnwand hinzugefügt.

Die Karten werden nicht aus dem Kanban-Board des Agile-Teams entfernt, und Änderungen des Kartenstatus werden mit beiden Boards synchronisiert. Sie können beide Pinnwände aktiviert lassen, bis Sie bereit sind, zu Workfront-Pinnwänden zu wechseln.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL -Anfrage] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Kanban-Karten auf eine neue Pinnwand migrieren

{{step1-to-team}}

1. Zugriff auf ein Kanban-Board.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie [!UICONTROL **Neue Pinnwand**] aus.
1. Geben Sie im [!UICONTROL Zu neuer Pinnwand hinzufügen] einen Namen für die neue Pinnwand ein (der Name der aktuellen [!UICONTROL Kanban]-Pinnwand wird automatisch angezeigt) und klicken Sie auf [!UICONTROL **Hinzufügen**].

   ![Kanban-Karten zu neuer Pinnwand hinzufügen](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Optional) Klicken Sie auf der angezeigten Erfolgsmeldung auf den Link, um das neue Board zu öffnen.

## Kanban-Karten zu einer vorhandenen Pinnwand migrieren

{{step1-to-team}}

1. Zugriff auf ein Kanban-Board.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie &quot;[!UICONTROL **Pinnwand“**].
1. Suchen Sie im Dialogfeld [!UICONTROL Zu vorhandener Pinnwand hinzufügen] nach der Pinnwand, auf die die Karten migriert werden sollen, und wählen Sie diese aus. Klicken Sie dann auf [!UICONTROL **Hinzufügen**].

   ![Kanban-Karten zu vorhandener Pinnwand hinzufügen](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Optional) Klicken Sie auf der angezeigten Erfolgsmeldung auf den Link, um das Board zu öffnen.
