---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Ersetzen Sie die Schaltfläche "Arbeiten auf diesem Gerät"durch eine Schaltfläche "Starten".
description: Die Standardkonfiguration von Adobe Workfront enthält eine Schaltfläche "Bearbeiten", die Aufgaben und Probleme enthält, die für Elemente angezeigt werden, denen Sie zugewiesen wurden.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Ersetzen Sie die Schaltfläche [!UICONTROL Bearbeiten ] durch eine Schaltfläche [!UICONTROL Starten] .

Die Standardkonfiguration von [!DNL Adobe Workfront] enthält eine Schaltfläche [!UICONTROL Bearbeiten darauf] für Aufgaben und Probleme, die für Elemente angezeigt werden, denen Sie zugewiesen wurden. Wenn Sie auf [!UICONTROL Bearbeiten] für Elemente klicken, die Ihnen zugewiesen sind, signalisieren Sie anderen Benutzern, dass Sie die Arbeit erhalten haben, und bestätigen, dass Sie daran arbeiten werden. Die Schaltfläche &quot;[!DNL Work On It]&quot; aktualisiert jedoch nicht den Status der Aufgabe oder des Problems, um zu signalisieren, dass die Arbeit tatsächlich gestartet wurde.

Sie können die Schaltfläche [!DNL Work On It] durch eine Schaltfläche [!UICONTROL Starten] für ein Team ersetzen, dem Sie angehören. In diesem Fall klicken Sie auf die Schaltfläche [!UICONTROL Starten] anstelle von [!UICONTROL Bearbeiten Sie es], wodurch der Status und das [!UICONTROL tatsächliche Startdatum] des Arbeitselements automatisch aktualisiert werden. Dies signalisiert, dass Sie mit der Arbeit begonnen haben. Informationen dazu, welche Einstellung das Team für Ihre Änderungen in der Schaltfläche [!UICONTROL Bearbeiten] festlegen kann, finden Sie im Abschnitt [Konfigurieren der Schaltfläche [!UICONTROL Starten]](#configure-the-uicontrol-start-button) in diesem Artikel.

>[!IMPORTANT]
>
>Wenn Sie auf die Schaltfläche [!UICONTROL Start] klicken, ändern sich der Status des Elements und das aktuelle Startdatum [!UICONTROL 3}. ] Wenn jemand anderer mit der Bearbeitung einer Aufgabe oder eines Problems begonnen hat (durch das der Status in &quot;[!UICONTROL Wird ausgeführt]&quot;geändert und das &quot;[!UICONTROL Tatsächliches Startdatum]&quot; gefüllt wurde), wird die Schaltfläche für das Element als &quot;[!UICONTROL Bearbeiten&quot;] angezeigt, selbst wenn die Schaltfläche in einem Team, dem Sie angehören, durch eine Schaltfläche &quot;[!UICONTROL Starten]&quot;ersetzt wurde.

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

## Konfigurieren der Schaltfläche [!UICONTROL Start]

Wenn Sie über eine [!UICONTROL Plan] -Lizenz verfügen, können Sie die Schaltfläche [!UICONTROL Start] für ein Team im Teamfenster [!UICONTROL Bearbeiten] konfigurieren. So funktioniert die Schaltfläche, nachdem sie für ein Team aktiviert wurde:

* **Das Team wird einem Arbeitselement zugewiesen**: Wenn dem Arbeitselement ein Team zugewiesen ist, sehen Mitglieder dieses Teams die Schaltfläche [!UICONTROL Start] und die für dieses Team konfigurierten Status.
* **Der Benutzer gehört zu einem Home-Team**: Wenn dem Arbeitselement kein Team zugewiesen ist, der Benutzer jedoch einem Home-Team in seinem Profil zugewiesen ist, wird dem Benutzer die Schaltfläche [!UICONTROL Start] sowie der für dieses Team konfigurierte Status angezeigt. Dies ist das Szenario, das wir empfehlen, wenn Sie möchten, dass Benutzer die Schaltfläche [!UICONTROL Starten] häufig verwenden.
* **Der Benutzer ist einem Arbeitselement zugewiesen**: Wenn dem Arbeitselement kein Team zugewiesen ist und dem Benutzer kein Home Team zugewiesen ist, der Benutzer jedoch dem Arbeitselement zugewiesen ist, sieht der Benutzer die Schaltfläche [!UICONTROL Start] und die für alle Teams konfigurierten kombinierten Status.
* **Der Benutzer ist keinem Team zugewiesen:** Wenn dem Arbeitselement kein Team und dem Benutzer kein Team zugewiesen ist, einschließlich des Startseiten-Teams, und das Element dem Benutzer zugewiesen ist, scheint der Benutzer die Schaltfläche [!UICONTROL Bearbeiten] zu verwenden.

>[!NOTE]
>
>Diese Funktion ist derzeit nicht in verfügbar.
>
>* Die [!DNL Workfront] mobile App
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] E-Mail-Benachrichtigungen
>

So konfigurieren Sie die Schaltfläche Start :

{{step1-to-team}}

1. Wählen Sie im Dropdownmenü **[!UICONTROL Teams]** ein Team aus.\
   oder\
   Klicken Sie auf **[!UICONTROL Neues Team erstellen]**.

1. Klicken Sie auf das Symbol **[!UICONTROL Mehr]** ![](assets/more-icon.png) und dann auf **[!UICONTROL Bearbeiten]**.

1. Suchen Sie unten auf der Seite [!UICONTROL Teams bearbeiten] den Schaltflächenabschnitt **[!UICONTROL Bearbeiten]** .
1. Wählen Sie die Schaltfläche **[!UICONTROL Ändern Sie die Schaltfläche &quot;Arbeit an Es bearbeiten&quot;in die Schaltfläche &quot;Start&quot;, um den Status eines Elements]** automatisch zu aktualisieren.
1. Wählen Sie für jeden Arbeitselementtyp einen oder mehrere Status aus. Wenn Sie mehr als einen Status auswählen, wird ein Dropdownmenü angezeigt, wenn Sie auf [!UICONTROL Start] klicken, in dem Sie den gewünschten Status auswählen können.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**. Benutzern wird jetzt die Schaltfläche [!UICONTROL Aufgabe starten] oder [!UICONTROL Problem starten] anstelle der Schaltfläche [!UICONTROL Bearbeiten] angezeigt, wenn ihnen ein Arbeitselement zugewiesen wird.

   >[!NOTE]
   >
   >Es wird empfohlen, das Team als Startseiten-Team des Benutzers festzulegen, damit die Schaltfläche &quot;Start&quot;für alle zugewiesenen Arbeitselemente angezeigt wird. Siehe [Verknüpfen von Benutzern mit einem Home-Team](#associate-users-with-a-home-team) unten.

## Benutzer einem Startseiten-Team zuordnen

So verknüpfen Sie Benutzer mit einem Home-Team:

{{step-1-to-users}}

1. Wählen Sie den oder die Benutzer aus, die Sie mit einem Home-Team verbinden möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   ![](assets/user-settings-nwe-350x291.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Organisation]** das Feld **[!UICONTROL Home Team]** aus. Geben Sie den Namen des Teams ein, dessen Einstellungen Sie den Benutzern zuweisen möchten. Klicken Sie auf den Namen des Teams, sobald es in der Liste angezeigt wird.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die von Ihnen ausgewählten Benutzer sind jetzt mit einem Home-Team verknüpft.

   Alle Teameinstellungen, einschließlich der Status, die mit der Schaltfläche [!UICONTROL Fertig] verknüpft sind, sind nun für diese Benutzer sichtbar.

