---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten des Prozentsatzes für Benutzer- oder Rollenzuweisung für Aufgaben
description: Der Zuordnungsprozentsatz stellt die Zeit dar, die eine zugewiesene Ressource für die Arbeit an einer Aufgabe an einem Tag geplant ist. Dies ist der Prozentsatz eines Arbeitstags (entsprechend dem Benutzer- oder Projektplan), zu dem eine Ressource während der gesamten Dauer der Aufgabe zugewiesen wird.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 0d525df9beacc989ec3c1c695a7757dff0ad77b3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# Verwalten des Prozentsatzes für Benutzer- oder Rollenzuweisung für Aufgaben

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im dritten Quartal](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Der Zuordnungsprozentsatz stellt die Zeit dar, die eine zugewiesene Ressource für die Arbeit an einer Aufgabe an einem Tag geplant ist. Dies ist der Prozentsatz eines Arbeitstags (entsprechend dem Benutzer- oder Projektplan), zu dem eine Ressource während der gesamten Dauer der Aufgabe zugewiesen wird.

>[!NOTE]
>
>Wenn Benutzer zur Arbeit zugewiesen werden, wirkt sich ihre Verfügbarkeit entsprechend ihren Zeitplänen auf die geplanten und geplanten Daten von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen oder höhere Berechtigungen zur Aufgabe</p> <p>Berechtigungen bearbeiten, um den Zuordnungsprozentsatz im Feld "Aufgabe bearbeiten"zu aktualisieren</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Ändern der Prozentzuweisungen für Aufgaben

* Benutzern wird standardmäßig ein gleicher Prozentsatz der Zeit zugewiesen, wie Aufgaben, denen sie zugewiesen sind.
* Sie können den Zuordnungsprozentsatz für Benutzer und den Aufgaben, die Aufgaben zugewiesen sind, nur manuell ändern, wenn der Aufgabentyp &quot;Berechnete Arbeit&quot;oder &quot;Aufwandsorientierung&quot;lautet.

  Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Sie können die Prozentzuordnung für Teams, die Aufgaben zugewiesen sind, nicht ändern.
* Sie können die Prozentzuordnung für Benutzer und Auftragsrollen, die Problemen zugewiesen sind, nicht ändern.

## Ändern der Benutzer- oder Rollenprozentzuordnung für eine Aufgabe

1. Gehen Sie zu einer Aufgabe, für deren Ressourcen Sie die Prozentzuordnung ändern.
1. Klicken Sie auf **Mehr** Menü ![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe klicken Sie auf **Bearbeiten**.

   Oder

   Klicken Sie auf **Zuweisungen** Bereich in der Aufgabenüberschrift und klicken Sie dann auf **Erweitert**.

1. Stellen Sie sicher, dass **Dauer Typ** einer der folgenden Aufgaben ist:

   * Berechnete Arbeit
   * Leistungsgesteuert

   >[!TIP]
   >
   >* Für den Typ &quot;Berechnete Zuweisungsdauer&quot;verwendet Workfront die folgende Formel zur Berechnung des Zuordnungsprozentsatzes für jeden Bevollmächtigten: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Für den Typ Einfache Dauer können Sie die Stunden schätzen, die jeder Ressource zugewiesen sind, nicht den Zuordnungsprozentsatz.

1. Klicks **Zuweisungen**, ändern Sie dann die **Zuordnungen** für jeden Aufgabenverantwortlichen.

   Sie können nur den Zuordnungsprozentsatz für Benutzer- und Auftragserrollenzuweisungen ändern.

   Sie können den Zuordnungsprozentsatz für ein Team, das einer Aufgabe zugewiesen ist, nicht ändern.

   Beispielbild in der Produktionsumgebung:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Beispielbild in der Vorschau-Umgebung:</span>
   ![Zuteilungsprozentsatz ändern](assets/advanced-assignments-allocation-percentage.png)

1. Klicken Sie auf **Speichern**.
