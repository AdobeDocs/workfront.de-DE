---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurieren der Schaltfläche "Fertig"für Aufgaben
description: Mit der Schaltfläche Fertig kann automatisch der Status einer Aufgabe oder eines Problems festgelegt werden. Standardmäßig markiert Adobe Workfront eine Aufgabe als abgeschlossen, wenn ein Bevollmächtigter auf Fertig für sein Arbeitselement klickt.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Konfigurieren Sie die [!UICONTROL Fertig] Schaltfläche für Aufgaben

Die [!UICONTROL Fertig] -Schaltfläche kann automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig [!UICONTROL Adobe Workfront] markiert eine Aufgabe als [!UICONTROL Abgeschlossen] wenn ein Bevollmächtigter auf Fertig für sein Arbeitselement klickt.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die [!UICONTROL Fertig] -Schaltfläche, um bestimmte Status im System widerzuspiegeln. Es gibt zwei verschiedene Möglichkeiten: [!UICONTROL Fertig] Schaltfläche funktioniert für Aufgaben in [!UICONTROL Workfront]:

* Wenn dem Benutzer ein Home Team zugewiesen wurde, wird ein [!DNL Workfront] Administrator oder Benutzer mit [!UICONTROL Plan] -Lizenz kann die [!UICONTROL Fertig] -Schaltfläche, um bestimmte Status für Teammitglieder widerzuspiegeln. Siehe [Konfigurieren Sie die [!UICONTROL Fertig] Schaltfläche für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn dem Benutzer kein Home Team zugewiesen ist, wird die [!UICONTROL Fertig] -Schaltfläche für Aufgaben ist an einen vollständigen Status gebunden. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die [!UICONTROL Fertig] -Schaltfläche wird automatisch auf diesen Status festgelegt.

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
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Konfigurieren Sie die [!UICONTROL Fertig] Schaltfläche für ein Team

Sie können ändern, welcher Status auf das Arbeitselement angewendet wird, indem Sie die [!UICONTROL Fertig] Schaltfläche. Sie können auch mehrere Status festlegen und dem Benutzer die Auswahl des entsprechenden Status ermöglichen.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Teams]**.

1. Klicken Sie auf **[!UICONTROL Switch Team]** und wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Suchen Sie die **[!UICONTROL Schaltfläche &quot;Fertig&quot;]** -Abschnitt unten im **[!UICONTROL Team-Einstellungen]** Seite.

1. Wählen Sie für jeden Arbeitselementtyp einen oder mehrere Status aus.

   >[!NOTE]
   >
   >Beachten Sie bei der Auswahl von Status für Aufgaben oder Probleme Folgendes:
   >
   >* Wenn Sie für jeden Arbeitselement-Typ einen Status auswählen, wird der Status der Aufgabe oder des Problems auf diesen Status festgelegt, wenn ein Benutzer auf [!UICONTROL Fertig] auf ihren Posten. Wenn Sie mehrere Status für jeden Arbeitselement-Typ festlegen, wird ein Dropdown-Menü zum [!UICONTROL Fertig] und der Benutzer muss einen Status auswählen, um den Status des Arbeitselements zu ändern.
   >* Sie können nur Status auf Systemebene mit dem [!UICONTROL Fertig] Schaltfläche. Sie können keine gruppenspezifischen Status mit den Status der Arbeitselemente verknüpfen.
   >* Wenn ein dem Element zugewiesener Benutzer das Element in den Status setzt, der dem Element zugeordnet ist [!UICONTROL Fertig] Schaltfläche, wird das Element als [!UICONTROL Fertig] für diesen Benutzer, unabhängig davon, ob der von Ihnen ausgewählte Status ein [!UICONTROL Abgeschlossen] oder [!UICONTROL Geschlossen] Status oder Arbeitsstatus.

   >   
   >   
   >  Beispiel: das [!UICONTROL Fertig] Schaltfläche mit [!UICONTROL In Bearbeitung] bewirkt, dass das Arbeitselement als [!UICONTROL Fertig] für den Benutzer, der den Status ändert von [!UICONTROL Neu] nach [!UICONTROL In Bearbeitung].
   >   
   >* Problemtypen können angepasst werden und können andere Namen haben als die unten in Ihrer Umgebung aufgelisteten.\
      >  Im Folgenden finden Sie die Standardaufgaben und Problemtypen:
      >     
      >   * [!UICONTROL Aufgaben]
      >   * [!UICONTROL Probleme]
      >   * [!UICONTROL Anfrage]
      >   * [!UICONTROL Änderungsanforderung]
      >   * [!UICONTROL Bug-Bericht]


   Wenn die Aufgabe oder das Problem mehreren Benutzern zugewiesen ist, wird ein[!UICONTROL Fertig mit meinem Teil]&quot; im Dropdown-Menü neben den verschiedenen Status, die für Ihr Team ausgewählt wurden.

1. Klicken **[!UICONTROL Änderungen speichern]**.

## Benutzer einem Startseiten-Team zuordnen

So nehmen Sie die Änderungen an der [!UICONTROL Fertig] -Schaltflächenfunktionalität für Benutzer sichtbar machen, können Sie das Team, dessen Einstellungen Sie geändert haben, zum Startseiten-Team der Benutzer machen.

So verknüpfen Sie Benutzer mit einem Home-Team:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].

1. Klicken **[!UICONTROL Benutzer]** und wählen Sie dann den oder die Benutzer aus, die Sie mit einem Home Team verbinden möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Im **[!UICONTROL Einrichtung]** auswählen, wählen Sie die **[!UICONTROL Startseite]** -Feld. Beginnen Sie mit der Eingabe des Namens des Teams, dessen Einstellungen Sie mit den Benutzern verknüpfen möchten. Klicken Sie auf den Namen des Teams, sobald es in der Liste angezeigt wird.

1. Klicken **[!UICONTROL Änderungen speichern]**.\
   Die von Ihnen ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.
Alle Teameinstellungen, einschließlich der Status, die mit dem [!UICONTROL Fertig] -Schaltfläche nun für diese Benutzer sichtbar.
