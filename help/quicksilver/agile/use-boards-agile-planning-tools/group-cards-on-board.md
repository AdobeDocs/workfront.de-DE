---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Gruppen auf einer Pinnwand verwenden
description: Sie können Karten auf einer Pinnwand nach Verantwortlichen oder Tag gruppieren. Wenn Sie eine Gruppierungsoption auswählen, werden die Karten im Swimlane-Format angezeigt.
author: Lisa
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Gruppen auf einer Pinnwand verwenden

Sie können Karten auf einer Pinnwand nach Verantwortlichen oder Tag gruppieren. Wenn Sie eine Gruppierungsoption auswählen, werden die Karten im Swimlane-Format angezeigt. Nicht zugewiesene Karten oder Karten ohne Tags werden in ihrer eigenen Swimlane angezeigt.

>[!NOTE]
>
>Alle Karten in der Ansaugspalte sind nicht in einer Gruppe enthalten, und die Ansauspalte wird ausgeblendet, wenn eine Gruppe angewendet wird. Informationen zur Ansauspalte finden Sie unter [Hinzufügen einer Ansauspalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

## Gruppieren von Karten auf einer Pinnwand

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf **[!UICONTROL Gruppe]** , um den Gruppenbereich links auf der Pinnwand zu öffnen.

   >[!NOTE]
   >
   >Die Standardeinstellung für die Gruppierung nach ist **[!UICONTROL None]**. Sie können diese Option jederzeit auswählen, um eine Gruppe zu entfernen und nur die Spalten auf der Pinnwand anzuzeigen.

1. Um die Karten zu gruppieren, wählen Sie **[!UICONTROL Zuweisungen]** oder **[!UICONTROL Tags]** aus.

   Die Karten werden automatisch gruppiert. Klicken Sie auf den Pfeil neben dem Gruppennamen, um die Gruppe zu reduzieren und zu erweitern.

   ![Gruppierte Karten auf einer Pinnwand](assets/group-by-assignee.png)

1. Wählen Sie aus, was passiert, wenn eine Karte in eine andere Gruppe verschoben wird.

   * **[!UICONTROL Auf Bevollmächtigten hinzufügen] / [!UICONTROL Auf Tags hinzufügen]:** Die Bevollmächtigten oder Tags in der neuen Gruppe werden der vorhandenen Liste der Bevollmächtigten oder Tags auf der Karte hinzugefügt.
   * **[!UICONTROL Zuweisung überschreiben] / [!UICONTROL Tags überschreiben]:** Die Bevollmächtigten oder Tags in der neuen Gruppe überschreiben alle anderen Bevollmächtigten oder Tags und werden zu den einzigen Bevollmächtigten oder Tags auf der Karte.

   ![[!UICONTROL Nach Optionen gruppieren]](assets/group-by-rail.png)

1. Klicken Sie auf **[!UICONTROL Gruppen ausblenden]** , um das Gruppenbedienfeld auszublenden und die gesamte Pinnwand anzuzeigen.
