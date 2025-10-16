---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Zeitplan erstellen
description: Sie können die Arbeitswochen Ihrer Benutzer mit Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder Projekt verknüpfen. Dies ermöglicht  [!DNL Workfront]  Berechnung von Zeitplänen und Benutzerverfügbarkeit.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: e8c89b68a022ae1c0cf5da20257cd8bc36e94d4c
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Zeitplan erstellen

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Als [!DNL Adobe Workfront] können Sie Ihre Arbeitswoche mit Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder Projekt verknüpfen. Auf diese Weise können [!DNL Workfront] Timelines und die Benutzerverfügbarkeit berechnen.

Wenn Sie Benutzer haben, die in verschiedenen Zeitzonen arbeiten, wird durch die Erstellung eines Zeitplans in jeder Zeitzone und die Verknüpfung mit diesen Benutzern sichergestellt, dass ihre Arbeit in [!DNL Workfront] in Echtzeit aufgezeichnet wird und dass ihre Verfügbarkeit immer korrekt ist, je nachdem, wann sie arbeiten.

Informationen zum Verknüpfen von Zeitplänen mit Benutzern und Projekten [&#x200B; Sie unter &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) eines Benutzers bearbeiten und [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Gruppenadministratoren können auch Zeitpläne erstellen, die mit den von ihnen verwalteten Gruppen verknüpft sind. Weitere Informationen finden Sie unter [Erstellen und Ändern der Zeitpläne einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Informationen zur Verwendung von Zeitplänen zur Unterstützung der Zusammenarbeit von Benutzenden in [!DNL Workfront] über Zeitzonen hinweg finden Sie [Arbeiten über Zeitzonen hinweg](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Informationen zur Verwendung von Zeitplänen in der Ressourcenplanung finden Sie unter [Zeitpläne - Übersicht](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) und [Ressourcenplaner - Übersicht](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL -Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zeitplan erstellen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Zeitpläne]**.
1. Klicken Sie **[!UICONTROL Neuer Zeitplan]**.
1. Geben Sie einen Namen für den Zeitplan ein.
1. (Optional) Wählen Sie **[!UICONTROL Standardzeitplan]**, um diesen Zeitplan als Standard festzulegen.

   Sie müssen mindestens einen Zeitplan in [!DNL Workfront] haben. Wenn Sie nur einen haben, wird dieser als Standardzeitplan festgelegt.

   Sie können mehrere Zeitpläne haben, aber Sie können nur einen Standardzeitplan haben.

   >[!NOTE]
   >
   >Wenn Sie Gruppenadministrator sind, können Sie keinen Zeitplan als Standardzeitplan festlegen. Nur ein [!DNL Workfront] kann einen Zeitplan als Standard für das System festlegen.

   ![Neuer Zeitplan](assets/new-schedule.png)

1. Wählen **[!UICONTROL auf der Registerkarte]** Zeitplan“ einen täglichen Zeitplan aus, indem Sie die blaue Kontur über die Blöcke ziehen, um sie zu markieren.

   Es wird empfohlen, 8 einstündige Blöcke über einen Zeitraum von 9 Stunden auszuwählen. Hier kann man Mittag- oder andere Pausen einlegen.

   ![Zeitblöcke in einem Zeitplan](assets/new-schedule-with-exceptions.png)

1. Geben Sie auf **[!UICONTROL Registerkarte]** die folgenden Informationen ein:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL -Gruppe mit Administratorzugriff]</td>
     <td><p>Wählen Sie die Gruppe aus, deren Administratoren berechtigt sind, diesen Zeitplan zu bearbeiten.</p>
     <p><b>WICHTIG</b>:</p>
      <ul>
       <li>
       <p>Wenn Sie ein Gruppenadministrator sind und einen Zeitplan erstellen, ist dieses Feld obligatorisch.</p>
       <p>Als Gruppenadministrator können Sie einen Zeitplan nur erstellen, wenn er für eine Gruppe oder Untergruppe vorgesehen ist, für die Sie als Administrator vorgesehen sind.</p>
       <p>Wenn Sie nur eine Gruppe verwalten, ist diese Gruppe standardmäßig in diesem Feld ausgewählt.</p>
       <p>Wenn Sie mehrere Gruppen verwalten, müssen Sie eine Gruppe in diesem Feld auswählen, bevor Sie den Zeitplan speichern können.</p></li>
       <li>Wenn Sie [!DNL Workfront] sind und einen Zeitplan erstellen, ist dieses Feld optional. Wenn Sie einen Zeitplan erstellen, ohne ihn einer Gruppe zuzuordnen, wird er als Zeitplan auf Systemebene gespeichert und kann nicht von einem Gruppenadministrator einer Gruppe verwaltet werden.
       <p>Zeitpläne, die Konten oder Projekten zugewiesen sind, sind für alle Benutzer sichtbar, die diese Objekte bearbeiten können. Dies gilt sowohl für Zeitpläne auf Systemebene als auch für Zeitpläne auf Gruppenebene.</p>
       </li>
       <p>Wenn Sie eine Gruppe mit Administratorzugriff für einen Zeitplan angeben, wird der Zeitplan nicht den Benutzenden in der Gruppe zugewiesen; es können nur die Gruppenadministratoren in der Gruppe den Zeitplan bearbeiten, löschen und kopieren.</p>
       <p>Gruppenadministratoren können keine Zeitpläne auf Systemebene bearbeiten, löschen oder kopieren. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Gruppen mit Ansichtszugriff]</td>
     <td><p>Wählen Sie die Gruppen mit Zugriff auf [!UICONTROL View] aus, die diesen Zeitplan sehen können.</p>
     <p>Nur die Benutzer in den hier angegebenen Gruppen können den Zeitplan im Dropdown-Menü finden, wenn sie ihn Benutzern oder Projekten zuweisen.</p></tr>
    <tr>
     <td>[!UICONTROL Zeitzone]</td>
     <td><p>Wählen Sie die Zeitzone für den Zeitplan aus.</p>
     <p>Wenn Sie den Zeitplan mit einem Benutzer verknüpfen, empfehlen wir, dass die Zeitzone des Zeitplans mit der des Benutzers übereinstimmt. Informationen zu den Zeitzonen der Benutzenden finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils.
     </td>
    </tr>
   </table>


1. Geben Sie auf **[!UICONTROL Registerkarte]** alle Ausnahmen für den Zeitplan an.

   Ausnahmen sind volle oder halbe Tage, die aus dem Zeitplan ausgeschlossen werden müssen, z. B. Feiertage oder Firmenveranstaltungen.

   >[!NOTE]
   >
   >Wenn Sie bereits wissen, was Ihre wiederkehrenden Zeitplanausnahmen sind, können Sie Ihre Zeitplanausnahmen für viele Jahre in der Zukunft definieren.

   Volle oder partielle Tage können aus dem Arbeitsplan ausgeschlossen werden. Klicken Sie auf das Datum, um es als Ausnahme auszuwählen, und wählen Sie dann das Feld **[!UICONTROL Alle Tage]**, um anzugeben, ob die Ausnahme ein ganzer Tag ist oder nicht.

   ![Ganztägige Ausnahme](assets/schedule-adding-an-all-day-exception.png)

1. Geben Sie die Anfangs- und Endzeit für die partiellen Tagesausnahmen ein.

   ![Teilweise Tagesausnahme](assets/partial-day-exception-on-schedules.png)

1. Klicken Sie **[!UICONTROL Speichern]** und dann auf **[!UICONTROL Speichern] Änderungen**.

1. (Optional) Verknüpfen Sie den Zeitplan mit einem Benutzer.

   Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Optional) Verknüpfen Sie den Zeitplan mit einem Projekt.

   Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
