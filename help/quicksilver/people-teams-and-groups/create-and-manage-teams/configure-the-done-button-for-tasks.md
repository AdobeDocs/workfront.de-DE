---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurieren der Schaltfläche "Fertig"für Aufgaben
description: Mit der Schaltfläche Fertig kann automatisch der Status einer Aufgabe oder eines Problems festgelegt werden. Standardmäßig markiert Adobe Workfront eine Aufgabe als abgeschlossen, wenn ein Bevollmächtigter auf Fertig für sein Arbeitselement klickt.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# Konfigurieren der Schaltfläche [!UICONTROL Fertig] für Aufgaben

Mit der Schaltfläche [!UICONTROL Fertig] können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig kennzeichnet [!UICONTROL Adobe Workfront] eine Aufgabe als [!UICONTROL Abgeschlossen], wenn ein Bevollmächtigter wie bei seinem Arbeitselement ausgeführt auf &quot;Mark&quot;klickt.

>[!NOTE]
>
>Die Schaltfläche Fertig wird als Markierung angezeigt, wie in allen Bereichen von Workfront ausgeführt.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die Schaltfläche [!UICONTROL Fertig] konfigurieren, um sie bestimmten Status im System zuzuordnen. Die Schaltfläche [!UICONTROL Fertig] funktioniert auf zwei verschiedene Arten für Aufgaben in [!UICONTROL Workfront]:

* Wenn dem Benutzer ein Home Team zugewiesen ist, kann ein [!DNL Workfront] -Administrator oder ein Benutzer mit der Lizenz [!UICONTROL Plan] die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass bestimmte Status für Teammitglieder angezeigt werden. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn der Benutzer über kein [!UICONTROL Home-Team] verfügt, jedoch über [!UICONTROL Other Teams] in seinem Profil verfügt, sucht Workfront nach der Einstellung der Schaltfläche [!UICONTROL Fertig] für eines der mit dem Benutzer verknüpften Teams. Die Auswahl ist zufällig und der Status, der mit einem der Teams verknüpft ist, wird für die Aufgabe verwendet.
* Wenn dem Benutzer kein Home-Team zugewiesen ist, wird die Schaltfläche [!UICONTROL Fertig] für Aufgaben an den vollständigen Status gebunden. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die Schaltfläche [!UICONTROL Fertig] erhält automatisch diesen Status.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team

Mit der Schaltfläche [!UICONTROL Fertig] können Sie ändern, welcher Status auf das Arbeitselement angewendet wird. Sie können auch mehrere Status festlegen und dem Benutzer die Auswahl des entsprechenden Status ermöglichen.

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und dann auf **[!UICONTROL Bearbeiten]**.
1. Suchen Sie den Abschnitt **[!UICONTROL Fertige Schaltfläche]** unten auf der Seite **[!UICONTROL Team-Einstellungen]** .

1. Wählen Sie für jeden Arbeitselementtyp einen oder mehrere Status aus.

   >[!NOTE]
   >
   >Beachten Sie bei der Auswahl von Status für Aufgaben oder Probleme Folgendes:
   >
   >* Wenn Sie für jeden Arbeitselement-Typ einen Status auswählen, wird der Status der Aufgabe oder des Problems auf diesen Status festgelegt, wenn ein Benutzer auf [!UICONTROL Fertig] für sein Element klickt. Wenn Sie für jeden Arbeitselement-Typ mehrere Status festlegen, wird der Schaltfläche [!UICONTROL Fertig] ein Dropdown-Menü hinzugefügt und der Benutzer muss einen Status auswählen, um den Status des Arbeitselements zu ändern.
   >* Sie können nur Status auf Systemebene mit der Schaltfläche [!UICONTROL Fertig] verknüpfen. Sie können keine gruppenspezifischen Status mit den Status der Arbeitselemente verknüpfen.
   >* Wenn ein dem Element zugewiesener Benutzer das Element in den Status setzt, der mit der Schaltfläche [!UICONTROL Fertig] verknüpft ist, wird das Element für diesen Benutzer als [!UICONTROL Fertig] angezeigt, unabhängig davon, ob es sich bei dem ausgewählten Status um den Status [!UICONTROL Abgeschlossen] oder [!UICONTROL Geschlossen] oder um einen Arbeitsstatus handelt.
   >   
   >   
   >  Wenn Sie beispielsweise die Schaltfläche [!UICONTROL Fertig] mit [!UICONTROL In Bearbeitung] verknüpfen, wird das Arbeitselement für den Benutzer, der den Status von [!UICONTROL Neu] in [!UICONTROL Gestartet] ändert, als [!UICONTROL Fertig] angezeigt.
   >   
   >* Problemtypen können angepasst werden und können andere Namen haben als die unten in Ihrer Umgebung aufgelisteten.\
   >  Im Folgenden finden Sie die Standardaufgaben und Problemtypen:
   >     
   >   * [!UICONTROL Aufgaben]
   >   * [!UICONTROL Probleme]
   >   * [!UICONTROL Anfrage]
   >   * [!UICONTROL Änderungsanforderung]
   >   * [!UICONTROL Bug-Bericht]

   Wenn die Aufgabe oder das Problem mehreren Benutzern zugewiesen ist, wird im Dropdown-Menü neben den für Ihr Team ausgewählten verschiedenen Status die Option &quot;[!UICONTROL Fertig mit meinem Teil]&quot; angezeigt.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Benutzer einem Startseiten-Team zuordnen

Um die Änderungen an der Schaltflächenfunktion [!UICONTROL Fertig] für Benutzer sichtbar zu machen, können Sie das Team, dessen Einstellungen Sie geändert haben, zum Startseiten-Team der Benutzer machen.

So verknüpfen Sie Benutzer mit einem Home-Team:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].

1. Klicken Sie auf **[!UICONTROL Benutzer]** und wählen Sie dann den Benutzer aus, den/die Sie mit einem Home-Team verbinden möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und dann auf **[!UICONTROL Bearbeiten]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Organisation]** das Feld **[!UICONTROL Home Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie den Benutzern zuweisen möchten. Klicken Sie auf den Namen des Teams, sobald es in der Liste angezeigt wird.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die von Ihnen ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.
Alle Teameinstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind nun für diese Benutzer sichtbar.
