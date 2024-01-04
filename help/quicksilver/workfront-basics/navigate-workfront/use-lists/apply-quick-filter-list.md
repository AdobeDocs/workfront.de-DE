---
navigation-topic: use-lists
title: Schnellfilter auf Listen anwenden
description: Sie können den Schnellfilter in einer Liste von Objekten verwenden, um nur für Sie wichtige Elemente zu finden, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# Schnellfilter auf Listen anwenden

<!--
{{highlighted-preview}}
-->

Sie können den Schnellfilter in einer Liste von Objekten verwenden, um nur für Sie wichtige Elemente zu finden, damit Sie sie schnell überprüfen, aktualisieren oder für andere freigeben können.

>[!IMPORTANT]
>
>Mithilfe von Quick Filtern können Sie Elemente finden, die ein Suchwort enthalten, unabhängig davon, ob dieses Element physisch auf dem Bildschirm angezeigt wurde oder angezeigt wird, nachdem Sie zum unteren Seitenrand gescrollt haben. Wenn Sie die Suchfunktionen Ihres Browsers verwenden, können Sie nur Elemente finden, die physisch auf dem Bildschirm angezeigt werden. Wenn Ihre Liste mehrere Seiten enthält, finden Schnellfilter keine Elemente auf Seiten, die nicht angezeigt werden.

Wenn Sie einen Schnellfilter speichern möchten, empfehlen wir, stattdessen einen permanenten Filter für Ihre Liste zu erstellen.\
Informationen zum Erstellen von Filtern in [!DNL Adobe Workfront], siehe Artikel [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Der Schnellfilter ist derzeit in den folgenden Bereichen verfügbar:


Sie können temporäre Schnellfilter in allen Listen verwenden, mit Ausnahme der folgenden:

* Die [!UICONTROL Berichte] area
* Dokumentlisten und Berichte
* Mehrere [!UICONTROL Einrichtung] Gebiete
  >[!NOTE]
  >
  >Schnellfilter sind in den folgenden Setup-Bereichen verfügbar: [!UICONTROL Gruppen], [!UICONTROL Teams], [!UICONTROL Unternehmen], [!UICONTROL Zeitpläne], [!UICONTROL Layout-Vorlagen], und [!UICONTROL Benutzerdefinierte Forms].


Beachten Sie beim Anwenden von Schnellfiltern auf eine Liste Folgendes:

* Sie können Suchbegriffe verwenden, um nach jedem Feld zu filtern, das in der Listenansicht angezeigt wird. Dazu gehören benutzerdefinierte Felder oder komplexe Felder wie [!UICONTROL Vorgänger], [!UICONTROL Zuweisungen], [!UICONTROL Zuweisung] und [!UICONTROL Status], [!UICONTROL Genehmiger] und [!UICONTROL Status], usw.
* Wenn Ihre Liste ausgeblendete Gruppierungen enthält, werden diese bei Verwendung von Schnellfiltern automatisch erweitert. Wenn Sie den Schnellfilter entfernen, werden die Gruppierungen erneut reduziert.
* Bei Gruppierungen werden die aggregierten Informationen der ursprünglichen Liste beibehalten, unabhängig von den angewendeten Schnellfiltern oder den an den Objekten in der Liste vorgenommenen Änderungen.
* Schnellfilter sind temporär. Durch das Ändern der Gruppierung, Ansicht, Filterung oder Sortierung der Liste werden die Kriterien für Schnellfilter entfernt.
* Schnellfilter können nicht gespeichert werden. Wenn Sie einen Filter speichern möchten, um ihn erneut zu verwenden, sollten Sie einen permanenten Filter für die Liste erstellen.
* Wenn mehrere Gruppierungen in der Liste vorhanden sind und der Schnellfilter Elemente in nur einer Gruppierung findet, wird nur diese Gruppierung mit den gefundenen Elementen angezeigt. Alle anderen Gruppierungen sind ausgeblendet.
* In einer Aufgaben- oder Unteraufgabenliste wird die Aufgabenhierarchie entfernt, wenn die Ergebnisse des Schnellfilters angezeigt werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plan*</b></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] license*</b></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Konfigurationen auf Zugriffsebene*</b></td> 
   <td> <p>Zugriff auf den Bereich anzeigen, in dem sich die Liste befindet</p> <p>Um beispielsweise einen Schnellfilter auf ein Projekt anzuwenden, benötigen Sie Zugriff auf die [!UICONTROL Ansicht] auf Projekte.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen.<br>Informationen zur Verwendung von [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Objektberechtigungen</b></td> 
   <td> <p>[!UICONTROL Ansicht]</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Kurzfilter auf Listen anwenden

1. Markieren Sie eine Liste oder einen Bericht, der schnelle Filter unterstützt, und klicken Sie auf die Schaltfläche **[!UICONTROL Schnellfilter] icon** ![](assets/qs-quick-filter-icon.png) in der Symbolleiste.

   Oder

   Drücken Sie je nach Betriebssystem oder Browser und bei Verwendung einer standardmäßigen QWERTY-Tastatur den folgenden Befehlssatz, um den Schnellfilter zu starten:

   * ALT+F für [!DNL Windows] Computer
   * ALT/ Option + F für [!DNL Mac] Computer

     >[!TIP]
     >
     >Wenn Sie STRG+F oder CMD+F drücken, wird neben dem Schnellfilter eine QuickInfo angezeigt, um Sie an diese Befehle zu erinnern. Die Befehle werden auch im Suchfeld für Schnellfilter angezeigt.

1. Im **[!UICONTROL Seite filtern]** Geben Sie den Suchbegriff ein, nach dem Sie filtern möchten.

   Sie können jedes Wort verwenden, das derzeit in der Listenansicht angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie ein Wort verwenden, das möglicherweise auf einer anderen Seite der Liste angezeigt wird, findet der Schnellfilter keine Ergebnisse.

   Eine Liste von Elementen, die den Suchkriterien entsprechen, wird beim Eingeben dynamisch in der Liste angezeigt. Alle anderen Elemente werden ausgeblendet. Der von Ihnen bei der Suche verwendete Suchbegriff wird in allen eigenständigen und komplexen Feldern gelb hervorgehoben. Beispiele für komplexe Felder sind gemeinsame Spalten oder eine der folgenden Aktionen: [!UICONTROL Zuweisungen], [!UICONTROL Zuweisungen] und [!UICONTROL Status], [!UICONTROL Prozent abgeschlossen], [!UICONTROL Vorgänger], [!UICONTROL Genehmiger und Status], [!UICONTROL Ressourcen-Manager], [!UICONTROL Kategorien], [!UICONTROL Bedingung], [!UICONTROL Bedingungsaktualisierung], usw.

1. (Optional) Um die durch den Schnellfilter gefundenen Elemente stapelweise zu bearbeiten, gehen Sie folgendermaßen vor:

   1. Wählen Sie alle oder mehrere Elemente in der Liste aus und klicken Sie auf **[!UICONTROL Bearbeiten]** , um die Elemente stapelweise zu bearbeiten.
   1. Klicken Sie nach Abschluss der Bearbeitung auf **[!UICONTROL Änderungen speichern]**.

1. (Optional) Um die durch den Schnellfilter gefundenen Elemente zu exportieren, wählen Sie alle oder mehrere Elemente in der Liste aus und klicken Sie auf **[!UICONTROL Export]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Nur die Elemente, die Sie in der Schnellfiltersuche gefunden haben, werden in die ausgewählte Datei exportiert. Wenn Sie vor dem Export der Liste keine Elemente auswählen, wird die vollständige, ungefilterte Liste exportiert.\
   >Weitere Informationen finden Sie unter [Liste exportieren](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Optional) Klicken Sie auf die Schaltfläche **[!UICONTROL Schnellfilter]** in der oberen rechten Ecke des Fensters.\
   Oder\
   Aktualisieren Sie die Seite.
