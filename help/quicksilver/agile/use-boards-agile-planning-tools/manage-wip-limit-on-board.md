---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Verwalten der Grenze für laufende Arbeiten (WIP) auf einer Pinnwand
description: Sie können für jede Spalte auf einer Pinnwand eine Grenze für laufende Arbeit (Work In Progress, WIP) konfigurieren.
author: Lisa
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Verwalten der Beschränkung [!UICONTROL Laufende Arbeit] (WIP) auf einer Pinnwand

Sie können für jede Spalte auf einer Pinnwand eine Beschränkung für [!UICONTROL laufende Arbeit] (WIP) konfigurieren.

Die WIP-Beschränkung ist lediglich eine visuelle Warnung und schränkt nicht ein, dass in jeder Spalte mehr Elemente vorhanden sind als in der von Ihnen festgelegten Begrenzung.

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

## Setzen der WIP-Beschränkung auf eine Spalte

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Suchen Sie die Spalte, der Sie die WIP-Beschränkung hinzufügen möchten.

   Informationen zum Hinzufügen einer neuen Spalte finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]** aus, um den Einstellungsbereich zu öffnen.
1. Aktivieren Sie unter [!UICONTROL Spaltenrichtlinien] die Richtlinie **[!UICONTROL Laufende Arbeit] - Limit** , um die Anzahl der Karten zu begrenzen, die der Spalte hinzugefügt werden können.
1. Geben Sie die Höchstzahl in das Feld **[!UICONTROL Begrenzung festlegen]** ein.

   ![WIP-Limit für Spalte](assets/boards-wip-limit-in-column.png)

   Die Anzahl der Karten und die Begrenzung werden oben in der Spalte angezeigt. Wenn die Spalte mehr Karten enthält als das Limit, wird der Zähler rot.

   ![WIP-Grenzwert-Zähler](assets/boards-wip-limit-counter.png)

1. Klicken Sie auf **[!UICONTROL Schließen]** , um den Bereich [!UICONTROL Einstellungen] zu verlassen und die Spalte und deren Karten anzuzeigen.
