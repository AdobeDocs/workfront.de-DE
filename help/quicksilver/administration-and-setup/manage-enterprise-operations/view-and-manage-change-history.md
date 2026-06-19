---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Verlauf ändern
description: Mit dem Änderungsverlauf können Sie ein Änderungsprotokoll für Workfront-Objekte anzeigen
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 44292bc9cf8654d1ecfb398b0f118a6c001f544f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 7%

---

# Änderungsverlauf anzeigen und verwalten

Sie können den Änderungsverlauf, einschließlich der Auditprotokolle, im Bereich „Änderungsverfolgung“ von Setup einsehen.

* **Auditprotokolle** sind Änderungen, die von Benutzern ausgelöst werden.
Weitere Informationen zu Auditprotokollen und zum Bereich Auditprotokolle finden Sie unter [Übersicht über Auditprotokolle](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **Konfiguration** zeigt an, welche Felder für die Liste „Änderungsverlauf“ verfolgt werden.
Die Konfiguration ist derzeit nur als Information verfügbar und kann nicht geändert werden. Die Möglichkeit, zu ändern, welche Felder verfolgt werden, wird in naher Zukunft verfügbar sein.
* Mit der Liste „Änderungsverlauf“ können Sie ein Protokoll der Änderungen an Workfront-Objekten anzeigen, einschließlich Attributen wie:

   * Objekt
   * Objekttyp
   * Art der Änderung (Vorgang)
   * Source der Änderung, z. B. bestimmte Benutzende, APIs, Workfront Fusion, KI-LLMs oder das Workfront-System

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein, um den Änderungsverlauf anzeigen zu können</td> 
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
1. Um nach einem bestimmten Begriff zu suchen, klicken Sie auf die Suchleiste und geben Sie den Begriff ein. Die Ergebnisse werden bei der Eingabe gefiltert.
1. (Optional) Informationen zum Filtern nach einer Spalte finden Sie unter [Filtern von Elementen in einer erweiterten Liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) im Artikel Verwenden von erweiterten Listen.
1. (Optional) Informationen zum Ausblenden, Anzeigen oder Neuanordnen von Spalten finden Sie unter [Spalten anpassen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) im Artikel Verwenden von Verbesserungslisten.
1. Informationen zum Hinzufügen oder Entfernen von Spalten finden [ unter „Hinzufügen und Entfernen von Spalten mit ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) Spaltenmanager“ im Artikel Verwenden von erweiterten Listen.
1. Informationen zum Anpassen der Zeilenhöhe finden [ unter „Ändern der Zeilenhöhe in einer Ansicht](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) im Artikel Verwenden von Verbesserungslisten.





