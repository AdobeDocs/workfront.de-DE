---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Alte Portfolios in Adobe Cloud-Speicher konvertieren
description: Konvertieren Sie vorhandene alte Workfront-Speicherportfolios in Adobe-Cloud-Speicher aus dem Bereich „Speichereinstellungen“ in den Systemeinstellungen.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 9%

---

# Alte Portfolios in Adobe Cloud-Speicher konvertieren

Als Workfront-Administrator können Sie bestehende Workfront-Speicherportfolios über den Bereich „Speichereinstellungen“ in den Systemeinstellungen in Adobe-Cloud-Speicher umwandeln. Nachdem ein Portfolio konvertiert wurde, verhält es sich wie jedes andere Adobe-Cloud-Speicherportfolio.

Weitere Informationen dazu, wie sich konvertierte Portfolios verhalten und wie sich ihre untergeordneten Objekte auswirken, finden Sie unter [Objektportabilität](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) in [Wechseln zu Workfront im Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebiges Workflow-Paket</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Vor der Konvertierung eines Portfolios

Bevor Sie ein Legacy-Speicherportfolio von Workfront konvertieren, sollten Sie Folgendes beachten:

* Die Konversion betrifft nur das Portfolio selbst. Untergeordnete Projekte und Programme, die alten Workfront-Speicher verwenden, bleiben auf dem alten Speicher.

  >[!NOTE]
  >
  >Ein untergeordnetes Legacy-Programm kann nur dann automatisch in den Adobe-Cloud-Speicher konvertiert werden, wenn ihm manuell ein Adobe-Cloud-Speicherprojekt hinzugefügt wird.
* Dokumente und Dokumentordner im Portfolio verbleiben nach der Konvertierung im alten Workfront-Speicher.
* Nach der Konversion können Sie keine Legacy-Workfront-Speicherprojekte zum Portfolio hinzufügen.

## Alte Portfolios in Adobe Cloud-Speicher konvertieren

So konvertieren Sie ein oder mehrere alte Workfront-Speicherportfolios in Adobe Cloud-Speicher:

{{step-1-to-setup}}

1. Wählen Sie **linken Navigationsbereich** System“ und dann **Voreinstellungen** aus.

1. Scrollen Sie nach unten zum Abschnitt **Speichereinstellungen**.

1. Wählen **im Feld Portfolios auswählen, die in Adobe Cloud-Speicher** werden sollen ein oder mehrere Legacy-Workfront-Speicherportfolios aus.

1. Klicken Sie auf **Speichern**.

   Es wird eine Bestätigungsmeldung angezeigt, die beschreibt, was passiert, wenn ein Portfolio konvertiert wird:

   * Ältere Workfront-Speicherprojekte können nicht mehr in das Portfolio verschoben werden.
   * Alle neuen Projekte, die im Portfolio erstellt werden, verwenden den Adobe Cloud-Speicher.
   * Frame.io ist der Viewer für Dokumente in den Adobe Cloud-Speicherprojekten des Portfolios.
   * Untergeordnete Projekte, die älteren Workfront-Speicher verwenden, bleiben auf dem alten Speicher.
   * Untergeordnete Programme verbleiben im alten Speicher.

1. Klicken Sie **Bestätigung** Konvertieren).

   Die ausgewählten Portfolios werden in Adobe Cloud-Speicher konvertiert.
