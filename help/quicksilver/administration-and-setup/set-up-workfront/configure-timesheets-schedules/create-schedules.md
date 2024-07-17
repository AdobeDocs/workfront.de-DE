---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Zeitplan erstellen
description: Sie können die Arbeitswochen Ihrer Benutzer mit Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder einem Projekt verknüpfen. Dadurch kann [!DNL Workfront] die Zeitpläne und die Benutzerverfügbarkeit berechnen.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Zeitplan erstellen

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Als [!DNL Adobe Workfront] -Administrator können Sie Ihre Arbeitswoche mit Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder einem Projekt verknüpfen. Dadurch kann [!DNL Workfront] die Zeitpläne und die Benutzerverfügbarkeit berechnen.

Wenn Sie Benutzer haben, die in verschiedenen Zeitzonen arbeiten, stellen Sie durch Erstellen eines Zeitplans in jeder Zeitzone und die Zuordnung dieses Zeitplans zu diesen Benutzern sicher, dass ihre Arbeit in [!DNL Workfront] in Echtzeit aufgezeichnet wird und dass ihre Verfügbarkeit immer genau ist, je nachdem, wann sie funktionieren.

Informationen zum Verknüpfen von Zeitplänen mit Benutzern und Projekten finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) und [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Gruppenadministratoren können auch Zeitpläne erstellen, die mit den von ihnen verwalteten Gruppen verknüpft sind. Weitere Informationen finden Sie unter [Erstellen und Ändern der Zeitpläne einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Informationen zur Verwendung von Zeitplänen zur Unterstützung der Zusammenarbeit von Benutzern in [!DNL Workfront] über Zeitzonen hinweg finden Sie unter [Arbeiten über Zeitzonen hinweg](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Informationen zur Verwendung von Zeitplänen in der Ressourcenplanung finden Sie unter [Zeitplanübersicht](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) und [Ressourcenplanübersicht](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
       <p>Oder</p>
       <p>Aktuell: [!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zeitplan erstellen

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Zeitpläne]**.
1. Klicken Sie auf **[!UICONTROL Neuer Zeitplan]**.
1. Geben Sie einen Namen für den Zeitplan ein.
1. (Optional) Wählen Sie **[!UICONTROL Standardzeitplan]** aus, um diesen Zeitplan als Ihren Standardwert zu kennzeichnen.

   Sie müssen mindestens einen Zeitplan in [!DNL Workfront] haben. Wenn Sie nur eine haben, wird sie als Standardzeitplan festgelegt.

   Sie können mehrere Zeitpläne haben, aber Sie können nur einen Standardzeitplan haben.

   >[!NOTE]
   >
   >Wenn Sie Gruppenadministrator sind, können Sie einen Zeitplan nicht als Standardzeitplan festlegen. Nur ein [!DNL Workfront] -Administrator kann einen Zeitplan als Standard für das System festlegen.

   ![Neuer Zeitplan](assets/new-schedule.png)

1. Wählen Sie auf der Registerkarte **[!UICONTROL Plan]** einen täglichen Zeitplan aus, indem Sie die blaue Umrisslinie über mehrere Stunden ziehen, um sie hervorzuheben.

   Es wird empfohlen, 8 einstündige Blöcke über einen Zeitraum von 9 Stunden auszuwählen. Hier kann man zu Mittag oder zu anderen Pausen essen.

   ![Zeitblöcke eines Zeitplans](assets/new-schedule-with-exceptions.png)

1. Geben Sie auf der Registerkarte **[!UICONTROL Details]** die folgenden Informationen ein:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Gruppe mit Administratorzugriff]</td>
     <td><p>Wählen Sie die Gruppe aus, deren Administratoren zur Bearbeitung dieses Zeitplans berechtigt sind.</p>
     <p><b>WICHTIG</b>:</p>
      <ul>
       <li>
       <p>Wenn Sie Gruppenadministrator sind und einen Zeitplan erstellen, ist dieses Feld obligatorisch.</p>
       <p>Als Gruppenadministrator können Sie einen Zeitplan nur erstellen, wenn er für eine Gruppe oder Untergruppe bestimmt ist, für die Sie als Administrator bestimmt sind.</p>
       <p>Wenn Sie nur eine Gruppe verwalten, wird diese Gruppe in diesem Feld standardmäßig ausgewählt.</p>
       <p>Wenn Sie mehrere Gruppen verwalten, müssen Sie in diesem Feld eine Gruppe auswählen, bevor Sie den Zeitplan speichern können.</p></li>
       <li>Wenn Sie ein [!DNL Workfront] -Administrator sind und einen Zeitplan erstellen, ist dieses Feld optional. Wenn Sie einen Zeitplan erstellen, ohne ihn mit einer Gruppe zu verknüpfen, wird er als Plan auf Systemebene gespeichert und kann nicht von einem Gruppenadministrator einer beliebigen Gruppe verwaltet werden.
       <p>Zeitpläne, die Konten oder Projekten zugewiesen sind, sind für alle Benutzer sichtbar, die diese Objekte bearbeiten können. Dies gilt sowohl für Zeitpläne auf Systemebene als auch auf Gruppenebene.</p>
       </li>
       <p>Wenn Sie eine Gruppe mit Administratorzugriff für einen Zeitplan festlegen, wird der Zeitplan nicht den Benutzern der Gruppe zugewiesen. Er ermöglicht nur Gruppenadministratoren in der Gruppe, den Zeitplan zu bearbeiten, zu löschen und zu kopieren.</p>
       <p>Gruppenadministratoren können Zeitpläne auf Systemebene nicht bearbeiten, löschen oder kopieren. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Gruppen mit Zugriff auf Ansicht]</td>
     <td><p>Wählen Sie die Gruppen mit Zugriff auf die [!UICONTROL Ansicht] aus, die diesen Zeitplan sehen können.</p>
     <p>Nur die Benutzer in den hier angegebenen Gruppen können den Zeitplan im Dropdown-Menü finden, wenn sie ihn Benutzern oder Projekten zuweisen.</p></tr>
    <tr>
     <td>[!UICONTROL Zeitzone]</td>
     <td><p>Wählen Sie die Zeitzone für den Zeitplan aus.</p>
     <p>Wenn Sie den Zeitplan mit einem Benutzer verknüpfen, empfehlen wir, dass die Zeitzone des Zeitplans mit der des Benutzers übereinstimmt. Informationen zu den Zeitzonen des Benutzers finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils.
     </td>
    </tr>
   </table>


1. Geben Sie auf der Registerkarte **[!UICONTROL Ausnahmen]** Ausnahmen vom Zeitplan an.

   Ausnahmen sind volle oder halbe Tage, die vom Zeitplan ausgeschlossen werden müssen, wie Feiertage oder Firmenveranstaltungen.

   >[!NOTE]
   >
   >Wenn Sie bereits wissen, welche Ausnahmen beim wiederkehrenden Zeitplan vorliegen, können Sie in der Zukunft für viele Jahre Ausnahmen festlegen.

   Vollständige oder teilweise Tage können vom Arbeitsplan ausgeschlossen werden. Klicken Sie auf das Datum, um es als Ausnahme auszuwählen, und wählen Sie dann das Feld **[!UICONTROL Alle Tage]** aus, um anzugeben, ob es sich bei der Ausnahme um einen vollen Tag handelt oder nicht.

   ![Gesamter Tagesausschluss](assets/schedule-adding-an-all-day-exception.png)

1. Geben Sie die Start- und Endzeit für die partiellen Tagesausnahmen ein.

   ![Unvollständiger Tag-Ausnahmefehler](assets/partial-day-exception-on-schedules.png)

1. Klicken Sie auf **[!UICONTROL Speichern]** und dann auf **[!UICONTROL Speichern] Änderungen**.

1. (Optional) Verknüpfen Sie den Zeitplan mit einem Benutzer.

   Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Optional) Verknüpfen Sie den Zeitplan mit einem Projekt.

   Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
