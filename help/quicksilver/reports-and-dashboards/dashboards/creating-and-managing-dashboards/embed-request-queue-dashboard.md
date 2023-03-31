---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Einbetten einer Anforderungswarteschlange in ein Dashboard
description: Sie können eine neue Anforderungswarteschlange in ein Dashboard einbetten, um Ihren Benutzern direkten Zugriff auf die Anforderungswarteschlange zu ermöglichen, ohne zum Bereich Anforderungen wechseln zu müssen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 2894161b61a00dab04c17ef642ace4a45179eb17
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# Einbetten einer Anforderungswarteschlange in ein Dashboard

Sie können eine neue Anforderungswarteschlange in ein Dashboard einbetten, um Ihren Benutzern direkten Zugriff auf die Anforderungswarteschlange zu ermöglichen, ohne zum Bereich Anforderungen wechseln zu müssen. 

Wenn Sie beispielsweise über eine Anforderungswarteschlange verfügen, die für Ihr gesamtes Unternehmen geöffnet ist, z. B. eine Help Desk Queue oder eine PTO Request-Warteschlange, auf die jeder regelmäßig zugreifen muss, kann es praktisch sein, die Anforderungswarteschlange direkt in eines seiner Dashboards einzufügen, um schnellen und einfachen Zugriff zu erhalten. Die Einrichtung erfolgt ähnlich wie die Erstellung einer externen Seite in einem Dashboard.

Zunächst müssen Sie eine URL für die Anforderungswarteschlange abrufen. Zweitens können Sie die URL in ein Dashboard einbetten, indem Sie eine externe Seite hinzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für das Dashboard verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie eine Anforderungswarteschlange in ein Dashboard einbetten können, müssen Sie beide folgenden Elemente erstellen:

* **Das Dashboard**: Informationen zum Erstellen von Dashboards finden Sie unter [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **Die Anforderungswarteschlange**: Informationen zum Erstellen von Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## URL der Anforderungswarteschlange abrufen {#obtain-the-url-of-the-request-queue}

Sie können die URL einer Anforderungswarteschlange auf verschiedene Weise abrufen, je nachdem, welcher Teil der Anforderungswarteschlange den Benutzern angezeigt werden soll, wenn sie über ein Dashboard darauf zugreifen.

* [Link zu einem bestimmten Warteschlangenthema mit der Möglichkeit, den Anfragetyp zu ändern](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [Link zu einer Anforderungswarteschlange abrufen und Anfragetyp ändern](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [Link zu einer Anforderungswarteschlange ohne Möglichkeit zum Ändern des Anfragetyps abrufen](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Link zu einem bestimmten Warteschlangenthema mit der Möglichkeit, den Anfragetyp zu ändern {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Wenn Sie einen Link zu einem bestimmten Warteschlangenthema für andere Benutzer freigeben, wird das Anforderungsformular im exakten Warteschlangenthema geöffnet, das zum Senden der Anforderung verwendet werden muss. Dies ist hilfreich, wenn Benutzer möglicherweise nicht sicher sind, welches Warteschlangenthema beim Protokollieren von Anforderungen für eine bestimmte Anforderungswarteschlange ausgewählt werden soll.

Benutzer können den Anfragetyp ändern oder bei Bedarf ein anderes Thema auswählen. Auch die Navigation im Bereich Anforderungen wird angezeigt.

1. Klicken Sie auf **Hauptmenü** > **Anforderungen** > **Neue Anforderung**.
1. Wenn Sie bestimmte Warteschlangen freigeben möchten, wählen Sie weiterhin Themengruppen und Warteschlangenthemen aus, bis Sie die Warteschlange erreichen, die Sie im Dashboard freigeben möchten. Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >Die Auswahl von Themengruppen und Themen in der Warteschlange ist optional.

1. Klicken **Freigabepfad** in der oberen rechten Ecke des Bereichs &quot;Neue Anforderung&quot;.

   Dadurch wird der Link in die Anforderungswarteschlange oder das Warteschlangenthema kopiert, während Sie ihn auf dem Bildschirm anzeigen. Benutzer können den Anfragetyp oder eine der verfügbaren Themengruppen und Warteschlangenthemen aktualisieren.

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Link zu einer Anforderungswarteschlange abrufen und Anfragetyp ändern {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Wenn Sie einen Link für einen Anfragetyp freigeben, wird der Anfragetyp für den Benutzer ausgewählt. Dies ist hilfreich, wenn Benutzer aus mehreren Themengruppen oder Themen in der Warteschlange für denselben Anfragetyp wählen müssen. Benutzer können den Anfragetyp ändern und einen anderen wählen. Auch die Navigation im Bereich Anforderungen wird angezeigt.

1. Wechseln Sie zu einem Projekt, das als Anforderungswarteschlange bezeichnet wurde.

   Informationen zum Erstellen einer Anforderungswarteschlange aus einem Projekt finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Navigieren Sie zu **Warteschlangendetails**.
1. Kopieren Sie den Code, den Sie im **Direct Access-URL** -Feld.

   Der Code sollte in etwa wie folgt aussehen:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Dies ist der Link zur Anforderungswarteschlange, die mit dem ausgewählten Projekt verknüpft ist. Der Anfragetyp ist vorausgewählt.

   Benutzer können eine beliebige Themengruppe oder ein beliebiges Warteschlangenthema auswählen oder einen anderen Anfragetyp auswählen.

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Link zu einer Anforderungswarteschlange ohne Möglichkeit zum Ändern des Anfragetyps abrufen {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Wenn Sie einen Link für einen vorab ausgewählten Anfragetyp freigeben, wird der Anfragetyp für den Benutzer ausgewählt und kann nicht geändert werden (abgeblendet). Benutzer können die Themengruppen oder Themen in der Warteschlange auswählen, die sie benötigen. Dies ist hilfreich, wenn Sie nicht möchten, dass Benutzer andere Anfragetypen anzeigen und auswählen können. Die Navigation des Anforderungsbereichs wird nicht angezeigt.

1. Wechseln Sie zu einem Projekt, das als Anforderungswarteschlange bezeichnet wurde.

   Informationen zum Erstellen einer Anforderungswarteschlange aus einem Projekt finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Navigieren Sie zu **Warteschlangendetails**.
1. Kopieren Sie den Code, den Sie im **Eingebetteter Code** -Feld.

   Der Code sollte in etwa wie folgt aussehen:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Bearbeiten Sie den Code so, dass nur die folgenden Informationen beibehalten werden:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Sie können eine `<samp>iframe </samp>` -Tag, wenn Sie den Code in eine andere Anwendung als Workfront einbetten.

   Dies ist der Link zur Anforderungswarteschlange, die mit dem ausgewählten Projekt verknüpft ist. Der Anfragetyp ist vorausgewählt und kann nicht geändert werden.

   Benutzer können eine beliebige Themengruppe oder ein beliebiges Thema für die Warteschlange auswählen, die bzw. das sie für den ausgewählten Anfragetyp benötigen. Benutzer können keinen anderen Anfragetyp auswählen.

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Einbetten einer Anforderungswarteschlange in ein Dashboard

Sie können einen Link zur Anforderungswarteschlange oder zu einem Warteschlangenthema, das unter einer Anforderungswarteschlange verschachtelt ist, in ein Dashboard einbetten, um Benutzern direkten Zugriff auf die Eingabe von Anforderungen zu ermöglichen.

1. Rufen Sie eine Anforderungs-Warteschlangen-URL mit einer der im Abschnitt [URL der Anforderungswarteschlange abrufen](#obtain-the-url-of-the-request-queue) Abschnitt dieses Artikels.
1. Klicken Sie auf **Hauptmenü** > **Dashboards** > **Neues Dashboard**.
1. Geben Sie einen **Name** für das Dashboard. Dies ist ein Pflichtfeld.
1. Klicken **Externe Seite hinzufügen**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. Im **Externe Seite hinzufügen** Bearbeiten Sie die folgenden Felder:

   * **Name**: Geben Sie den Namen der Anforderungswarteschlange so ein, wie er im Dashboard angezeigt werden soll. Dies ist ein Pflichtfeld.

   * **Beschreibung**: Geben Sie eine Beschreibung ein, die diese externe Seite anzeigt. Dies ist kein erforderliches Feld und nur für Berichtszwecke wichtig. Sie wird nicht im Dashboard angezeigt.
   * **URL**: Fügen Sie die URL ein, die Sie mit einer der in Schritt 1 beschriebenen Methoden erhalten haben.

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **Höhe**: Geben Sie die Höhe der externen Seite ein. Dadurch wird festgelegt, wie viel Platz die externe Seite, die die Anforderungswarteschlange enthält, im Dashboard belegt. Dies ist ein erforderliches Feld und der Standardwert ist 500.

1. Klicken Sie auf **Speichern**.
1. Klicken **Speichern und schließen**. 

   Die Anforderungswarteschlange wird im Dashboard als separate Dashboard-Komponente angezeigt.

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. (Optional) Klicken Sie auf **Dashboard-Aktionen**, dann **Bearbeiten** , um dem Dashboard Berichte, Kalender oder zusätzliche externe Seiten hinzuzufügen.\
   Informationen zum Hinzufügen von Komponenten zu einem Dashboard finden Sie unter [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

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
