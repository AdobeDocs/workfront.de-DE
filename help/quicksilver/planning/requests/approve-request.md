---
title: Genehmigen einer Anforderung in Adobe Workfront Planning
description: Wenn ein(e) Benutzende(r) eine Anfrage an ein Anforderungsformular sendet, das mit einer Genehmigung in Adobe Workfront Planning verknüpft ist, erhalten genehmigende Personen eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 1%

---

# Genehmigen einer Anforderung in Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Wenn ein(e) Benutzende(r) eine Anfrage an ein Anforderungsformular sendet, das mit einer Genehmigung in Adobe Workfront Planning verknüpft ist, erhalten genehmigende Personen eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager eine Anforderung genehmigen kann, die für Workfront Planning zum Erstellen eines Datensatzes gesendet wurde.

Es wird empfohlen, auch die folgenden Artikel anzuzeigen:

* [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)
* [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Überlegungen zur Genehmigung von Anfragen

* Gesendete Anfragen werden im Bereich Anfragen in Workfront auf der Registerkarte Planung des Abschnitts Gesendet mit einem der folgenden Anfragestatus angezeigt:

   * **Überprüfung ausstehend** Dieser Status wird angezeigt, wenn keine der genehmigenden Personen das Anfrageobjekt geöffnet hat.
   * **In Überprüfung**: Der Status **Ausstehende Überprüfung** ändert sich in **In Überprüfung**, wenn mindestens eine genehmigende Person das Anfrageobjekt öffnet. Der Status der Anfrage bleibt **In Überprüfung** bis alle genehmigenden Personen die Anfrage genehmigt haben.
   * **Genehmigt**: Wenn eine genehmigende Person das Anfrageobjekt genehmigt, wird ihr individueller Status **Genehmigt**, aber der Gesamtstatus des Anfrageobjekts bleibt **In Überprüfung**, bis alle genehmigenden Personen ihre Entscheidung getroffen haben. Wenn alle genehmigenden Personen eine Anfrage genehmigen, wird der Anfragestatus **Genehmigt**.
   * **Abgeschlossen**: Wenn alle genehmigenden Personen das Anfrageobjekt genehmigen, ändert sich sein Status in **Abgeschlossen** oder wenn für die Anfrage keine Genehmigung erforderlich ist.
   * **Abgelehnt**: Wenn eine genehmigende Person das Anfrageobjekt ablehnt, wird der Status **Abgelehnt**. Es wird kein Datensatz erstellt und es muss eine neue Anfrage gesendet werden, um den Datensatz zu erstellen.

* Sie können Genehmigungsinformationen zu einem Datensatz anzeigen, der durch Senden eines Anforderungsformulars in den Feldern Genehmigt von und Genehmigt am erstellt wurde. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<ul><li><p>Beliebiges Workfront-Paket</p></li>
Und
<li><p>Beliebiges Planungspaket</p></li></ul>
Oder
<ul><li><p>Beliebiges Workflow-Paket</p></li>
Und
<li><p>Beliebiges Planungspaket</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p> 
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

## Genehmigen einer Anfrage zum Erstellen eines Datensatzes

Nachdem Benutzer Anforderungen zu einem Datensatztyp-Anfrageformular hinzugefügt haben, das mit einer Genehmigung verknüpft ist, wird die Anforderung an die genehmigenden Personen gesendet.

Genehmigende Personen erhalten die folgenden Benachrichtigungen über eine Anfrage, deren Genehmigung noch aussteht:

* In-App-Benachrichtigung
* Eine E-Mail-Benachrichtigung

>[!NOTE]
>
>Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.

So validieren Sie eine Anfrage:

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie Zugriff auf Workfront Planning haben und mindestens einen Arbeitsbereich anzeigen können, klicken Sie auf **Hauptmenü** ![Punkte-](assets/dots-menu.png) oben rechts im Bildschirm oder auf das **&#x200B;**&#x200B;Hauptmenü![Zeilen-Hauptmenü](assets/lines-menu.png) oben links, falls verfügbar. Klicken Sie dann auf **Anfragen** > **Eingereicht** > **Planung** und klicken Sie auf die Anfrage mit dem Status **Ausstehende Überprüfung** oder **In Überprüfung**.

     >[!TIP]
     >
     >Wenn Sie keinen Zugriff auf Workfront Planning haben oder keinen Zugriff zum Anzeigen von Arbeitsbereichen haben, können Sie nur über Ihre E-Mail- oder In-App-Benachrichtigungen auf eine Genehmigungsanfrage zugreifen.

   * Klicken Sie **oben rechts** Bildschirm auf das Bereichssymbol ![Benachrichtigungsbereich) &#x200B;](assets/notifications-area-icon-unified-shell.png)Benachrichtigungen in Unified Shell“ und dann auf die Benachrichtigung über eine Anforderung mit ausstehender Genehmigung, um die Anforderung zu öffnen.
   * Wechseln Sie zur E-Mail-Benachrichtigung in Ihrer E-Mail, die Sie über eine Anfrage informiert, deren Genehmigung noch aussteht, und klicken Sie dann auf **Anfrage öffnen**, um die Anfrage zu öffnen. <!--add the name of the button here, from the email-->

   Die Anfrageseite wird im schreibgeschützten Modus geöffnet.

   ![Schreibgeschützte Anfrageseite im Prüfungsstatus](assets/read-only-reqeust-page-in-review-status.png)

1. (Optional) Klicken Sie auf **Genehmigungen** Symbol ![Genehmigungen](assets/approvals-icon.png) in der rechten oberen Ecke der Anfrage, um die genehmigenden Personen anzuzeigen.
1. Klicken Sie **Überprüfen und genehmigen** und wählen Sie dann eine der folgenden Optionen:

   * **Genehmigen**: Dadurch wird die Anfrage genehmigt. Ein Datensatz wird sofort für den mit dem Antragsformular verknüpften Datensatztyp erstellt, nachdem alle Genehmiger den Antrag genehmigt haben.
   * **Ablehnen**: Hiermit wird die Anforderung abgelehnt, selbst wenn Sie die einzige genehmigende Person sind, die sie ablehnt. Für den mit dem Anfrageformular verknüpften Datensatztyp wird kein Datensatz erstellt.

   Der Benutzer, der die Anfrage gesendet hat, erhält eine E-Mail und In-App-Benachrichtigungen, wenn seine Anfrage genehmigt oder abgelehnt wird.

   Der Status der Anfrage ändert sich je nach Genehmigungsentscheidung in Folgendes:

   * **Abgeschlossen**: Die Anfrage wurde genehmigt.
   * **Abgelehnt**: Die Anfrage wird abgelehnt.

   Die Anfrage verbleibt auf der Registerkarte Planung im Abschnitt Gesendet im Bereich Anfragen in Workfront.
