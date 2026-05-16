---
product-area: documents
navigation-topic: approvals
title: Erstellen einer Validierungs-Workflow-Vorlage für Dokumente
description: Sie können Validierungsvorlagen erstellen, um Ihren Validierungsprozess zu optimieren.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 13%

---

# Erstellen einer Validierungs-Workflow-Vorlage für Dokumente

Im Bereich Workfront Setup können Benutzende mit einer Standardlizenz wiederverwendbare Genehmigungsvorlagen erstellen. Nach der Erstellung können Validierungsvorlagen auf Assets im Dokumentbereich eines Objekts angewendet werden.
>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Jedes Workfront-Paket zur Verwaltung von Genehmigungen unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Abo</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
ß

## Erstellen einer Validierungsvorlage

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Überprüfen und**) > **Genehmigungsvorlagen**.
1. Klicken **rechts auf** Seite auf „Neue Vorlage“.

1. Füllen Sie die folgenden Details aus:

   <table>
     <tr>
   <td><strong>Vorlagenname</strong></td>
   <td>Fügen Sie einen Vorlagennamen hinzu. </td>
   </tr>
   <tr>
   <td><strong>Name der Phase</strong></td>
   <td>Einen Namen für das Stadium hinzufügen. Sie können den Namen in einen aussagekräftigeren Namen ändern, z. B<em> „Erstprüfung</em> oder "<em> Genehmigung</em>.</td>
   </tr>
   <tr>
   <td><strong>Namen oder E-Mails hinzufügen</strong></td>
   <td>Beginnen Sie mit der Eingabe eines Benutzer- oder Team-Namens, der als genehmigende Person oder Prüfende Person hinzugefügt werden soll. Wenn Sie nur über Validierungsverantwortliche verfügen, werden diese benachrichtigt und haben die Möglichkeit, die Überprüfung abzuschließen. Es ist jedoch keine Entscheidung erforderlich oder getroffen.</td>
   </tr>
   <tr>
   <td><strong>Eine Entscheidung erforderlich (optional)</strong></td>
   <td>Die erste Person, die eine Entscheidung trifft, schließt die Phase ab.</td>
   </tr>
   <tr>
   <td><strong>Werktage bis Fälligkeitsdatum</strong></td>
   <td>Wählen Sie aus, wie viele Arbeitstage nach der Aktivierung eines Stadiums bis zur fälligen Genehmigung verbleiben.</td>
   </tr>
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Schritte nach Bedarf hinzuzufügen.

   >[!NOTE]
   >
   >Wenn Sie mehrere Phasen hinzufügen, wird der Genehmigungs-Workflow in der Reihenfolge fortgesetzt, in der die Phasen aufgelistet sind. Wenn alle erforderlichen Entscheidungen getroffen werden, beginnt die nächste Phase und die vorherige Phase wird gesperrt.

   ![Dokumentdetails](assets/new-stage.png)

1. Klicken Sie auf **Speichern**.

Nachdem die Vorlage erstellt wurde, kann sie auf Dokumente im Bereich Dokumente eines Objekts angewendet werden, um den formalen Prüfungs- und Genehmigungsprozess in Workfront zu starten.



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
