---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurieren der Schaltfläche „Fertig“ für Aufgaben
description: Mit der Schaltfläche Fertig können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig kennzeichnet Adobe Workfront eine Aufgabe als abgeschlossen, wenn ein Verantwortlicher auf Fertig klickt.
author: Jenny
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 2%

---

# Konfigurieren der Schaltfläche [!UICONTROL Fertig] für Aufgaben

Mit [!UICONTROL &#x200B; Schaltfläche &#x200B;]Fertig“ können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig markiert [!UICONTROL Adobe Workfront] eine Aufgabe als [!UICONTROL Abgeschlossen] wenn ein Verantwortlicher in seinem Arbeitselement auf Als abgeschlossen markieren klickt.

>[!NOTE]
>
>Die Schaltfläche Fertig wird in allen Bereichen von Workfront als Erledigt markiert angezeigt.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die Schaltfläche [!UICONTROL Fertig] konfigurieren, um sie mit bestimmten Status im System zu verknüpfen. Es gibt zwei verschiedene Möglichkeiten, wie die Schaltfläche [!UICONTROL Fertig] für Aufgaben in [!UICONTROL Workfront funktioniert]:

* Wenn dem Benutzer ein Home-Team zugewiesen ist, kann ein [!DNL Workfront] oder ein Benutzer mit einer [!UICONTROL Plan]-Lizenz die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass bestimmte Status für Team-Mitglieder angezeigt werden. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn der/die Benutzende kein [!UICONTROL Home-Team] hat, aber [!UICONTROL Andere Teams] in seinem/ihrem Profil hat, sucht Workfront nach der Einstellung der Schaltfläche [!UICONTROL Fertig] in jedem der Teams, die dem/der Benutzenden zugeordnet sind. Die Auswahl erfolgt nach dem Zufallsprinzip, und der mit einem der Teams verknüpfte Status wird für die Aufgabe verwendet.
* Wenn dem Benutzer kein Home-Team zugewiesen ist, ist die Schaltfläche [!UICONTROL Fertig] für Aufgaben an den Status „Abgeschlossen“ gebunden. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die Schaltfläche [!UICONTROL Fertig] wird automatisch auf diesen Status zurückgesetzt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team

Mit der Schaltfläche [!UICONTROL Fertig“ können Sie ändern, welcher Status dem Arbeitselement &#x200B;] wird. Sie können auch mehrere Status festlegen und es den Benutzenden ermöglichen, den entsprechenden Status auszuwählen.

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]** Symbol und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und dann auf **[!UICONTROL Bearbeiten]**.
1. Suchen Sie den Abschnitt **[!UICONTROL Fertig]** unten auf der Seite **[!UICONTROL Team-Einstellungen]**.

1. Wählen Sie für jeden Arbeitselementtyp einen Status oder mehrere Status aus.

   >[!NOTE]
   >
   >Beachten Sie beim Auswählen von Status für Aufgaben oder Probleme Folgendes:
   >
   >* Wenn Sie einen Status für jeden Typ von Arbeitselement auswählen, wird der Aufgaben- oder Problemstatus auf diesen Status gesetzt, wenn ein Benutzer auf [!UICONTROL Fertig] auf sein Element klickt. Wenn Sie mehrere Status für jeden Typ von Arbeitselement festlegen, wird der Schaltfläche [!UICONTROL Fertig] ein Dropdown-Menü hinzugefügt und der Benutzer muss einen Status auswählen, um den Status des Arbeitselements zu ändern.
   >* Sie können mit der Schaltfläche „Fertig“ nur Status [!UICONTROL &#x200B; Systemebene &#x200B;]. Sie können keine gruppenspezifischen Status mit Arbeitselementstatus verknüpfen.
   >* Wenn ein(e) Benutzende(r), der/die dem Element zugewiesen ist, das Element in dem mit der Schaltfläche [!UICONTROL Fertig] verknüpften Status platziert, wird das Element für [!UICONTROL /] Benutzende angezeigt, unabhängig davon, ob der ausgewählte Status ein [!UICONTROL Abgeschlossen]- oder [!UICONTROL Geschlossen]-Status oder ein Arbeitsstatus ist.
   >   
   >   
   >  Wenn Sie beispielsweise die Schaltfläche [!UICONTROL Fertig] mit [!UICONTROL In Bearbeitung] verknüpfen, wird das Arbeitselement für den Benutzer als [!UICONTROL Fertig] angezeigt, der den Status von [!UICONTROL Neu] in [!UICONTROL In Bearbeitung] ändert.
   >   
   >* Anfragetypen können angepasst werden und haben in Ihrer Umgebung möglicherweise andere Namen als die unten aufgeführten.\
   >  Im Folgenden finden Sie die standardmäßigen Aufgaben und Problemtypen:
   >     
   >   * [!UICONTROL Aufgaben]
   >   * [!UICONTROL Probleme]
   >   * [!UICONTROL Anfrage]
   >   * [!UICONTROL Änderungsanforderung]
   >   * [!UICONTROL Fehlerbericht]

   Wenn die Aufgabe oder das Problem mehreren Benutzern zugewiesen ist, wird im Dropdown-Menü neben den mehreren für Ihr Team ausgewählten Status die Option &quot;[!UICONTROL Fertig mit meinem Teil]&quot; angezeigt.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Verknüpfen von Benutzern mit einem Home-Team

Um die Änderungen an der [!UICONTROL Fertig]-Schaltflächenfunktion für Benutzer sichtbar zu machen, können Sie das Team, dessen Einstellungen Sie geändert haben, als Home-Team der Benutzer festlegen.

So verknüpfen Sie Benutzer mit einem Home-Team:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].

1. Klicken Sie **[!UICONTROL Benutzer]** und wählen Sie dann den/die Benutzer aus, den/die Sie mit einem Home-Team verknüpfen möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und dann auf **[!UICONTROL Bearbeiten]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie **[!UICONTROL Abschnitt]** Organisation“ das Feld **[!UICONTROL Home-Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie mit den Benutzern verknüpfen möchten. Klicken Sie auf den Namen des Teams, wenn Sie es in der Liste sehen.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.
Alle Team-Einstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind jetzt für diese Benutzer sichtbar.
