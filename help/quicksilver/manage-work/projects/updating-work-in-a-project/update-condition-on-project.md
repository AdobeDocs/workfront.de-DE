---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für ein Projekt
description: Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird und anzeigt, ob die damit verbundene Arbeit reibungslos verläuft oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der angibt, ob Sie aktiv daran arbeiten oder nicht.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 4%

---

# Aktualisierungsbedingung für ein Projekt

Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird und anzeigt, ob die damit verbundene Arbeit reibungslos verläuft oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der angibt, ob Sie aktiv daran arbeiten oder nicht.

Sie können die Bedingung eines Projekts entweder automatisch oder manuell festlegen. Um die Bedingung eines Projekts manuell zu ändern, müssen Sie Projektinhaber sein oder über Verwaltungsrechte dafür verfügen.

Der Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
  <p>Standard</p>
   <p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Zugriff auf Aufgaben und Probleme bearbeiten </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern der Berechtigungen für Aufgaben und Probleme zum Anzeigen ihrer Bedingung</p>
   <p>Berechtigungen für Aufgaben und Probleme verwalten, um die Bedingung zu aktualisieren</p>
     </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the new licenses:
  <p>Standard</p>
   
   For current licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
     </td> 
  </tr> 
 </tbody> 
</table>-->

## Bedingung automatisch festlegen

Das automatische Festlegen der Bedingung eines Projekts wird durch den Bedingungstyp des Projekts bestimmt. Der Bedingungstyp muss auf Fortschrittsstatus festgelegt sein, damit Workfront die Bedingung des Projekts automatisch festlegt.

Der Workfront- oder Gruppenadministrator bestimmt den Standard des Felds „Bedingungstyp“ für neue Projekte in Ihrem System, wenn Sie im Bereich „Setup“ die Projektvoreinstellungen festlegen. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Wenn Sie ein Projekt erstellen, wird die Bedingung des Projekts automatisch so festgelegt, dass sie dem Fortschrittsstatus des Projekts zu diesem Zeitpunkt entspricht. Der Fortschrittsstatus des Projekts hängt vom Fortschritt der Aufgaben im Projekt ab.

Informationen zu Projektbedingungen und wie sie auf Grundlage des Fortschrittsstatus berechnet werden, finden Sie unter [Übersicht über den Projektfortschritt](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Bedingung für ein Projekt manuell aktualisieren

Wenn Sie den Bedingungstyp Ihres Projekts auf Manuell anstelle des Fortschrittsstatus festlegen, können Sie die Bedingung eines Projekts manuell aktualisieren.

1. Wechseln Sie zu dem Projekt, für das Sie die Bedingung aktualisieren möchten.
1. Klicken Sie **linken Bedienfeld auf** Abschnitt „Projektdetails“.

1. Stellen Sie sicher **dass das Feld** Bedingungstyp“ auf &quot;**&quot;**.

   ![Projektdetailübersicht - Bedingung auswählen](assets/project-details-overview-select-condition.png)

1. Wählen Sie im Feld **Bedingung** die aus den folgenden Optionen diejenige aus, die Ihrem Verständnis dafür entspricht, ob die damit verbundene Arbeit reibungslos verläuft oder ob es Verzögerungen gibt:

   * **Im Zielbereich**
   * **Gefährdet**
   * **In Schwierigkeiten**

   Weitere Informationen zu Projektbedingungen finden Sie unter [Übersicht über Projektbedingungen und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Die Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung möglicherweise mehr als drei Optionen für die Bedingung finden. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klicken Sie auf **Änderungen speichern**.
