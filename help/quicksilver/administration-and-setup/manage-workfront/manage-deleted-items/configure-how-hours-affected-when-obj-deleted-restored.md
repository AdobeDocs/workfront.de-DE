---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Konfigurieren der Auswirkungen auf Stunden, wenn ein Objekt gelöscht und wiederhergestellt wird
description: Sie können konfigurieren, was mit Stunden passiert, wenn jemand ein Projekt, eine Aufgabe oder ein Problem löscht, für das bzw. das die Stunden protokolliert werden. Die von Ihnen gewählte Option bestimmt auch, was mit den Stunden passiert, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter Wiederherstellen gelöschter Elemente.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Auswirkungen auf Stunden konfigurieren, wenn ein Objekt gelöscht und wiederhergestellt wird

Sie können konfigurieren, was mit Stunden passiert, wenn jemand ein Projekt, eine Aufgabe oder ein Problem löscht, für das bzw. das die Stunden protokolliert werden. Die von Ihnen gewählte Option bestimmt auch, was mit den Stunden passiert, wenn das Projekt, die Aufgabe oder das Problem zu einem späteren Zeitpunkt wiederhergestellt wird. (Weitere Informationen zum Wiederherstellen von Elementen in Workfront finden Sie unter [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
