---
navigation-topic: use-lists
title: Anzeige einer Liste ändern
description: In [!DNL Adobe Workfront] können Sie anpassen, wie eine Liste für Sie angezeigt wird. Andere Benutzer, die die Liste anzeigen, sehen Ihre Änderungen nicht.
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# Anzeige einer Liste ändern

In [!DNL Adobe Workfront] können Sie anpassen, wie eine Liste für Sie angezeigt wird. Andere Benutzer, die die Liste anzeigen, sehen Ihre Änderungen nicht.

Sie können die folgenden Anpassungen vornehmen:

* Die Anzahl der angezeigten Elemente
* Spaltenbreite oder -anordnung
* Ob Gruppierungen erweitert oder reduziert werden

>[!NOTE]
>
>Die obigen Änderungen der Anzeige werden zurückgesetzt, wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen. Diese Änderungen können auch nach einem Zeitraum von 8 Stunden rückgängig gemacht werden.

Zusätzlich zu den oben genannten temporären Anpassungen können Sie auch anpassen, nach welchen Spalten die Liste sortiert wird und welche [!DNL Workfront] auch nach dem Abmelden oder Schließen des Browsers beibehalten wird. Wenn jedoch jemand die Sortieroptionen in der Ansicht einer Liste bearbeitet, wird die vorherige Sortierungsauswahl nicht beibehalten.

Informationen zum Ändern der in Ihrer Liste angezeigten Informationen finden Sie unter [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf den Bereich, in dem sich die Liste befindet</p> <p>Um beispielsweise die Ansicht eines Projekts zu ändern, benötigen Sie Zugriff auf die [!UICONTROL Ansicht] auf Projekte.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.<br>Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebene erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für die Ansicht, die auf die Liste angewendet wird</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeige einer Liste ändern

1. Rufen Sie die Liste in [!DNL Workfront] auf, die Sie ändern möchten.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Optional und bedingt) Wenn die Gruppierungen in der Liste ausgeblendet sind und Sie weitere Informationen anzeigen möchten, klicken Sie auf die gewünschte Gruppierung, um die Liste zu erweitern und die darin aufgelisteten Informationen anzuzeigen.

   Oder

   Um alle Gruppierungen zu erweitern, klicken Sie in der Spaltenüberschrift auf den Pfeil rechts neben dem Kontrollkästchen.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Optional und bedingt) Wenn Sie eine bestimmte Anzahl von Elementen auf dem Bildschirm anzeigen möchten, klicken Sie auf das Dropdown-Menü **[!UICONTROL Anzeigen]** in der rechten unteren Ecke des Bildschirms und wählen Sie dann die Anzeige **100**, **250**, **500**, **[!UICONTROL Alle]** oder **20 00** Elemente.

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >Standardmäßig werden 2.000 Elemente für aktualisierte Listen und 100 Elemente für veraltete Listen angezeigt. Wenn die Liste mehr als 2.000 Elemente enthält, können Sie nicht alle Elemente auf einer Seite anzeigen.
   >
   >
   >Für eine optimale Leistung bei großen Listen, in denen Objekte formatierte Textfelder enthalten, empfehlen wir, diese Zahl auf 250 zu begrenzen.
   >
   >
   >Weitere Informationen zu den beiden Listentypen finden Sie im Abschnitt [Der Unterschied zwischen der aktualisierten und der alten Liste](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) im Artikel [Erste Schritte mit Listen in  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Die Ergebnisse Ihrer Liste werden paginiert, um die ausgewählte Anzahl von Elementen pro Seite anzuzeigen. Sie können auf die Ergebnisse auf anderen Seiten zugreifen, indem Sie auf die Pfeile nach hinten und nach vorne klicken oder eine bestimmte Seite auswählen.

1. Um die Breite einer Spalte zu ändern, bewegen Sie den Mauszeiger über die Zeile, die zwei Spalten trennt, und klicken Sie dann auf , um sie auf die gewünschte Breite zu ziehen.

   Die Größe der Spalte wird geändert, bis Sie den Cache im Browser löschen oder die Größe manuell ändern.

1. Um die Spalten in einer Liste neu anzuordnen, halten Sie den Mauszeiger über eine Spaltenüberschrift, um das Handwerkzeug anzuzeigen, und klicken Sie dann auf , um die Spalte an die gewünschte Position zu ziehen.

   Die Position der Spalte wird gespeichert, bis Sie die Seite aktualisieren.\
   Weitere Informationen zum Anpassen der Breite und Reihenfolge der Spalten in einer Liste finden Sie im Artikel [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Um die Sortierreihenfolge einer Liste anzupassen, klicken Sie auf eine Spaltenüberschrift, um sie auszuwählen. Halten Sie dann die CMD-Taste (bei [!DNL Mac]) oder die STRG-Taste (bei [!DNL Windows]) auf der Tastatur gedrückt und wählen Sie bis zu 2 zusätzliche Spaltenüberschriften aus, um nach ihnen zu sortieren.

   Die Liste wird nach den ausgewählten Spalten in der Reihenfolge der Auswahl sortiert.

   Alle Änderungen an der Liste werden sofort gespeichert.

   >[!NOTE]
   >
   >Wenn Sie Gruppen im Bereich [!UICONTROL Gruppen] in der [!UICONTROL Einrichtung] sortieren, wird die Hierarchieansicht von Gruppen und deren Untergruppen nicht aufgeschlüsselt, wenn Sie die Sortierung der Liste ändern. Untergruppen bleiben bei ihren übergeordneten Gruppen. Die Liste wird zuerst nach Gruppen der obersten Ebene sortiert. Anschließend wird unter jeder übergeordneten Gruppe die Liste der Untergruppen auf derselben Ebene sortiert.
