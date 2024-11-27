---
title: Eine Anforderung genehmigen
description: Wenn ein Benutzer eine Anforderung an ein Anforderungsformular sendet, das mit einer Genehmigung in der Adobe Workfront-Planung verknüpft ist, erhalten Genehmiger eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 1%

---


<!--

---
title: Approve a Request
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->


# Anfrage genehmigen

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Wenn ein Benutzer eine Anforderung an ein Anforderungsformular sendet, das mit einer Genehmigung in der Adobe Workfront-Planung verknüpft ist, erhalten Genehmiger eine Benachrichtigung und eine E-Mail über die ausstehende Genehmigung. Sie müssen die Anfrage genehmigen, bevor Workfront Planning ein Objekt erstellt.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager eine Anforderung genehmigen kann, die für die Workfront-Planung eingereicht wurde, um einen Datensatz zu erstellen.

Es wird empfohlen, auch die folgenden Artikel anzuzeigen:

* [Anforderungsformular in der Adobe Workfront-Planung erstellen und verwalten](/help/quicksilver/planning/requests/create-request-form.md)
* [Planungsanfragen für Adobe Workfront zur Erstellung von Datensätzen übermitteln](/help/quicksilver/planning/requests/submit-requests.md)
* [Hinzufügen einer Validierung zu einem Anforderungsformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Überlegungen zum Genehmigen von Anforderungen und Anfragestatus

Gesendete Anfragen werden im Tab Planung des Abschnitts Gesendet im Bereich Anforderungen von Workfront mit einem der folgenden Anfragestatus angezeigt:

* **Ausstehende Überprüfung**: Dieser Status wird angezeigt, wenn keiner der Genehmiger das Anfrageobjekt geöffnet hat.
* **Im Review**: Der Status ändert sich in **Im Review** , wenn mindestens ein Genehmiger das Anfrageobjekt öffnet.
* **Genehmigt**: Wenn ein Genehmiger das Anfrageobjekt genehmigt, wird sein individueller Status zu
* **Genehmigt**, aber der Gesamtstatus des Anfrageobjekts bleibt **In Überprüfung**, bis alle Genehmiger ihre Entscheidungen getroffen haben.
* **Abgeschlossen**: Wenn alle Genehmiger das Anfrageobjekt genehmigen, ändert sich sein Status in **Abgeschlossen** oder wenn für die Anfrage keine Genehmigung erforderlich ist.
* **Abgelehnt**: Wenn ein Genehmiger das Anfrageobjekt ablehnt, erhält der Status den Status **Abgelehnt** .

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkte</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront-Planung<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td>
   <td>
<p>Die folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td>
   <td>
<p>Alle </p>  
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Berechtigungen für einen Arbeitsbereich verwalten</p></li>
    <li><p>Systemadministratoren können nicht erstellte Arbeitsbereiche verwalten. </p></li>
    </ul>
   <p>Informationen zum Freigeben von Berechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Überblick über die Freigabe von Berechtigungen in der Adobe Workfront-Planung</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anfrage zum Erstellen eines Datensatzes genehmigen

Nachdem Benutzer Anforderungen zu einem Anforderungsformular für den Datensatztyp hinzugefügt haben, das mit einer Genehmigung verknüpft ist, wird die Anforderung an die Genehmiger gesendet.

Validierungsverantwortliche erhalten die folgenden Benachrichtigungen zu einer Anfrage, die noch nicht genehmigt wurde:

* In-App-Benachrichtigung
* Eine E-Mail-Benachrichtigung

So genehmigen Sie eine Anforderung:

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in Ihrem Workfront-Hauptmenü **** ![](assets/dots-menu.png) oben rechts auf dem Bildschirm oder, falls verfügbar, im Menü **Hauptmenü** ![](assets/lines-menu.png) oben links auf **Anforderungen** > **Gesendet** > **Planung** und klicken Sie auf die Anfrage mit dem Status **Im Review** <!--did they change this to Pending approval; logged  a bug-->. 4}
   * Gehen Sie in den Bereich **Benachrichtigungen** oben rechts im Bildschirm und klicken Sie auf die Benachrichtigung über eine Anforderung, deren Genehmigung aussteht, um die Anfrage zu öffnen.
   * Rufen Sie die E-Mail-Benachrichtigung in Ihrer E-Mail auf, die Sie über eine Anforderung informiert, deren Genehmigung noch aussteht, und klicken Sie dann auf , um die Anfrage zu öffnen. <!--add the name of the button here, from the email-->

   Die Anfrageseite wird im schreibgeschützten Modus geöffnet.

   ![](assets/read-only-reqeust-page-in-review-status.png)
1. (Optional) Klicken Sie oben rechts in der Anfrage auf das Symbol **Genehmigungen** ![](assets/approvals-icon.png) , um die Genehmiger anzuzeigen.
1. Klicken Sie auf **Überprüfen und genehmigen** und wählen Sie dann eine der folgenden Optionen: <!--did they fix the button and removed the &??-->

   * **Genehmigen**: Um die Anfrage zu genehmigen. Für den mit dem Anfrageformular verknüpften Datensatztyp wird sofort ein Datensatz erstellt.
   * **Ablehnen**: Um die Anfrage abzulehnen. Für den mit dem Anfrageformular verknüpften Datensatztyp wird kein Datensatz erstellt. <!--check to see if there is a notification sent to the requestor about it being rejected OR approved??-->
