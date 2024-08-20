---
navigation-topic: notifications
title: Anpassen von E-Mail-Objekten für Ereignisbenachrichtigungen
description: Sie können die Betreffzeile der E-Mails anpassen, die durch Ereignisbenachrichtigungen ausgelöst werden.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 4%

---

# Anpassen von E-Mail-Betreffs für Ereignisbenachrichtigungen

Sie können die Betreffzeile der E-Mails anpassen, die durch Ereignisbenachrichtigungen ausgelöst werden:

Das Ändern der Betreffzeilen wirkt sich unabhängig von der Zugriffsebene des Empfängers auf alle Benutzer im System aus. Benutzer sehen alle Objekte und Felder, die im E-Mail-Betreff enthalten sind.

Einige Ereignisbenachrichtigungen haben mehrere Betreffzeilen, d. h. diese Ereignisbenachrichtigungen können je nach Funktionalität mehrere E-Mail-Betreffs aufweisen.

>[!IMPORTANT]
>
>Seien Sie beim Löschen von Standardfeldern vorsichtig, wenn die Betreffzeilen auf mehrere Objekte verweisen. Im Folgenden finden Sie eine Liste der Ereignisbenachrichtigungen, die solche Betreffzeilen enthalten:
>
>* Jemand bezieht mich in eine gezielte Aktualisierung ein
>* Jemand bezieht mein Team in eine gezielte Aktualisierung ein
>* Kommentar zum Arbeitselement an Thread-Teilnehmer
>* Kommentar zum Arbeitselement an Zugewiesene(n) des Arbeitselements
>

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
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Planung oder höher mit Administratorzugriff auf Erinnerungsbenachrichtigungen</p> <p>Informationen zum Gewähren eines administrativen Zugriffs für einen Planbenutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von Benutzern administrativen Zugriff auf bestimmte Bereiche</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## E-Mail-Betreffzeilen für Ereignisbenachrichtigungen anpassen {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **E-Mail** > **Benachrichtigungen**.

1. Klicken Sie auf die Registerkarte **Ereignisbenachrichtigungen**.
1. Klicken Sie auf den Namen der Ereignisbenachrichtigung, die Sie anpassen möchten, um das Feld **Ereignisbenachrichtigung** zu öffnen.
1. Ändern Sie im Feld **E-Mail-Betreffzeile** den Text und die Felder, einschließlich der benutzerdefinierten Felder, im E-Mail-Betreff.

   Die Namen der hinzugefügten Felder müssen mit der Binnenmajuskel-Schreibweise-Syntax unserer Datenbankstruktur übereinstimmen. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Klicken Sie auf **Aktualisieren** , um die neuen Betreffzeilen für Ihre E-Mails zu speichern.

## E-Mail-Betreffzeilen für E-Mails mit mehreren Objekten anpassen

Einige Ereignisbenachrichtigungen haben mehrere Betreffzeilen, je nachdem, welche Objekte sie Trigger haben.

Zum Beispiel hat &quot;Jemand hat mich bei einer direkten Aktualisierung mit eingeschlossen&quot;zwei Betreffzeilen: erstens für Aufgaben, Probleme, Vorlagenaufgaben und Dokumente (auch als &quot;referenceObject&quot;bezeichnet) und zweitens für Objekte, mit denen Benutzer Kommentare abgeben können, wie z. B. Portfolio, Programm usw. (auch als &quot;topReferenceObject&quot;bezeichnet).

![](assets/Ev-not-mult-subj-lines.png)

Wenn ein Benutzer in eine Konversation über die Aufgabe, das Problem, die Vorlagenaufgabe oder das Dokument einbezogen wird, wird eine E-Mail mit der ersten Betreffzeile generiert. Die Betreffzeile enthält &quot;referenceObject:name&quot;, das System definiert das Objekt und zeigt den entsprechenden Namen im Betrefffeld an. Die Betreffzeile der E-Mail würde in etwa so aussehen: &quot;Kommentar zu Aufgabe 123 zu Projekt-ABC.&quot;

Wenn eine E-Mail zum zweiten Betreff hinzugefügt wird, wird eine E-Mail generiert. Hier enthält die Betreffzeile &quot;topReferenceObject:name&quot;und Workfront gibt erneut an, auf welches Objekt verwiesen wurde, und gibt diesen Objektnamen anstelle von &quot;topReferenceObject:name&quot;im Betreff zurück. Die Betreffzeile der E-Mail würde in etwa so aussehen: &quot;Kommentar zu Projekt ABC&quot;.

Informationen zum Bearbeiten der E-Mail-Betreffzeilen und zum Hinzufügen zusätzlicher Felder zu beiden Betreffzeilen finden Sie unter [Anpassen der E-Mail-Betreffzeilen für Ereignisbenachrichtigungen](#customize-email-subject-lines-for-event-notifications) in diesem Artikel.

## E-Mail-Betreffzeilen für E-Mails mit mehreren Aktionen anpassen

Einige Ereignisbenachrichtigungen enthalten auch mehrere E-Mail-Betreffs, um die verschiedenen Aktionen zu skizzieren, die an den Objekten durchgeführt werden.

Wenn Sie beispielsweise ein Dokument anfordern, das einem Problem hinzugefügt werden soll, können zwei verschiedene E-Mails Trigger werden: eine für den Zeitpunkt, zu dem das Dokument hinzugefügt wird, und eine für den Zeitpunkt, zu dem das Dokument bearbeitet wird.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Informationen zum Bearbeiten der E-Mail-Betreffzeilen und zum Hinzufügen zusätzlicher Felder zu beiden Betreffzeilen finden Sie unter [Anpassen der E-Mail-Betreffzeilen für Ereignisbenachrichtigungen](#customize-email-subject-lines-for-event-notifications) in diesem Artikel.
