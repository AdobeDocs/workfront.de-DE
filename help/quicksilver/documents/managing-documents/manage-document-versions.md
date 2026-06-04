---
product-area: documents
navigation-topic: manage-documents
title: Verwalten von Dokumentversionen
description: Sie können mehrere Versionen eines Dokuments in Workfront verwalten.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
TQID: https://experienceleague.adobe.com/rCnj3Gx1SB3-UziuppQfifv2hJ6q3OjepNO9FcEEHEk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 634
ht-degree: 8%

---

# Verwalten von Dokumentversionen

<!-- Audited: 5/2025 -->

Sie können mehrere Versionen eines Dokuments in Workfront verwalten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit dem Adobe Cloud-Speicher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf das Dokument</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

* In diesem Artikel wird davon ausgegangen, dass das Dokument mehrere Versionen aufweist.

  Informationen zum Hochladen neuer Versionen eines Dokuments in Workfront finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md).

## Anzeigen einer Liste aller Versionen eines Dokuments

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ ein Dokument in der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Versionen**, um alle Dokumentversionen anzuzeigen.

## Anzeigen und Verwalten von Details für eine frühere Dokumentversion

{{step1-to-documents}}

1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf **Dokumentdetails**.

1. Klicken Sie oben auf der Seite **Dokumentdetails** auf das Dropdown-Menü neben dem Namen und dann auf den Namen der Version, die Sie anzeigen und verwalten möchten.

   ![Dropdown-Liste „Version“ auf der Seite „Dokumentdetails“](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Neben der Anzeige der Versionsdetails können Sie Änderungen an der Version vornehmen, z. B. an ihrem Namen, ihren Metadaten und den Proofing-Einstellungen (wenn es sich um einen Dokument-Korrekturabzug handelt).

## Einzelne Dokumentversion herunterladen

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ ein Dokument in der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Klicken Sie **Abschnitt** Versionen“ auf das Menü **Mehr** ![Mehr](assets/more-icon.png) rechts von der Version und klicken Sie dann in der angezeigten Dropdown-Liste auf **Herunterladen**.

   ![Ein einzelnes Dokument herunterladen](assets/more-versions-350x143.png)

## Herunterladen aller Versionen eines Dokuments

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ ein Dokument in der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Versionen** und klicken Sie dann auf **Alle herunterladen**.

## Dokumentversion löschen

Wenn Sie versehentlich eine Version eines Dokuments hochladen oder eine Version nicht mehr benötigt wird, können Sie die Version löschen und das Originaldokument beibehalten.

>[!IMPORTANT]
>
>Sie können eine Dokumentversion, die Sie einzeln löschen, nicht wiederherstellen.

Beachten Sie beim Löschen einer Dokumentversion Folgendes:

* Es kann jeweils nur eine Version gelöscht werden. Wenn eine Version gelöscht wird, wird diese Aktion im Abschnitt Aktualisierungen des Dokuments angezeigt.
* Wenn Sie nach dem Löschen einer Version eine neue Version hochladen, erhält die neue Version die nächste sequenzielle Nummer. Wenn es beispielsweise drei Versionen eines Dokuments gibt und Sie Version 3 löschen, wird als nächstes Dokument Version 4 hochgeladen.
* Systemaktualisierungen und Kommentare zu einer Version werden nach dem Löschen der Version in Workfront beibehalten.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Löschen einer Dokumentversion:

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ das Dokument aus der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Versionen**, um alle Dokumentversionen anzuzeigen.
1. Klicken Sie **Abschnitt** Versionen“ auf das Menü **Mehr** ![Mehr](assets/more-icon.png) rechts von der Version und klicken Sie dann in der angezeigten Dropdown-Liste auf **Löschen**.

   >[!NOTE]
   >
   >* Die **Löschen**-Option ist nur sichtbar, wenn mindestens zwei Versionen vorhanden sind.
   >* Wenn das Dokument mit einer externen Quelle verknüpft ist, wird dieser Link gelöscht und das Dokument ist nicht mehr über Workfront zugänglich.

   ![Löschen Sie die Dokumentversion](assets/more-versions-350x143.png)
