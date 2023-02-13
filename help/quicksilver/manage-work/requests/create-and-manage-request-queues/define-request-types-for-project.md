---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Anforderungstypen für ein Projekt definieren
description: Sie können die Art der in Adobe Workfront protokollierten Probleme oder Anforderungen nach Anfragetypen organisieren.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Anforderungstypen für ein Projekt definieren

Sie können die Art der in Adobe Workfront protokollierten Probleme oder Anforderungen nach Anfragetypen organisieren.

Diese Organisation ist nützlich, um Berichterstellungsgründe zu berücksichtigen und Benutzern zu helfen, zu verstehen, welche Art von unerwarteter Arbeit während der Lebensdauer eines Projekts auftreten kann.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a>*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront-Lizenz</a>*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Projekt verwenden oder erstellen

   Weitere Informationen zum Erstellen von Projekten finden Sie unter [Projekt erstellen](../../../manage-work/projects/create-projects/create-project.md).

## Überlegungen zu Anforderungstypen

* Sie können den Typ der Probleme oder Anforderungen angeben, die bei der Konfiguration der **Warteschlangendetails** Bereich für das Projekt.
* Sie müssen das Projekt nicht als Anforderungswarteschlange aktivieren, um Anforderungstypen für ein Projekt definieren zu können. Alle für ein Projekt protokollierten Probleme können mit einem anderen Anforderungstyp gekennzeichnet werden.
* Wenn Sie Ihrem Projekt Warteschlangenthemen hinzufügen, müssen Sie Anfragetypen für jedes Warteschlangenthema definieren, damit sie beim Hinzufügen eines neuen Problems oder einer neuen Anforderung angezeigt werden. Weitere Informationen finden Sie unter [Erstellen von Warteschlangenthemen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Problem- oder Anfragetypen für ein Projekt definieren

1. Klicken **Projekte** im Hauptmenü. ![](assets/main-menu-icon.png)

1. Klicken Sie auf den Namen des Projekts, um es zu öffnen.
1. Klicken Sie im linken Bereich auf **Warteschlangendetails**.
1. Im **Eigenschaften der Warteschlange** auswählen, wählen Sie die **Anfragetypen** Sie möchten für das Projekt.

   >[!NOTE]
   >
   >Sie müssen mindestens einen Anfragetyp ausgewählt haben. Sie können mehrere Anfragetypen auswählen.

   Wählen Sie aus den folgenden Typen aus:

   * Bug-Bericht
   * Änderungsanforderung
   * Anfrage
   * Anfrage

   >[!TIP]
   >
   >Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. Weitere Informationen finden Sie unter [Anfragetypen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicken Sie auf **Speichern**.

   Die von Ihnen angegebenen Anforderungstypen können ausgewählt werden, wenn Sie ein neues Problem in einer Aufgabe oder einem Projekt eingeben oder wenn Sie eine neue Anforderung an das Projekt senden, wenn das Projekt als Anforderungswarteschlange aktiviert ist.
