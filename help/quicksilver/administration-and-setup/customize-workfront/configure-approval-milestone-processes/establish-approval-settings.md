---
title: Konfigurieren der globalen Genehmigungseinstellungen
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als Adobe Workfront-Administrator können Sie die globalen Einstellungen für Genehmigungsprozesse in Workfront festlegen. Diese Einstellungen wirken sich auf alle Arbeitselementgenehmigungsprozesse in Ihrem System aus.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
TQID: https://experienceleague.adobe.com/PQtVOIc3szHch0vLX3Lqn-PDCvYeXUXZWmF1enuICeY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 835
ht-degree: 8%

---

# Konfigurieren der globalen Validierungseinstellungen

Als Adobe Workfront-Administrator können Sie die globalen Einstellungen für Genehmigungsprozesse in Workfront festlegen. Diese Einstellungen wirken sich auf alle Arbeitselementgenehmigungsprozesse in Ihrem System aus.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Plan</p>
   <p>Standard<p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen entweder Systemadministrator sein oder über eine Planlizenz mit administrativem Zugriff auf Genehmigungsprozesse verfügen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Konfigurieren der globalen Validierungseinstellungen

{{step-1-to-setup}}

1. Klicken Sie **Prozesse** > **Genehmigungen**.

1. Klicken Sie auf **Einstellungen**-Symbol ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png) neben dem Bereichsnamen **Genehmigungen**.

1. Geben **im daraufhin angezeigten** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fügen Sie &lt;number&gt; Tage zum geplanten Abschlussdatum hinzu, um Genehmigungsprozesse zu berücksichtigen</td> 
      <td> <p>Geben Sie die Anzahl der Minuten, Stunden, Tage, Wochen oder Monate an, um Zeit zum geplanten Abschlussdatum der Aufgabe hinzuzufügen, die genehmigt werden muss. Wählen Sie „Verstrichene“ Minuten, Stunden, Tage oder Wochen aus, um die Zeit hinzuzufügen, die alle Wochenenden, Feiertage und arbeitsfreien Stunden enthält, die im Systemarbeitszeitplan-Kalender angegeben wurden.</p> 
      <p>Wenn beispielsweise eine Aufgabe am Freitag zugewiesen wurde und eine Dauer von 3 verstrichenen Tagen hat, wird das Abschlussdatum der Aufgabe auf Montag festgelegt (unter der Annahme, dass Samstag und Sonntag ein Wochenende ist). Wenn die Aufgabe eine Dauer von 3 Tagen hat (nicht abgelaufen), wird das Abschlussdatum der Aufgabe auf Mittwoch festgelegt.</p>
      <p><b>HINWEIS</b>: Wenn Sie zusätzliche Zeit für die Genehmigung von Aufgaben hinzufügen, wirkt sich dies auf die Zeitleiste der Aufgabe und des Projekts aus.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigende Person muss nicht Mitglied des Projektteams sein (für Genehmigungsprozesse, die eine Rolle beinhalten)</td> 
      <td> <p>Wählen Sie diese Option aus, wenn eine genehmigende Person nicht dem Projektteam angehören muss, wenn ein Genehmigungsprozess eine Rolle beinhaltet. Jeder Benutzer mit diesem Aufgabengebiet erhält die Genehmigungsanfrage, unabhängig davon, ob er zum Projektteam gehört oder nicht, obwohl ihm nicht automatisch Zugriff auf das Projekt gewährt wird. Informationen zum Bearbeiten der Projektrolle eines Benutzers finden Sie unter <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Verwalten des Projektteams</a>. </p> 
      <p><b>TIPP</b>: Wenn Sie eine Genehmigung einer Funktion zuweisen und die Option <b>Genehmigende Person muss nicht dem Projektteam angehören (für Genehmigungsprozesse, die eine Funktion beinhalten)</b> deaktiviert ist, aber es gibt keine Funktionen im Projektteam, die mit der Funktion in der Genehmigung übereinstimmen, wird die Genehmigung dem Projektbesitzer neu zugewiesen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsdelegierung deaktivieren</td> 
      <td> <p>Wählen Sie diese Option aus, um die Funktion für Benutzer in Ihrem System zu deaktivieren, Genehmigungen an andere Benutzer zu delegieren. Wenn diese Option ausgewählt ist, wird die Option zum Delegieren von Genehmigungen aus Workfront entfernt und alle vorhandenen Genehmigungsdelegierungen werden gestoppt.</p> <p>Weitere Informationen zum Delegieren von Genehmigungen in Workfront finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegieren von Genehmigungsanfragen</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zulassen, dass das benutzerdefinierte Formular bearbeitet werden kann, wenn das Projekt, die Aufgabe oder das Problem den Status „Ausstehende Genehmigung“ aufweist</td> 
      <td> <p>Wählen Sie diese Option aus, damit Benutzer das benutzerdefinierte Formular von Projekten, Aufgaben und Problemen bearbeiten können, wenn sie sich im Status Ausstehende Genehmigung befinden. Dies ist die Standardeinstellung.</p> 
      <p>Wenn diese Option ausgewählt ist:</p> 
       <ul> 
       <li>Alle genehmigenden Personen (und alle anderen Benutzenden, die Zugriff zum Bearbeiten des benutzerdefinierten Formulars haben) können Änderungen am benutzerdefinierten Formular vornehmen, wenn die Genehmigung für das Objekt aussteht, unabhängig vom aktuellen Genehmigungspfad oder Genehmigungsschritt.</li> 
       <li>Änderungen, die während eines Genehmigungsprozesses am benutzerdefinierten Formular vorgenommen werden, wirken sich nicht auf Genehmigungsentscheidungen aus, die vor der Änderung getroffen wurden.</li> 
       <li> <p>Alle Änderungen am Projekt, an der Aufgabe oder am Problem werden unabhängig von dieser Einstellung auf die gleiche Weise verfolgt. </p> <p>Wenn Sie beispielsweise benutzerdefinierte Formularfelder hinzugefügt haben, die im Aktualisierungsverlauf verfolgt werden sollen, werden alle Änderungen am Formular im Aktualisierungsverlauf des Objekts verfolgt.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzern ermöglichen, neu erstellte Anforderungen mit ausstehender Genehmigung zurückzurufen</td> 
      <td> <p>Wählen Sie diese Option aus, um zu konfigurieren, ob Benutzer ein Problem zurückrufen oder eine Anfrage mit ausstehender Genehmigung für ihren ersten Status stellen können. Sie können den ersten Status eines Problems oder einer Anfrage mit einem Genehmigungsprozess verknüpfen, indem Sie Anforderungswarteschlangen konfigurieren. </p> 
      <p>Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>.</p> 
      <p>Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
       <li>Wählen Sie diese Option aus, damit Benutzer eine Genehmigung für den ersten Status eines Problems oder einer Anfrage zurückrufen können. In diesem Fall wird eine Rückruf&lt;-Schaltfläche für ein neues Problem oder eine Anfrage mit dem Status „Genehmigung steht aus“ angezeigt. Wenn er/sie sich dafür entscheidet, das Problem zurückzurufen, erhält er/sie eine Warnung, dass das Problem ebenfalls gelöscht wird. Das Problem wird gelöscht, nachdem der Abruf bestätigt wurde. </li> 
       <li> <p>Deaktivieren Sie diese Option, um zu verhindern, dass Benutzer ein Problem oder eine Anfrage mit dem ersten Status „Genehmigung ausstehend“ zurückrufen. Für das neue Problem oder die neue Anfrage wird keine Rückruf&lt;-Schaltfläche angezeigt und die Genehmigung muss erteilt werden. Dies ist die Standardoption.</p> 
       <p>Weitere Informationen zur Überprüfung von Elementen, die auf eine Genehmigung warten, finden Sie unter <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Genehmigungen anzeigen </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Änderungen speichern.**
