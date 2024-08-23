---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Zugriff auf Anforderungswarteschlangen gewähren
description: Wenn Sie Zugriff auf eine Anforderungswarteschlange gewähren, bestimmen Sie, wer in Ihrem Unternehmen die Anforderungswarteschlange im Anforderungsbereich von Adobe Workfront anzeigen kann.
author: Lisa
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Zugriff auf Anforderungswarteschlangen gewähren

Wenn Sie Zugriff auf eine Anforderungswarteschlange gewähren, bestimmen Sie, wer in Ihrem Unternehmen die Anforderungswarteschlange im Anforderungsbereich von Adobe Workfront anzeigen kann.

Sie können verschiedenen Benutzern Zugriff auf eine Anforderungswarteschlange gewähren, je nachdem, ob sie zum Projektteam, zur Projektgruppe oder zum Projektunternehmen gehören. Sie können auch allen Benutzern des Systems Zugriff auf eine Anforderungswarteschlange gewähren. 

Dies ist nützlich bei Organisationen, die externe Interessengruppen in Workfront einladen und den Zugriff von Benutzern auf bestimmte Bereiche beschränken möchten - in diesem Fall ist eine Anforderungswarteschlange nur für die mit dem Unternehmen oder der Projektgruppe verknüpften Benutzer verfügbar, die die Sichtbarkeit für externe Projektbeteiligte einschränkt. Wenn Sie allen Benutzern Zugriff gewähren, wird die Anfrage sowohl für interne als auch externe Interessengruppen sichtbar.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neue Lizenz: Standard </p>
   Oder
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Berechtigungen für das Projekt verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor die Anforderungswarteschlange für Benutzer im Bereich Anforderungen verfügbar ist, müssen Sie ein Projekt mit den folgenden Einstellungen erstellen:

* Legen Sie ihn als Anforderungswarteschlange fest. Weitere Informationen zum Erstellen einer Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Aktualisieren Sie den Status des Projekts auf Aktuell .

## Zugriff auf eine Anforderungswarteschlange gewähren

1. Wechseln Sie zu dem Projekt, in dem Sie Zugriff auf die Anforderungswarteschlangen gewähren möchten.

   >[!NOTE]
   >
   >Im Bereich Anforderungen werden nur Projekte mit dem Status Aktuell angezeigt.

1. Klicken Sie im linken Bereich auf **Queue Details** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Warteschlangendetails** klicken.
1. Wählen Sie **Publish als Hilfedokumentwarteschlange** aus, um das Projekt als Anforderungswarteschlange zu kennzeichnen.
1. Wählen Sie aus den folgenden Optionen aus:

   * **Jeder**: Jeder Benutzer kann Anforderungen anzeigen und zur Anforderungswarteschlange hinzufügen.
   * **Personen mit Ansichtszugriff auf dieses Projekt**: Benutzer mit Ansichtsberechtigungen für das Projekt können Anforderungen anzeigen und zur Anforderungswarteschlange hinzufügen. 
   * **Personen in der Firma dieses Projekts**: Benutzer, die mit der Firma des Projekts verknüpft sind, können Anforderungen anzeigen und hinzufügen. Das mit dem Projekt verknüpfte Unternehmen wird in Klammern neben dieser Option aufgeführt. 
   * **Personen in der Gruppe dieses Projekts**:Benutzer, die der Gruppe des Projekts zugeordnet sind, können Anforderungen anzeigen und hinzufügen. Die mit dem Projekt verknüpfte Gruppe wird in Klammern neben dieser Option aufgeführt.

     Gruppenwarteschlangen sind nützlich, wenn mehrere Abteilungen ein Workfront-Konto gemeinsam nutzen, um eindeutige Organisationsziele zu erreichen. Jede Abteilung kann über eigene Warteschlangen verfügen, die Mitglieder anderer Gruppen nicht sehen können sollten.

     Weitere Informationen dazu, wer über Berechtigungen für ein Projekt verfügt, finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Gruppen und Unternehmen können beim Bearbeiten des Projekts mit dem Projekt verknüpft werden. Weitere Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie auf **Speichern**.
