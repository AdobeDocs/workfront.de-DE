---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Anforderungstypen für ein Projekt definieren
description: Sie können die Art der Probleme oder Anfragen, die in Adobe Workfront protokolliert werden, nach Anfragetypen organisieren.
author: Becky
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 3%

---

# Anforderungstypen für ein Projekt definieren

<!-- Audited: 6/2025 -->

Sie können die Art der Probleme oder Anfragen, die in Adobe Workfront protokolliert werden, nach Anfragetypen organisieren. Dies ist aus Gründen der Berichterstellung nützlich und hilft Benutzenden zu verstehen, welche Art von unerwarteter Arbeit während der Lebensdauer eines Projekts auftreten kann.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Ein Projekt haben oder erstellen.

  Informationen zum Erstellen von Projekten finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

## Überlegungen zu Anfragetypen

* Sie können die Art der Probleme oder Anfragen, die für ein Projekt protokolliert werden können, angeben, wenn Sie den Bereich Warteschlangendetails für das Projekt konfigurieren.
* Sie müssen das Projekt nicht aktivieren, um eine Anfrage-Warteschlange zu sein, um Anfragetypen für ein Projekt definieren zu können. Alle für ein Projekt protokollierten Probleme können mit einem anderen Anfragetyp gekennzeichnet werden.
* Wenn Sie Ihrem Projekt Warteschlangenthemen hinzufügen, müssen Sie für jedes Warteschlangenthema Anfragetypen definieren, um diese beim Hinzufügen eines neuen Problems oder einer neuen Anfrage anzuzeigen. Weitere Informationen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## Anfrage- oder Anfragetypen für ein Projekt definieren

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie im linken Bedienfeld auf **Warteschlangendetails**.
1. Wählen Sie **Abschnitt** die **Anfragetypen“ aus** die Sie für das Projekt verwenden möchten:
   * Fehlerbericht
   * Änderungsanforderung
   * Problem
   * Anfrage

   >[!NOTE]
   >
   >* Mindestens ein Anfragetyp muss ausgewählt sein. Sie können mehrere Typen auswählen.
   >* Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. Weitere Informationen finden Sie [Konfigurieren von Anfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Klicken Sie auf **Speichern**. Die angegebenen Anfragetypen stehen zur Auswahl, wenn Sie eine neue Anfrage für eine Aufgabe oder ein Projekt eingeben oder wenn Sie eine neue Anfrage an das Projekt senden (wenn das Projekt als Anfragewarteschlange aktiviert ist).
