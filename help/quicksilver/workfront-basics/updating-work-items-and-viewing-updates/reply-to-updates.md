---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Antworten auf Aktualisierungen
description: Wenn ein Benutzer ein Update zu einem Arbeitsobjekt hinzufügt oder darauf antwortet, wird seine Antwort im Kommunikations-Thread im Abschnitt Updates des Objekts angezeigt. Sie können eine Antwort zu einem Update hinzufügen oder auf "Gefällt mir"-Klicks klicken, wenn Sie Zugriff auf das Objekt "Ansicht"haben.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# Antworten auf Aktualisierungen

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers only in the Preview environment.</span>-->

>[!NOTE]
>
>Die Kommentarerfahrung in Adobe Workfront wird derzeit umgestaltet.
>
>Weitere Informationen zum neuen Kommentierungserlebnis finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>Für die folgenden Objekte können Sie auf das neue Erlebnis zugreifen:
> * Probleme, Projekte, Aufgaben und Dokumente.
>
>     Dies ist verfügbar, wenn Sie das Beta-Kommentar-Erlebnis aktivieren.
>
>     Diese Funktion ist nur für den Abschnitt Updates verfügbar und nicht für die folgenden Bereiche:
>
>     * Startseite
>     * Zusammenfassungsbereich in Listen
>     * Zusammenfassungsbereich in Timesheets
>
> * Ziele, Karten im Bereich der Foren
>
>   Das neue Kommentarerlebnis ist das einzige Erlebnis für Ziele und Karten. Sie benötigen eine zusätzliche Lizenz für den Zugriff auf Workfront Goals. Weitere Informationen finden Sie unter [Anforderungen für die Verwendung von Workfront-Zielen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     Sie können Karten im Bereich &quot;Pinnwände&quot;um Aktualisierungen ergänzen und anzeigen, wenn Sie die Abschnitte &quot;Kommentare&quot;und &quot;Systemaktivität&quot;auf einer Karte aktivieren. Weitere Informationen finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md).


Wenn ein Benutzer auf einen Kommentar oder ein Systemaktualisierung zu einem Arbeitsobjekt antwortet, wird seine Antwort im Kommunikations-Thread im Abschnitt Updates für das Objekt angezeigt.

>[!IMPORTANT]
>
>Es ist nicht möglich, auf Systemaktualisierungen im neuen Beta-Kommentarerlebnis zu antworten. Weitere Informationen finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


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
   <td> <p>Anfrage oder höher für Probleme und Dokumente; Überprüfen oder höher für alle anderen Objekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Anforderer oder höher für Probleme und Dokumente; Für alle anderen Objekte validieren oder höher</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf das Objekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Antworten auf ein Update oder eine Antwort

Sie können auf einen Kommentar im Thread eines Objekts antworten, das Sie anzeigen können, oder sich als Workfront- oder Gruppenadministrator anmelden und im Namen eines anderen Benutzers auf einen Kommentar antworten. Weitere Informationen finden Sie unter [Anmelden als anderer Benutzer](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Die Antwort auf einen Kommentar oder eine Antwort hängt davon ab, welches Erlebnis und welches Objekt Sie auswählen.

### Antworten auf ein Update oder eine Antwort im Abschnitt &quot;Aktuelle Updates&quot;

1. Markieren Sie das Objekt, dem Sie eine Antwort hinzufügen möchten.
1. Im **Updates** -Registerkarte für das Objekt, suchen Sie nach der Aktualisierung oder Antwort, auf die Sie antworten möchten.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um ein Bild in der vorhandenen Aktualisierung anzuzeigen:

   * Klicken Sie auf **Vorschau** icon ![](assets/previewimageicon-31x31.png) auf der Miniaturansicht des Bildes, um das Bild in voller Größe in einer neuen Browser-Registerkarte zu öffnen.
   * Klicken Sie auf **Download** icon ![](assets/downloadimageicon.png) auf der Miniaturansicht, um das Bild herunterzuladen.

1. Klicken **Antwort** Geben Sie bei der Aktualisierung eine Antwort in das angezeigte Feld ein.

   Oben in diesem Aktualisierungs-Thread können Sie die Benutzer sehen, die aktiv an der Konversation beteiligt sind oder in jeder Antwort getaggt sind. Diese Benutzer erhalten zusammen mit allen Benutzern, die das Objekt abonniert haben, eine Benachrichtigung, sobald ein Objekt aktualisiert oder beantwortet wird. Sie können auch weitere Benutzer taggen, um sie in Ihre Antwort einzubeziehen.  Informationen zum Tagging weiterer Benutzer finden Sie unter [Tagging anderer Benutzer auf Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Optional) Wenn Sie Text aus einer vorherigen Aktualisierung in Ihre Antwort aufnehmen möchten, klicken Sie auf die **Mehr** neben der Aktualisierung oder Antwort, die Sie zitieren möchten, klicken Sie auf **Antwort zitieren**. Text aus der vorherigen Aktualisierung wird im Eingabefeld mit einer vertikalen grauen Linie markiert.
1. (Optional) Verwenden Sie Formatierungen, Emojis, Include-Links oder Bilder, wie im Artikel &quot;Verwenden von Rich Text in einem Workfront-Update&quot;beschrieben. [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Klicken **Antwort** , um die Antwort zu speichern.

### Antworten auf einen Kommentar bei Verwendung des Beta-Kommentars

Informationen darüber, welche Funktionen für das neue Kommentierungserlebnis verfügbar sind und welche Objekte verfügbar sind, finden Sie unter [Neues Kommentierungserlebnis](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Markieren Sie das Objekt, dem Sie eine Antwort hinzufügen möchten.
1. Klicken **Updates** und klicken Sie dann auf **Kommentare** für das Objekt ein und suchen Sie nach dem Kommentar oder der Antwort, auf den/die Sie antworten möchten.
1. (Optional) Wenn Sie Text aus einer vorherigen Aktualisierung in Ihre Antwort aufnehmen möchten, klicken Sie auf die **Mehr** neben der Aktualisierung oder Antwort, die Sie zitieren möchten, klicken Sie auf **Anführungsantwort**. Text aus der vorherigen Aktualisierung wird im Eingabefeld mit einer vertikalen grauen Linie markiert.
1. Klicken **Antwort**.

   Sie können die Benutzer sehen, die aktiv an der Unterhaltung beteiligt sind am unteren Rand der **Neuer Kommentar** und Sie können weitere hinzufügen oder die nicht mehr relevanten entfernen. Diese Benutzer erhalten zusammen mit allen Benutzern, die das Objekt abonniert haben, eine Benachrichtigung, sobald ein Objekt aktualisiert oder beantwortet wird. Sie können auch weitere Benutzer taggen, um sie in Ihre Antwort einzubeziehen.  Informationen zum Tagging weiterer Benutzer finden Sie unter [Tagging anderer Benutzer auf Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Beginnen Sie mit der Eingabe Ihrer Antwort und verwenden Sie zusätzliche Optionen aus der Rich-Text-Symbolleiste. Informationen zur Verwendung von Rich Text oder anderen Aktualisierungsfunktionen finden Sie unter [Update der Arbeit](../updating-work-items-and-viewing-updates/update-work.md).

1. Klicken **Einsenden** , um die Antwort zu speichern.

1. (Optional) Klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) neben der Aktualisierung finden Sie weitere Optionen zum Verwalten der Antwort. Weitere Informationen finden Sie unter [Update der Arbeit](../updating-work-items-and-viewing-updates/update-work.md).


## Antworten auf eine Aktualisierung per E-Mail-Benachrichtigung

Abhängig von der Konfiguration Ihrer E-Mail-Benachrichtigungen erhalten Sie möglicherweise eine E-Mail-Benachrichtigung, wenn eine Aktualisierung an bestimmten Objekten vorgenommen wird, auf die Sie Zugriff haben.

>[!NOTE]
>
>Die Antwort auf Updates per E-Mail ist für Umgebungen auf Cluster 6 nicht verfügbar.

Im Folgenden finden Sie ein Beispiel für eine E-Mail-Benachrichtigung, die durch eine Aktualisierung ausgelöst wird, die auf dem Tab Aktualisierungen einer Aufgabe vorgenommen wurde:

![email.png](assets/email-350x202.png)

Sie können aus der E-Mail einfach eine Antwort direkt zum Kommunikations-Thread des Objekts in Workfront hinzufügen. Sie können auch eine Antwort hinzufügen, ohne sich bei Workfront anzumelden, und zwar in einer E-Mail, die aus Kommentaren generiert wird, die an folgende Objekte gesendet wurden:

* Projekt
* Aufgabe
* Problem
* Dokument
* Vorlagen- und Vorlagenaufgaben
* Portfolio
* Programm
* Wiederholung
* Arbeitszeittabelle

### Antwort auf eine Aktualisierung einer E-Mail-Benachrichtigung

Wenn Sie eine E-Mail-Benachrichtigung erhalten, können Sie das zugehörige Workfront-Objekt schnell öffnen und eine Antwort direkt zum Kommunikations-Thread hinzufügen.

1. Klicken **Kommentar** in der E-Mail-Benachrichtigung.

   Die Detailseite für das Objekt wird in Workfront geöffnet.

1. Gehen Sie zu der Aktualisierung, auf die Sie eine Antwort hinzufügen möchten.

   Neben der Anzeige der Benutzer, die aktiv an der Konversation beteiligt sind, können Sie in jeder Antwort sehen, wer in diesem Aktualisierungs-Thread getaggt wurde. Diese Benutzer sowie alle Benutzer, die das Objekt abonniert haben, erhalten eine Benachrichtigung, sobald eine Aktualisierung oder Antwort am Objekt vorgenommen wird. Informationen zum Tagging weiterer Benutzer finden Sie unter [Tagging anderer Benutzer auf Updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Klicken **Antwort,** Geben Sie Ihre Antwort ein und klicken Sie auf **Antwort**.

### Hinzufügen einer Aktualisierung zu einem Objekt außerhalb von Workfront

Wenn Sie eine Workfront-E-Mail-Benachrichtigung erhalten, können Sie schnell eine Aktualisierung zum Kommunikations-Thread hinzufügen, ohne sich bei Workfront anzumelden.

So fügen Sie einer Workfront-E-Mail ein Update hinzu:

1. Öffnen Sie in Ihrer E-Mail-Anwendung die Workfront-E-Mail, auf die Sie antworten möchten, und öffnen Sie dann ein E-Mail-Fenster für Antworten.
1. Geben Sie Ihre Aktualisierung ein.\
   Anhänge sind nicht zulässig und Rich-Text-Formatierungen, die auf eine Aktualisierung in einer E-Mail angewendet werden, werden nicht in der Aktualisierung angezeigt, wenn sie auf der Registerkarte Aktualisierungen angezeigt werden.
1. Klicken **Senden**.

   Ihre Aktualisierung wird dem Kommunikations-Thread des -Objekts hinzugefügt.
