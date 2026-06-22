---
title: Genehmigen einer Anforderung in Adobe Workfront Planning
description: Wenn ein(e) Benutzende(r) eine Anfrage an ein Anforderungsformular sendet, das mit einer Genehmigung in Adobe Workfront Planning verknüpft ist, erhalten genehmigende Personen eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/u8dbV85NLabPjFj0-gsjPO1vz3mrmgU9yKxRBttHhtY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 999
ht-degree: 5%

---

# Genehmigen einer Anfrage in Adobe Workfront-Planung

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Wenn ein(e) Benutzende(r) eine Anfrage an ein Anforderungsformular sendet, das mit einer Genehmigung in Adobe Workfront Planning verknüpft ist, erhalten genehmigende Personen eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager eine Anforderung genehmigen kann, die für Workfront Planning zum Erstellen eines Datensatzes gesendet wurde.

Es wird empfohlen, auch die folgenden Artikel anzuzeigen:

* [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md)
* [Senden von Anfragen zum Erstellen von Einträgen in Adobe Workfront-Planung](/help/quicksilver/planning/requests/submit-requests.md)
* [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Überlegungen zur Genehmigung von Anfragen

* Gesendete Anfragen werden im Bereich Anfragen von Workfront mit einem der folgenden Anfragestatus angezeigt:

   * **Überprüfung ausstehend** Dieser Status wird angezeigt, wenn keine der genehmigenden Personen das Anfrageobjekt geöffnet hat.
   * **In Überprüfung**: Der Status **Ausstehende Überprüfung** ändert sich in **In Überprüfung**, wenn mindestens eine genehmigende Person das Anfrageobjekt öffnet. Der Status der Anfrage bleibt **In Überprüfung** bis alle genehmigenden Personen die Anfrage genehmigt haben.
   * **Genehmigt**: Wenn eine genehmigende Person das Anfrageobjekt genehmigt, wird ihr individueller Status **Genehmigt**, aber der Gesamtstatus des Anfrageobjekts bleibt **In Überprüfung**, bis alle genehmigenden Personen ihre Entscheidung getroffen haben. Wenn alle genehmigenden Personen eine Anfrage genehmigen, wird der Anfragestatus **Genehmigt**.
   * **Abgeschlossen**: Wenn alle genehmigenden Personen das Anfrageobjekt genehmigen, ändert sich sein Status in **Abgeschlossen** oder wenn für die Anfrage keine Genehmigung erforderlich ist.
   * **Abgelehnt**: Wenn eine genehmigende Person das Anfrageobjekt ablehnt, wird der Status **Abgelehnt**. Es wird kein Datensatz erstellt und es muss eine neue Anfrage gesendet werden, um den Datensatz zu erstellen.

* Sie können Genehmigungsinformationen zu einem Datensatz anzeigen, der durch Senden eines Anforderungsformulars in den Feldern Genehmigt von und Genehmigt am erstellt wurde. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Jedes Workfront-Paket und jedes Planungspaket</p>
ODER
<p>Beliebiges Workflow-Paket und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Planungsanfrage zum Erstellen eines Datensatzes genehmigen

Nachdem Benutzer Anforderungen zu einem Datensatztyp-Anfrageformular hinzugefügt haben, das mit einer Genehmigung verknüpft ist, wird die Anforderung an die genehmigenden Personen gesendet.

Genehmigende Personen erhalten die folgenden Benachrichtigungen über eine Anfrage, deren Genehmigung noch aussteht:

* In-App-Benachrichtigung
* Eine E-Mail-Benachrichtigung

Informationen zum Genehmigen von Anfragen aus Benachrichtigungen finden Sie in den folgenden Artikeln:

* [Verwalten von E-Mail-Benachrichtigungen in Adobe Workfront-Planung](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md)
* [Verwalten von In-App-Benachrichtigungen in Adobe Workfront-Planung](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md)

>[!NOTE]
>
>Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.

Sie können Anfragen genehmigen, um Datensätze aus der Anfrage selbst oder aus dem Widget Meine Genehmigungen auf der Startseite zu erstellen.

### Planungsanfragen über eine Benachrichtigung oder den Bereich Anfragen genehmigen

1. Öffnen Sie die Anfrage, indem Sie einen der folgenden Schritte ausführen:

   * Klicken Sie auf **Hauptmenü** ![Zeilen-](assets/lines-menu.png) in der oberen linken Ecke und klicken Sie dann auf **Anfragen** > **Neues Erlebnis verwenden** und klicken Sie auf die Anfrage mit dem Status **Überprüfung ausstehend**.

     >[!TIP]
     >
     >* Wenn Sie keinen Zugriff auf Workfront Planning haben oder keinen Zugriff zum Anzeigen von Arbeitsbereichen haben, können Sie nur über Ihre E-Mail- oder In-App-Benachrichtigungen auf eine Genehmigungsanfrage zugreifen.
     >* Über das Erlebnis für ältere Anfragen können Sie nicht auf Planungsanfragen zugreifen.

   * Klicken Sie **oben rechts** Bildschirm auf das Bereichssymbol ![Benachrichtigungsbereich) &#x200B;](assets/notifications-area-icon-unified-shell.png)Benachrichtigungen in Unified Shell“ und dann auf die Benachrichtigung über eine Anforderung mit ausstehender Genehmigung, um die Anforderung zu öffnen.
   * Wechseln Sie zur E-Mail-Benachrichtigung in Ihrer E-Mail, die Sie über eine Anfrage informiert, deren Genehmigung noch aussteht, und klicken Sie dann auf **Anfrage öffnen**, um die Anfrage zu öffnen.

   Die Anfrageseite wird im schreibgeschützten Modus geöffnet.

   ![Schreibgeschützte Anfrageseite im Prüfungsstatus](assets/read-only-reqeust-page-in-review-status.png)
1. (Optional) Klicken Sie auf **Genehmigungen** Symbol ![Genehmigungen](assets/approvals-icon.png) in der rechten oberen Ecke der Anfrage, um die genehmigenden Personen anzuzeigen.
1. Klicken Sie **Überprüfen und genehmigen** und wählen Sie dann eine der folgenden Optionen:

   * **Genehmigen**: Dadurch wird die Anfrage genehmigt. Ein Datensatz wird sofort für den mit dem Antragsformular verknüpften Datensatztyp erstellt, nachdem alle Genehmiger den Antrag genehmigt haben.
   * **Ablehnen**: Hiermit wird die Anforderung abgelehnt, selbst wenn Sie die einzige genehmigende Person sind, die sie ablehnt. Für den mit dem Anfrageformular verknüpften Datensatztyp wird kein Datensatz erstellt.

   Der Benutzer, der die Anfrage gesendet hat, erhält eine E-Mail- und In-App-Benachrichtigung, wenn seine Anfrage genehmigt oder abgelehnt wird.

   Der Status der Anfrage ändert sich je nach Genehmigungsentscheidung in Folgendes:

   * **Abgeschlossen**: Die Anfrage wurde genehmigt.
   * **Abgelehnt**: Die Anfrage wird abgelehnt.

   Die Anfrage verbleibt im Bereich **Anfragen** von Workfront.

### Genehmigen einer Anfrage über das Widget Meine Genehmigungen auf der Startseite

{{step1-to-home}}

1. Gehen Sie zum Widget **Meine Genehmigungen** in **Startseite**.

   ![Widget „Meine Genehmigungen“ auf der Startseite](assets/my-approvals-widget-in-home.png)
1. Suchen Sie die Planungsanfrage, die Sie genehmigen oder ablehnen möchten.

1. (Optional) Fügen Sie einen Kommentar hinzu, indem Sie auf den Dropdown-Pfeil neben **Genehmigen** oder **Ablehnen** klicken, die Anmerkung eingeben und auf **Hinzufügen** klicken.

1. Klicken Sie auf eine der folgenden Optionen:

   * **Genehmigen**: Dadurch wird die Anfrage genehmigt. Ein Datensatz wird sofort für den mit dem Antragsformular verknüpften Datensatztyp erstellt, nachdem alle Genehmiger den Antrag genehmigt haben.
   * **Ablehnen**: Hiermit wird die Anforderung abgelehnt, selbst wenn Sie die einzige genehmigende Person sind, die sie ablehnt. Für den mit dem Anfrageformular verknüpften Datensatztyp wird kein Datensatz erstellt.

   Der Benutzer, der die Anfrage gesendet hat, erhält eine E-Mail- und In-App-Benachrichtigung, wenn seine Anfrage genehmigt oder abgelehnt wird.

   Der Status der Anfrage ändert sich je nach Genehmigungsentscheidung in Folgendes:

   * **Abgeschlossen**: Die Anfrage wurde genehmigt.
   * **Abgelehnt**: Die Anfrage wird abgelehnt.

