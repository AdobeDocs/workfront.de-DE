---
product-area: projects
navigation-topic: use-predecessors
title: Erstellen projektübergreifender Vorgänger
description: Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (als Nachfolgeaufgabe bezeichnet) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Vorrang vor der abhängigen (Nachfolger-)Aufgabe hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe zuerst als Fertig gestellt markiert werden muss, bevor die abhängige Aufgabe beginnen kann.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Erstellen projektübergreifender Vorgänger

Ein projektübergreifender Vorgänger ist eine Aufgabe, von der eine andere Aufgabe (als Nachfolgeaufgabe bezeichnet) in einem anderen Projekt abhängt. Der Vorgänger ist die Aufgabe, die Vorrang vor der abhängigen (Nachfolger-)Aufgabe hat. Sie können beispielsweise eine Abhängigkeit erstellen, bei der die Vorgängeraufgabe zuerst als Fertig gestellt markiert werden muss, bevor die abhängige Aufgabe beginnen kann.

Wie Vorgänger innerhalb eines Projekts ermöglicht Adobe Workfront, dass Aufgaben von Aufgaben in anderen Projekten abhängig sind.

**BEISPIEL**

Wenn ein Baggerunternehmen nur über einen Backhoe verfügt und zwei gleichzeitige Projekte Aufgaben haben, die die Verwendung des Backhofs erfordern, kann der Projektmanager die Aufgabe im ersten Projekt von der Aufgabe im zweiten Projekt abhängig machen, um zu veranschaulichen, dass die Ausgrabung beginnen kann, wenn das vorherige Projekt den Hintergrund aufhebt.
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
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
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

1. Gehen Sie zu der Aufgabe, die Ihr Nachfolger sein wird.
1. Klicken **Vorgänger** im linken Bereich.
1. Klicken **Fügen Sie den Vorgänger hinzu.**
1. Im **Übergeordnetes Projekt** eingeben, beginnen Sie mit der Eingabe des Namens des Projekts, das die Aufgabe enthält, die von Ihrer aktuellen Aufgabe abhängig sein soll.
1. Klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Im **Aufgaben** eingeben, beginnen Sie mit der Eingabe des Namens der Aufgabe, die von der aktuellen Aufgabe abhängig sein soll.
1. Geben Sie die folgenden Informationen zum Definieren der Beziehung zwischen dem Vorgänger und der abhängigen Aufgabe an:

   * **Abhängigkeitstyp:** Wählen Sie die Beziehung aus, die die Aufgabe mit der abhängigen Aufgabe haben soll. Die Standardbeziehung lautet &quot;Finish-Start&quot;. Das bedeutet, dass die Vorgängeraufgabe beendet werden muss, bevor die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Abhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **Lag:** Geben Sie den Zeitraum an, der nach dem Abschluss eines erzwungenen Vorgängers verstreichen muss, bis die abhängige Aufgabe beginnen kann. Weitere Informationen zu den verschiedenen Arten von Verzögerungen finden Sie unter [Übersicht über die Lag-Typen](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Erzwungen:** Wenn diese Option aktiviert ist, kann die Abhängigkeitsbeziehung zwischen den beiden Aufgaben nicht umgangen werden, wenn Benutzer Aufgaben frühzeitig starten. Wenn Sie beispielsweise eine Beziehung zwischen Aufgabe A und Aufgabe B erzwingen, kann Aufgabe B erst gestartet werden, wenn Aufgabe A abgeschlossen ist. Weitere Informationen zur Durchsetzung von Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      Wenn diese Option nicht ausgewählt ist, wird die Abhängigkeit wie ein Vorschlag für Benutzer behandelt. Beispielsweise können Benutzer Aufgabe B starten, bevor Aufgabe A abgeschlossen ist.

1. Klicken Sie auf **Speichern**.

   Aufgaben mit einem projektübergreifenden Vorgänger zeigen die Referenznummer des Projekts an, zu dem der Vorgänger gehört, und die Nummer der Aufgabe, getrennt durch einen Doppelpunkt in der Spalte &quot;Vorgänger&quot;einer Aufgabenliste.

   ![Projektübergreifender Vorgänger](assets/cross-project-predecessor-in-list-view.png)

   Das Vorgängersymbol wird grün, wenn die Vorgängeraufgabe als abgeschlossen markiert ist. Dies signalisiert, dass die abhängige Aufgabe einsatzbereit ist.

   Bewegen Sie den Mauszeiger über diesen Wert, um weitere Informationen zum Vorgänger, zum Projekt und zu den Daten zu erhalten. Klicken Sie im Detailfeld auf den projektübergreifenden Vorgänger, um die Aufgabe zu öffnen. Klicken **Siehe Projekt** , um das Projekt zu öffnen.

   ![Projektübergreifende Vorgängerdetails](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   Die **Siehe Projekt** wird nur bei der Anzeige eines projektübergreifenden Vorgängers angezeigt.

