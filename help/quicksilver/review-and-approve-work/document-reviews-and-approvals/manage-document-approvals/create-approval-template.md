---
product-area: documents
navigation-topic: approvals
title: Erstellen einer Validierungs-Workflow-Vorlage für Dokumente
description: Sie können Validierungsvorlagen erstellen, um Ihren Validierungsprozess zu optimieren.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jsEcIKopi-lJOSXQitDnufu3j0AmkWkPmCXtCR0V6nk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5e9318366f0dff85591a5d5a752920027f5c9b0e
workflow-type: tm+mt
source-wordcount: 895
ht-degree: 5%

---

# Erstellen einer Validierungs-Workflow-Vorlage für Dokumente

{{highlighted-preview}}

Im Bereich Workfront Setup können Benutzende mit einer Standardlizenz wiederverwendbare Genehmigungsvorlagen erstellen. Nach der Erstellung können Validierungsvorlagen auf Assets im Dokumentbereich eines Objekts angewendet werden.
>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt &#x200B;](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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

## Erstellen einer Validierungsvorlage in der Produktionsumgebung

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

<div class="preview">

## Erstellen einer Validierungsvorlage in der Vorschau

Das Dialogfeld für die Validierungsvorlage wird immer im erweiterten Modus geöffnet. Es gibt keinen Standardmodus für Vorlagen. Sie können bis zu 30 parallele Pfade in einer Vorlage mit insgesamt bis zu 100 Phasen konfigurieren. Jeder Pfad wird unabhängig voneinander ausgeführt und kann eine oder mehrere sequenzielle Phasen enthalten.

So erstellen Sie eine Validierungsvorlage:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Überprüfen und**) > **Genehmigungsvorlagen**.

1. Klicken **rechts auf** Seite auf „Neue Vorlage“.

1. Fügen Sie einen **Vorlagennamen“**.

1. Füllen Sie die Details für Schritt 1 von Pfad 1 aus:

   <table>
   <tr>
   <td><strong>Name der Phase</strong></td>
   <td>Stadien werden standardmäßig <em>Stadium 1</em>, <em>Stadium 2</em> usw. benannt. Benennen Sie die Phase in eine aussagekräftigere Bezeichnung um, z. B<em> „Erstprüfung</em> oder "<em> Genehmigung</em>.</td>
   </tr>
   <tr>
   <td><strong>Namen oder E-Mails hinzufügen (optional)</strong></td>
   <td>Beginnen Sie mit der Eingabe eines Benutzer- oder Team-Namens, der als genehmigende Person oder Prüfende Person hinzugefügt werden soll. Die Teilnehmer sind in Vorlagen optional. Sie können sie hinzufügen, wenn die Vorlage auf ein Dokument angewendet wird.<p>Hinweis: Ein Reviewer oder eine genehmigende Person kann jeweils nur einem offenen Schritt im selben Asset zugewiesen werden. Wenn mehrere parallele Stadien gleichzeitig geöffnet sind, kann dieselbe Person nicht zu mehr als einer hinzugefügt werden.</p></td>
   </tr>
   <tr>
   <td><strong>Nur eine Entscheidung erforderlich (optional)</strong></td>
   <td>Die erste Person, die eine Entscheidung trifft, schließt die Phase ab.</td>
   </tr>
   <tr>
   <td><strong>Tage bis Fälligkeitsdatum (optional)</strong></td>
   <td>Wählen Sie aus, wie viele Arbeitstage die Phase nach dem Öffnen benötigen soll. Die erste Phase jedes Pfads unterstützt auch ein absolutes Fälligkeitsdatum. Jede nachfolgende Phase im Pfad unterstützt nur ein relatives Fälligkeitsdatum.</td>
   </tr>
   <tr>
   <td><strong>Benutzerdefinierte Nachricht hinzufügen (optional)</strong></td>
   <td>Geben Sie eine Nachricht in das Textfeld <strong>Benutzerdefinierte Nachricht hinzufügen</strong> ein. Wenn die Vorlage auf ein Dokument angewendet wird, wird die Nachricht in der E-Mail-Benachrichtigung zur Genehmigung und auf der Registerkarte Genehmigungen in Workfront angezeigt.<p>Wenn Sie ein zweites Stadium hinzufügen<strong> wird „Diese Nachricht auf allen Stadien anzeigen</strong> standardmäßig ausgewählt. Lassen Sie die Option aktiviert, damit in jedem Schritt dieselbe Nachricht verwendet wird. Um für jede Phase eine andere Nachricht zu verwenden, deaktivieren Sie <strong>Diese Nachricht in allen Phasen anzeigen</strong> und geben Sie dann die phasenspezifische Nachricht in das Textfeld <strong>Benutzerdefinierte Nachricht hinzufügen</strong> für jede Phase ein.</p></td>
   </tr>
   </table>

   ![Phase hinzufügen](assets/add-stage.png)

1. (Optional) Klicken Sie auf **Phase hinzufügen**, um dem Pfad eine weitere Phase hinzuzufügen. Die Phasen innerhalb eines Pfads werden nacheinander in der angegebenen Reihenfolge ausgeführt. Wenn alle erforderlichen Entscheidungen in einer Phase getroffen werden, beginnt die nächste Phase in diesem Pfad und die vorherige Phase wird gesperrt. Sie können Stadien innerhalb eines Pfads neu anordnen, aber Sie können eine Phase nicht von einem Pfad in einen anderen verschieben. Jeder Pfad kann eine andere Anzahl von Phasen aufweisen.

1. (Optional) Klicken Sie unter **Parallele Pfade** auf **Pfad hinzufügen**, um einen weiteren Pfad hinzuzufügen. Der neue Pfad beginnt mit einem leeren Schritt und wird zum ausgewählten Pfad. Pfade können nicht neu angeordnet werden.

   ![Parallele Pfade hinzufügen](assets/add-path.png)

1. (Optional) Um einen Pfad umzubenennen, bewegen Sie den Mauszeiger über die Pfadbeschriftung, klicken Sie auf das Stiftsymbol und geben Sie dann einen neuen Namen ein. Um einen Pfad zu entfernen, bewegen Sie den Mauszeiger über die Pfadbeschriftung und klicken Sie auf das Papierkorbsymbol. **Pfad 1** kann nicht entfernt werden, und andere Pfade können nur entfernt werden, wenn kein Schritt innerhalb des Pfads gesperrt oder abgeschlossen ist.

1. (Optional) Um alle Pfade und Phasen zu löschen und von vorne zu beginnen, klicken **oben** auf „Zurücksetzen“.

1. Klicken Sie auf **Speichern**.

Nachdem die Vorlage erstellt wurde, kann sie auf Dokumente im Bereich Dokumente eines Objekts angewendet werden, um den formalen Prüfungs- und Genehmigungsprozess in Workfront zu starten.

</div>



<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
