---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Konfigurieren der Auswirkungen auf Stunden, wenn ein Objekt gelöscht und wiederhergestellt wird
description: Sie können konfigurieren, was mit Stunden passiert, wenn jemand ein Projekt, eine Aufgabe oder ein Problem löscht, für das bzw. das die Stunden protokolliert werden. Die von Ihnen gewählte Option bestimmt auch, was mit den Stunden passiert, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter Wiederherstellen gelöschter Elemente.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
TQID: https://experienceleague.adobe.com/-qjytcjOGAEltoclAl6xXJ-EuvW9hD0CrwMy8T3c-5g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 10%

---

# Auswirkungen auf Stunden konfigurieren, wenn ein Objekt gelöscht und wiederhergestellt wird

Sie können konfigurieren, was mit Stunden passiert, wenn jemand ein Projekt, eine Aufgabe oder ein Problem löscht, für das bzw. das die Stunden protokolliert werden. Die von Ihnen gewählte Option bestimmt auch, was mit den Stunden passiert, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadmin</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren der Verwaltung von Stunden beim Löschen und Wiederherstellen eines Elements

{{step-1-to-setup}}

1. Erweitern Sie **Arbeitszeittabellen und Stunden** und klicken Sie dann auf **Voreinstellungen**.

1. Suchen Sie den Abschnitt **Voreinstellungen für die Löschung von Projekten, Aufgaben oder**.
1. (Bedingt) Um zu konfigurieren, wie Stunden beim Löschen eines Projekts verwaltet werden, wählen Sie eine der folgenden Optionen im Abschnitt **Beim Löschen von Projekten**:

   * Protokollierte Stunden, die Arbeitszeittabellen bereits hinzugefügt wurden, als allgemeine Stunden beibehalten (Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, verbleiben die Stunden in der Arbeitszeittabelle)\
     Diese Option ist standardmäßig ausgewählt.
   * Protokollierte Stunden löschen. (Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, werden protokollierte Stunden im Projekt wiederhergestellt.)

1. (Bedingt) Um zu konfigurieren, wie Stunden beim Löschen einer Aufgabe oder eines Problems verwaltet werden, wählen Sie eine der folgenden Optionen im Abschnitt **Beim Löschen von Aufgaben oder**&quot;:

   * Protokollierte Stunden in das Projekt verschieben, in dem sich die Aufgabe oder Anfrage befindet (Wenn diese Aufgabe oder Anfrage zu einem späteren Zeitpunkt wiederhergestellt wird, verbleiben die Stunden im Projekt)\
     Diese Option ist standardmäßig ausgewählt.
   * Protokollierte Stunden löschen. (Wenn diese Aufgabe oder Anfrage zu einem späteren Zeitpunkt wiederhergestellt wird, werden protokollierte Stunden in der Aufgabe oder Anfrage wiederhergestellt.)

1. Klicken Sie auf **Speichern**.
