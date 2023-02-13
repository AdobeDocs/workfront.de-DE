---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Ersetzen der Schaltfläche "Work On It"durch die Schaltfläche Start
description: Die Standardkonfiguration von Adobe Workfront enthält eine Schaltfläche "Bearbeiten", die Aufgaben und Probleme enthält, die für Elemente angezeigt werden, denen Sie zugewiesen wurden.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Ersetzen Sie die [!UICONTROL Arbeiten daran] Schaltfläche mit [!UICONTROL Starten] button

[!DNL Adobe Workfront]Die Standardkonfiguration umfasst eine [!UICONTROL Arbeiten daran] für Aufgaben und Probleme, die für Elemente angezeigt werden, denen Sie zugewiesen wurden. Wenn Sie auf [!UICONTROL Arbeiten daran] bei Artikeln, die Ihnen zugewiesen sind, signalisieren Sie anderen Benutzern, dass Sie die Arbeit erhalten haben, und bestätigen, dass Sie daran arbeiten werden. Die Variable [!DNL Work On It] -Schaltfläche aktualisiert die Aufgabe oder den Problemstatus nicht, um zu signalisieren, dass die Arbeit tatsächlich gestartet wurde.

Sie können die [!DNL Work On It] Schaltfläche mit [!UICONTROL Starten] Schaltfläche für ein Team, dem Sie angehören. In diesem Fall klicken Sie auf die [!UICONTROL Starten] anstelle von [!UICONTROL Arbeiten daran], wodurch automatisch der Status und die [!UICONTROL Tatsächliches Startdatum] des Arbeitselements angezeigt, dass Sie mit der Arbeit begonnen haben. Informationen darüber, welche Teams sich auf Ihre Änderungen in der [!UICONTROL Arbeiten daran] -Schaltfläche, siehe Abschnitt [Konfigurieren Sie die [!UICONTROL Starten] button](#configure-the-uicontrol-start-button) in diesem Artikel.

>[!IMPORTANT]
>
>Klicken Sie auf [!UICONTROL Starten] -Schaltfläche ändert den Status des Elements und [!UICONTROL Tatsächliches Startdatum]. Wenn jemand anderer mit der Bearbeitung einer Aufgabe oder eines Problems begonnen hat (wodurch der Status in [!UICONTROL In Bearbeitung] und die [!UICONTROL Tatsächliches Startdatum]), wird die Schaltfläche für das Element als [!UICONTROL Arbeiten daran] auch wenn die Schaltfläche eines Teams, dem Sie angehören, durch eine [!UICONTROL Starten] Schaltfläche.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Konfigurieren Sie die [!UICONTROL Starten] button

Wenn Sie [!UICONTROL Plan] -Lizenz können Sie die [!UICONTROL Starten] Schaltfläche für ein Team im [!UICONTROL Bearbeiten] Teamfenster. So funktioniert die Schaltfläche, nachdem sie für ein Team aktiviert wurde:

* **Das Team wird einem Arbeitselement zugewiesen**: Wenn ein Team dem Arbeitselement zugewiesen ist, sehen die Mitglieder dieses Teams die [!UICONTROL Starten] und die für dieses Team konfigurierten Status.
* **Der Benutzer gehört zu einem Startseiten-Team**: Wenn dem Arbeitselement kein Team zugewiesen ist, der Benutzer jedoch einem Home Team in seinem Profil zugewiesen ist, wird dem Benutzer die [!UICONTROL Starten] und die für dieses Team konfigurierten Status. Dies ist das Szenario, das wir empfehlen, wenn Sie möchten, dass Benutzer die [!UICONTROL Starten] angezeigt.
* **Der Benutzer wird einem Arbeitselement zugewiesen**: Wenn dem Arbeitselement kein Team zugewiesen ist und dem Benutzer kein Home Team zugewiesen ist, der Benutzer jedoch dem Arbeitselement zugewiesen ist, wird dem Benutzer die [!UICONTROL Starten] und die kombinierten Status, die für alle Teams konfiguriert sind, denen sie zugewiesen sind.
* **Der Benutzer wird keinem Team zugewiesen:** Wenn dem Arbeitselement kein Team und dem Benutzer kein Team zugewiesen ist, einschließlich des Home-Teams, und das Element dem Benutzer zugewiesen ist, scheint der Benutzer die [!UICONTROL Arbeiten daran] Schaltfläche.

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in verfügbar.
>
>* Die [!DNL Workfront] mobile App
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] E-Mail-Benachrichtigungen
>


So konfigurieren Sie die Schaltfläche Start :

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Teams]**.

1. Im **[!UICONTROL Teams]** ein Team aus.\
   oder\
   Klicken **[!UICONTROL Team erstellen]**.

1. Klicken Sie auf **[!UICONTROL Mehr]** icon ![](assets/more-icon.png)Klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Suchen Sie die **[!UICONTROL Arbeiten daran]** Schaltflächenbereich unten im [!UICONTROL Teams bearbeiten] Seite.
1. Wählen Sie die **[!UICONTROL Ändern Sie die Schaltfläche &quot;Bearbeiten&quot;in die Schaltfläche &quot;Starten&quot;, um den Status eines Elements automatisch zu aktualisieren.]** aktivieren.
1. Wählen Sie für jeden Arbeitselementtyp einen oder mehrere Status aus. Wenn Sie mehr als einen Status auswählen, wird beim Klicken auf [!UICONTROL Starten] wo Sie den gewünschten Status auswählen können.
1. Klicken **[!UICONTROL Änderungen speichern]**. Benutzern wird nun eine [!UICONTROL Aufgabe starten] oder [!UICONTROL Startproblem] anstelle der [!UICONTROL Arbeiten daran] -Schaltfläche, wenn ihnen ein Arbeitselement zugewiesen wird.

   >[!NOTE]
   >
   >Es wird empfohlen, das Team als Startseiten-Team des Benutzers festzulegen, damit die Schaltfläche &quot;Start&quot;für alle zugewiesenen Arbeitselemente angezeigt wird. Siehe [Benutzer einem Startseiten-Team zuordnen](#associate-users-with-a-home-team) unten.

## Benutzer einem Startseiten-Team zuordnen

So verknüpfen Sie Benutzer mit einem Home-Team:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].

1. Klicken **[!UICONTROL Benutzer]** und wählen Sie dann den oder die Benutzer aus, die Sie mit einem Home Team verbinden möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. Im **[!UICONTROL Einrichtung]** auswählen, wählen Sie die **[!UICONTROL Startseite]** -Feld. Beginnen Sie mit der Eingabe des Namens des Teams, dessen Einstellungen Sie mit den Benutzern verknüpfen möchten. Klicken Sie auf den Namen des Teams, sobald es in der Liste angezeigt wird.

1. Klicken **[!UICONTROL Änderungen speichern]**.\
   Die von Ihnen ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.

   Alle Teameinstellungen, einschließlich der Status, die mit dem [!UICONTROL Fertig] -Schaltfläche nun für diese Benutzer sichtbar.

