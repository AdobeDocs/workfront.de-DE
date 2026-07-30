---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Verlauf ändern
description: Mit dem Änderungsverlauf können Sie ein Änderungsprotokoll für Workfront-Objekte anzeigen
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: ba1843cf6be446a809f9526608a3ae3bef69c494
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 6%

---

# Änderungsverlauf anzeigen und verwalten

Sie können den Änderungsverlauf, einschließlich der Auditprotokolle, im Bereich „Änderungsverfolgung“ von Setup einsehen.

* **Auditprotokolle** sind Änderungen, die von Benutzern ausgelöst werden.
Weitere Informationen zu Auditprotokollen und zum Bereich Auditprotokolle finden Sie unter [Übersicht über Auditprotokolle](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **Konfiguration** zeigt an, welche Felder für die Liste „Änderungsverlauf“ verfolgt werden.
Die Konfiguration ist derzeit nur als Information verfügbar und kann nicht geändert werden. Die Möglichkeit, zu ändern, welche Felder verfolgt werden, wird in naher Zukunft verfügbar sein.
* **Liste der**: Ermöglicht die Anzeige eines Protokolls mit Änderungen an Workfront-Objekten, einschließlich Attributen wie:

  * Objekt
  * Objekttyp
  * Art der Änderung (Vorgang)
  * Source der Änderung, z. B. bestimmte Benutzende, APIs, Workfront Fusion, KI-LLMs oder das Workfront-System

  <span class="preview">Die Workflow-Aktivität „Einheitliche Überprüfung und Genehmigung“ wird im Änderungsverlauf erfasst, einschließlich Teilnehmern und Entscheidungen.</span>

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Audit-Protokolle anzeigen und verwalten

Informationen zum Anzeigen und Verwalten von Auditprotokollen finden Sie [Anzeigen und Exportieren von Auditprotokollen](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Anzeigen des Konfigurationsbereichs für die Änderungsnachverfolgung

>[!NOTE]
>
>Die Konfiguration ist derzeit nur als Information verfügbar und kann nicht geändert werden. Die Möglichkeit, zu ändern, welche Felder verfolgt werden, wird in naher Zukunft verfügbar sein.

So zeigen Sie die verfolgten Änderungstypen an:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern** ![Verlaufssymbol ändern](assets/change-history-icon.png).
1. Klicken Sie **Konfiguration**.

   Die Felder werden nach Objekttyp gruppiert angezeigt.

1. Um Felder unter einem bestimmten Objekt anzuzeigen, klicken Sie auf den Dropdown-Pfeil neben dem Objekttyp.

## Anzeigen des Änderungsverlaufs

Workfront-Administratoren können den Änderungsverlauf im Bereich „Setup“ anzeigen.

Die Liste „Änderungsverlauf“ ist eine erweiterte Liste und enthält Filter, Spalten, Zeilenhöhe, eine Datumsauswahl und eine Suchleiste.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern** ![Verlaufssymbol ändern](assets/change-history-icon.png).
1. Klicken Sie **Verlaufsliste ändern**.

   Die Liste „Änderungsverlauf“ wird geöffnet.

1. Um die Datumsangaben anzupassen, für die Änderungen angezeigt werden, klicken Sie auf die Datumsauswahl und wählen Sie die neuen Datumsangaben aus.

   Änderungen sind für die letzten 90 Tage verfügbar.

1. Um nach einem bestimmten Begriff zu suchen, klicken Sie auf die Suchleiste und geben Sie den Begriff ein. Die Ergebnisse werden bei der Eingabe in der Liste hervorgehoben.
1. (Optional) Informationen zum Filtern nach einer Spalte finden Sie unter [Filtern von Elementen in einer erweiterten Liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Ausblenden, Anzeigen oder Neuanordnen von Spalten finden Sie unter [Spalten anpassen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Hinzufügen oder Entfernen von Spalten finden Sie unter [Hinzufügen und Entfernen von Spalten mit ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) Spaltenmanager“ im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Optional) Informationen zum Anpassen der Zeilenhöhe finden Sie unter [Ändern der Zeilenhöhe in einer Ansicht](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) im Artikel [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Änderungsverlauf exportieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern > Verlaufsliste**.
1. Filtern Sie die Liste, um die zu exportierenden Elemente anzuzeigen.
1. Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png) und wählen Sie aus, ob Sie im XLSX- oder CSV-Format speichern möchten.

   Das Feld Datei speichern wird geöffnet, und Sie können die exportierte Datei auf Ihrem Computer speichern.
   Speichern der exportierten Datei beenden Sie können ihn jetzt auf Ihrem Computer finden und für andere freigeben.



