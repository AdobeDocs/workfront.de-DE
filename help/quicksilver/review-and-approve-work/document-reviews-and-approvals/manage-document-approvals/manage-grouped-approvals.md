---
product-area: documents
navigation-topic: approvals
title: Gruppierte Genehmigungen verwalten
description: In einer gruppierten Genehmigung können Sie Teilnehmer und Dokumente hinzufügen oder entfernen, ohne den Workflow für den Rest der Gruppe zu unterbrechen.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 9459c6251b2576207e1766d94e6cb634f65f1f68
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 5%
---

# Gruppierte Genehmigungen verwalten

Bei einer gruppierten Genehmigung werden mehrere Dokumente in einem einzigen Genehmigungs-Workflow gebündelt, sodass alle Dokumente dieselben Phasen gemeinsam durchlaufen, anstatt pro Dokument eine separate Genehmigung erforderlich zu machen. Sie können Teilnehmer und Dokumente in einer aktiven gruppierten Genehmigung hinzufügen oder entfernen, ohne den Workflow neu zu erstellen.

Gruppierte Validierungen unterstützen den einfachen und erweiterten Modus, mehrere Phasen und parallele Pfade auf die gleiche Weise wie Genehmigungen für einzelne Assets. Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Gruppierte Validierungen sind nur im Bereich Neue Dokumente verfügbar. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

   ![Genehmigende Personen in der Dokumentzusammenfassung entfernen](assets/approvals-icon-new.png)

1. Klicken Sie **Workflow bearbeiten**.

1. Suchen Sie den Teilnehmer, den Sie aus dem aktiven Stadium entfernen möchten, und klicken Sie auf das Symbol **Entfernen** neben seinem Namen.

1. Klicken Sie auf **Speichern**.

## Dokumente zu einer gruppierten Genehmigung hinzufügen

Sie können einer gruppierten Genehmigung Dokumente hinzufügen, bis deren erster Schritt gesperrt ist. Sobald der erste Schritt gesperrt ist, können Sie keine Dokumente mehr hinzufügen.

So fügen Sie einer gruppierten Genehmigung ein Dokument hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf ein beliebiges Dokument in der Gruppe **dann auf** Symbol „Genehmigungen“ rechts auf der Seite.

1. Klicken Sie **Workflow bearbeiten** und dann auf die Registerkarte **Dokumente**.

1. Wählen Sie das Dokument oder die Dokumente aus, die Sie der Gruppe hinzufügen möchten.

1. Klicken Sie auf **Speichern**.

   Alle Mitglieder der Gruppe werden darüber informiert, dass ihnen ein zusätzliches Dokument zur Überprüfung hinzugefügt wurde.

## Entfernen von Dokumenten aus einer gruppierten Genehmigung

Sie können ein Dokument jederzeit aus einer gruppierten Genehmigung im Workflow entfernen. Das entfernte Dokument wird zu einer eigenen eigenständigen Genehmigung und speichert alle vorhandenen Entscheidungen, Kommentare und den Verlauf, ohne neu gestartet zu werden. Da das Dokument bereits mit einer Genehmigungsentscheidung versehen ist, können Sie es später nicht mehr zu einer gruppierten Genehmigung hinzufügen.

So entfernen Sie ein Dokument aus einer gruppierten Genehmigung:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das die gruppierte Genehmigung enthält, und wählen Sie **Dokumente** im linken Bereich aus.

1. Klicken Sie auf das Dokument, das Sie entfernen möchten, und dann auf **Symbol** Genehmigungen“ auf der rechten Seite der Seite.

1. Klicken Sie **Workflow bearbeiten** und dann auf die Registerkarte **Dokumente**. Das ausgewählte Dokument ist oben in der Liste angeheftet und bereits aktiviert.

1. Deaktivieren Sie die Auswahl für das Dokument, das Sie aus der Gruppe entfernen möchten.

1. Klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Der Genehmigungsstatus des Dokuments bleibt ab dem Zeitpunkt sichtbar und unverändert, zu dem es entfernt wurde. Die gruppierte Genehmigungsansicht wird aktualisiert und zeigt die verbleibenden Dokumente in der Gruppe an.


## Auflösen einer Entscheidung „Arbeit erforderlich“ für ein einzelnes Dokument in einer mehrstufigen gruppierten Genehmigung

Bei einer mehrstufigen gruppierten Genehmigung müssen alle Dokumente in einem Schritt zu einer Entscheidung gelangen, bevor die Gruppe zum nächsten Schritt übergehen kann. Wenn ein Dokument als **Arbeit erforderlich** gekennzeichnet ist, kann es mit dem Rest der Gruppe nicht weiterentwickelt werden, daher muss es manuell aus der Gruppe entfernt werden, damit der Schritt fortgesetzt wird.

Wenn Sie das Dokument aus der Gruppe entfernen, wird es zu einer eigenen eigenständigen Genehmigung und behält alle vorhandenen Entscheidungen, Kommentare und den Verlauf bei, ohne neu gestartet zu werden. Sie können das überarbeitete Dokument als neue Version zur eigenständigen Genehmigung hinzufügen oder eine neue gruppierte Genehmigung damit erstellen.

So beheben Sie eine Entscheidung mit dem Status „Arbeit erforderlich“:

1. Entfernen Sie das Dokument, das mit &quot;**Arbeit erforderlich** gekennzeichnet wurde, aus der Gruppe. Weitere Informationen finden Sie unter [Entfernen von Dokumenten aus einer gruppierten Genehmigung](#remove-documents-from-a-grouped-approval). Das entfernte Dokument wird zu einer eigenen eigenständigen Genehmigung und behält seine vorhandenen Entscheidungen, Kommentare und den Verlauf bei.

1. Laden Sie das Dokument nach dem Aktualisieren als neue Version hoch und fordern Sie die Genehmigung erneut an oder fügen Sie es als Teil einer neuen Gruppe hinzu.

   Weitere Informationen finden Sie unter

   * [Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)
   * [Erstellen eines Workflows für die Dokumentvalidierung](create-a-document-approval.md)
   * [Erstellen einer gruppierten Genehmigung](create-a-grouped-approval.md)


## Bekannte Einschränkungen

Es gibt ein temporäres Synchronisationsproblem mit Frame.io, wenn Sie Dokumente in einer gruppierten Genehmigung hinzufügen oder entfernen. Die Änderungen werden erst dann in Frame.io übernommen, wenn das Dokument das nächste Mal synchronisiert wird.