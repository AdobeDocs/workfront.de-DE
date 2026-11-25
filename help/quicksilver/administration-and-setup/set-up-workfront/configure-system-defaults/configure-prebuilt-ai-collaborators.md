---
user-type: administrator
product-area: system-administration;setup
title: Konfigurieren von vordefinierten KI-Mitwirkenden
description: Als Adobe Workfront-Administrator können Sie vorgefertigte KI-Mitwirkende aus Adobe, wie z. B. den Aufnahmekoordinator, als Arbeitsagenten konfigurieren, die Benutzende Aufgaben und Problemen zuweisen können.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: ee344fe88ba7e4fb78a6d80ccbfe5cfa1ecbec47
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 8%
---
# Konfigurieren von vordefinierten KI-Mitwirkenden

## Überblick

Vordefinierte KI-Mitwirkende sind vorgefertigte Arbeitsagenten von Adobe, die für eine bestimmte Aufgabe eingerichtet sind, z. B. zum Überprüfen von Anfragen auf fehlende Informationen. Sie sind als native Adobe-Arbeitsagenten verfügbar, sodass Sie keinen Agenten in einer externen Plattform konfigurieren oder Anmeldeinformationen für externe Plattformen angeben müssen.

Wenn Sie einen Arbeitsagenten konfigurieren, wählen Sie einen vordefinierten Mitarbeiter als Quelle des Agenten aus. Anschließend können Sie den Arbeitsagenten benennen, seine Zugriffsebene festlegen und die Aktionen auswählen, die er ausführen kann. Benutzer weisen den konfigurierten Arbeitsagenten Aufgaben oder Problemen auf dieselbe Weise zu wie andere Arbeitsagenten. Benutzer müssen nicht wissen, dass es sich bei dem Agenten um einen vorgefertigten Mitarbeiter handelt.

Weitere Informationen zu Arbeitsagenten und den anderen KI-Mitwirkungstypen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

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
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator] oder Gruppenadministrator</td> 
  </tr> 
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Für Ihr Unternehmen muss Adobe CX Coworker aktiviert sein. Weitere Informationen finden Sie unter [Übersicht über CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

## Konfigurieren eines vordefinierten KI-Mitwirkenden

Sie konfigurieren einen vordefinierten KI-Mitwirkenden, wenn Sie einen Arbeitsagenten konfigurieren. Wählen Sie im Bereich **Herkunft des Agenten auswählen** die Option **Adobe nativ** und wählen Sie dann aus der folgenden Liste den vorgefertigten Mitarbeiter aus, den Sie verwenden möchten.

Die vollständigen Schritte finden Sie unter [Konfigurieren eines Arbeitsagenten in Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront).

Nachdem der Mitarbeiter konfiguriert wurde, können Benutzer ihn Aufgaben oder Problemen zuweisen. Weitere Informationen finden Sie unter [Verwenden von Arbeitsagenten](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

## Verfügbare vordefinierte KI-Mitwirkende

### CX Enterprise Coworker {#cx-enterprise-coworker}

Ein CX Enterprise Coworker-Agent, der von Adobe Agent Orchestrator unterstützt wird.

Weitere Informationen finden Sie unter [Übersicht über CX Enterprise Coworker in Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

### Intake-Koordinator {#intake-coordinator}

Der Aufnahmekoordinator prüft die Details, benutzerdefinierten Formulare und Anhänge von Anfragen auf fehlende, unklare oder inkonsistente Informationen. Es veröffentlicht Feedback oder nimmt Änderungen mit Genehmigung des Benutzers vor.

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
