---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen von projektübergreifenden Vorgängern
description: Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (eine so genannte Nachfolgeaufgabe) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Priorität vor der abhängigen Aufgabe (Nachfolger) hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe als abgeschlossen markiert werden muss, bevor die abhängige Aufgabe gestartet werden kann.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Erstellen von projektübergreifenden Vorgängern

<!--Audited: 12/2024-->

Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (eine so genannte Nachfolgeaufgabe) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Priorität vor der abhängigen Aufgabe (Nachfolger) hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe als abgeschlossen markiert werden muss, bevor die abhängige Aufgabe gestartet werden kann.

Adobe Workfront ermöglicht es, dass Aufgaben von Aufgaben in anderen Projekten abhängig sind, genau wie es Vorgänger innerhalb eines einzigen Projekts ermöglicht.

>[!INFO]
>
>Beispielsweise verfügt ein Baggerunternehmen nur über einen Bagger, und zwei Projekte haben Aufgaben, die die Verwendung des Baggers erfordern. Der Projektmanager kann die Aufgabe im ersten Projekt zu einem Vorgänger der Aufgabe im zweiten Projekt machen. Dies zeigt, dass das zweite Projekt mit der Verwendung des Backhores beginnen kann, wenn das erste Projekt damit abgeschlossen ist.

Wenn Sie Projekte über projektübergreifende Vorgänger verknüpfen, wirken sich die Daten des primären Projekts (das mit der Vorgängeraufgabe) auf das sekundäre Projekt aus (das mit der Nachfolgeaufgabe).

>[!TIP]
>
>Sie müssen die Zeitleisten für die Projekte neu berechnen, damit die Daten für das sekundäre Projekt aktualisiert werden. Weitere Informationen zur Neuberechnung von Zeitleisten finden Sie unter [Konfigurieren von Zeitleisten-Neuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Weitere Informationen zu Vorgängerbeziehungen finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Standard </p>

<p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgaben und Projekte</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines projektübergreifenden Vorgängers

>[!TIP]
>
>Obwohl das Erstellen von Vorlagenaufgaben mit dem Erstellen von Vorlagenaufgaben-Vorgängern vergleichbar ist, können Sie keine vorlagenübergreifenden Vorgänger für Vorlagenaufgaben erstellen.


1. Wechseln Sie zu der Aufgabe, die Ihr Nachfolger sein wird (abhängige Aufgabe).
1. Klicken Sie **linken Bedienfeld auf** Vorgänger“.

   >[!TIP]
   >
   >   Ihr Workfront- oder Gruppenadministrator kann den Abschnitt **Vorgänger** oder andere Abschnitte aus dem linken Bedienfeld entfernen.

1. Klicken Sie auf **Vorgänger hinzufügen.**
1. Beginnen Sie **Feld Übergeordnetes Projekt** den Namen des Projekts einzugeben, das die Aufgabe enthält, deren Vorgänger Sie Ihrer aktuellen Aufgabe sein möchten.
1. Klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Beginnen Sie **Feld Aufgaben** mit der Eingabe des Namens der Aufgabe, die Sie als Vorgänger Ihrer aktuellen Aufgabe verwenden möchten.
1. Geben Sie die folgenden Informationen zum Definieren der Beziehung zwischen dem Vorgänger und der abhängigen Aufgabe an:


   * **Abhängigkeitstyp** Wählen Sie die Beziehung aus, die die Vorgängeraufgabe mit der abhängigen Aufgabe haben soll. Die Standardbeziehung ist „Beenden-Start“, was bedeutet, dass die Vorgängeraufgabe abgeschlossen sein muss, bevor die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Verzögerung** Geben Sie die Zeit an, die nach Abschluss eines erzwungenen Vorgängers vergehen muss, bis die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Verzögerungsarten finden Sie unter [Verzögerungsarten - Übersicht](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Erzwungen:** Wenn diese Option aktiviert ist, kann die Abhängigkeitsbeziehung zwischen den beiden Aufgaben nicht dadurch umgangen werden, dass Benutzer die Aufgaben frühzeitig beginnen. Wenn Sie beispielsweise eine Beziehung zwischen Aufgabe A und Aufgabe B erzwingen, kann Aufgabe B erst gestartet werden, wenn Aufgabe A abgeschlossen ist. Weitere Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Wenn diese Option nicht ausgewählt ist, wird die Abhängigkeit für die Benutzer wie ein Vorschlag behandelt. Beispielsweise können Benutzer Aufgabe B starten, bevor Aufgabe A abgeschlossen ist.

1. Klicken Sie auf **Speichern**.

   Aufgaben mit einem projektübergreifenden Vorgänger zeigen die Referenznummer des Projekts, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, getrennt durch einen Doppelpunkt, in der Spalte Vorgänger in einer Aufgabenliste an.

   ![Projektübergreifender Vorgänger](assets/cross-project-predecessor-in-list-view.png)

   Das Symbol Vorgänger wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe arbeitsbereit ist.

   Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen über den Vorgänger, das Projekt und die Daten zu erhalten. Klicken Sie auf den projektübergreifenden Vorgänger im Feld Details , um die Aufgabe zu öffnen.

   Klicken Sie oben im Fenster, um weitere Informationen zum Vorgängerprojekt anzuzeigen.

   Klicken Sie **Projekt anzeigen**, um das Projekt des Vorgängers zu öffnen.

   ![Projektübergreifende Vorgängerdetails](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Die Option **Projekt anzeigen** wird nur angezeigt, wenn ein projektübergreifender Vorgänger angezeigt wird.

