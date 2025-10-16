---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Persönliche Aufgaben erstellen
description: Persönliche Aufgaben sind Ad-hoc-Arbeitsanfragen, die Sie an einen Benutzer bzw. an sich selbst senden, oder Aufgaben, die Sie für sich selbst in Ihrem Home-Bereich erstellen. Workfront speichert Ad-hoc-Arbeitsanfragen und erledigt Elemente als persönliche Aufgaben.
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Persönliche Aufgaben erstellen

<!--Audited: 10/2024-->

Persönliche Aufgaben sind Ad-hoc-Arbeitsanfragen, die Sie an einen Benutzer senden oder selbst an ihn senden oder hinzufügen.

Adobe Workfront speichert Ad-hoc-Arbeitsanfragen und erledigt Elemente als persönliche Aufgaben für das persönliche Projekt eines Benutzers, das Workfront automatisch für jeden Benutzer erstellt.

Im Folgenden finden Sie Merkmale des persönlichen Projekts eines Benutzers:

* Alle Benutzer von Workfront verfügen über ein persönliches Projekt mit dem Namen „Aufgaben des &lt; vollständigen Namens des Benutzers>&quot;. Beispiel: „Aufgaben von John Smith“.
* Das persönliche Projekt jedes Benutzers wird nicht in Suchvorgängen angezeigt und es ist ausgeblendet.
* Ein persönliches Projekt kann nicht gelöscht werden, auch wenn Benutzer deaktiviert wurden.
* Der Status eines persönlichen Projekts ist immer Aktuell. Persönliche Projekte können nicht abgeschlossen oder abgebrochen werden.
* Alle persönlichen Aufgaben werden im persönlichen Projekt eines Benutzers gespeichert.
* Bei Bedarf können Sie persönliche Aufgaben in ein anderes Projekt verschieben.

Sie können persönliche Aufgaben wie folgt erstellen:

* Erstellen eines Aufgabenelements im Bereich Startseite

  Weitere Informationen finden Sie [Erstellen von Arbeitselementen und Projekten im Bereich Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Erstellen und Senden einer persönlichen Arbeitsanfrage an einen anderen Benutzer über die Benutzerprofilseite
* Erstellen Sie eine persönliche Arbeitsanfrage und senden Sie sie über Ihre Benutzerprofilseite an sich selbst.

In diesem Artikel wird beschrieben, wie Sie eine persönliche Arbeitsanfrage für einen Benutzer oder für sich selbst über die Benutzerprofilseite erstellen können.

Unabhängig davon, wie Sie eine persönliche Aufgabe hinzufügen, finden Sie sie in denselben Bereichen von Workfront. Weitere Informationen finden Sie im Abschnitt [Persönliche Aufgabe suchen](#locate-personal-tasks) in diesem Artikel.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Paket</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz</strong></td> 
   <td> 
   <p>Standard<p>
   <p>Plan</p>
   <p>Dies ist die Lizenz, die benötigt wird, um Anfragen an andere Benutzer zu senden. Alle Benutzer können einen Arbeitsauftrag für sich selbst erstellen.</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Benutzer, um einen Arbeitsauftrag für sie zu erstellen. Zeigen Sie den Zugriff an, um einen persönlichen Arbeitsauftrag für sich selbst zu erstellen. </p>
   </td> 
  </tr>

</tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## Persönlichen Arbeitsauftrag erstellen

1. Wechseln Sie zur Profilseite Ihres Benutzers oder zur Profilseite eines anderen Benutzers, auf die Sie Zugriff haben.

   >[!TIP]
   >
   >Ihr Workfront-Administrator kann möglicherweise verhindern, dass bestimmte Benutzende angezeigt werden, wenn sie Ihre Zugriffsebene konfigurieren.

1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Benutzers in der Kopfzeile.
1. Klicken Sie **Arbeitsauftrag senden**.
Das **Benutzer eine Arbeitsanfrage senden** wird angezeigt.

   ![](assets/personal-task-box.png)
1. Aktualisieren Sie die folgenden Informationen:

   * **Aufgabenname**: Dies ist der Name der Ad-hoc-Arbeitsanfrage oder der persönlichen Aufgabe.
   * **Beschreibung**: Fügen Sie eine Beschreibung für die Aufgabe hinzu.
   * **Zuweisen zu**: Der Name des ausgewählten Benutzers wird standardmäßig angezeigt. Sie können weitere Benutzer oder Teams hinzufügen.
   * **Fälligkeitsdatum**: Dies ist das Datum, bis zu dem diese Aufgabe abgeschlossen sein soll. Standardmäßig ist dies das heutige Datum. Es kann kein Datum in der Vergangenheit ausgewählt werden
   * **Zeit**: Dies ist der Zeitpunkt, zu dem diese Aufgabe abgeschlossen sein soll. Standardmäßig ist dies die aktuelle Zeit.

1. Klicken Sie **Anforderung senden** um die Arbeitsanfrage zu speichern.

   Die Arbeitsanfrage wird in Workfront als persönliche Aufgabe gespeichert und dem Aufgaben-Widget des Benutzers auf seiner Startseite hinzugefügt. Wenn Sie die Arbeitsanfrage an sich selbst senden, wird sie in Ihrem Aufgaben-Widget auf der Startseite angezeigt.


## Persönliche Aufgaben suchen

Sie können persönliche Aufgaben in den folgenden Bereichen suchen:

* Das Aufgaben-Widget im Home-Bereich des Benutzers, an den die persönliche Anfrage gesendet wurde.

  Weitere Informationen finden Sie [Erstellen von Arbeitselementen und Projekten im Bereich Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

* Ein persönlicher Aufgabenbericht oder eine Liste. Sie können einen Filter für persönliche Aufgaben erstellen und auf einen Aufgabenbericht oder eine Aufgabenliste anwenden, um nur persönliche Aufgaben anzuzeigen und Projektaufgaben auszuschließen.

  Weitere Informationen finden Sie [Filter: Persönliche Aufgaben](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
