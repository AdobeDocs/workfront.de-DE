---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Konfigurieren der Schaltfläche „Fertig“ für Probleme
description: Mit der Schaltfläche Fertig können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig kennzeichnet Adobe Workfront ein Problem als „Gelöst“, wenn ein Verantwortlicher auf „Fertig“ für sein Arbeitselement klickt.
author: Jenny
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 1%

---

# Konfigurieren der Schaltfläche [!UICONTROL Fertig] für Probleme

Mit [!UICONTROL  Schaltfläche ]Fertig“ können Sie automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig markiert [!DNL Adobe Workfront] ein Problem als [!UICONTROL Gelöst] wenn ein Verantwortlicher auf [!UICONTROL Fertig] auf sein Arbeitselement klickt.

>[!NOTE]
>
>Die Schaltfläche Fertig wird in allen Bereichen von Workfront als Erledigt markiert angezeigt.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass sie bestimmte Status im System widerspiegelt. Es gibt 3 verschiedene Möglichkeiten, wie die Schaltfläche [!UICONTROL Fertig] für Probleme in [!DNL Workfront] funktioniert:

* Wenn dem Benutzer eine [!UICONTROL Home-Team] zugewiesen ist, kann ein [!DNL Workfront] oder ein Benutzer mit einer [!UICONTROL Plan]-Lizenz die Schaltfläche [!UICONTROL Fertig] so konfigurieren, dass bestimmte Status für Team-Mitglieder angezeigt werden. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn der/die Benutzende kein [!UICONTROL Home-Team] hat, aber [!UICONTROL Andere Teams] in seinem/ihrem Profil hat, sucht Workfront nach der Einstellung der Schaltfläche [!UICONTROL Fertig] in jedem der Teams, die dem/der Benutzenden zugeordnet sind. Die Auswahl erfolgt nach dem Zufallsprinzip, und der mit einem der Teams verknüpfte Status wird für das Problem verwendet.
* Wenn dem Benutzer kein [!UICONTROL Home-Team] zugewiesen ist, ist die Schaltfläche [!UICONTROL Fertig] für Probleme an einen systemgenerierten [!UICONTROL Gelöst]-Status gebunden, der den aus drei Buchstaben bestehenden Code [!UICONTROL RLV] aufweist. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die Schaltfläche [!UICONTROL Fertig] wird automatisch auf diesen Status zurückgesetzt.
* Wenn der Status [!UICONTROL Behoben] ([!UICONTROL RLV]) gelöscht wird und der Benutzer, der das Problem als [!UICONTROL Fertig] markiert, über kein [!UICONTROL Home-Team] verfügt, ist der standardmäßige Problemstatus an das gebunden, was als Standard für [!UICONTROL Geschlossen] für die Gruppe festgelegt wurde, zu der das Problem gehört. Der Workfront-Administrator kann eine systemweite Standardeinstellung für die Gruppe konfigurieren. Siehe [Konfigurieren der Schaltfläche [!UICONTROL Fertig] wenn der Status [!UICONTROL Gelöst] gelöscht wurde](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in diesem Artikel.

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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministratorzugriff ist erforderlich, um die Schaltfläche „Fertig“ zu konfigurieren, wenn der Status „Gelöst“ gelöscht wird</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Schaltfläche [!UICONTROL Fertig] für ein Team

Mit der Schaltfläche [!UICONTROL Fertig“ können Sie ändern, welcher Status dem Arbeitselement ] wird. Sie können auch mehrere Status festlegen und es den Benutzenden ermöglichen, den entsprechenden Status auszuwählen.

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
   >* Sie können mit der Schaltfläche „Fertig“ nur Status [!UICONTROL  Systemebene ]. Sie können keine gruppenspezifischen Status mit Arbeitselementstatus verknüpfen.
   >* Wenn ein(e) Benutzende(r), der/die dem Element zugewiesen ist, das Element in dem mit der Schaltfläche [!UICONTROL Fertig] verknüpften Status platziert, wird das Element für [!UICONTROL /] Benutzende angezeigt, unabhängig davon, ob der ausgewählte Status ein [!UICONTROL Abgeschlossen]- oder [!UICONTROL Geschlossen]-Status oder ein Arbeitsstatus ist.
   >   
   >   
   >  Wenn Sie beispielsweise die Schaltfläche [!UICONTROL Fertig] mit In Bearbeitung verknüpfen, wird das Arbeitselement für den Benutzer, [!UICONTROL  den Status von Neu in In Bearbeitung ändert, als Fertig] angezeigt.
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
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie **[!UICONTROL Abschnitt]** Organisation“ das Feld **[!UICONTROL Home-Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie mit den Benutzern verknüpfen möchten. Klicken Sie auf den Namen des Teams, wenn Sie es in der Liste sehen.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.
Alle Team-Einstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind jetzt für diese Benutzer sichtbar.

## Konfigurieren Sie [!UICONTROL  Schaltfläche ]Fertig“, wenn der Status [!UICONTROL Gelöst] gelöscht wurde

Wenn ein(e) Benutzende(r) kein Home-Team hat und der systemweite Standard für [!UICONTROL Resolved] ([!UICONTROL RLV]) gelöscht wurde, kann ein [!DNL Workfront]-Administrator den [!UICONTROL Closed]-Status für die Gruppe im Projekt konfigurieren. [!DNL Workfront] wählt diesen Status für ein geschlossenes Problem aus, wenn der Benutzer auf die Schaltfläche [!DNL Done] klickt.

### Die mit dem Projekt verknüpfte Gruppe suchen

Wenn ein(e) Benutzende(r) ein Projekt erstellt, wird seine/ihre Hauptgruppe automatisch dem Projekt zugewiesen. Benutzer mit [!UICONTROL Verwalten]-Zugriff auf das Projekt können diese Gruppe jederzeit im Abschnitt [!UICONTROL Projektdetails] ändern. Um zu verstehen, welchen Status [!DNL Workfront] in diesem Fall für ein abgeschlossenes Problem verwendet, müssen Sie wissen, welche Gruppe mit dem Projekt verknüpft ist, in dem sich das Problem befindet, und was der Standardstatus für [!UICONTROL Geschlossen] diese Gruppe für Probleme ist.

So suchen Sie die mit dem Projekt verknüpfte Gruppe:

1. Gehe zu einem Projekt.
1. Klicken Sie links auf der Seite auf &quot;**[!UICONTROL &quot;]**.
1. Suchen Sie den Abschnitt **[!UICONTROL Projektverknüpfung]** und suchen Sie nach **[!UICONTROL Gruppe]**.\
   Dies ist der Gruppenname, mit dem Sie den Status im Bereich Setup überprüfen müssen. Im folgenden Abschnitt finden Sie Anweisungen zum Aktualisieren des Standardstatus für eine bestimmte Gruppe.

### Standardstatus für eine bestimmte Gruppe aktualisieren

Als [!UICONTROL Workfront]-Administrator können Sie den Status für eine bestimmte Gruppe aktualisieren:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klicken Sie im linken Bereich auf **[!UICONTROL Projektvoreinstellungen]** und dann auf **[!UICONTROL Status]**.

1. Klicken Sie **[!UICONTROL Probleme]** und geben Sie dann den Namen der Gruppe in das Suchfeld **[!UICONTROL Systemstatus]** auf der rechten Seite ein.

1. Wählen Sie die Gruppe.
1. Klicken Sie auf **[!UICONTROL Dropdown-Menü]** Standardstatus festlegen) und wählen Sie dann einen Standardstatus für [!UICONTROL Geschlossen]. [!DNL Workfront] verwendet diesen Status für ein geschlossenes Problem, wenn ein Benutzer auf die Schaltfläche [!UICONTROL Fertig] klickt.

   >[!IMPORTANT]
   >
   >Dieser Status wird nur verwendet, wenn dem Benutzer kein Home-Team zugewiesen ist und der [!UICONTROL RLV]-Status gelöscht wurde.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
