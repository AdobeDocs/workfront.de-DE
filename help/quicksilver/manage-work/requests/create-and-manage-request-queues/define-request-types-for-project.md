---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Definieren von Anforderungstypen für ein Projekt
description: Sie können die Art der in Adobe Workfront protokollierten Probleme oder Anforderungen nach Anfragetypen organisieren.
author: Lisa
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 2%

---

# Anforderungstypen für ein Projekt definieren

Sie können die Art der in Adobe Workfront protokollierten Probleme oder Anforderungen nach Anfragetypen organisieren.

Diese Organisation ist nützlich, um Berichterstellungsgründe zu berücksichtigen und Benutzern zu helfen, zu verstehen, welche Art von unerwarteter Arbeit während der Lebensdauer eines Projekts auftreten kann.

## Zugriffsanforderungen

+++

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Neu: Standard</p>
    <p>oder</p>
    <p>Aktuell: Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Projekt verwenden oder erstellen

  Weitere Informationen zum Erstellen von Projekten finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

## Überlegungen zu Anforderungstypen

* Sie können den Typ der Probleme oder Anforderungen angeben, die bei einem Projekt protokolliert werden können, wenn Sie den Bereich **Warteschlangendetails** für das Projekt konfigurieren.
* Sie müssen das Projekt nicht als Anforderungswarteschlange aktivieren, um Anforderungstypen für ein Projekt definieren zu können. Alle für ein Projekt protokollierten Probleme können mit einem anderen Anforderungstyp gekennzeichnet werden.
* Wenn Sie Ihrem Projekt Warteschlangenthemen hinzufügen, müssen Sie Anfragetypen für jedes Warteschlangenthema definieren, damit sie beim Hinzufügen eines neuen Problems oder einer neuen Anforderung angezeigt werden. Weitere Informationen finden Sie unter [Themen für Warteschlangen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Problem- oder Anfragetypen für ein Projekt definieren

{{step1-to-projects}}

1. Klicken Sie auf den Namen des Projekts, um es zu öffnen.
1. Klicken Sie im linken Bereich auf **Warteschlangendetails**.
1. Wählen Sie im Abschnitt **Eigenschaften der Warteschlange** die **Anforderungstypen** aus, die Sie für das Projekt benötigen.

   >[!NOTE]
   >
   >Sie müssen mindestens einen Anfragetyp ausgewählt haben. Sie können mehrere Anfragetypen auswählen.

   Wählen Sie aus den folgenden Typen aus:

   * Fehlerbericht
   * Änderungsanforderung
   * Problem
   * Anfrage

   >[!TIP]
   >
   >Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. Weitere Informationen finden Sie unter [Konfigurieren von Anfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicken Sie auf **Speichern**.

   Die von Ihnen angegebenen Anforderungstypen können ausgewählt werden, wenn Sie ein neues Problem in einer Aufgabe oder einem Projekt eingeben oder wenn Sie eine neue Anforderung an das Projekt senden, wenn das Projekt als Anforderungswarteschlange aktiviert ist.
