---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Zugriff auf Anfrage-Warteschlangen gewähren
description: Wenn Sie Zugriff auf eine Anfrage-Warteschlange gewähren, legen Sie fest, wer in Ihrem Unternehmen die Anfrage-Warteschlange im Bereich Anfragen von Adobe Workfront anzeigen kann.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Zugriff auf Anfrage-Warteschlangen gewähren

Wenn Sie Zugriff auf eine Anfrage-Warteschlange gewähren, legen Sie fest, wer in Ihrem Unternehmen die Anfrage-Warteschlange im Bereich Anfragen von Adobe Workfront anzeigen kann.

Sie können verschiedenen Benutzern Zugriff auf eine Anfrage-Warteschlange gewähren, je nachdem, ob sie Teil des Projektteams, der Projektgruppe oder der Projektfirma sind. Sie können auch allen Personen im System Zugriff auf eine Anfrage-Warteschlange gewähren.

Dies ist besonders nützlich für Unternehmen, die externe Stakeholder in Workfront einladen und den Zugriff von Benutzenden auf bestimmte Bereiche beschränken möchten. In diesem Fall schränkt eine Anfrage-Warteschlange, die nur für die mit dem Unternehmen oder der Gruppe des Projekts verbundenen Benutzenden geöffnet ist, die Sichtbarkeit auf externe Stakeholder ein. Wenn Sie jedem Zugriff gewähren, wird die Anfrage sowohl für interne als auch externe Stakeholder sichtbar.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neue Lizenz: Standard </p>
   Oder
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor die Anfrage-Warteschlange im Bereich Anfragen für Benutzer verfügbar ist, müssen Sie ein Projekt mit den folgenden Einstellungen erstellen:

* Weisen Sie sie als Anfrage-Warteschlange zu. Weitere Informationen zum Erstellen einer Anfrage-Warteschlange finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Status des Projekts auf „Aktuell“ aktualisieren.

## Zugriff auf eine Anfrage-Warteschlange gewähren

1. Wechseln Sie zu dem Projekt, in dem Sie Zugriff auf die Anfrage-Warteschlangen gewähren möchten.

   >[!NOTE]
   >
   >Nur Projekte mit dem Status „Aktuell“ werden im Bereich Anfragen angezeigt.

1. Klicken Sie **linken Bedienfeld** Warteschlangendetails“.
1. Wählen **Als Warteschlange für Hilfeanfragen veröffentlichen**, um das Projekt als Warteschlange für Anfragen festzulegen.
1. Wählen Sie aus den folgenden Optionen aus:

   * **Beliebig**: Jeder Benutzer kann Anfragen anzeigen und zur Anfragewarteschlange hinzufügen.
   * **Benutzer mit Ansichtszugriff auf dieses Projekt**: Benutzer mit Ansichtsberechtigungen für das Projekt können Anfragen anzeigen und zur Anfragewarteschlange hinzufügen.
   * **Personen im Unternehmen dieses Projekts**: Benutzer, die mit dem Unternehmen des Projekts verknüpft sind, können Anfragen anzeigen und hinzufügen. Das mit dem Projekt verknüpfte Unternehmen wird neben dieser Option in Klammern aufgeführt.
   * **Personen in der Gruppe dieses Projekts**: Benutzer, die mit der Gruppe des Projekts verknüpft sind, können Anfragen anzeigen und hinzufügen. Die mit dem Projekt verknüpfte Gruppe wird neben dieser Option in Klammern aufgeführt.

     Gruppen-Warteschlangen sind nützlich, wenn mehrere Abteilungen ein Workfront-Konto gemeinsam nutzen, um individuelle Unternehmensziele zu erreichen. Jede Abteilung kann ihre eigenen Warteschlangen haben, die Mitglieder anderer Gruppen nicht sehen dürfen.

     Informationen dazu, wer über Berechtigungen für ein Projekt verfügt, finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Gruppen und Unternehmen können beim Bearbeiten des Projekts mit dem Projekt verknüpft werden. Weitere Informationen zum Bearbeiten von Projekten finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie auf **Speichern**.
