---
navigation-topic: use-lists
title: Anwenden des Schnellfilters auf eine Liste
description: Sie können den Schnellfilter in einer Liste von Objekten verwenden, um nur Elemente zu finden, die für Sie wichtig sind, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.
feature: Get Started with Workfront
author: Nolan
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# Anwenden des Schnellfilters auf eine Liste

<!--Audited:11/2024-->

Sie können den Schnellfilter in einer Liste von Objekten verwenden, um nur Elemente zu finden, die für Sie wichtig sind, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.

>[!IMPORTANT]
>
>Sie können Elemente, die ein Suchwort enthalten, mithilfe von Schnellfiltern finden, unabhängig davon, ob dieses Element physisch auf Ihrem Bildschirm angezeigt wurde oder angezeigt wird, nachdem Sie zum Seitenende gescrollt haben. Wenn Sie die Suchfunktionen Ihres Browsers verwenden, können Sie nur Elemente finden, die physisch auf dem Bildschirm angezeigt werden. Wenn Ihre Liste mehrere Seiten umfasst, finden Schnellfilter keine Elemente auf Seiten, die nicht angezeigt werden.

Wenn Sie einen Schnellfilter speichern möchten, empfehlen wir, stattdessen einen permanenten Filter für Ihre Liste zu erstellen.\
Informationen zum Erstellen von Filtern in [!DNL Adobe Workfront] finden Sie im Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Der Schnellfilter ist derzeit in den folgenden Bereichen verfügbar


Temporäre Schnellfilter können in allen Listen mit Ausnahme der folgenden verwendet werden:

* Der Bereich [!UICONTROL Berichte]
* Dokumentlisten und Berichte
* Mehrere [!UICONTROL Setup]-Bereiche

  >[!NOTE]
  >
  >Schnellfilter sind in den folgenden Einrichtungsbereichen verfügbar: [!UICONTROL Gruppen], [!UICONTROL Teams], [!UICONTROL Firmen], [!UICONTROL Zeitpläne], [!UICONTROL Layout-Vorlagen] und [!UICONTROL Custom Forms].


Beachten Sie beim Anwenden von Schnellfiltern auf eine Liste Folgendes:

* Sie können Keywords verwenden, um nach allen Feldern zu filtern, die in der Ansicht der Liste angezeigt werden. Dazu gehören benutzerdefinierte Felder oder komplexe Felder wie [!UICONTROL Vorgänger], [!UICONTROL Arbeitsaufträge], [!UICONTROL Arbeitsauftrag] und [!UICONTROL Status], [!UICONTROL Genehmiger] und [!UICONTROL Status] usw.
* Wenn Ihre Liste reduzierte Gruppierungen enthält, werden diese automatisch erweitert, wenn Sie Schnellfilter verwenden. Wenn Sie den Schnellfilter entfernen, werden die Gruppierungen erneut reduziert.
* Gruppierungen behalten die aggregierten Informationen der ursprünglichen Liste bei, unabhängig von den angewendeten Schnellfiltern oder vorgenommenen Änderungen an den Objekten auf der Liste.
* Schnellfilter sind temporär. Wenn Sie Gruppierung, Ansicht, Filter oder Sortierung der Liste ändern, werden die Schnellfilterkriterien entfernt.
* Schnellfilter können nicht gespeichert werden. Wenn Sie einen Filter speichern möchten, um ihn erneut zu verwenden, sollten Sie einen permanenten Filter für die Liste erstellen.
* Wenn die Liste mehr als eine Gruppierung enthält und der Schnellfilter Elemente in nur einer Gruppierung findet, wird nur diese Gruppierung mit den gefundenen Elementen angezeigt. Alle anderen Gruppierungen sind ausgeblendet.
* In einer Aufgaben- oder Teilaufgabenliste wird die Aufgabenhierarchie entfernt, wenn die Ergebnisse des Schnellfilters angezeigt werden.

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
   <td> <p>Zugriff auf den Bereich anzeigen, in dem sich die Liste befindet</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View]-Berechtigungen für das Objekt, in dem sich die Liste befindet</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Anwenden eines Schnellfilters auf eine Liste

1. Navigieren Sie zu einer Liste oder einem Bericht, die bzw. der Schnellfilter unterstützt, und klicken Sie **[!UICONTROL der Symbolleiste auf &#x200B;]Schnellfilter** Symbol ![Schnellfilter](assets/qs-quick-filter-icon.png)Symbol .

   Oder

   Drücken Sie je nach Betriebssystem oder Browser und bei Verwendung einer Standard-QWERTY-Tastatur die folgenden Befehle, um den Schnellfilter zu starten:

   * ALT+F für [!DNL Windows] Computer
   * ALT/Wahltaste+F für [!DNL Mac] Computer

     >[!TIP]
     >
     >Wenn Sie Strg+F bzw. Befehl+F drücken, wird neben dem Schnellfilter eine QuickInfo angezeigt, die Sie an diese Befehle erinnert. Die Befehle werden auch im Feld Schnellfilter-Suche angezeigt.

1. Geben **[!UICONTROL im Feld]** das Keyword ein, nach dem Sie filtern möchten.

   Sie können jedes Wort verwenden, das derzeit in der Listenansicht angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie ein Wort verwenden, das möglicherweise auf einer anderen Seite der Liste angezeigt wird, findet der Schnellfilter keine Ergebnisse.

   Eine Liste von Elementen, die den Suchkriterien entsprechen, wird beim Eingeben dynamisch in der Liste angezeigt, und alle anderen Elemente werden ausgeblendet. Das für die Suche verwendete Keyword ist in allen eigenständigen und komplexen Feldern gelb hervorgehoben. Einige Beispiele für komplexe Felder sind freigegebene Spalten oder eine der folgenden: [!UICONTROL Arbeitsaufträge], [!UICONTROL Arbeitsaufträge] und [!UICONTROL Status], [!UICONTROL Prozent abgeschlossen], [!UICONTROL Vorgänger], [!UICONTROL Genehmiger und Status], [!UICONTROL Ressourcenmanager], [!UICONTROL Kategorien], [!UICONTROL Bedingung], [!UICONTROL Bedingungsaktualisierung] usw.

1. (Optional) Zum Massenbearbeiten der vom Schnellfilter gefundenen Elemente:

   1. Wählen Sie alle oder mehrere Elemente in der Liste aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**, um die Elemente stapelweise zu bearbeiten.
   1. Klicken Sie nach Abschluss der Änderungen auf **[!UICONTROL Änderungen speichern]**.

1. (Optional) Um die vom Schnellfilter gefundenen Elemente zu exportieren, wählen Sie alle oder mehrere Elemente in der Liste aus und klicken Sie dann auf das Symbol **[!UICONTROL Exportieren]** ![Exportieren](assets/export.png).

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Nur die Elemente, die Sie im Schnellfilter-Suchexport gefunden haben, exportieren in die von Ihnen ausgewählte Datei. Wenn Sie vor dem Exportieren der Liste keine Elemente auswählen, wird die vollständige, ungefilterte Liste exportiert.\
   >Weitere Informationen finden Sie unter [Liste exportieren](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Optional) Um die gefilterten Ergebnisse zu löschen, klicken Sie auf **[!UICONTROL Schnellfilter]** Symbol oben rechts im Fenster.
oder
Aktualisieren Sie die Seite.
