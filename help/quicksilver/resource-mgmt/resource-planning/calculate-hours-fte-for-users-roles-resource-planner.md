---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer
description: Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Sie können die Zuordnung und Verfügbarkeit Ihrer Ressourcen im Ressourcenplaner nach Stunden, FTE oder Kosten anzeigen.\
Weitere Informationen zur Berechnung der Kosten im Ressourcenplaner finden Sie unter [Kosten im Ressourcenplaner berechnen](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot;steht für Vollzeitäquivalent. Es handelt sich dabei um eine Zeitangabe, die angibt, wie viele Stunden während eines Tages oder einer Woche für einen Benutzer oder eine berufliche Rolle für eine echte Arbeit aufgewendet werden.

Die folgenden Ressourcendaten werden im Ressourcenplaner unterschiedlich berechnet:

* Die Werte Verfügbare Stunden oder FTE werden auf Grundlage der Konfiguration der Voreinstellungen für die Ressourcenverwaltung in Ihrem System durch Ihren Systemadministrator berechnet.\
   Weitere Informationen zur Berechnung der Werte für verfügbare Stunden und VZÄ finden Sie unter [Berechnen der verfügbaren Stunden oder der FTE für Benutzer und Stellenrollen im Resource Planer](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
   Weitere Informationen zum Definieren der Voreinstellungen für die Ressourcenverwaltung für das Adobe Workfront-System finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Alle anderen FTE-Werte werden auf der Grundlage des Systemstandardzeitplans berechnet.\
   Weitere Informationen dazu, wie die anderen Werte bei Verwendung von FTE im Resource Planer angezeigt werden, finden Sie im Abschnitt [Berechnen Sie alle anderen Stunden- und FTE-Werte für Benutzer und Rollen im Resource Planer.](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) in diesem Artikel.

Es ist wichtig zu verstehen, was die FTE für jeden Ihrer Benutzer und seine Aufgabenrollen ist, um Ihre Ressourcen genau zu verwalten, während Sie sie für die Arbeit zuweisen.

## Berechnen der verfügbaren Stunden oder der FTE für Benutzer und Stellenrollen im Resource Planer {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Berechnen der verfügbaren Stunden und der FTE für einen Benutzer im Resource Planer](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Berechnen Sie die verfügbaren Stunden und die FTE für eine Rolle im Ressourcenplaner.](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Berechnen Sie die verfügbaren Stunden und die FTE für einen Benutzer im Ressourcen-Planer (Beispiel).](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Berechnen der verfügbaren Stunden und der FTE für einen Benutzer im Resource Planer {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Der Workfront-Administrator bestimmt, wie die verfügbare Zeit für einen Benutzer berechnet wird, indem er im Bereich &quot;Ressourcenverwaltung&quot;unter &quot;Einrichtung&quot;eine der folgenden Optionen auswählt:

* Der Standardzeitplan des Systems und die FTE des Benutzers.
* Der Zeitplan des Benutzers.

Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### Berechnen Sie die verfügbaren Stunden und die FTE für eine Rolle im Ressourcenplaner. {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Sie müssen zunächst die Benutzerverfügbarkeit berechnen und dann die Verfügbarkeit der einzelnen Rollen berechnen.

Bei der Verfügbarkeit von Stellenrollen im Ressourcenplaner werden die Gesamtverfügbarkeit des Benutzers und die **Prozentsatz der VZÄ-Verfügbarkeit** mit jeder Benutzerrolle verknüpft ist.\
![percent_of_fte_available_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Weitere Informationen zum Verknüpfen eines **Prozentsatz der VZÄ-Verfügbarkeit** -Wert mit einer Vorgangsrolle für einen Benutzer finden Sie unter [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Wenn beispielsweise der Wert Verfügbare Stunden für einen Benutzer 40 beträgt und er eine Primäre Rolle für 75 % dieser Zeit und eine andere Rolle für 25 % dieser Zeit erfüllen kann, zeigt der Ressourcenplaner, dass die Variable **Verfügbare Stunden** -Wert für die Primäre Rolle für eine Woche 30 Stunden beträgt und dass die **Verfügbare Stunden** -Wert für &quot;Sonstige Rolle&quot;10 Stunden beträgt. In diesem Fall beträgt die VZÄ für die Primäre Rolle 0,75 und die VZÄ für die andere Rolle 0,25.

>[!NOTE]
>
>Die für den Benutzer insgesamt verfügbare Zeit wird anhand einer der beiden im Abschnitt [Berechnen der verfügbaren Stunden und der FTE für einen Benutzer im Resource Planer](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) in diesem Artikel.

Beim Anzeigen des Ressourcenplaners in der Rollenansicht entspricht die Verfügbarkeit einer Arbeitsplatzrolle der Verfügbarkeit aller Benutzer, die diese Rolle erfüllen können.\
Weitere Informationen zur Verfügbarkeit von Ressourcen im Ressourcen-Planer finden Sie im Abschnitt [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Berechnen Sie die verfügbaren Stunden und die FTE für einen Benutzer im Ressourcen-Planer (Beispiel). {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Die folgende Tabelle zeigt, wie die verfügbaren Stunden und die verfügbare FTE für den Benutzer im Ressourcenplaner berechnet werden, je nachdem, welche Methode der Systemadministrator in den Voreinstellungen für die Ressourcenverwaltung für die FTE-Berechnung verwendet.

Für dieses Beispiel verwenden wir die folgenden Zahlen:

* Standardzeitplan des Systems beträgt 40 Stunden
* Ein Benutzerzeitplan von 20 Stunden
* Ein FTE-Nutzer von 0,75.

| Methode zur Berechnung der FTE (Systemeinstellung) | **Stunden vom Zeitplan des Benutzers** | **Stunden ab Standardzeitplan** | **Feld für Benutzer-FTE** | **Verfügbare Stunden im Ressourcenplaner** | **Verfügbare FTE im Ressourcenplaner** |
|---|---|---|---|---|---|
| **Der Standardzeitplan** | Ignoriert | 40 | 0.75 | **30** (berechnet) | **0.75** |
| **Der Zeitplan des Benutzers** | 20 | 40 | Ignoriert | **20** | **0,5** (berechnet) |

Eine zeitliche Abrechnung von Ausnahmen und Zeitüberschreitungen kann sich auf die geplante Stundenzahl oder die VZÄ auswirken. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Berechnen Sie alle anderen Stunden- und FTE-Werte für Benutzer und Rollen im Resource Planer. {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Zusätzlich zu den verfügbaren Stunden oder VZÄ werden im Ressourcenplaner auch die folgenden Zeitinformationen angezeigt:

* Geplante Stunden
* Budgetierte Stunden
* Stundenvarianz
* Netzstunden\
   Weitere Informationen zu diesen Werten finden Sie unter [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Stundendifferenz\
   Weitere Informationen dazu, was dieser Wert darstellt, finden Sie unter [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Sie können dieselben Informationen im Ressourcenplaner als FTE oder als Stunden anzeigen.

Workfront verwendet die folgende Formel, um alle anderen Werte als FTE im Ressourcenplaner anzuzeigen:

```
FTE = Resource Planner Hours/ Default Schedule Hours
```

>[!NOTE]
>
>Der Zeitplan des Benutzers wird bei der Berechnung der FTE für alle Werte außer den verfügbaren (AVL) FTE-Werten im Resource Planer ignoriert. Für die Berechnung wird nur der Standardzeitplan berücksichtigt.

Diese Berechnung gilt für die folgenden Werte:

* Geplante VZÄ (PLN)
* Budgetierte VZÄ (BDG)
* FTE-Varianz (VAR)
* NET FTE
* FTE-Differenz (DIF)
