---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen projektübergreifender Vorgänger
description: Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (als Nachfolgeaufgabe bezeichnet) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Vorrang vor der abhängigen (Nachfolger-)Aufgabe hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe zuerst als Fertig gestellt markiert werden muss, bevor die abhängige Aufgabe beginnen kann.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Erstellen projektübergreifender Vorgänger

<!--Audited: 12/2023-->

Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (als Nachfolgeaufgabe bezeichnet) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Vorrang vor der abhängigen (Nachfolger-)Aufgabe hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe zuerst als Fertig gestellt markiert werden muss, bevor die abhängige Aufgabe beginnen kann.

Adobe Workfront ermöglicht es, Aufgaben von Aufgaben in anderen Projekten abhängig zu machen, so wie es Vorgänger in einem einzelnen Projekt ermöglicht.

>[!INFO]
>
>So verfügt beispielsweise ein Grabunternehmen nur über einen Hintergrund und zwei Projekte haben Aufgaben, die die Verwendung des Backhofs erfordern. Der Projektmanager kann die Aufgabe im ersten Projekt als Vorgänger der Aufgabe im zweiten Projekt festlegen. Dies zeigt, dass das zweite Projekt mit der Verwendung des Backhofs beginnen kann, wenn das erste Projekt damit fertig ist.

Bei der Verknüpfung von Projekten über projektübergreifende Vorläufer wirken sich die Daten des Primärprojekts (das Datum, an dem die Vorgängeraufgabe erfolgt) auf das sekundäre Projekt aus (das Projekt, das die Nachfolgeaufgabe hat).

>[!TIP]
>
>Sie müssen die Zeitpläne für die Projekte neu berechnen, damit die Daten für das sekundäre Projekt aktualisiert werden. Weitere Informationen zur Neuberechnung von Zeitleisten finden Sie unter [Konfigurieren von Timeline-Neuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Weitere Informationen zu Vorgängerbeziehungen finden Sie unter [Übersicht über Aufgabenvorherigen](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard </p> 
   Oder
   <p>Aktuell: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben und Projekte verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines projektübergreifenden Vorgängers

1. Wechseln Sie zu der Aufgabe, die Ihr Nachfolger ist (abhängige Aufgabe).
1. Klicken Sie im linken Bereich auf **Vorgänger** .
1. Klicken Sie auf **Vorgänger hinzufügen**.
1. Geben Sie im Feld **Übergeordnetes Projekt** den Namen des Projekts ein, das die Aufgabe enthält, die Sie der aktuellen Aufgabe voranstellen möchten.
1. Klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Geben Sie im Feld **Aufgaben** den Namen der Aufgabe ein, die der Vorgänger der aktuellen Aufgabe sein soll.
1. Geben Sie die folgenden Informationen zum Definieren der Beziehung zwischen dem Vorgänger und der abhängigen Aufgabe an:

   * **Abhängigkeitstyp:** Wählen Sie die Beziehung aus, die die Vorgängeraufgabe mit der abhängigen Aufgabe haben soll. Die Standardbeziehung lautet &quot;Finish-Start&quot;. Das bedeutet, dass die Vorgängeraufgabe beendet werden muss, bevor die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **lange:** Geben Sie die Zeit an, die nach Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Arten von Verzögerung finden Sie unter [Übersicht über die Lag-Typen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Erzwungen:** Wenn diese Option ausgewählt ist, kann die Abhängigkeitsbeziehung zwischen den beiden Aufgaben nicht umgangen werden, indem Benutzer Aufgaben frühzeitig starten. Wenn Sie beispielsweise eine Beziehung zwischen Aufgabe A und Aufgabe B erzwingen, kann Aufgabe B erst gestartet werden, wenn Aufgabe A abgeschlossen ist. Weitere Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Wenn diese Option nicht ausgewählt ist, wird die Abhängigkeit wie ein Vorschlag für Benutzer behandelt. Beispielsweise können Benutzer Aufgabe B starten, bevor Aufgabe A abgeschlossen ist.

1. Klicken Sie auf **Speichern**.

   Aufgaben mit einem projektübergreifenden Vorgänger zeigen die Referenznummer des Projekts an, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, durch einen Doppelpunkt getrennt, in der Spalte &quot;Vorgänger&quot;einer Aufgabenliste an.

   ![Projektübergreifender Vorgänger](assets/cross-project-predecessor-in-list-view.png)

   Das Vorgängersymbol wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe einsatzbereit ist.

   Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen zum Vorgänger, zum Projekt und zu den Daten zu erhalten. Klicken Sie im Detailfeld auf den projektübergreifenden Vorgänger, um die Aufgabe zu öffnen.

   Klicken Sie oben im Mauszeiger-Fenster auf , um weitere Informationen zum Projekt des Vorgängers anzuzeigen.

   Klicken Sie auf **Siehe Projekt** , um das Projekt des Vorgängers zu öffnen.

   ![Projektübergreifende Vorgängerdetails](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Die Option **Siehe Projekt** wird nur angezeigt, wenn ein projektübergreifender Vorgänger angezeigt wird.

