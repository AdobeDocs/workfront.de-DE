---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: Konfigurieren von Ereignisabonnements in Workfront
description: Als Adobe Workfront-Administrator können Sie Ereignisabonnements über den Bereich „Setup“ erstellen, anzeigen und löschen, um Workfront-Ereignisse an einen externen Endpunkt zu senden.
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 9%
---

# Konfigurieren von Ereignisabonnements in Workfront

{{highlighted-preview-article-level}}

Als Adobe Workfront-Administrator können Sie Ereignisabonnements über den Bereich „Setup“ erstellen, anzeigen und löschen. Ereignisabonnements senden Workfront-Ereignisinformationen an einen externen Endpunkt, wenn angegebene Ereignisse eintreten.

Sie können Ereignisabonnements in Workfront erstellen und löschen, ein bestehendes Abonnement jedoch nicht bearbeiten. Wenn Sie ein Abonnement ändern müssen, löschen Sie es und erstellen Sie ein neues.

Weitere Informationen zu Ereignisabonnements finden Sie in den Artikeln unter [Ereignisabonnements](/help/quicksilver/wf-api/api/event-subscriptions.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront-Paket</td>
   <td>Beliebig</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td>
    <p>Standard</p>
    <p>Abo</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Konfigurationen der Zugriffsebene</td>
   <td>Sie müssen ein Workfront-Administrator sein.</td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Erstellen eines Ereignisabonnements

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **System** und dann auf **Ereignisabonnements**.
1. Klicken Sie **Neues Ereignisabonnement**.
1. Wählen Sie im **Objekt** das Workfront-Objekt aus, das Sie überwachen möchten.
1. Wählen **im Feld Ereignistyp** aus, ob das Ereignisabonnement beim Erstellen, Aktualisieren, Löschen oder Freigeben des Objekts an den Trigger weitergeleitet werden soll.
1. Geben Sie im Feld **Webhook** URL den Endpunkt ein, der die Ereignis-Payload erhalten soll.
1. Geben Sie im Feld **Authentifizierungs** Token) das Token ein, mit dem die Anfrage an Ihren Endpunkt authentifiziert wird.
1. Wenn Sie möchten, dass Workfront die Payload vor dem Versand kodiert, aktivieren Sie die Option zum Senden der Payload als Base64.
1. Fügen Sie bei Bedarf einen oder mehrere Filter hinzu, um zu begrenzen, durch welche Trigger das Abonnement beeinträchtigt wird. Die verfügbaren Filter basieren auf dem ausgewählten Objekt.
1. Klicken Sie auf **Erstellen**.

Informationen zu den Endpunktanforderungen finden Sie [Versandanforderungen für Ereignisabonnements](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md).

## Ereignisabonnements anzeigen

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **System** und dann auf **Ereignisabonnements**.

Auf der Seite „Ereignisabonnements“ können Sie die für Ihre Umgebung konfigurierten Abonnements überprüfen. Sie können auch sehen, wie viele Abonnements Ihre Organisation insgesamt hat und wie viele davon aktiv, deaktiviert oder eingefroren sind.

* **Deaktivierte Abonnements**: Diese Abonnements wurden aufgrund wiederholter Versandfehler automatisch deaktiviert.
* **Eingefrorene Abonnements**: Diese Abonnements sind aufgrund von Versandproblemen vorübergehend eingefroren.

## Löschen eines Ereignisabonnements

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **System** und dann auf **Ereignisabonnements**.
1. Wählen Sie das Ereignisabonnement aus, das Sie entfernen möchten.
1. Klicken Sie auf **Löschen**.
