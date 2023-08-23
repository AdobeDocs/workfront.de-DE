---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Anpassen der angezeigten Felder auf einer Karte
description: Sie können anpassen, welche Felder auf einer Karte angezeigt werden, indem Sie ein Feld deaktivieren, damit es nicht in der vollständigen Karten- oder gekürzten Ansicht angezeigt wird, oder ein Feld in der gekürzten Kartenansicht ausblenden.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 0beb96dc3869e6f913d87f699aa9a51c5aaa8f79
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Anpassen der angezeigten Felder auf einer Karte

Standardmäßig werden alle verfügbaren Felder auf einer Karte angezeigt, sowohl in der Vollansicht beim Öffnen der Karte als auch in der verdichteten Kartenansicht auf der Pinnwand. Sie können anpassen, welche Felder angezeigt werden durch:

* Deaktivieren eines Felds, sodass es in keiner Ansicht angezeigt wird
* Ausblenden eines Felds in der verdichteten Kartenansicht

Wenn ein Feld einen Wert enthält und Sie das Feld deaktivieren, wird der Wert beibehalten, wenn Sie das Feld später erneut aktivieren.

Abschnitte (die in den Kartendetails als linke Navigationsoptionen angezeigt werden) stehen auch zum Ein- und Ausblenden zur Verfügung.

Sie können auch benutzerdefinierte Felder anzeigen, die zuvor erstellt wurden. Sie können keine neuen benutzerdefinierten Felder in einer Pinnwand entwerfen und erstellen.

>[!NOTE]
>
>Alle Feldanpassungen, die Sie vornehmen, gelten nur für die Pinnwand, in der Sie arbeiten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Karten konfigurieren {#configure-cards}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Pinnwände]**.
1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicks [!UICONTROL **Konfigurieren**] auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Erweitern [!UICONTROL **Karten**].

   Die meisten Felder und Abschnitte sind standardmäßig aktiviert.

1. Deaktivieren Sie ein Feld oder einen Abschnitt, um es in beiden Kartenansichten zu deaktivieren.
1. Klicken Sie auf das Symbol Ausblenden . ![Symbol &quot;Ausblenden&quot;](assets/eye-hide-icon.png) neben einem Feld oder Abschnitt, um es in der gekürzten Ansicht auszublenden.
1. Um alle Felder und Abschnitte in beiden Ansichten anzuzeigen, klicken Sie auf [!UICONTROL **Alle Felder standardmäßig wiederherstellen**].
1. Klicks [!UICONTROL **Konfigurieren ausblenden**] , um das Fenster &quot;Konfigurieren&quot;zu schließen.

## Hinzufügen benutzerdefinierter Felder zu Karten

Benutzerdefinierte Felder sind auf verbundenen Karten verfügbar. Sie sind nur in der vollständigen Kartenansicht sichtbar, nicht in der gekürzten Ansicht auf der Pinnwand.

>[!NOTE]
>
>Wenn Sie Ihren Karten ein benutzerdefiniertes Feld hinzufügen, sind die Daten auf der Karte schreibgeschützt.

1. Öffnen Sie die Pinnwand und klicken Sie auf [!UICONTROL **Konfigurieren**] , um den Bereich Konfigurieren zu öffnen.
1. Erweitern [!UICONTROL **Karten**].
1. under [!UICONTROL Kartenfelder]klicken [!UICONTROL **Benutzerdefiniertes Feld hinzufügen**].
1. Auswählen [!UICONTROL **Aufgabe**] oder [!UICONTROL **Problem**].

   Die Kategorien der verfügbaren Felder für Aufgaben oder Probleme werden angezeigt. Erweitern Sie eine Kategorie, um alle Felder anzuzeigen. Sie können auch nach einem Feld suchen.

   ![Nach benutzerdefinierten Feldern suchen](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Die folgenden Feldtypen können nicht zu Karten hinzugefügt werden: Adobe XD, Bild, PDF, Video.

1. Wählen Sie den Feldnamen aus.
1. (Optional) Klicken Sie auf die Schaltfläche **[!UICONTROL Feldwert]** um dieses benutzerdefinierte Feld in ein anderes zu ändern.
1. (Optional) Ändern Sie die **[!UICONTROL Feldbezeichnung]** auf den Feldnamen, der auf Karten angezeigt werden soll.
1. Wenn Sie alle Änderungen vorgenommen haben, klicken Sie auf [!UICONTROL **Feld speichern**].

   ![Benutzerdefinierter Feldwert und Titel](assets/save-custom-field-value-label.png)

   Das benutzerdefinierte Feld wird zur Liste der verfügbaren Felder hinzugefügt und ist standardmäßig aktiviert. Sie können das benutzerdefinierte Feld entsprechend den Schritten im Abschnitt [Karten konfigurieren](customize-fields-on-card.md#configure-cards) Bearbeiten Sie das Feld oder löschen Sie es aus allen Karten.

>[!NOTE]
>
>Wenn Sie das benutzerdefinierte Feld später in Workfront umbenennen, müssen Sie die Feldbeschriftung im Fenster &quot;Für Übereinstimmung konfigurieren&quot;bearbeiten. Andernfalls wird das Feld nicht auf den Karten angezeigt.
