---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Anforderungstypen für ein Projekt definieren
description: Sie können die Art der Probleme oder Anfragen, die in Adobe Workfront protokolliert werden, nach Anfragetypen organisieren.
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 16%

---

# Definieren von Anfragetypen für ein Projekt

<!-- Audited: 6/2025 -->

Sie können die Art der Probleme oder Anfragen, die in Adobe Workfront protokolliert werden, nach Anfragetypen organisieren. Dies ist aus Gründen der Berichterstellung nützlich und hilft Benutzenden zu verstehen, welche Art von unerwarteter Arbeit während der Lebensdauer eines Projekts auftreten kann.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
    <p>Abo</p></td>  
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Ein Projekt haben oder erstellen.

  Informationen zum Erstellen von Projekten finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

## Überlegungen zu Anfragetypen

* Sie können die Art der Probleme oder Anfragen, die für ein Projekt protokolliert werden können, angeben, wenn Sie den Bereich Warteschlangendetails für das Projekt konfigurieren.
* Sie müssen das Projekt nicht aktivieren, um eine Anfrage-Warteschlange zu sein, um Anfragetypen für ein Projekt definieren zu können. Alle für ein Projekt protokollierten Probleme können mit einem anderen Anfragetyp gekennzeichnet werden.
* Wenn Sie Ihrem Projekt Warteschlangenthemen hinzufügen, müssen Sie für jedes Warteschlangenthema Anfragetypen definieren, um diese beim Hinzufügen eines neuen Problems oder einer neuen Anfrage anzuzeigen. Weitere Informationen finden Sie unter [Erstellen von Warteschlangenthemen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

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
