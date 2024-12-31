---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Ersetzen Sie die Schaltfläche „Bearbeiten“ durch eine Schaltfläche „Starten“
description: Die Standardkonfiguration von Adobe Workfront enthält eine Schaltfläche „Bearbeiten“ für Aufgaben und Probleme, die für Elemente angezeigt wird, denen Sie zugewiesen wurden.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Ersetzen Sie [!UICONTROL  Schaltfläche „Bearbeiten] durch eine Schaltfläche [!UICONTROL Starten].

Die Standardkonfiguration von [!DNL Adobe Workfront] enthält eine Schaltfläche [!UICONTROL Bearbeiten] für Aufgaben und Probleme, die für Elemente angezeigt wird, denen Sie zugewiesen wurden. Wenn Sie auf [!UICONTROL Bearbeiten] auf Ihnen zugewiesene Elemente klicken, signalisieren Sie anderen Benutzern, dass Sie die Arbeit erhalten haben, und bestätigen, dass Sie daran arbeiten werden. Mit der Schaltfläche &quot;[!DNL Work On It]&quot; wird der Aufgaben- oder Problemstatus jedoch nicht aktualisiert, um darauf hinzuweisen, dass die Arbeit tatsächlich begonnen hat.

Sie können die Schaltfläche [!DNL Work On It] durch eine Schaltfläche [!UICONTROL Starten] für ein Team ersetzen, dem Sie angehören. In diesem Fall klicken Sie auf die Schaltfläche [!UICONTROL Start] anstelle von [!UICONTROL Bearbeiten], wodurch der Status und das [!UICONTROL Tatsächliche Startdatum] des Arbeitselements automatisch aktualisiert werden, was Ihnen signalisiert, dass Sie mit der Arbeit begonnen haben. Informationen dazu, welche Einstellungen sich auf Ihre Änderungen an der Schaltfläche [!UICONTROL Bearbeiten] auswirken können, finden Sie im Abschnitt [Konfigurieren der Schaltfläche [!UICONTROL Starten] in ](#configure-the-uicontrol-start-button) Artikel.

>[!IMPORTANT]
>
>Durch Klicken auf [!UICONTROL Start]-Schaltfläche wird der Status des Elements und das [!UICONTROL Tatsächliche Startdatum] geändert. Wenn eine andere Person mit der Arbeit an einer Aufgabe oder einem Problem begonnen hat (wodurch der Status in [!UICONTROL In Bearbeitung] geändert und das [!UICONTROL Tatsächliches Startdatum] ausgefüllt wurde), wird die Schaltfläche für das Element als [!UICONTROL Bearbeiten] angezeigt, auch wenn die Schaltfläche für ein Team, dem Sie angehören, durch eine [!UICONTROL Start]-Schaltfläche ersetzt wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Schaltfläche [!UICONTROL Starten]

Wenn Sie über eine [!UICONTROL Plan]-Lizenz verfügen, können Sie die Schaltfläche [!UICONTROL Starten] für ein Team im Fenster [!UICONTROL Bearbeiten] konfigurieren. So funktioniert die Schaltfläche, nachdem sie für ein Team aktiviert wurde:

* **Das Team ist einem Arbeitselement zugewiesen**: Wenn ein Team dem Arbeitselement zugewiesen ist, sehen die Mitglieder dieses Teams die Schaltfläche [!UICONTROL Starten] und die für dieses Team konfigurierten Status.
* **Der Benutzer gehört zu einem Home-Team**: Wenn dem Arbeitselement kein Team zugewiesen ist, der Benutzer jedoch einem Home-Team in seinem Profil zugewiesen ist, wird die Schaltfläche [!UICONTROL Starten] und die für dieses Team konfigurierten Status angezeigt. Dies ist das Szenario, das wir empfehlen, wenn Sie möchten, dass Benutzer die Schaltfläche [!UICONTROL Starten] häufig verwenden.
* **Der Benutzer wird einem Arbeitselement zugewiesen**: Wenn dem Arbeitselement kein Team und dem Benutzer kein Home-Team zugewiesen ist, der Benutzer jedoch dem Arbeitselement zugewiesen ist, wird dem Benutzer die Schaltfläche [!UICONTROL Starten] und die kombinierten Status angezeigt, die für alle Teams konfiguriert wurden, denen er zugewiesen ist.
* **Der Benutzer ist keinem Team zugewiesen:** Wenn dem Arbeitselement kein Team und dem Benutzer kein Team zugewiesen ist, einschließlich des Home-Teams, und das Element dem Benutzer zugewiesen ist, dann erscheint der Benutzer auf der Schaltfläche [!UICONTROL Bearbeiten].

>[!NOTE]
>
>Diese Funktion ist derzeit in nicht verfügbar.
>
>* Die Mobile App von [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* E-Mail-Benachrichtigungen [!DNL Workfront]
>

So konfigurieren Sie die Schaltfläche Start:

{{step1-to-team}}

1. Wählen **[!UICONTROL im Dropdown]** Menü „Teams“ ein Team aus.\
   oder\
   Klicken Sie **[!UICONTROL Neues Team erstellen]**.

1. Klicken Sie auf das **[!UICONTROL Mehr]**-![](assets/more-icon.png) und dann auf **[!UICONTROL Bearbeiten]**.

1. Suchen Sie **[!UICONTROL Abschnitt mit der Schaltfläche]** Bearbeiten“ unten auf der Seite [!UICONTROL Teams bearbeiten].
1. Aktivieren **[!UICONTROL das Kontrollkästchen „Bearbeiten-Schaltfläche in Start-Schaltfläche ändern, um den Status eines Elements automatisch]** aktualisieren“.
1. Wählen Sie für jeden Arbeitselementtyp einen oder mehrere Status aus. Wenn Sie mehr als einen Status auswählen, wird beim Klicken auf &quot;[!UICONTROL &quot; ein Dropdown-Menü ], in dem Sie den gewünschten Status auswählen können.
1. Klicken Sie **[!UICONTROL Änderungen speichern]**. Wenn Benutzenden ein Arbeitselement zugewiesen wird[!UICONTROL  wird ] Schaltfläche „Aufgabe starten[!UICONTROL  oder ]Problem starten“ anstelle [!UICONTROL  Schaltfläche &quot;] bearbeiten“ angezeigt.

   >[!NOTE]
   >
   >Es wird empfohlen, das Team als Startseiten-Team eines Benutzers festzulegen, sodass die Schaltfläche Starten für alle ihm zugewiesenen Arbeitselemente angezeigt wird. Siehe [Verknüpfen von Benutzern mit einem Home-Team](#associate-users-with-a-home-team) unten.

## Verknüpfen von Benutzern mit einem Home-Team

So verknüpfen Sie Benutzer mit einem Home-Team:

{{step-1-to-users}}

1. Wählen Sie den/die Benutzer aus, den/die Sie mit einem Home-Team verknüpfen möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie **[!UICONTROL Abschnitt]** Organisation“ das Feld **[!UICONTROL Home-Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie mit den Benutzern verknüpfen möchten. Klicken Sie auf den Namen des Teams, wenn Sie es in der Liste sehen.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.

   Alle Team-Einstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind jetzt für diese Benutzer sichtbar.

