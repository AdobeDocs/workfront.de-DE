---
navigation-topic: notifications
title: E-Mail-Betreffe für Ereignisbenachrichtigungen anpassen
description: Sie können die Betreffzeile der E-Mails anpassen, die von Ereignisbenachrichtigungen ausgelöst werden.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2f39a091-aec2-4013-a835-0ab1c8789dc3
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 4%

---

# E-Mail-Betreffe für Ereignisbenachrichtigungen anpassen

Sie können die Betreffzeile der E-Mails anpassen, die von Ereignisbenachrichtigungen ausgelöst werden:

Das Ändern der Betreffzeilen wirkt sich auf alle Benutzenden im System aus, unabhängig von der Zugriffsebene des Empfängers. Benutzer sehen alle Objekte und Felder, die im E-Mail-Betreff enthalten sind.

Einige Ereignisbenachrichtigungen haben mehrere Betreffzeilen, d. h. diese Ereignisbenachrichtigungen können je nach Funktion mehrere E-Mail-Betreffe haben.

>[!IMPORTANT]
>
>Gehen Sie beim Löschen von Standardfeldern vorsichtig vor, wenn die Betreffzeilen auf mehrere Objekte verweisen. Im Folgenden finden Sie die Liste der Ereignisbenachrichtigungen, die solche Betreffzeilen enthalten:
>
>* Jemand bezieht mich in eine gezielte Aktualisierung ein
>* Jemand bezieht mein Team in eine gezielte Aktualisierung ein
>* Kommentar zum Arbeitselement an Thread-Teilnehmer
>* Kommentar zum Arbeitselement an Zugewiesene(n) des Arbeitselements
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Planer oder höher mit administrativem Zugriff auf Erinnerungsnachrichten</p> <p>Informationen dazu, wie Sie einem Planbenutzer administrativen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## E-Mail-Betreffzeilen für Ereignisbenachrichtigungen anpassen {#customize-email-subject-lines-for-event-notifications}

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **E-Mail** > **Benachrichtigungen**.

1. Klicken Sie auf **Registerkarte** Ereignisbenachrichtigungen“.
1. Klicken Sie auf den Namen der Ereignisbenachrichtigung, die Sie anpassen möchten, um das Feld **Ereignisbenachrichtigung** zu öffnen.
1. Ändern Sie im Feld **E-Mail** Betreffzeile) den Text und die Felder, einschließlich der benutzerdefinierten Felder, im E-Mail-Betreff.

   Die Namen der hinzugefügten Felder müssen mit der Binnenmajuskeln-Syntax unserer Datenbankstruktur übereinstimmen. <!--For more information about how our objects and their fields are named in the Workfront database, see the [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

1. Klicken Sie **Aktualisieren**, um die neuen Betreffzeilen für Ihre E-Mails zu speichern.

## Anpassen der Betreffzeilen von E-Mails mit mehreren Objekten

Einige Ereignisbenachrichtigungen haben mehrere Betreffzeilen, je nachdem, welche Objekte sie Trigger haben.

Beispiel: „Jemand nimmt mich in eine direkte Aktualisierung auf“ hat zwei verschiedene Betreffzeilen: die erste ist für Aufgaben, Probleme, Vorlagenaufgaben und Dokumente (auch als „referenceObject“ bezeichnet) und die zweite für Objekte, die es Benutzern ermöglichen, Kommentare zu machen, wie Portfolio, Programm usw. (auch als „topReferenceObject“ bezeichnet).

![](assets/Ev-not-mult-subj-lines.png)

Wenn ein(e) Benutzende(r) in eine Konversation über die Aufgabe, das Problem, die Vorlagenaufgabe oder das Dokument einbezogen wird, wird eine E-Mail mit der ersten Betreffzeile generiert. Die Betreffzeile enthält „referenceObject:name“, und das System definiert das Objekt und zeigt den entsprechenden Namen im Feld Betreff an. Die Betreffzeile der E-Mail sieht in etwa so aus: „Kommentar zu Aufgabe 123 im Projekt-ABC“.

Wird eine Konversation zu einem Projekt hinzugefügt, wird eine E-Mail mit dem zweiten Betreff generiert. Hier enthält die Betreffzeile „topReferenceObject:name“, und Workfront identifiziert erneut, auf welches Objekt verwiesen wurde, und gibt diesen Objektnamen anstelle von „topReferenceObject:name“ im Betreff zurück. Die Betreffzeile der E-Mail sieht in etwa so aus: „Kommentar zu Projekt-ABC“.

Informationen zum Bearbeiten der E-Mail-Betreffzeilen und Hinzufügen zusätzlicher Felder zu den Betreffzeilen finden Sie unter [Anpassen der E-Mail-Betreffzeilen für ](#customize-email-subject-lines-for-event-notifications)) in diesem Artikel.

## E-Mail-Betreffzeilen für E-Mails mit mehreren Aktionen anpassen

Einige Ereignisbenachrichtigungen haben auch mehrere E-Mail-Betreffe, um die verschiedenen Aktionen zu beschreiben, die mit den Objekten durchgeführt werden.

Die Anforderung, ein Dokument zu einem Problem hinzuzufügen, ist beispielsweise ein Ereignis, das zwei verschiedene E-Mails in Trigger setzen kann: eine für den Zeitpunkt, zu dem das Dokument hinzugefügt wird, und eine für den Zeitpunkt, zu dem das Dokument bearbeitet wird.

![](assets/ev-not-mult-subj-lines-diff-actions.png)

Informationen zum Bearbeiten der E-Mail-Betreffzeilen und Hinzufügen zusätzlicher Felder zu den Betreffzeilen finden Sie unter [Anpassen der E-Mail-Betreffzeilen für ](#customize-email-subject-lines-for-event-notifications)) in diesem Artikel.
