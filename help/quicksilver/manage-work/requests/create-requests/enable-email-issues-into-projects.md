---
product-area: requests
navigation-topic: create-requests
title: Benutzer können ein Problem per E-Mail an ein Anforderungswarteschlangenprojekt senden
description: Benutzer können ein Problem per E-Mail an ein Anforderungswarteschlangenprojekt senden
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 9cda6fd41ba7fcb9b9f412a7c2b7ffd39f3fe189
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Benutzer können ein Problem per E-Mail an ein Anforderungswarteschlangenprojekt senden

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Sie können ein Projekt so konfigurieren, dass Benutzer Probleme per E-Mail zum Projekt hinzufügen können. Sie können zulassen, dass Probleme nur dann per E-Mail an ein Projekt gesendet werden, wenn das Projekt als Anforderungswarteschlange festgelegt ist. Weitere Informationen zum Erstellen eines Projekts für eine Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Die folgenden Voraussetzungen sind erforderlich, um ein Projekt zu konfigurieren, damit Benutzer Probleme per E-Mail zum Projekt hinzufügen können.

Diese Bedingungen müssen erfüllt sein, bevor diese Funktion aktiviert wird:

* Benutzer, die Probleme per E-Mail an dieses Konto senden, müssen aktive Benutzer mit einer Lizenz für Workfront sein.
* Benutzer, die Probleme per E-Mail an dieses Konto senden, müssen über die Berechtigung &quot;Problem hinzufügen&quot;für das Projekt verfügen.
* Externe Benutzer können Probleme nicht per E-Mail an eine Anforderungswarteschlange senden, da sie keinen Zugriff zum Erstellen von Problemen haben.
* Es dürfen nur E-Mails von einer E-Mail-Adresse gesendet werden, die mit einem aktiven Workfront-Benutzer verknüpft ist. E-Mails, die von einer mit einem Workfront-Konto nicht verknüpften E-Mail an einen aktiven Workfront-Benutzer weitergeleitet werden, können keine Probleme im Rahmen des Projekts erstellen, da die E-Mail-Adresse des ursprünglichen Absenders mit einem aktiven Workfront-Konto verknüpft werden muss.
* Das Projekt wird als Anforderungswarteschlange eingerichtet.
* Das mit dem Projekt verknüpfte E-Mail-Konto ist nicht mit einem Workfront-Benutzerkonto verknüpft.

## Konfigurieren des Projekts in Workfront

>[!NOTE]
>
>Beachten Sie Folgendes bei der Aktivierung der E-Mail-Warteschlangeneinstellungen:
>
>* Workfront ermöglicht eine eindeutige E-Mail pro Anforderungswarteschlange für alle Cluster. Wenn Sie Ihre Anforderungswarteschlange deaktivieren, behalten Sie die von Ihnen erstellte E-Mail-Adresse bei, solange sie sich noch im Feld E-Mail-Adresse aufnehmen befindet. Wenn Sie die Verwendung der Aufnahme-E-Mail einstellen möchten, müssen Sie sie aus dem Feld E-Mail aufnehmen löschen, damit sie für die zukünftige Verwendung verfügbar ist.
>
>* Wenn die Anforderungswarteschlange über mehrere Warteschlangenthemen oder Themengruppen verfügt, wählt Workfront zufällig das Warteschlangenthema aus, zu dem die E-Mail-Anfragen gesendet werden, wodurch die Verwaltung von E-Mail-Anfragen erschwert wird.
>Es wird empfohlen, dass das Projekt, das Sie für den Empfang von Anfragen über E-Mails einrichten, nicht mehr als ein Warteschlangenthema enthält. Wenn die gesendeten Anfragen für verschiedene Ressourcen oder Projekte bestimmt sind, sollten Sie sie nach dem Senden manuell weiterleiten oder verschieben.

1. Gehen Sie zu dem Projekt, das Sie für den Empfang von Problemen per E-Mail aktivieren möchten.
1. Klicken Sie im linken Bereich auf **Queue Details** . Möglicherweise müssen Sie zuerst auf **Mehr anzeigen** klicken.
1. Wählen Sie im Bereich **Queue Type** die Option **Publish as Help Request Queue**.

1. Scrollen Sie nach unten zum Bereich **E-Mail-Warteschlangeneinstellungen** und wählen Sie dann **Aufnahme der Anforderung per E-Mail aktivieren** aus.

1. Geben Sie den Anfang der E-Mail-Adresse in das Feld **E-Mail-Adresse aufnehmen** ein.

   Sie müssen eine eindeutige E-Mail-Adresse erstellen. Es wird empfohlen, den Firmennamen als Teil Ihrer Anruf-E-Mail-Adresse zu verwenden.

   >[!CAUTION]
   >
   >* Diese E-Mail-Adresse kann nicht aus dem Papierkorb abgerufen werden, wenn das Projekt, das die Anforderungswarteschlange enthält, gelöscht wird.
   >
   >* Da diese E-Mail-Adresse eindeutig sein muss, ist sie in Zukunft möglicherweise nicht verfügbar, wenn sie gelöscht wird.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Optional) Wählen Sie &quot;**Weiterleiten aller Probleme, die nicht per E-Mail gesendet werden&quot;**&quot;, und geben Sie dann im Feld unten eine Weiterleitungs-E-Mail-Adresse ein.

   Diese E-Mail-Adresse erhält Informationen zu E-Mails, die nicht an das Projekt gesendet werden konnten.

1. Klicken Sie auf **Speichern**. Wenn jetzt Benutzer mit einem aktiven Workfront-Konto eine E-Mail an diese E-Mail-Adresse senden, wird im Workfront-Projekt ein Problem erstellt.

   >[!NOTE]
   >
   >Benutzer müssen Zugriff haben, um Probleme im Projekt erstellen zu können, damit sie per E-Mail senden können. Sie können diesen Zugriff im Dialogfeld Freigabe unter Erweiterte Einstellungen gewähren.
   >
   >Externe Benutzer können Probleme nicht per E-Mail an eine Anforderungswarteschlange senden, da sie keinen Zugriff zum Erstellen von Problemen haben.

## Problem in Workfront erhalten

Wenn ein Workfront-Benutzer eine E-Mail an Workfront sendet, geschieht Folgendes:

* Die Betreffzeile der E-Mail wird zum Problemnamen.
* Der Hauptteil der E-Mail wird zur Beschreibung des Problems.
* Wenn der E-Mail Dokumente angehängt sind, werden diese an das Problem in Workfront angehängt.
* Der Benutzer, der die E-Mail sendet, wird zum Primären Ansprechpartner für das neue Problem in Workfront.
* Der Haupttext der E-Mail darf 4.000 Zeichen nicht überschreiten.
* E-Mail-Anhänge dürfen insgesamt 7 MB nicht überschreiten.
