---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Einbetten einer Anfrage-Warteschlange in ein Dashboard
description: Sie können eine neue Anfrage-Warteschlange in ein Dashboard einbetten, um Ihren Benutzern direkten Zugriff auf die Anfrage-Warteschlange zu ermöglichen, ohne den Bereich Anfragen aufrufen zu müssen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 1%

---

# Einbetten einer Anfrage-Warteschlange in ein Dashboard

<!-- Audited: 1/2025 -->

Sie können eine neue Anfrage-Warteschlange in ein Dashboard einbetten, um Ihren Benutzern direkten Zugriff auf die Anfrage-Warteschlange zu ermöglichen, ohne den Bereich Anfragen aufrufen zu müssen.

Wenn Sie beispielsweise über eine Anfrage-Warteschlange verfügen, die für Ihr gesamtes Unternehmen offen ist, z. B. eine Helpdesk-Warteschlange oder eine PTO-Anfrage-Warteschlange, auf die alle Benutzer regelmäßig zugreifen müssen, kann es praktisch sein, die Anfrage-Warteschlange direkt in eines ihrer Dashboards einzufügen, um einen schnellen und einfachen Zugriff zu ermöglichen. Der Prozess der Einrichtung ähnelt dem Prozess der Erstellung einer externen Seite in einem Dashboard.

Zunächst müssen Sie eine URL für die Anfrage-Warteschlange abrufen. Zweitens können Sie die URL in ein Dashboard einbetten, indem Sie eine externe Seite hinzufügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Dashboard</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Voraussetzungen

Beide der folgenden Schritte müssen erstellt werden, bevor Sie eine Anfrage-Warteschlange in ein Dashboard einbetten können:

* **Das Dashboard**: Informationen zum Erstellen von Dashboards finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

* **Die Anfrage-Warteschlange**: Informationen zum Erstellen von Anfrage-Warteschlangen finden Sie [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Abrufen der URL der Anfrage-Warteschlange {#obtain-the-url-of-the-request-queue}

Sie können die URL einer Anfrage-Warteschlange auf verschiedene Arten abrufen, je nachdem, welchen Teil der Anfrage-Warteschlange Sie den Benutzern bereitstellen möchten, wenn sie über ein Dashboard darauf zugreifen.

* [Erhalten Sie einen Link zu einem bestimmten Warteschlangen-Thema mit der Möglichkeit, den Anfragetyp zu ändern](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [Erhalten Sie einen Link zu einer Anfrage-Warteschlange und die Möglichkeit, den Anfragetyp zu ändern](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [Abrufen eines Links zu einer Anfrage-Warteschlange ohne Möglichkeit, den Anfragetyp zu ändern](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Abrufen eines Links zu einem bestimmten Warteschlangenthema mit der Möglichkeit, den Anfragetyp zu ändern {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Wenn Sie einen Link zu einem bestimmten Warteschlangenthema für andere Benutzer freigeben, wird das Anfrageformular mit genau dem Warteschlangenthema geöffnet, das diese Benutzer zum Senden der Anfrage verwenden müssen. Dies ist hilfreich, wenn Benutzende möglicherweise nicht sicher sind, welches Warteschlangen-Thema beim Protokollieren von Anfragen für eine bestimmte Anfragewarteschlange ausgewählt werden soll.

Benutzer können bei Bedarf den Anfragetyp ändern oder ein anderes Thema auswählen. Die Navigation im Bereich Anfragen wird ebenfalls angezeigt.

1. Klicken Sie auf **Hauptmenü** > **Anfragen** > **Neue Anfrage**.
1. Wählen Sie weiterhin Themengruppen und Warteschlangenthemen aus, bis Sie die Warteschlange erreichen, die Sie im Dashboard freigeben möchten, falls Sie eine bestimmte Warteschlange freigeben möchten. Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >Die Auswahl von Themengruppen und Warteschlangenthemen ist optional.

1. Klicken Sie **Freigabepfad** in der oberen rechten Ecke des Bereichs Neue Anfrage .

   Dadurch wird der Link in die Anfrage-Warteschlange oder das Warteschlangen-Thema so kopiert, wie Sie es auf dem Bildschirm anzeigen. Benutzer können den Anfragetyp oder eine beliebige Themengruppe und Warteschlangenthemen aktualisieren, die verfügbar sind.

   ![Anfrage-Warteschlange mit Freigabepfad](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Anforderungswarteschlange und Möglichkeit zum Ändern des Anforderungstyps verknüpfen {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Wenn Sie einen Link für einen Anfragetyp freigeben, wird der Anfragetyp für den Benutzer ausgewählt. Dies ist hilfreich, wenn Benutzende aus mehreren Themengruppen oder Warteschlangenthemen für denselben Anfragetyp auswählen müssen. Benutzer können den Anfragetyp ändern und einen anderen auswählen. Die Navigation im Bereich Anfragen wird ebenfalls angezeigt.

1. Zu einem Projekt gehen, das als Anfrage-Warteschlange bezeichnet wird.

   Informationen zum Erstellen einer Anfrage-Warteschlange aus einem Projekt finden Sie unter [Erstellen einer Anfrage-](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Navigieren Sie zu **Warteschlangendetails**.
1. Kopieren Sie den Code, den Sie im Feld **URL für den direkten Zugriff** finden.

   Der Code sollte etwa wie folgt aussehen:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Dies ist der Link zur Anfrage-Warteschlange, die mit dem ausgewählten Projekt verknüpft ist. Der Anfragetyp ist vorausgewählt.

   Benutzende können eine beliebige Themengruppe oder ein Warteschlangen-Thema auswählen oder einen anderen Anfragetyp auswählen.

   ![Anfrage-Warteschlangen-URL](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Abrufen eines Links zu einer Anfrage-Warteschlange ohne Möglichkeit, den Anfragetyp zu ändern {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Wenn Sie einen Link für einen vorab ausgewählten Anfragetyp freigeben, ist der Anfragetyp für den Benutzer ausgewählt und kann nicht geändert werden (er ist abgeblendet). Benutzer können die Themengruppen oder Warteschlangenthemen auswählen, die sie benötigen. Dies ist hilfreich, wenn Sie nicht möchten, dass Benutzer andere Anfragetypen anzeigen und auswählen. Die Navigation im Bereich Anfragen wird nicht angezeigt.

1. Zu einem Projekt gehen, das als Anfrage-Warteschlange bezeichnet wird.

   Informationen zum Erstellen einer Anfrage-Warteschlange aus einem Projekt finden Sie unter [Erstellen einer Anfrage-](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Navigieren Sie zu **Warteschlangendetails**.
1. Kopieren Sie den Code, den Sie im Feld **Eingebetteter Code** finden.

   Der Code sollte etwa wie folgt aussehen:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Bearbeiten Sie den Code so, dass nur die folgenden Informationen beibehalten werden:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Sie können ein `<samp>iframe </samp>`-Tag hinzufügen, wenn Sie den Code in eine andere Anwendung als Workfront einbetten.

   Dies ist der Link zur Anfrage-Warteschlange, die mit dem ausgewählten Projekt verknüpft ist. Der Anfragetyp ist vorausgewählt und kann nicht geändert werden.

   Benutzende können eine beliebige Themengruppe oder ein Warteschlangenthema auswählen, das sie für den ausgewählten Anfragetyp benötigen. Benutzende können keinen anderen Anfragetyp auswählen.

   ![Anfrage-Warteschlangen-Code](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Einbetten einer Anfrage-Warteschlange in ein Dashboard

Sie können einen Link zur Anfragewarteschlange oder zu einem Warteschlangen-Thema, das unter einer Anfragewarteschlange verschachtelt ist, in ein Dashboard einbetten, um Benutzern direkten Zugriff auf eingegebene Anfragen zu gewähren.

1. Rufen Sie eine URL für die Anforderungswarteschlange mit einer der Methoden ab, die im Abschnitt [Abrufen der URL &#x200B;](#obtain-the-url-of-the-request-queue) Anforderungswarteschlange“ dieses Artikels beschrieben sind.

1. Klicken Sie auf **Hauptmenü** > **Dashboards** > **Neues Dashboard**.

1. Geben Sie **Dashboard** Name“ ein. Dies ist ein Pflichtfeld.

1. Klicken Sie **Externe Seite hinzufügen**.

   ![Externe Seite](assets/add-external-page-highlighted---nwe-350x214.png)

1. Bearbeiten **im Feld** Externe Seite hinzufügen“ die folgenden Felder:

   * **Name**: Geben Sie den Namen der Anfrage-Warteschlange ein, wie er im Dashboard angezeigt werden soll. Dies ist ein Pflichtfeld.

   * **Beschreibung**: Geben Sie eine Beschreibung ein, über die diese externe Seite angezeigt wird. Dies ist kein Pflichtfeld und nur für Berichtszwecke wichtig. Er wird nicht im Dashboard angezeigt.

   * **URL**: Fügen Sie die URL ein, die Sie mit einer der in Schritt 1 beschriebenen Methoden erhalten haben.

   * **Höhe**: Geben Sie die Höhe der externen Seite ein. Dadurch wird festgelegt, wie viel Platz die externe Seite, die die Anfrage-Warteschlange enthält, im Dashboard belegt. Dies ist ein Pflichtfeld und der Standardwert ist 500.

1. Klicken Sie auf **Speichern**.

1. Klicken Sie auf **Speichern + schließen**.

   Die Anfrage-Warteschlange wird im Dashboard als separate Dashboard-Komponente angezeigt.

1. (Optional) Klicken Sie auf **Dashboard-Aktionen** und dann **Bearbeiten**, um Berichte, Kalender oder zusätzliche externe Seiten zum selben Dashboard hinzuzufügen.

   Informationen zum Hinzufügen von Komponenten zu einem Dashboard finden Sie unter [Erstellen eines Dashboards](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
