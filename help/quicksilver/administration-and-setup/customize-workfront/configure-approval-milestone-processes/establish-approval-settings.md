---
title: Globale Genehmigungseinstellungen konfigurieren
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als Adobe Workfront-Administrator können Sie die globalen Einstellungen für Genehmigungsprozesse in Workfront festlegen. Diese Einstellungen wirken sich auf alle Prozesse zur Genehmigung von Arbeitselementen in Ihrem System aus.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 1%

---

# Globale Genehmigungseinstellungen konfigurieren

Als Adobe Workfront-Administrator können Sie die globalen Einstellungen für Genehmigungsprozesse in Workfront festlegen. Diese Einstellungen wirken sich auf alle Prozesse zur Genehmigung von Arbeitselementen in Ihrem System aus.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen entweder Systemadministrator sein oder über eine Planungslizenz mit Administratorzugriff auf Genehmigungsprozesse verfügen.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Globale Genehmigungseinstellungen konfigurieren

1. Melden Sie sich bei Workfront als Workfront-Administrator an.
1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Prozesse** > **Genehmigungen** .

1. Klicken Sie auf das Symbol **Einstellungen** ![](assets/gear-icon-settings.png) neben dem Bereichsnamen **Genehmigungen**.

1. Geben Sie im angezeigten Feld **Genehmigungseinstellungen** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fügen Sie dem geplanten Abschlussdatum &lt;Zahl&gt; Tage hinzu, um Genehmigungsprozesse zu ermöglichen.</td> 
      <td> <p>Geben Sie die Anzahl der Minuten, Stunden, Tage, Wochen oder Monate an, um dem geplanten Abschlussdatum der Aufgabe, für die eine Genehmigung erforderlich ist, Zeit hinzuzufügen. Wählen Sie "Verstrichene"Minuten, Stunden, Tage oder Wochen aus, um Zeit hinzuzufügen, die alle im Kalender des Systemarbeitszeitplans festgelegten Wochenenden, Feiertage und Arbeitsstunden umfasst.</p> 
      <p>Wenn beispielsweise eine Aufgabe am Freitag zugewiesen wird und eine Dauer von 3 verstrichenen Tagen hat, wird das Datum für die Aufgabenfertigstellung auf Montag gesetzt (vorausgesetzt Samstag und Sonntag sind Wochenende). Wenn die Aufgabe eine Dauer von 3 Tagen hat (nicht verstrichen), wird das Datum für den Abschluss der Aufgabe auf Mittwoch festgelegt.</p>
      <p><b>HINWEIS</b>: Wenn Sie das Hinzufügen zusätzlicher Zeit aktivieren, um die Genehmigung für Aufgaben aufzunehmen, wirkt sich dies auf den Zeitrahmen der Aufgabe und des Projekts aus.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmiger muss nicht im Projektteam sein (für Genehmigungsprozesse, die eine Rolle enthalten)</td> 
      <td> <p>Wählen Sie diese Option aus, wenn ein Genehmiger nicht im Projektteam sein muss, wenn ein Genehmigungsprozess eine Rolle enthält. Bei der Zuweisung der Genehmigungsentscheidung zu einer Auftragsrolle wird nur Benutzern, denen eine Rolle im Projekt zugeordnet ist, die Genehmigung angezeigt. Wenn Sie diese Einstellung aktivieren, erhält jeder Benutzer mit dieser Auftragsrolle die Genehmigungsanfrage, unabhängig davon, ob er sich im Projektteam befindet oder nicht. Informationen zum Bearbeiten der Projektrolle eines Benutzers finden Sie unter <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Verwalten des Projektteams</a>. </p> 
      <p><b>TIPP</b>: Wenn Sie einer Rolle eine Genehmigung zuweisen und die Option "<b>Genehmiger nicht im Projektteam sein muss (für Genehmigungsprozesse, die eine Rolle enthalten)</b>"deaktiviert ist, es jedoch keine Rollen im Projektteam gibt, die mit der Rolle in der Genehmigung übereinstimmen, wird die Genehmigung dem Projekteigentümer neu zugewiesen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsdelegierung deaktivieren</td> 
      <td> <p>Wählen Sie diese Option aus, um die Funktionalität zu deaktivieren, mit der Benutzer in Ihrem System Genehmigungen an einen anderen Benutzer delegieren können. Wenn diese Option aktiviert ist, wird die Option zum Delegieren von Genehmigungen aus Workfront entfernt und alle vorhandenen Genehmigungsdelegationen werden angehalten.</p> <p>Weitere Informationen zum Delegieren von Genehmigungen in Workfront finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Genehmigungsanfrage delegieren</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zulassen Die Bearbeitung des benutzerdefinierten Formulars, wenn das Projekt, die Aufgabe oder das Problem den Status "Genehmigung ausstehend"aufweist</td> 
      <td> <p>Wählen Sie diese Option, damit Benutzer das benutzerdefinierte Formular von Projekten, Aufgaben und Problemen im Status Ausstehende Genehmigung bearbeiten können. Dies ist die Standardeinstellung.</p> 
      <p>Wenn diese Option ausgewählt ist:</p> 
       <ul> 
       <li>Alle Genehmiger (und alle anderen Benutzer, die Zugriff auf die Bearbeitung des benutzerdefinierten Formulars haben) können Änderungen am benutzerdefinierten Formular vornehmen, wenn die Genehmigung des Objekts aussteht, unabhängig vom aktuellen Genehmigungspfad oder Genehmigungsschritt.</li> 
       <li>Änderungen am benutzerdefinierten Formular während eines Genehmigungsprozesses wirken sich nicht auf Genehmigungsentscheidungen aus, die vor der Änderung vorgenommen wurden.</li> 
       <li> <p>Änderungen am Projekt, an der Aufgabe oder am Problem werden unabhängig von dieser Einstellung auf die gleiche Weise verfolgt. </p> <p>Wenn Sie beispielsweise benutzerdefinierte Formularfelder hinzugefügt haben, die im Aktualisierungsstream verfolgt werden sollen, werden alle Änderungen am Formular im Aktualisierungsstream des Objekts verfolgt.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzern ermöglichen, neu erstellte Anforderungen mit ausstehender Genehmigung zurückzurufen</td> 
      <td> <p>Wählen Sie diese Option, um zu konfigurieren, ob Benutzer sich an ein Problem erinnern können oder eine Anfrage bis zur Genehmigung für ihren ersten Status ausstehen. Sie können den ersten Status eines Problems oder einer Anfrage mit einem Genehmigungsprozess verknüpfen, indem Sie Anforderungswarteschlangen konfigurieren. </p> 
      <p>Weitere Informationen zu Anforderungswarteschlangen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>.</p> 
      <p>Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
       <li>Aktivieren Sie diese Option, damit Benutzer eine Genehmigung für den ersten Status eines Problems oder einer Anfrage zurückrufen können. In diesem Fall wird ihnen die Schaltfläche Recall&lt; zu einem neuen Problem oder einer Anfrage angezeigt, die noch nicht genehmigt wurde. Wenn sie sich dafür entscheiden, das Problem erneut aufzudecken, erhalten sie eine Warnung, dass das Problem ebenfalls gelöscht wird. Das Problem wird gelöscht, nachdem der Benutzer seine Erinnerung bestätigt hat. </li> 
       <li> <p>Deaktivieren Sie diese Option, um zu verhindern, dass Benutzer ein Problem oder eine Anfrage erneut aufrufen, deren erster Status auf die Genehmigung wartet. Sie können die Schaltfläche Recall&lt; für das neue Problem oder die neue Anfrage nicht sehen. Die Genehmigung muss erteilt werden. Dies ist die Standardoption.</p> 
       <p>Weitere Informationen zum Überprüfen von Elementen, die auf die Genehmigung warten, finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Genehmigungen anzeigen </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Änderungen speichern.**
