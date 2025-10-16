---
title: Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wenn für die Bedingungsart eines Projekts der Fortschrittsstatus anstelle der manuellen festgelegt wurde, zeigt Adobe Workfront im Verlauf des Vorgangs automatisch eine von drei integrierten Standardbedingungen für das Projekt an (Zielgruppe, Gefährdet oder In Schwierigkeiten), wie unter Übersicht über Projektbedingung und Bedingungstyp erläutert.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 2%

---

# Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte

Wenn für die Bedingungsart eines Projekts der Fortschrittsstatus anstelle der manuellen festgelegt wurde, zeigt Adobe Workfront automatisch eine von drei integrierten Standardbedingungen für das Projekt an (Zielgruppengerecht, Gefährdet oder In Schwierigkeiten), während es fortgesetzt wird, wie unter [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md) erläutert.

![Bedingung in Projekt-Kopfzeile und Details](assets/condition-of-project-0825.png)

Sie können Ihre benutzerdefinierten Bedingungen als Standardbedingungen festlegen, anstatt diese drei integrierten Standardbedingungen zu verwenden. Sie können beispielsweise die Standardbedingung On Target so ändern, dass sie in allen Projekten als Tracking Well angezeigt wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legen Sie eine benutzerdefinierte Bedingung als Standardbedingung für alle Projekte fest:

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Bedingungen**.

1. Klicken Sie auf **Registerkarte** Projekte“.
1. Klicken Sie **Standardbedingungen festlegen**.
1. Klicken Sie im Dropdown-Menü für die Standardbedingung, die Sie ändern möchten, auf die benutzerdefinierte Bedingung, die Sie stattdessen verwenden möchten.
1. Wiederholen Sie den vorherigen Schritt für jede andere Standardbedingung, die Sie ändern möchten.
1. Klicken Sie auf **Speichern**.

Informationen zum Festlegen einer benutzerdefinierten Bedingung als Standardbedingung für Aufgaben und Probleme finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standardbedingung für Aufgaben und Probleme](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Informationen zum Einrichten eines Projekts, damit Benutzer seine Bedingung manuell aktualisieren können, finden Sie unter [Bedingung für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
