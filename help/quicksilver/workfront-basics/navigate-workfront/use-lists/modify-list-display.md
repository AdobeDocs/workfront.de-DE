---
navigation-topic: use-lists
title: Ändern der Anzeige einer Liste
description: In [!DNL Adobe Workfront] können Sie anpassen, wie eine Liste für Sie angezeigt wird. Andere Benutzer, die die Liste anzeigen, sehen Ihre Änderungen nicht.
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Ändern der Anzeige einer Liste

<!--Audited: 11/2024-->

In [!DNL Adobe Workfront] können Sie anpassen, wie eine Liste für Sie angezeigt wird. Andere Benutzer, die die Liste anzeigen, sehen Ihre Änderungen nicht.

Sie können die folgenden Anpassungen vornehmen:

* Die Anzahl der angezeigten Elemente
* Spaltenbreite oder -reihenfolge
* Ob Gruppierungen erweitert oder reduziert werden

>[!NOTE]
>
>Die obigen Änderungen an der Anzeige, die Sie vornehmen, werden rückgängig gemacht, wenn Sie sich von [!DNL Workfront] abmelden oder Ihren Browser schließen. Diese Veränderungen können auch nach einem Zeitraum von 8 Stunden rückgängig gemacht werden.

Zusätzlich zu den oben genannten temporären Anpassungen können Sie auch anpassen, nach welchen Spalten die Liste sortiert, wobei der [!DNL Workfront] auch nach dem Abmelden oder Schließen des Browsers beibehalten wird. Wenn jedoch jemand die Sortieroptionen in der Ansicht einer Liste bearbeitet, wird die vorherige Sortierauswahl nicht beibehalten.

Informationen zum Ändern der in Ihrer Liste angezeigten Informationen finden Sie unter [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender oder höher </p></li>
   </ul>

<p>Aktuell:</p>
   <ul><li><p>Anfrage oder höher</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL View] Zugriff auf den Bereich der Liste</p> <p>Um beispielsweise die Ansicht in einem Projekt zu ändern, benötigen Sie [!UICONTROL View]-Zugriff auf Projekte.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für die Ansicht, die auf die Liste angewendet wird</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Liste ändern

1. Navigieren Sie zur Liste in [!DNL Workfront], die Sie ändern möchten.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Optional und bedingt) Wenn die Gruppierungen in der Liste reduziert sind und Sie weitere Informationen anzeigen möchten, klicken Sie auf die gewünschte Gruppierung, um die Liste zu erweitern und die darin aufgeführten Informationen anzuzeigen.

   Oder

   Um alle Gruppierungen zu erweitern, klicken Sie auf den Pfeil rechts neben dem Kontrollkästchen in der Spaltenüberschrift.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Optional und bedingt) Wenn Sie eine bestimmte Anzahl von Elementen auf dem Bildschirm anzeigen möchten, klicken Sie auf das **[!UICONTROL Anzeigen]** Dropdown-Menü in der rechten unteren Ecke des Bildschirms und wählen Sie dann die Anzeige von **100**, **250**, **500**, **[!UICONTROL Alle]** oder **2000** Elementen aus.

   ![Listennummer auf Seite](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >Standardmäßig werden 2.000 Elemente für aktualisierte Listen und 100 Elemente für ältere Listen angezeigt. Wenn die Liste mehr als 2.000 Elemente enthält, können Sie nicht alle Elemente auf einer Seite anzeigen.
   >
   >
   >Zur Erzielung einer optimalen Leistung bei großen Listen, in denen Objekte formatierte Textfelder enthalten, wird empfohlen, diese Zahl auf 250 zu beschränken.
   >
   >
   >Weitere Informationen zu den beiden Listentypen finden Sie im Abschnitt [Der Unterschied zwischen den aktualisierten und den alten Listen](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) im Artikel [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Die Ergebnisse Ihrer Liste werden paginiert, um die ausgewählte Anzahl von Elementen pro Seite anzuzeigen. Sie können auf die Ergebnisse auf anderen Seiten zugreifen, indem Sie auf die Rückwärts- und Vorwärtspfeile klicken oder eine bestimmte Seite auswählen.

1. Um die Breite einer Spalte zu ändern, bewegen Sie den Mauszeiger über die Trennlinie zwischen zwei Spalten und klicken Sie dann, um sie auf die gewünschte Breite zu ziehen.

   Die Größe der Spalte wird geändert, bis Sie den Cache im Browser löschen oder die Größe manuell ändern.

1. Um die Spalten in einer Liste neu anzuordnen, bewegen Sie den Mauszeiger über eine Spaltenüberschrift, um das Handwerkzeug anzuzeigen, und ziehen Sie dann die Spalte an die Position, an der sie angezeigt werden soll.

   Die Position der Spalte wird gespeichert, bis Sie die Seite aktualisieren.

   Weitere Informationen zum Anpassen der Breite und Reihenfolge der Spalten in einer Liste finden Sie im Artikel [Ändern der Spaltenbreite und -reihenfolge](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Um die Sortierreihenfolge einer Liste anzupassen, klicken Sie auf eine Spaltenüberschrift, um sie auszuwählen. Halten Sie dann die Befehlstaste ([!DNL Mac]) oder die Strg-Taste ([!DNL Windows]) gedrückt und wählen Sie bis zu zwei zusätzliche Spaltenüberschriften aus, um sie zu sortieren.

   Die Liste wird nach den ausgewählten Spalten in der Reihenfolge Ihrer Auswahl sortiert.

   Alle Änderungen, die Sie an der Liste vornehmen, werden sofort gespeichert.

   >[!NOTE]
   >
   >Wenn Sie Gruppen im Bereich [!UICONTROL Gruppen] in [!UICONTROL Setup] sortieren, wird die Hierarchieansicht der Gruppen und ihrer Untergruppen nicht unterbrochen, wenn Sie die Art der Sortierung der Liste ändern - Untergruppen verbleiben bei ihren übergeordneten Gruppen. Die Liste wird zuerst nach Gruppen der obersten Ebene sortiert. Anschließend wird unter jeder übergeordneten Gruppe die Liste der Untergruppen, die sich auf derselben Ebene befinden, zusammen sortiert.
