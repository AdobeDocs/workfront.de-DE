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
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Festlegen einer benutzerdefinierten Bedingung als Standard für Projekte

Wenn für die Bedingungsart eines Projekts der Fortschrittsstatus anstelle der manuellen festgelegt wurde, zeigt Adobe Workfront automatisch eine von drei integrierten Standardbedingungen für das Projekt an (Zielgruppengerecht, Gefährdet oder In Schwierigkeiten), während es fortgesetzt wird, wie unter [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md) erläutert.

![Bedingung in Projekt-Kopfzeile und Details](assets/condition-of-project-0825.png)

Sie können Ihre benutzerdefinierten Bedingungen als Standardbedingungen festlegen, anstatt diese drei integrierten Standardbedingungen zu verwenden. Sie können beispielsweise die Standardbedingung On Target so ändern, dass sie in allen Projekten als Tracking Well angezeigt wird.

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
