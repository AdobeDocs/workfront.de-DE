---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen einer Vorgängerbeziehung in der Aufgabenliste
description: Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei hosten (abhängige Aufgabe), bevor Sie die Einladungen versenden (Vorgängeraufgabe).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Erstellen einer Vorgängerbeziehung in der Aufgabenliste

<!-- Audited: 5/2025 -->

Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen. Sie möchten beispielsweise keine Partei hosten (abhängige Aufgabe), bevor Sie die Einladungen versenden (Vorgängeraufgabe).

In diesem Artikel erfahren Sie, wie Sie Vorgänger in der Aufgabenliste erstellen.

Sie können die Vorgänger von Aufgaben in den folgenden Bereichen von Adobe Workfront anzeigen:

* In der Aufgabenliste in der Spalte Vorgänger .
* Im Gantt-Diagramm.
* Im Abschnitt Vorgänger einer abhängigen Aufgabe.

Weitere Informationen finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgaben und das Projekt</p></td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Standard </p><p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Vorgänger erstellen

{{step1-to-projects}}

1. Wählen Sie ein Projekt auf der Seite **Projekte** aus.
1. Klicken Sie **linken** auf „Aufgaben“.
1. Wählen **in der Dropdown** Liste „Ansichten“ eine Ansicht aus, die die Spalte **Vorgänger** anzeigt, oder fügen Sie die Spalte zur aktuellen Ansicht hinzu.

1. Wählen Sie die Aufgabe aus, die Sie als abhängige Aufgabe festlegen möchten.
1. Klicken Sie in die Spalte **Vorgänger** der Aufgabe.
1. Geben Sie die Aufgabennummer ein, die Sie als Vorgänger der ausgewählten Aufgabe angeben möchten, und drücken Sie dann **Eingabetaste**.

   >[!TIP]
   >
   >Gehen Sie wie folgt vor, um einen projektübergreifenden Vorgänger hinzuzufügen:
   >
   >1. Klicken Sie auf das **Planmodus**-Symbol und wählen Sie **Automatisches Speichern**.
   >
   >1. Geben Sie die Referenznummer des Projekts des Vorgängers ein, gefolgt von einem Doppelpunkt und der Nummer der Aufgabe. Wenn Sie beispielsweise *765021:12* eingeben, wird die Referenznummer des Projekts des Vorgängers 765021 und der Vorgänger die Aufgabennummer 12 im Projekt.
   >
   >1. Fügen Sie den Abhängigkeitstyp für diesen Vorgänger hinzu. Weitere Informationen finden Sie unter [Erstellen von projektübergreifenden Vorgängern](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >1. Drücken Sie **ENTER**.
   >
   >**WICHTIG**
   >
   >Sie können keinen projektübergreifenden Vorgänger hinzufügen, wenn die Aufgabenliste im manuellen Speichermodus angezeigt wird.

   Das Symbol Vorgänger wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe arbeitsbereit ist.

   Weitere Informationen zu den in der Spalte „Vorgänger“ verfügbaren Beziehungstypen finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Anzeigen von Vorgängerdetails

Details zum Vorgänger können schnell in der Aufgabenliste angezeigt werden.

1. Bewegen Sie in der Aufgabenliste den Mauszeiger über die Vorgängernummer in der Spalte **Vorgänger**. Ein Feld mit den Vorgängerdetails wird angezeigt.

   ![Vorgängerdetails](assets/predecessor-details-in-task-list.png)

   Die folgenden Details werden angezeigt:

   **Name des Vorgängers:** Der Name des Vorgängers, auf den verwiesen wird. Die Aufgabennummer des Vorgängers ist enthalten. Klicken Sie auf den Aufgabennamen, um ihn zu öffnen.

   **Projektname:** Der Name des Projekts, in dem sich der Vorgänger befindet. Das Projekt wird als aktuelles Projekt identifiziert, wenn der Vorgänger zu denselben Projekten wie die Aufgabe gehört, oder als Kreuzprojekt, wenn der Vorgänger zu einem anderen Projekt gehört. Weitere Informationen zu projektübergreifenden Vorgängern finden Sie unter [Erstellen von projektübergreifenden Vorgängern](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Sie können die Projektdetails erweitern, um das geplante Start- und Enddatum des Projekts, die Bedingung, den Status, den abgeschlossenen Prozentsatz und den Eigentümer anzuzeigen. Bei einem projektübergreifenden Projekt können Sie dann auf **Projekt anzeigen** klicken, um das Projekt zu öffnen.

   **ID:** Die Referenznummer des Projekts, in dem sich der Vorgänger befindet.

   **Geplanter Start:** Das geplante Startdatum der Vorgängeraufgabe.

   **Geplantes Ende:** Das geplante Abschlussdatum der Vorgängeraufgabe.

   **Anzahl der Vorgänger:** Die Anzahl der Vorgänger für den Vorgänger, auf den verwiesen wird.

   **Anzahl der Nachfolger:** Die Anzahl der Nachfolger (oder abhängigen) Aufgaben für den Vorgänger, auf den verwiesen wird.
