---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Anpassen, welche Felder auf einer Karte angezeigt werden
description: Sie können anpassen, welche Felder auf einer Karte angezeigt werden, indem Sie ein Feld deaktivieren, sodass es nicht in der vollständigen oder verkürzten Ansicht angezeigt wird, oder ein Feld in der verkürzten Kartenansicht ausblenden.
author: Jenny
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Anpassen der auf einer Karte angezeigten Felder

Standardmäßig werden alle verfügbaren Felder auf einer Karte angezeigt, sowohl in der Vollansicht, wenn die Karte geöffnet ist, als auch in der reduzierten Kartenansicht auf der Pinnwand. Sie können wie folgt anpassen, welche Felder angezeigt werden:

* Deaktivieren eines Felds, damit es in keiner der Ansichten angezeigt wird
* Ausblenden eines Felds in der reduzierten Kartenansicht

Wenn ein Feld einen Wert enthält und Sie das Feld deaktivieren, wird der Wert beibehalten, wenn Sie das Feld später erneut aktivieren.

Es stehen auch -Abschnitte (die als linke Navigationsoptionen auf den Kartendetails angezeigt werden) zum Anzeigen und Ausblenden zur Verfügung.

Sie können auch benutzerdefinierte Felder anzeigen, die zuvor erstellt wurden. Es ist nicht möglich, benutzerdefinierte Felder in einer Pinnwand zu entwerfen und neu zu erstellen.

>[!NOTE]
>
>Feldanpassungen, die Sie vornehmen, gelten nur für das Board, in dem Sie arbeiten.

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

## Karten konfigurieren {#configure-cards}

{{step1-to-boards}}

1. Zugriff auf eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie [!UICONTROL **rechts auf**] Pinnwand auf „Konfigurieren“, um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Erweitern Sie [!UICONTROL **Karten**].

   Die meisten Felder und Abschnitte sind standardmäßig aktiviert.

1. Deaktivieren Sie ein Feld oder einen Abschnitt, um es bzw. ihn in beiden Kartenansichten zu deaktivieren.
1. Klicken Sie auf das Symbol „Ausblenden![ (Symbol „Ausblenden](assets/eye-hide-icon.png) neben einem Feld oder Abschnitt, um es bzw. ihn in der verkürzten Ansicht auszublenden.
1. Um alle Felder und Abschnitte in beiden Ansichten anzuzeigen, klicken Sie auf [!UICONTROL **Alle Felder auf Standard zurücksetzen**].
1. Klicken Sie [!UICONTROL **Konfigurieren ausblenden**], um das Bedienfeld „Konfigurieren“ zu schließen.

## Hinzufügen benutzerdefinierter Felder zu Karten

Benutzerdefinierte Felder sind auf verbundenen Karten verfügbar. Sie sind nur in der vollständigen Kartenansicht sichtbar, nicht in der verkürzten Ansicht auf der Pinnwand.

Die Daten in benutzerdefinierten Feldern können auf der Karte bearbeitet werden, obwohl bestimmte benutzerdefinierte Elemente möglicherweise nur im ursprünglichen Feld und nicht auf der Karte bearbeitet werden können.

1. Rufen Sie eine Pinnwand auf und klicken Sie auf [!UICONTROL **Konfigurieren**], um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Erweitern Sie [!UICONTROL **Karten**].
1. Klicken [!UICONTROL  unter &quot;]&quot; auf [!UICONTROL **Benutzerdefiniertes Feld hinzufügen**].
1. Wählen Sie [!UICONTROL **Aufgabe**] oder [!UICONTROL **Problem**] aus.

   Die Kategorien der verfügbaren Felder für Aufgaben oder Probleme werden angezeigt. Erweitern Sie eine Kategorie, um alle Felder anzuzeigen. Sie können auch nach einem Feld suchen.

   ![Nach benutzerdefiniertem Feld suchen](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Die folgenden Feldtypen können nicht zu Karten hinzugefügt werden: Adobe XD, Image, PDF, Video.

1. Wählen Sie den Feldnamen.
1. (Optional) Klicken Sie in das Feld **[!UICONTROL Feldwert]**, um dieses benutzerdefinierte Feld in ein anderes zu ändern.
1. (Optional) Ändern Sie **[!UICONTROL Feldbezeichnung]** in den Feldnamen, der auf Karten angezeigt werden soll.
1. Wenn Sie Ihre Änderungen abgeschlossen haben, klicken Sie auf [!UICONTROL **Feld speichern**].

   ![Benutzerdefinierter Feldwert und Titel](assets/save-custom-field-value-label.png)

   Das benutzerdefinierte Feld wird der Liste der verfügbaren Felder hinzugefügt und ist standardmäßig aktiviert. Sie können das benutzerdefinierte Feld gemäß den Schritten im Abschnitt [Konfigurieren von Karten](customize-fields-on-card.md#configure-cards) oben deaktivieren, das Feld bearbeiten oder es aus allen Karten löschen.

>[!NOTE]
>
>Wenn Sie das benutzerdefinierte Feld später in Workfront umbenennen, müssen Sie die Feldbezeichnung im Bedienfeld „Konfigurieren“ so bearbeiten, dass sie übereinstimmt, da das Feld sonst nicht auf den Karten angezeigt wird.

## Anzeigen oder Ausblenden archivierter Karten

Sie müssen eine Konfigurationseinstellung aktivieren, um archivierte Karten auf einer Pinnwand anzuzeigen.

1. Rufen Sie eine Pinnwand auf und klicken Sie auf [!UICONTROL **Konfigurieren**], um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Erweitern Sie [!UICONTROL **Karten**].
1. Schalten Sie [!UICONTROL **Anzeige archivierter Karten auf der Pinnwand**] ein.

   Jetzt können Sie die Pinnwand so filtern, dass alle Karten angezeigt werden, die archiviert wurden. Weitere Informationen finden Sie unter [Filtern und Suchen in einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Klicken Sie [!UICONTROL **Konfigurieren ausblenden**], um das Bedienfeld „Konfigurieren“ zu schließen.

## Konfigurieren von Karten-Falloff

Informationen zum automatischen Entfernen von Karten aus der Pinnwand nach einem bestimmten Zeitraum finden Sie unter [Konfigurieren von Karten-Falloff](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
