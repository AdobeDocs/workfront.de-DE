---
title: Verwenden des Projektkoordinators
content-type: reference
description: Erfahren Sie, wie Sie den Projektkoordinator verwenden, einen vorkonfigurierten KI-Mitarbeiter, der den Projektstatus überwacht und überfällige Aufgaben nachverfolgt.
author: Becky
feature: Work Management, Projects
source-git-commit: a4dfe29c0cf85f6029fd5f4398942c60bd3d6b5a
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 7%

---
# Verwenden des Projektkoordinators

{{highlighted-preview-article-level}}

Der Projektkoordinator ist ein vorkonfigurierter KI-Mitarbeiter, der Ihr Projekt überwacht und Stakeholder über wichtige Statusinformationen informiert.

Die Verwendung eines Projektkoordinators erfordert nicht, dass Sie einen Agenten außerhalb von Workfront konfigurieren.

Anweisungen zum Konfigurieren eines Projektkoordinators finden Sie unter [Konfigurieren eines Projektkoordinators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) im Artikel Konfigurieren von KI-Mitwirkenden.

Weitere Informationen zu KI-Mitwirkenden im Allgemeinen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Auswählen von, Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Sie müssen über Verwaltungsberechtigungen für Projekte verfügen, um einen Produktkoordinator zuzuweisen.</td> 
  </tr>
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Projektkoordinator - Übersicht

Der Projektkoordinator ist ein Virtual Project Manager (VPM), der Ihr Projekt überwacht und proaktiv hilft, die Arbeit auf Kurs zu halten. Wenn er als Projektinhaber zugewiesen wird, gilt Folgendes:

* Überprüft den Projektstatus und identifiziert überfällige und stagnierende Aufgaben.
* Sendet Anfragen zur Statusaktualisierung an Aufgabenbesitzer
* Kennzeichnet unvollständige Informationen in nativen Feldern und benutzerdefinierten Formularen
* Überwacht Dokumente auf Validierungsprobleme, fehlende Formulare oder Inaktivität
* Verfolgt Aufgabenabhängigkeiten und Flags, wenn Vorgänger abhängige Elemente gefährden
* Veröffentlicht Aktualisierungen und Folgemaßnahmen im Projekt-Update-Stream
* Hält den Projektinhaber über Projektprobleme auf dem Laufenden

Das Verhalten ist konfigurierbar, einschließlich der Aktionen, die der Mitarbeiter durchführt, und der Häufigkeit der Prüfung des Projektstatus.

## Hinzufügen des Projektkoordinators zu einem Projekt

Das Feld Projektkoordinator wird standardmäßig in der Kopfzeile des Projekts angezeigt. So weisen Sie einem Projekt einen Projektkoordinator zu:

1. Wechseln Sie zu dem Projekt, dem Sie einen Projektkoordinator zuweisen möchten.
1. Klicken Sie in der Kopfzeile des Projekts auf das Feld **Projektkoordinator**.
1. Wählen Sie den Projektkoordinator aus, den Sie zuweisen möchten.

   Im Fenster werden eine Beschreibung des ausgewählten Projektkoordinators sowie die Aktionen angezeigt, die der Projektkoordinator ausführt.
1. Klicken Sie auf **Übernehmen**.

## Konfigurieren des Projektkoordinators

Anweisungen zum Konfigurieren des Projektkoordinators finden Sie unter [Konfigurieren des Projektkoordinators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-the-project-coordinator) im Artikel Konfigurieren von KI-Mitwirkenden.
