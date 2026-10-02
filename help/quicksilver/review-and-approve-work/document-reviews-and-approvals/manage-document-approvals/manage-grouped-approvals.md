---
product-area: documents
navigation-topic: approvals
title: Gruppierte Genehmigungen verwalten
description: In einer gruppierten Genehmigung können Sie Teilnehmer und Assets hinzufügen oder entfernen, ohne den Workflow für den Rest der Gruppe zu unterbrechen.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8250a95bec88df91e3422c8da7c05ac802b3cb22
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 4%
---

# Gruppierte Genehmigungen verwalten

{{highlighted-preview-article-level}}

Bei einer gruppierten Genehmigung werden mehrere Assets in einem einzigen Genehmigungs-Workflow zusammengefasst, sodass alle Assets dieselben Phasen gemeinsam durchlaufen können, anstatt für jedes Asset eine separate Genehmigung erforderlich zu machen. Sie können Teilnehmer und Assets in einer aktiven gruppierten Genehmigung hinzufügen oder entfernen, ohne den Workflow neu zu erstellen.

Gruppierte Validierungen unterstützen den einfachen und erweiterten Modus, mehrere Phasen und parallele Pfade auf die gleiche Weise wie Genehmigungen für einzelne Assets. Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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
   <td> <p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td>
   <p>Mitwirkende oder höher</p>
   <p>Überprüfen oder höher</p>
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Konfigurationen der Zugriffsebene</td>
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objektberechtigungen</td>
   <td> <p>Verwalten des Zugriffs auf das mit der Anfrage oder Genehmigung verknüpfte Objekt</p></td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Hinzufügen von Teilnehmern zu einer aktiven gruppierten Genehmigung

Sie können einer gruppierten Genehmigung genehmigende Personen oder Prüfende Personen hinzufügen, während ein Schritt aktiv ist, ohne die bereits laufenden Genehmigungen zu unterbrechen.

So fügen Sie einer aktiven gruppierten Genehmigung Teilnehmer hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf ein beliebiges Dokument in der Gruppe **dann auf** Symbol „Genehmigungen“ rechts auf der Seite.

   ![Genehmigende Personen in der Dokumentzusammenfassung hinzufügen](assets/approvals-icon-new.png)

1. Klicken Sie **Workflow bearbeiten**.

1. Geben Sie den Benutzer, das Team oder die E-Mail in das Feld **Namen oder E-Mails hinzufügen** des aktiven Stadiums ein.

1. Wählen Sie für jede hinzugefügte Person aus, ob sie eine genehmigende Person oder eine prüfende Person ist.

1. Klicken Sie auf **Speichern**.

   Neue Teilnehmer sehen jede offene Genehmigung in der Gruppe in ihrer Warteschlange. Sie sehen keine Entscheidungen, die getroffen wurden, bevor sie hinzugefügt wurden, sodass sie immer noch alle derzeit offenen Genehmigungen selbst abschließen müssen.

## Teilnehmer aus einer aktiven gruppierten Genehmigung entfernen

Sie können genehmigende Personen oder Prüfende Personen aus einer gruppierten Genehmigung entfernen, während ein Schritt aktiv ist. Entfernte Teilnehmer sehen die Genehmigungen der Gruppe sofort nicht mehr in ihrer Warteschlange, aber die Entscheidungen, die sie bereits getroffen haben, werden beibehalten und nicht zurückgesetzt.

So entfernen Sie Teilnehmer aus einer aktiven gruppierten Genehmigung:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf ein beliebiges Dokument in der Gruppe **dann auf** Symbol „Genehmigungen“ rechts auf der Seite.

1. Klicken Sie **Workflow bearbeiten**.

1. Suchen Sie den Teilnehmer, den Sie aus dem aktiven Stadium entfernen möchten, und klicken Sie auf das Symbol **Entfernen** neben seinem Namen.

1. Klicken Sie auf **Speichern**.

   Der Genehmigungsstatus der verbleibenden Teilnehmer wird neu bewertet, um der Änderung Rechnung zu tragen.

## Hinzufügen von Assets zu einer gruppierten Validierung

Sie können einer gruppierten Genehmigung Assets hinzufügen, bis die erste Phase gesperrt ist. Sobald die erste Phase gesperrt ist, können Sie keine Assets mehr hinzufügen, da die Teilnehmer in dieser Phase keine Gelegenheit gehabt hätten, sie zu überprüfen.

So fügen Sie einer gruppierten Genehmigung ein Asset hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf ein beliebiges Dokument in der Gruppe **dann auf** Symbol „Genehmigungen“ rechts auf der Seite.

1. Klicken Sie **Workflow bearbeiten** und dann auf die Registerkarte **Dokumente**.

1. Wählen Sie das Asset bzw. die Assets aus, die Sie der Gruppe hinzufügen möchten.

1. Klicken Sie auf **Speichern**.

   Alle Mitglieder der Gruppe werden darüber informiert, dass ihnen ein zusätzliches Asset zur Überprüfung hinzugefügt wurde.

## Entfernen von Assets aus einer gruppierten Genehmigung

Sie können ein Asset jederzeit aus einer gruppierten Genehmigung im Workflow entfernen. Das entfernte Asset wird zu einer eigenen eigenständigen Genehmigung und speichert alle vorhandenen Entscheidungen, Kommentare und den Verlauf, ohne neu gestartet zu werden. Da das Asset bereits über eine Genehmigungsentscheidung verfügt, können Sie es später nicht mehr zu einer gruppierten Genehmigung hinzufügen.

So entfernen Sie ein Asset aus einer gruppierten Genehmigung:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das Dokument, das Sie entfernen möchten, und dann auf **Symbol** Genehmigungen“ auf der rechten Seite der Seite.

1. Klicken Sie **Workflow bearbeiten** und dann auf die Registerkarte **Dokumente**. Das ausgewählte Dokument ist oben in der Liste angeheftet und bereits aktiviert.

1. Deaktivieren Sie die Auswahl für das Dokument, das Sie aus der Gruppe entfernen möchten.

1. Klicken Sie auf **Speichern**.

   Der Genehmigungsstatus des Assets bleibt ab dem Zeitpunkt sichtbar und unverändert, zu dem es entfernt wurde. Die gruppierte Genehmigungsansicht wird aktualisiert und zeigt die verbleibenden Assets in der Gruppe an.

## Auflösen einer Entscheidung „Arbeit erforderlich“ in einer mehrstufigen gruppierten Genehmigung

Bei einer mehrstufigen gruppierten Genehmigung müssen alle Assets in einem Schritt zu einer Entscheidung gelangen, bevor die Gruppe zum nächsten Schritt übergehen kann. Wenn ein Asset mit **Arbeit erforderlich** gekennzeichnet ist, kann es mit dem Rest der Gruppe nicht weiterentwickelt werden, daher muss es aus der Gruppe entfernt werden, damit die Phase fortgesetzt wird.

So beheben Sie eine Entscheidung mit dem Status „Arbeit erforderlich“:

1. Entfernen Sie das mit &quot;**Arbeit erforderlich“ markierte** aus der Gruppe. Weitere Informationen finden Sie unter [Entfernen von Assets aus einer gruppierten Genehmigung](#remove-assets-from-a-grouped-approval). Das entfernte Asset wird zu einer eigenen eigenständigen Genehmigung und speichert seine vorhandenen Entscheidungen, Kommentare und den Verlauf.

1. Nachdem das Asset aktualisiert wurde, beantragen Sie erneut eine Genehmigung dafür, entweder als einzelnes Asset oder als Teil einer neuen Gruppe. Da das Asset bereits über eine Genehmigungsentscheidung verfügt, können Sie es nicht wieder zur ursprünglichen Gruppe hinzufügen.

   Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](create-a-document-approval.md) und [Erstellen einer gruppierten Genehmigung](create-a-grouped-approval.md).
