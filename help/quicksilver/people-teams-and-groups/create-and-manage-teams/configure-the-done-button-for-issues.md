---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Schaltfläche "Fertig"für Probleme konfigurieren
description: Mit der Schaltfläche Fertig kann automatisch der Status einer Aufgabe oder eines Problems festgelegt werden. Standardmäßig markiert Adobe Workfront ein Problem als gelöst, wenn ein Bevollmächtigter auf Fertig klickt.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 3793f68faf2ec0a8050f8f0c6e06a32579b43879
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# Konfigurieren Sie die [!UICONTROL Fertig] Schaltfläche für Probleme

Die [!UICONTROL Fertig] -Schaltfläche kann automatisch den Status einer Aufgabe oder eines Problems festlegen. Standardmäßig [!DNL Adobe Workfront] markiert ein Problem als [!UICONTROL Gelöst] wenn ein Bevollmächtigter klickt [!UICONTROL Fertig] auf ihrem Arbeitselement.

## Übersicht

Benutzer mit bestimmten Berechtigungen können die [!UICONTROL Fertig] -Schaltfläche, um bestimmte Status im System widerzuspiegeln. Es gibt 3 verschiedene Möglichkeiten, die [!UICONTROL Fertig] -Schaltfläche funktioniert bei Problemen in [!DNL Workfront]:

* Wenn dem Benutzer eine [!UICONTROL Startseite], [!DNL Workfront] Administrator oder Benutzer mit [!UICONTROL Plan] -Lizenz kann die [!UICONTROL Fertig] -Schaltfläche, um bestimmte Status für Teammitglieder widerzuspiegeln. Siehe [Konfigurieren Sie die [!UICONTROL Fertig] Schaltfläche für ein Team](#configure-the-uicontrol-done-button-for-a-team) in diesem Artikel.
* Wenn der Benutzer über keine [!UICONTROL Startseite], aber sie haben[!UICONTROL Sonstige Teams] in ihrem Profil sucht Workfront nach der Einstellung der [!UICONTROL Fertig] auf einem der mit dem Benutzer verknüpften Teams. Die Auswahl ist zufällig und der mit einem der Teams verknüpfte Status wird für das Problem verwendet.
* Wenn der Benutzer über keine [!UICONTROL Startseite] zugewiesen wurde, [!UICONTROL Fertig] -Schaltfläche für Probleme an ein systemgeneriertes [!UICONTROL Gelöst] Status mit dem dreistelligen Code [!UICONTROL RLV]. In diesem Szenario sind keine Konfigurationsoptionen verfügbar. Die [!UICONTROL Fertig] -Schaltfläche wird automatisch auf diesen Status festgelegt.
* Wenn die Variable [!UICONTROL Gelöst] ([!UICONTROL RLV]) wird gelöscht und der Benutzer markiert das Problem als [!UICONTROL Fertig] nein [!UICONTROL Startseite]festgelegt ist, wird der standardmäßige Problemstatus an das Problem gebunden, das als Standard für [!UICONTROL Geschlossen] für die Gruppe, die dem Projekt zugewiesen ist, zu der das Problem gehört. Der Workfront-Administrator kann eine systemweite Standardeinstellung für die Gruppe konfigurieren. Siehe [Konfigurieren Sie die [!UICONTROL Fertig] -Schaltfläche beim [!UICONTROL Gelöst] Status wurde gelöscht](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in diesem Artikel.

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
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td>Systemadministratorzugriff ist erforderlich, um die Schaltfläche [!UICONTROL Fertig] zu konfigurieren, wenn der Status [!UICONTROL Aufgelöst] gelöscht wird.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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
   >  Beispiel: das [!UICONTROL Fertig] Schaltfläche mit In Bearbeitung bewirkt, dass das Arbeitselement als [!UICONTROL Fertig] für den Benutzer, der den Status von Neu in Gestartet ändert.
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
Alle Teameinstellungen, einschließlich der Status, die mit dem [!UICONTROL Fertig] -Schaltfläche, sind nun für diese Benutzer sichtbar.

## Konfigurieren Sie die [!UICONTROL Fertig] -Schaltfläche beim [!UICONTROL Gelöst] Status wurde gelöscht

Wenn ein Benutzer kein Home Team hat und der systemweite Standard für [!UICONTROL Gelöst] ([!UICONTROL RLV]) gelöscht wurde, wurde ein [!DNL Workfront] Der Administrator kann die [!UICONTROL Geschlossen] Status für die Gruppe am Projekt. [!DNL Workfront] wählt diesen Status für ein geschlossenes Problem aus, wenn der Benutzer auf die [!DNL Done] Schaltfläche.

### Suchen Sie die mit dem Projekt verknüpfte Gruppe

Wenn ein Benutzer ein Projekt erstellt, wird seine Startseite automatisch dem Projekt zugewiesen. Benutzer mit [!UICONTROL Verwalten] Der Zugriff auf das Projekt kann diese Gruppe im [!UICONTROL Projektdetails] -Abschnitt zu einem beliebigen Zeitpunkt. So verstehen Sie den Status [!DNL Workfront] verwendet in diesem Fall ein abgeschlossenes Problem. Sie müssen wissen, welche Gruppe mit dem Projekt verbunden ist, in dem das Problem liegt, und welchen Standardstatus für [!UICONTROL Geschlossen] Diese Gruppe hat Probleme.

So suchen Sie die mit dem Projekt verknüpfte Gruppe:

1. Wechseln Sie zu einem Projekt.
1. Klicken Sie links auf der Seite auf **[!UICONTROL Projektdetails]**.
1. Suchen Sie die **[!UICONTROL Projektverknüpfung]** und suchen Sie dann **[!UICONTROL Gruppe]**.\
   Dies ist der Gruppenname, den Sie verwenden müssen, um den Status im Bereich Einrichtung zu überprüfen. Anweisungen zum Aktualisieren des Standardstatus für eine bestimmte Gruppe finden Sie im folgenden Abschnitt .

### Standardstatus für eine bestimmte Gruppe aktualisieren

Als [!UICONTROL Workfront] -Administrator können Sie den Status für eine bestimmte Gruppe aktualisieren:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Klicken Sie im linken Bereich auf **[!UICONTROL Projektvoreinstellungen]**, dann **[!UICONTROL Status]**.

1. Klicken **[!UICONTROL Probleme]** und geben Sie dann den Namen der Gruppe in die **[!UICONTROL Systemstatus]** Suchfeld auf der rechten Seite.

1. Wählen Sie die Gruppe aus.
1. Klicken Sie auf **[!UICONTROL Festlegen von Standardstatus]** Dropdown-Menü und wählen Sie dann einen Standardstatus für [!UICONTROL Geschlossen]. [!DNL Workfront] verwendet diesen Status für ein geschlossenes Problem, wenn ein Benutzer auf die [!UICONTROL Fertig] Schaltfläche.

   >[!IMPORTANT]
   >
   >Dieser Status wird nur verwendet, wenn dem Benutzer kein Home Team zugewiesen ist und die [!UICONTROL RLV] -Status gelöscht wurde.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
