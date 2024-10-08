---
content-type: reference
navigation-topic: boards
title: Migrieren von Agile Team Kanban Cards zu Workfront-Pinnwänden
description: Sie können Ihre Arbeitselemente von einem agilen Team Kanban Board zu einem neuen oder vorhandenen Workfront Board migrieren.
author: Lisa
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Migrieren von agilen Teams Kanban-Karten zu Workfront-Pinnwänden

Sie können Ihre Arbeitselemente von einem agilen Team Kanban Board zu einem neuen oder vorhandenen Workfront Board migrieren. Wenn Sie die Migration ausführen, werden alle Karten auf der Kanban-Pinnwand in die Workfront-Pinnwand kopiert. Es ist nicht erlaubt, bestimmte Karten auszuwählen.

Die Platzierung von Karten auf der Workfront-Pinnwand basiert auf Spaltenrichtlinien. (Beispielsweise könnte eine Richtlinie alle Karten mit dem Status &quot;Wird ausgeführt&quot;in eine bestimmte Spalte verschieben. Weitere Informationen zu Spaltenrichtlinien finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).) Wenn es keine Richtlinien gibt oder die Karten nicht mit den Richtlinien übereinstimmen, werden die Karten in der Spalte ganz links auf der Pinnwand platziert. Derzeit werden die Karten in der Spalte &quot;Backlog&quot;auf der alten Pinnwand nicht zur Workfront-Pinnwand hinzugefügt.

Die Karten werden nicht aus dem agilen Team Kanban Board entfernt, und Kartenstatusänderungen werden mit beiden Pinnwänden synchronisiert. Sie können beide Pinnwände aktiv halten, bis Sie zum Wechsel zu Workfront-Pinnwänden bereit sind.

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

## Kanban-Karten auf eine neue Pinnwand migrieren

{{step1-to-team}}

1. Greifen Sie auf ein Kanban-Board zu.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie [!UICONTROL **Neue Pinnwand**] aus.
1. Geben Sie im Dialogfeld [!UICONTROL Zur neuen Pinnwand hinzufügen] einen Namen für die neue Pinnwand ein (der Name der aktuellen Pinnwand [!UICONTROL Kanban] wird automatisch angezeigt) und klicken Sie auf [!UICONTROL **Hinzufügen**].

   ![Hinzufügen von Kanban-Karten zur neuen Pinnwand](assets/add-kanban-cards-to-new-board-dialog.png)

1. (Optional) Klicken Sie in der angezeigten Erfolgsmeldung auf den Link, um die neue Pinnwand zu öffnen.

## Kanban-Karten auf eine vorhandene Pinnwand migrieren

{{step1-to-team}}

1. Greifen Sie auf ein Kanban-Board zu.
1. Klicken Sie auf [!UICONTROL **Zu Pinnwänden hinzufügen**] und wählen Sie [!UICONTROL **Vorhandene Pinnwand**] aus.
1. Suchen Sie im Dialogfeld [!UICONTROL Zu vorhandener Pinnwand hinzufügen] nach der Pinnwand, auf die die Karten migriert werden sollen, und wählen Sie sie aus. Klicken Sie dann auf [!UICONTROL **Hinzufügen**].

   ![Hinzufügen von Kanban-Karten zur vorhandenen Pinnwand](assets/add-kanban-cards-to-existing-board-dialog.png)

1. (Optional) Klicken Sie in der angezeigten Erfolgsmeldung auf den Link, um die Pinnwand zu öffnen.
