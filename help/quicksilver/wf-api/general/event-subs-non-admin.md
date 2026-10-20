---
content-type: api
navigation-topic: general-api
title: Verwalten von Ereignisabonnements für Benutzer ohne Administratorrechte
description: Wenn Ihr Workfront-Zugriff dies zulässt, können Sie Ereignisabonnements erstellen, anzeigen und löschen, die innerhalb des durch Ihre Berechtigungen und Systemkonfiguration zulässigen Bereichs liegen.
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%
---

# Verwalten von Ereignisabonnements für Benutzer ohne Administratorrechte

Wenn Ihr Workfront-Zugriff dies zulässt, können Sie Ereignisabonnements im Bereich „Setup“ erstellen, anzeigen und löschen. Ihr Zugriff ist jedoch auf die Abonnements und Aktionen beschränkt, die für Ihre Rolle und durch die Systemkonfiguration Ihres Unternehmens autorisiert sind.

Diese Funktion steht nicht allen Benutzenden auf dieselbe Weise zur Verfügung wie Workfront-Admins. Benutzende mit dem erforderlichen Zugriff können Ereignisabonnements nur im Rahmen der ihnen gewährten Berechtigungen verwalten.

Beispielsweise können Sie mit Ihren Berechtigungen nur bestimmte Objekttypen, Ereignistypen oder Abonnements für einen definierten Arbeitssatz verwalten. Sie können keine Ereignisabonnements verwalten, die nicht in den von Ihrem Zugriff und Ihrer Konfiguration zulässigen Bereich fallen.

Informationen zum vom Administrator verwalteten Setup finden Sie unter [Konfigurieren von Ereignisabonnements in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md).

Informationen zur Ereignisabonnement-API finden Sie unter [Ereignisabonnement-API](/help/quicksilver/wf-api/general/event-subs-api.md).

>[!NOTE]
>
>Benutzer können Ereignisabonnements nur im Rahmen ihrer Berechtigungen und der Systemkonfiguration des Unternehmens verwalten. Der Zugriff entspricht nicht automatisch dem Administratorzugriff.

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
   <td>
    <p>Sie müssen über den entsprechenden Zugriff verfügen, um Ereignisabonnements verwalten zu können.</p>
    <p>Ihr Zugriff ist auf die Abonnements und Aktionen beschränkt, die aufgrund Ihrer Berechtigungen und der Systemkonfiguration Ihres Unternehmens zulässig sind.</p>
   </td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Arbeiten mit Ereignisabonnements

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **System** und dann auf **Ereignisabonnements**.
1. Überprüfen Sie die verfügbaren Abonnements.
1. Nur Abonnements erstellen, anzeigen oder löschen, die in Ihren autorisierten Bereich fallen.

Wenn Sie die erwarteten Optionen nicht sehen oder wenn Sie kein Abonnement erstellen oder verwalten können, wenden Sie sich an Ihren Workfront-Administrator, um zu bestätigen, ob Ihr Zugriff durch Rolle, Berechtigungen oder Systemkonfiguration beschränkt ist.

## Verwandte Artikel

* [Konfigurieren von Ereignisabonnements in Workfront](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [Ereignisabonnement-API](/help/quicksilver/wf-api/general/event-subs-api.md)
