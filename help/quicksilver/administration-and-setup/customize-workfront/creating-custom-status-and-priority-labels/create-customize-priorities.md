---
title: Erstellen und Anpassen von Prioritäten
description: Sie können die Prioritäten für Projekte, Aufgaben und Probleme im Bereich Setup von Workfront steuern. Prioritäten geben Ihren Projekten, Aufgaben oder Problemen in Adobe Workfront Bedeutung.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 4a7362ae663b73ce48f049556145b4de3e6a6ac9
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 1%

---

# Prioritäten erstellen und anpassen

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Sie können die Prioritäten für Projekte, Aufgaben und Probleme im Bereich Setup von Workfront steuern. Prioritäten geben Ihren Projekten, Aufgaben oder Problemen in Adobe Workfront Bedeutung.

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
     <p>Neu: Standard</p>
     <p>oder</p>
     <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassen vorhandener Prioritäten

Als Workfront-Administrator können Sie die folgenden Änderungen an den in Workfront bereitgestellten Standardprioritäten vornehmen:

* Prioritäten umbenennen.
* Die Prioritäten neu anordnen.

  Weitere Informationen zur Neuanordnung von Prioritäten finden Sie unter [Erstellen einer Priorität für ein Projekt, eine Aufgabe oder ein Problem](#create-a-priority-for-a-project-task-or-issue).

* Standardpriorität ändern.

  Weitere Informationen zur Funktionalität zum Ändern der Standardpriorität finden Sie unter [Erstellen einer Priorität für ein Projekt, eine Aufgabe oder ein Problem](#create-a-priority-for-a-project-task-or-issue).

* Bearbeiten Sie die Beschreibung der Prioritäten.
* Legen Sie für jede Priorität eine Farbe fest.

  Die Farbe der Priorität wird in Diagrammberichten verwendet, wenn Sie Ihre Ergebnisse nach **Priorität** gruppieren.

  Weitere Informationen zu Diagrammberichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Löschen von Prioritäten.

  Wenn Sie eine vorhandene Priorität löschen, müssen Sie eine Ersatzpriorität auswählen.

* Prioritäten ausblenden.

  Weitere Informationen zur Funktionalität zum Ausblenden von Prioritäten finden Sie unter [Erstellen einer Priorität für ein Projekt, eine Aufgabe oder ein Problem](#create-a-priority-for-a-project-task-or-issue).

  >[!NOTE]
  >
  >In Ihrem Workfront-Konto muss für jedes Objekt mindestens eine Priorität vorhanden sein.

Die standardmäßig für jeden Objekttyp (Projekt, Aufgabe und Problem) bereitgestellten Prioritäten sind identisch:

* Keine
* Niedrig
* Normal
* Hoch
* Dringend

## Erstellen einer Priorität für ein Projekt, eine Aufgabe oder ein Problem {#create-a-priority-for-a-project-task-or-issue}

Zusätzlich zu den in Workfront bereitgestellten Standardprioritäten können Sie entsprechend den Anforderungen Ihres Unternehmens eigene Prioritäten hinzufügen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** > **Prioritäten**.

1. Klicken Sie auf die Registerkarte für den Objekttyp, für den Sie eine Priorität erstellen möchten (**Projekt**, **Aufgabe** oder **Problem**).
1. Klicken Sie <span class="preview">**Neue** unten in der Tabelle</span> oder **Neue Priorität hinzufügen**.
1. Konfigurieren Sie die folgenden Optionen für die Priorität:

   * **Prioritätsname**: Geben Sie einen Namen für die Priorität ein.
   * **Wichtigkeit**: Beim Hinzufügen einer neuen Priorität wird ihr standardmäßig eine Zahl zugewiesen. Bearbeiten Sie diese Nummer, wenn sie nicht Ihren Anforderungen entspricht.

     Die Wichtigkeitsnummer für jede Priorität muss eindeutig sein. Die Zahl der Priorität spiegelt die Bedeutung des Projekts, der Aufgabe oder des Problems wider: Die höchste Zahl entspricht der höchsten Priorität.

     Sie können diese Zahl nach dem Speichern der Priorität nicht mehr bearbeiten.

   * **Color**: Wählen Sie eine Farbe für die Priorität aus.

     Die Farbe der Priorität wird in Diagrammberichten und Agile-Team-Einstellungen verwendet. Informationen zu Diagrammberichten finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md). Informationen zu Agile-Team-Einstellungen finden Sie unter [Erstellen eines Agile-Teams](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * **Standardpriorität**: Wählen Sie die Priorität aus, die Workfront automatisch auf alle neu erstellten Projekte, Aufgaben oder Probleme anwenden soll.

     **Normal** ist die Standardpriorität für alle Objekte in Workfront.

     Sie können eine ausgeblendete Priorität nicht als Standard festlegen.

     <div class="preview">

     Die Standardpriorität wird durch ein Symbol ![Standardprioritätssymbol](assets/default-icon.png) gekennzeichnet. Um einen neuen Standard auszuwählen, führen Sie einen der folgenden Schritte aus:

      * Aktivieren Sie das Kontrollkästchen neben dem Namen der Priorität und wählen **Als Standard festlegen** in der Aktionsleiste am unteren Bildschirmrand aus.
      * Bewegen Sie den Mauszeiger über den Namen der Priorität und klicken Sie auf das **Mehr** Menü, das angezeigt wird. Wählen Sie dann **Als Standard festlegen** aus.

        Die neue Standardpriorität ist mit dem Symbol gekennzeichnet.

     </div>

   * **Beschreibung**: Geben Sie eine Beschreibung für die Priorität ein, um ihre Funktion zu erklären.
   * <span class="preview">**Auswahl ausblenden**</span> oder **Ausblenden**: <span class="preview">Wählen Sie **Ja**</span> oder aktivieren Sie das Kontrollkästchen, um eine nicht mehr benötigte Priorität auszublenden.

     Eine ausgeblendete Priorität wird nirgendwo in Workfront angezeigt, sodass Benutzende sie nicht für ihre Projekte, Aufgaben oder Probleme auswählen können.

     >[!IMPORTANT]
     >
     >Anstatt Prioritäten zu löschen, die Sie nicht mehr verwenden möchten, empfehlen wir, sie auszublenden. Auf diese Weise behalten Sie alle historischen Daten zu Objekten, die bereits mit der Priorität abgeschlossen wurden, und verhindern gleichzeitig, dass Benutzer die Priorität in Zukunft verwenden.

1. (Optional) Ändern Sie die Auflistungsreihenfolge Ihrer Prioritäten durch Ziehen und Ablegen in der gewünschten Reihenfolge.

   Dadurch wird die Reihenfolge geändert, in der sie für Projekte, Aufgaben oder Probleme angezeigt werden. Die Zahl „Wichtigkeit **wird** geändert.

1. Klicken Sie auf **Speichern**.

Anweisungen zur Anwendung von Prioritäten auf Projekte, Aufgaben und Probleme finden Sie in den folgenden Artikeln:

* [Projektprioritäten verstehen und aktualisieren](../../../manage-work/projects/planning-a-project/project-priority.md)
* [Aufgabenpriorität aktualisieren](../../../manage-work/tasks/task-information/task-priority.md)
* [Anfragepriorität aktualisieren](../../../manage-work/issues/issue-information/update-issue-priority.md)
