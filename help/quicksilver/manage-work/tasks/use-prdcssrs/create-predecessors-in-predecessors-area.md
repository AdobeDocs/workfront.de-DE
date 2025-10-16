---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen einer Vorgängerbeziehung mithilfe des Bereichs „Vorgänger“
description: Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 1%

---

# Erstellen einer Vorgängerbeziehung mithilfe des Bereichs „Vorgänger“

<!-- Audited: 5/2025 -->

Sie können Vorgängeraufgaben (oder nur Vorgänger) verwenden, um Aufgaben, die von anderen Aufgaben abhängig sind, zu verknüpfen, um sie zu starten oder abzuschließen. Sie möchten beispielsweise keine Party (abhängige Aufgabe) hosten, bevor Sie die Einladungen senden (Vorgängeraufgabe).

Dieser Artikel zeigt, wie Sie in einer Aufgabe mithilfe der Registerkarte Vorgänger Vorgänger Vorgänger festlegen können.

Informationen zum Festlegen von Vorgängern in einer Aufgabenliste finden Sie unter [Erstellen einer Vorgängerbeziehung in der Aufgabenliste](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Sie können die Vorgänger von Aufgaben in den folgenden Bereichen von Adobe Workfront anzeigen:

* Im Abschnitt Vorgänger der abhängigen Aufgaben
* Im Gantt-Diagramm
* In der Aufgabenliste in der Spalte Vorgänger

Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

## Vorgänger für eine Aufgabe erstellen

Das Erstellen eines Vorgängers für eine Projektaufgabe mithilfe des Bereichs Vorgänger ähnelt dem Erstellen von Vorgängern für eine Vorlagenaufgabe in einer Vorlage.

Erstellen einer Vorgängeraufgabe für eine Projektaufgabe:

1. Navigieren Sie zu der Aufgabe, die Sie als abhängige Aufgabe festlegen möchten.

1. Klicken Sie im linken Bedienfeld auf **Vorgänger**.

1. Klicken Sie im Abschnitt **Vorgänger** auf **Vorgänger hinzufügen**. Das **Vorgänger hinzufügen** wird geöffnet.

1. (Optional) Um einen projektübergreifenden Vorgänger hinzuzufügen, ersetzen Sie den Namen des Projekts im Feld **Übergeordnetes Projekt** durch ein anderes Projekt.

   Weitere Informationen finden Sie [Erstellen von projektübergreifenden Vorgängern](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >Sie können keine vorlagenübergreifenden Vorgänger für Vorlagenaufgaben erstellen.


1. Geben Sie im Feld **Aufgaben** den Namen der Aufgabe(n) ein, die Sie als Vorgänger festlegen möchten, und wählen Sie sie aus, wenn sie in der Dropdown-Liste angezeigt werden.

1. Wählen Sie einen **Abhängigkeitstyp** aus.

   Weitere Informationen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Geben Sie einen **Verzögerung** Betrag ein.

   Weitere Informationen finden Sie unter &#x200B;[Übersicht über Verzögerungstypen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Dialogfeld „Vorgänger hinzufügen“](assets/add-predecessor-dialog-box.png)

1. Aktivieren Sie **Kontrollkästchen** Erzwungen“, wenn Sie die Vorgängerbeziehung zwischen den beiden Aufgaben erzwingen möchten.

   Weitere Informationen finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Klicken Sie auf **Speichern**.

1. (Optional) Um einen Vorgänger zu entfernen, wählen Sie ihn aus der Liste der Vorgänger aus und klicken Sie dann auf das **Entfernen**-Symbol ![Entfernen](assets/remove-or-delete-icon.png).

   Der Vorgänger wird aus der Liste entfernt. Die Vorgängeraufgabe wird nicht aus ihrem Projekt gelöscht.
