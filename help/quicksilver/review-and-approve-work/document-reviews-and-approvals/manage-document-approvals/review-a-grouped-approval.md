---
product-area: documents
navigation-topic: approvals
title: Überprüfen einer gruppierten Genehmigung
description: Sie können alle Dokumente in einer gruppierten Genehmigung über das Widget Meine Genehmigungen auf der Startseite oder im Frame.io-Viewer überprüfen und Entscheidungen treffen.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: ccb3d004feca5373473a872b101a7acff11de77f
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 6%
---

# Überprüfen einer gruppierten Genehmigung

<span class="preview">Die Informationen auf dieser Seite sind in der Sandbox-Vorschau-Umgebung nicht verfügbar, da die Frame.io-Integration dort nicht verfügbar ist. Diese Funktion ist ab 22. Oktober 2026 in Produktionsumgebungen verfügbar.</span>

Wenn Sie einer gruppierten Genehmigung zugewiesen sind, werden alle Dokumente in der Gruppe zusammen angezeigt, sodass Sie für jede Genehmigung eine Entscheidung treffen können. Sie können Änderungen an jedem Dokument gleichzeitig genehmigen oder anfordern oder eine Entscheidung für jedes Dokument einzeln treffen.

Wenn ein oder mehrere Dokumente in einer mehrstufigen **mit** Arbeit erforderlich“ gekennzeichnet sind, kann die Gruppe erst dann mit dem nächsten Schritt fortfahren, wenn für alle Dokumente in der Gruppe eine genehmigte Entscheidung vorliegt. Weitere Informationen finden Sie [Auflösen einer Entscheidung „Muss überarbeitet werden“ für ein einzelnes Dokument in einer mehrstufigen gruppierten Genehmigung](#resolve-a-needs-work-decision-on-a-single-document-in-a-multi-stage-grouped-approval).



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
   </td>
  </tr>
  <tr>
   <td role="rowheader">Konfigurationen der Zugriffsebene</td>
   <td> <p>Zugriff auf Objekte, die mit Genehmigungen verknüpft sind, anzeigen oder höher</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objektberechtigungen</td>
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verbunden sind</p></td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Überprüfen einer gruppierten Genehmigung über das Widget Meine Genehmigungen in der Startseite

Das Widget Meine Genehmigungen in Startseite fasst die Dokumente unter einer einzigen Genehmigung zusammen, sodass Sie alle gemeinsam bearbeiten können.

>[!NOTE]
>
>Möglicherweise müssen Sie das Widget Meine Genehmigungen zu Ihrer Startseite hinzufügen. Weitere Informationen finden Sie unter [Widgets auf der Startseite hinzufügen, bearbeiten oder &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).

1. Klicken Sie auf **Startseite** in der oberen linken Ecke von Adobe Workfront und suchen Sie das Widget **Meine Genehmigungen**.

1. Öffnen Sie die gruppierte Genehmigung. Alle Dokumente in der Gruppe werden zusammen aufgelistet, wobei die Anzahl der Elemente in der Gruppe oben angezeigt wird.

1. Treffen Sie eine Entscheidung mithilfe einer der folgenden Möglichkeiten:

   * **Alle als genehmigt markieren**: Zeichnet eine genehmigte Entscheidung gleichzeitig für jedes Dokument in der Gruppe auf.
   * **Alle Arbeitsaufträge markieren**: Zeichnet eine Entscheidung über den Arbeitsaufwand für jedes Dokument in der Gruppe gleichzeitig auf.
   * **Entscheidung treffen**: Eine einzelne Entscheidung über ein einzelnes Dokument treffen. Wiederholen Sie diesen Vorgang für jedes Dokument, über das Sie separat entscheiden möchten.


   ![Widget „Meine Genehmigungen“ - gruppierte Genehmigung](assets/my-approvals-group.png)

## Überprüfen einer gruppierten Genehmigung im Frame.io-Viewer

Im Frame.io-Viewer werden alle Dokumente in der Gruppe zusammen angezeigt, sodass Sie für jedes Dokument eine schnelle Entscheidung treffen können. Alternativ können Sie ein Dokument öffnen, um es im Detail zu überprüfen.

1. Wechseln Sie zu Ihrer E-Mail-Benachrichtigung zur Überprüfung und klicken Sie **Zum Überprüfen wechseln** oder öffnen Sie die gruppierte Genehmigung über das Widget **Meine Genehmigungen** auf der Startseite.

1. Führen Sie einen der folgenden Schritte aus:

   * Treffen Sie eine schnelle Entscheidung für jedes Dokument direkt auf der Gruppenseite, ohne es zu öffnen.
   * Klicken Sie auf ein Dokument, um es zu öffnen, fügen Sie Kommentare oder Markup hinzu und gehen Sie dann mit dem Pfeil zum nächsten Dokument in der Gruppe. Der Dokumentzähler (z. B. **1 von 2**) zeigt Ihren Platz in der Gruppe an.

   Weitere Informationen zu Kommentaren und Markup im Frame.io-Viewer finden Sie unter [Überprüfen und Genehmigen mit dem Frame.io-Viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md).

1. Wählen Sie für jedes Dokument eine Entscheidung:

   * **Genehmigt**: Das Dokument muss nicht geändert werden und ist einsatzbereit.
   * **Muss überarbeitet werden**: Das Dokument muss geändert werden und ist nicht einsatzbereit.

   Weitere Informationen zu Entscheidungen finden Sie unter [Übersicht über den &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

   ![Frame.io Viewer Gruppierte Genehmigung](assets/frame-group-approval.png)

## Weitere Ressourcen

Dieser Artikel enthält Informationen zum Überprüfen einer Gruppe von Dokumenten. Informationen zum Treffen einer Entscheidung für ein einzelnes Dokument, Hinzufügen von Markup und mehr finden Sie unter

* [Genehmigen eines Dokuments in Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/approve-a-document.md)
* [Überprüfen eines Dokuments in Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-a-document.md)
* [Überprüfen und Genehmigen mit dem Frame.io-Viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)