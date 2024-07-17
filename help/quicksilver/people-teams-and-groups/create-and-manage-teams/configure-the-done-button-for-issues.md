---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Schaltfläche "Fertig"für Probleme konfigurieren
description: Mit der Schaltfläche Fertig kann automatisch der Status einer Aufgabe oder eines Problems festgelegt werden. Standardmäßig markiert Adobe Workfront ein Problem als gelöst, wenn ein Bevollmächtigter auf Fertig klickt.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 1%

---

# Konfigurieren der Schaltfläche [!UICONTROL Fertig] für Probleme

Mit der Schaltfläche [!UICONTROL Fertig] können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig markiert [!DNL Adobe Workfront] ein Problem als [!UICONTROL Gelöst], wenn ein Bevollmächtigter auf [!UICONTROL Fertig] für sein Arbeitselement klickt.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass sie bestimmte Status im System widerspiegelt. Die Schaltfläche [!UICONTROL Fertig] funktioniert auf drei verschiedene Arten bei Problemen in [!DNL Workfront]:

* Wenn dem Benutzer das [!UICONTROL Home Team] zugewiesen wurde, kann ein [!DNL Workfront] -Administrator oder ein Benutzer mit der Lizenz [!UICONTROL Plan] die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass bestimmte Status für Teammitglieder angezeigt werden. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn der Benutzer über kein [!UICONTROL Home-Team] verfügt, jedoch über [!UICONTROL Other Teams] in seinem Profil verfügt, sucht Workfront nach der Einstellung der Schaltfläche [!UICONTROL Fertig] für eines der mit dem Benutzer verknüpften Teams. Die Auswahl ist zufällig und der Status, der mit einem der Teams verknüpft ist, wird für das Problem verwendet.
* Wenn dem Benutzer kein [!UICONTROL Home Team] zugewiesen ist, ist die Schaltfläche [!UICONTROL Fertig] für Probleme an einen vom System generierten [!UICONTROL Resolved] -Status gebunden, der den aus drei Buchstaben bestehenden Code [!UICONTROL RLV] aufweist. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die Schaltfläche [!UICONTROL Fertig] erhält automatisch diesen Status.
* Wenn der Status [!UICONTROL Gelöst] ([!UICONTROL RLV]) gelöscht wird und der Benutzer, der das Problem als [!UICONTROL Fertig] kennzeichnet, keinen [!UICONTROL Startseite] aufweist, wird der standardmäßige Problemstatus an den Status gebunden, der für die Gruppe, der das Problem zugewiesen ist, als Standard für [!UICONTROL Geschlossen] festgelegt ist. Der Workfront-Administrator kann eine systemweite Standardeinstellung für die Gruppe konfigurieren. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] , wenn der Status [!UICONTROL Gelöst] gelöscht wurde](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in diesem Artikel.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td>Systemadministratorzugriff ist erforderlich, um die Schaltfläche [!UICONTROL Fertig] zu konfigurieren, wenn der Status [!UICONTROL Aufgelöst] gelöscht wird</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team

Mit der Schaltfläche [!UICONTROL Fertig] können Sie ändern, welcher Status auf das Arbeitselement angewendet wird. Sie können auch mehrere Status festlegen und dem Benutzer die Auswahl des entsprechenden Status ermöglichen.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in Adobe Workfront und klicken Sie dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

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
   >  Wenn Sie beispielsweise die Schaltfläche [!UICONTROL Fertig] mit &quot;In Progress&quot;verknüpfen, wird das Arbeitselement für den Benutzer, der den Status von &quot;Neu&quot;in &quot;Gestartet&quot;ändert, als [!UICONTROL Fertig] angezeigt.
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
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Organisation]** das Feld **[!UICONTROL Home Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie den Benutzern zuweisen möchten. Klicken Sie auf den Namen des Teams, sobald es in der Liste angezeigt wird.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die von Ihnen ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.
Alle Teameinstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind nun für diese Benutzer sichtbar.

## Konfigurieren Sie die Schaltfläche [!UICONTROL Fertig] , wenn der Status [!UICONTROL Aufgelöst] gelöscht wurde.

Wenn ein Benutzer kein Home-Team hat und der systemweite Standard für [!UICONTROL Resolved] ([!UICONTROL RLV]) gelöscht wurde, kann ein [!DNL Workfront] -Administrator den Status [!UICONTROL Closed] für die Gruppe auf dem Projekt konfigurieren. [!DNL Workfront] markiert diesen Status für ein geschlossenes Problem, wenn der Benutzer auf die Schaltfläche [!DNL Done] klickt.

### Suchen Sie die mit dem Projekt verknüpfte Gruppe.

Wenn ein Benutzer ein Projekt erstellt, wird seine Startseite automatisch dem Projekt zugewiesen. Benutzer mit Zugriff auf das Projekt [!UICONTROL Verwalten] können diese Gruppe im Abschnitt [!UICONTROL Projektdetails] jederzeit ändern. Um zu verstehen, welchen Status [!DNL Workfront] in diesem Fall für ein abgeschlossenes Problem verwendet, müssen Sie wissen, welche Gruppe mit dem Projekt verknüpft ist, in dem das Problem auftritt, und welchen Standardstatus diese Gruppe für [!UICONTROL Abgeschlossen] für Probleme hat.

So suchen Sie die mit dem Projekt verknüpfte Gruppe:

1. Wechseln Sie zu einem Projekt.
1. Klicken Sie auf der linken Seite der Seite auf **[!UICONTROL Projektdetails]**.
1. Suchen Sie den Abschnitt **[!UICONTROL Projektverknüpfung]** und suchen Sie dann nach **[!UICONTROL Gruppe]**.\
   Dies ist der Gruppenname, den Sie verwenden müssen, um den Status im Bereich Einrichtung zu überprüfen. Anweisungen zum Aktualisieren des Standardstatus für eine bestimmte Gruppe finden Sie im folgenden Abschnitt .

### Standardstatus für eine bestimmte Gruppe aktualisieren

Als Administrator von [!UICONTROL Workfront] können Sie den Status für eine bestimmte Gruppe aktualisieren:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in Adobe Workfront und klicken Sie dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)
1. Klicken Sie im linken Bereich auf **[!UICONTROL Projekteinstellungen]** und dann auf **[!UICONTROL Status]**.

1. Klicken Sie auf **[!UICONTROL Probleme]** und geben Sie dann den Namen der Gruppe in das Suchfeld **[!UICONTROL Systemstatus]** auf der rechten Seite ein.

1. Wählen Sie die Gruppe aus.
1. Klicken Sie auf das Dropdownmenü **[!UICONTROL Standardstatus festlegen]** und wählen Sie dann einen Standardstatus für [!UICONTROL Geschlossen] aus. [!DNL Workfront] verwendet diesen Status für ein geschlossenes Problem, wenn ein Benutzer auf die Schaltfläche [!UICONTROL Fertig] klickt.

   >[!IMPORTANT]
   >
   >Dieser Status wird nur verwendet, wenn dem Benutzer kein Home Team zugewiesen wurde und der Status [!UICONTROL RLV] gelöscht wurde.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
