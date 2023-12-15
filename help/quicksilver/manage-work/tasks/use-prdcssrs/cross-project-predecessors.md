---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen projektübergreifender Vorgänger
description: Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (als Nachfolgeaufgabe bezeichnet) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Vorrang vor der abhängigen (Nachfolger-)Aufgabe hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe zuerst als Fertig gestellt markiert werden muss, bevor die abhängige Aufgabe beginnen kann.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '766'
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
>Sie müssen die Zeitpläne für die Projekte neu berechnen, damit die Daten für das sekundäre Projekt aktualisiert werden. Weitere Informationen zur Neuberechnung der Zeitpläne finden Sie unter [Konfigurieren von Timeline-Neuberechnungen für Projekte](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Weitere Informationen zu Vorgängerbeziehungen finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Zugriffsanforderungen

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
  <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
 </tr>   <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben und Projekte verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines projektübergreifenden Vorgängers

1. Wechseln Sie zu der Aufgabe, die Ihr Nachfolger ist (abhängige Aufgabe).
1. Klicks **Vorgänger** im linken Bereich.
1. Klicks **Add Predecessor.**
1. Im **Übergeordnetes Projekt** eingeben, beginnen Sie mit der Eingabe des Namens des Projekts, das die Aufgabe enthält, die Sie der aktuellen Aufgabe voranstellen möchten.
1. Klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Im **Aufgaben** eingeben, beginnen Sie mit der Eingabe des Namens der Aufgabe, die Sie der aktuellen Aufgabe voranstellen möchten.
1. Geben Sie die folgenden Informationen zum Definieren der Beziehung zwischen dem Vorgänger und der abhängigen Aufgabe an:

   * **Abhängigkeitstyp:** Wählen Sie die Beziehung aus, die die Vorgängeraufgabe mit der abhängigen Aufgabe haben soll. Die Standardbeziehung lautet &quot;Finish-Start&quot;. Das bedeutet, dass die Vorgängeraufgabe beendet werden muss, bevor die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Lag:** Geben Sie den Zeitraum an, der nach dem Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Arten von Verzögerungen finden Sie unter [Übersicht über die Lag-Typen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Erzwungen:** Wenn diese Option aktiviert ist, kann die Abhängigkeitsbeziehung zwischen den beiden Aufgaben nicht umgangen werden, wenn Benutzer Aufgaben frühzeitig starten. Wenn Sie beispielsweise eine Beziehung zwischen Aufgabe A und Aufgabe B erzwingen, kann Aufgabe B erst gestartet werden, wenn Aufgabe A abgeschlossen ist. Weitere Informationen zur Durchsetzung von Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Wenn diese Option nicht ausgewählt ist, wird die Abhängigkeit wie ein Vorschlag für Benutzer behandelt. Beispielsweise können Benutzer Aufgabe B starten, bevor Aufgabe A abgeschlossen ist.

1. Klicken Sie auf **Speichern**.

   Aufgaben mit einem projektübergreifenden Vorgänger zeigen die Referenznummer des Projekts an, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, durch einen Doppelpunkt getrennt, in der Spalte &quot;Vorgänger&quot;einer Aufgabenliste an.

   ![Projektübergreifender Vorgänger](assets/cross-project-predecessor-in-list-view.png)

   Das Vorgängersymbol wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe einsatzbereit ist.

   Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen zum Vorgänger, zum Projekt und zu den Daten zu erhalten. Klicken Sie im Detailfeld auf den projektübergreifenden Vorgänger, um die Aufgabe zu öffnen.

   Klicken Sie oben im Mauszeiger-Fenster auf , um weitere Informationen zum Projekt des Vorgängers anzuzeigen.

   Klicks **Siehe Projekt** , um das Projekt des Vorgängers zu öffnen.

   ![Projektübergreifende Vorgängerdetails](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Die **Siehe Projekt** wird nur bei der Anzeige eines projektübergreifenden Vorgängers angezeigt.

