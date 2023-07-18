---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer
description: Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '1379'
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

![Systemeinstellung für Benutzerzeitpläne](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Dadurch wird bestimmt, wie die Ressourcenverfügbarkeit auf Systemebene berechnet wird. Weitere Informationen zum Definieren der Voreinstellungen für die Ressourcenverwaltung für das System finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Je nachdem, wie diese Einstellung konfiguriert ist, wird die Verfügbarkeit der Benutzer im Ressourcen-Planer (Stunden sowie FTE-Verfügbarkeit) anhand der folgenden Methoden berechnet:

* **Standardzeitplan**: Der Standardzeitplan des Systems und die FTE des Benutzers werden verwendet, um den Wert Verfügbare Stunden und FTE für den Benutzer im Ressourcenplaner zu bestimmen. Der Zeitplan des Benutzers wird ignoriert. In diesem Fall:

   * Die **Verfügbare Stunden** werden im Ressourcen-Planer anhand der folgenden Formel berechnet:

     `User Available Hours = Default Schedule Hours * User FTE value`

     Wenn beispielsweise der Standardzeitplan eine Arbeitszeit von 40 Stunden pro Woche vorsieht und der Benutzer-FTE-Wert 0,5 beträgt, kann der Benutzer im Ressourcenplaner 20 Stunden pro Woche arbeiten.

     Weitere Informationen zu Zeitplänen, einschließlich des Standardzeitplans, finden Sie unter [Zeitplan erstellen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Die **Verfügbare FTE** für den Benutzer im Ressourcenplaner identisch mit der in den Benutzereinstellungen angegebenen FTE für den Benutzer ist.
Wenn das FTE-Format des Benutzers beispielsweise 0,5 in den Benutzereinstellungen beträgt, beträgt die verfügbare FTE des Benutzers 0,5 im Resource Planer. Weitere Informationen zum Wert der FTE des Benutzers, wie er in den Benutzereinstellungen angezeigt wird, finden Sie unter [Benutzerprofil bearbeiten](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **Zeitplan des Benutzers**: Der Zeitplan des Benutzers wird verwendet, um die Verfügbarkeit des Benutzers im Ressourcen-Planer zu bestimmen. Der Wert der FTE des Benutzers wird ignoriert. In diesem Fall:

   * Die **Verfügbare Stunden** im Ressourcenplaner sind mit den Stunden aus dem Zeitplan des Benutzers identisch.

  Wenn beispielsweise der Zeitplan des Benutzers 40 Stunden pro Woche für die Arbeit zur Verfügung hat, ist der Benutzer für 40 Stunden pro Woche im Ressourcen-Planer verfügbar.

   * Die **Verfügbare FTE** wird im Ressourcenplaner anhand der folgenden Formel berechnet:

  `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

  Wenn beispielsweise der Zeitplan des Benutzers 20 Stunden zur Arbeit zur Verfügung hat und der Standardzeitplan in Workfront 40 Stunden zur Verfügung hat, beträgt die FTE des Benutzers 0,5.

  Weitere Informationen zu Zeitplänen, einschließlich des Standardzeitplans, finden Sie unter [Zeitplan erstellen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Wenn der Benutzer keinem Zeitplan zugeordnet ist, werden die für den Benutzer verfügbaren Stunden anhand des Standardzeitplans berechnet.

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
* VZÄ eines Benutzers von 0,75

| Methode zur Berechnung der FTE (Systemeinstellung) | **Stunden vom Zeitplan des Benutzers** | **Stunden ab Standardzeitplan** | **Feld für Benutzer-FTE** | **Verfügbare Stunden im Ressourcenplaner** | **Verfügbare FTE im Ressourcenplaner** |
|---|---|---|---|---|---|
| **Der Standardzeitplan** | Ignoriert | 40 | 0.8 | **32** (berechnet) | **0.8** |
| **Der Zeitplan des Benutzers** | 20 | 40 | Ignoriert | **20** | **0,5** (berechnet) |

Eine zeitliche Abrechnung von Ausnahmen und Zeitüberschreitungen kann sich auf die geplante Stundenzahl oder die VZÄ auswirken. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Beispiel für eine Ressourcenplaneransicht nach Benutzer und Stunden:

![Ressourcenplaneransicht nach Benutzer und Stunden](assets/resource-planner-by-user-by-hours.png)

Beispiel-Ressourcenplaneransicht nach Benutzer und FTE:

![Ressourcenplaneransicht nach Benutzer und FTE](assets/resource-planner-by-user-by-fte.png)

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

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>Der Zeitplan des Benutzers wird bei der Berechnung der FTE für alle Werte außer den verfügbaren (AVL) FTE-Werten im Resource Planer ignoriert. Für die Berechnung wird nur der Standardzeitplan berücksichtigt.

Diese Berechnung gilt für die folgenden Werte:

* Geplante VZÄ (PLN)
* Budgetierte VZÄ (BDG)
* FTE-Varianz (VAR)
* NET FTE
* FTE-Differenz (DIF)
