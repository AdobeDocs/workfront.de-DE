---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für ein Projekt
description: Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird, um anzugeben, ob die damit verbundenen Arbeiten reibungslos verlaufen oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der anzeigt, ob Sie aktiv daran arbeiten oder nicht.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 1%

---

# Aktualisierungsbedingung für ein Projekt

Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird, um anzugeben, ob die damit verbundenen Arbeiten reibungslos verlaufen oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der anzeigt, ob Sie aktiv daran arbeiten oder nicht.

Sie können die Bedingung eines Projekts entweder automatisch oder manuell festlegen. Um die Bedingung eines Projekts manuell zu ändern, müssen Sie Projekteigentümer sein oder über Administratorrechte verfügen.

Der Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
  <p>Standard</p>
   
   For legacy licenses:
   <ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Bedingung automatisch festlegen

Das automatische Festlegen der Bedingung eines Projekts wird durch den Bedingungstyp des Projekts bestimmt. Der Bedingungstyp muss auf Fortschrittsstatus gesetzt werden, damit Workfront die Projektbedingung automatisch festlegt.

Ihr Workfront- oder Gruppenadministrator legt die Standardeinstellung des Felds Bedingungstyp für neue Projekte in Ihrem System fest, wenn Sie Projektvoreinstellungen im Bereich Einrichtung festlegen. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Wenn Sie ein Projekt erstellen, wird die Bedingung des Projekts automatisch so festgelegt, dass sie dem Fortschrittsstatus des Projekts zu diesem Zeitpunkt entspricht. Der Fortschrittsstatus des Projekts basiert auf dem Fortschritt der Aufgaben im Projekt.

Informationen zu den Projektbedingungen und dazu, wie sie basierend auf dem Fortschrittsstatus berechnet werden, finden Sie unter [Übersicht über den Projektstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Manuelles Aktualisieren der Bedingung für ein Projekt

Wenn Sie den Bedingungstyp Ihres Projekts auf &quot;Manuell&quot;anstelle von &quot;Fortschrittsstatus&quot;festlegen, können Sie die Bedingung eines Projekts manuell aktualisieren.

1. Wechseln Sie zu dem Projekt, für das Sie die Bedingung aktualisieren möchten.
1. Klicken Sie auf **Projektdetails** Abschnitt.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Stellen Sie sicher, dass **Bedingungstyp** -Feld auf **Manuell**.

1. Im **Bedingung** Wählen Sie aus den folgenden Optionen die Option aus, die Ihrem Verständnis entspricht, ob die damit verbundenen Arbeiten reibungslos laufen oder ob es Verzögerungen gibt:

   * **Im Zielbereich**
   * **Gefährdet**
   * **In Schwierigkeiten**

   Weitere Informationen zu den Projektbedingungen finden Sie unter [Übersicht über Projektbedingung und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klicken **Speichern**.click **Änderungen speichern**.
