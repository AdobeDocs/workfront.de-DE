---
product-area: documents
navigation-topic: manage-documents
title: Dokumentversionen verwalten
description: Sie können mehrere Versionen eines Dokuments in Workfront verwalten.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Dokumentversionen verwalten

Sie können mehrere Versionen eines Dokuments in Workfront verwalten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Dokument anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Voraussetzungen

* In diesem Artikel wird davon ausgegangen, dass das Dokument über mehrere Versionen verfügt.

  Informationen zum Hochladen neuer Dokumentversionen in Workfront finden Sie unter [Hochladen einer neuen Dokumentversion](../../documents/managing-documents/upload-new-document-version.md).

## Liste aller Versionen eines Dokuments anzeigen

1. Scrollen Sie in der Zusammenfassung zum Bereich **Alle Versionen** . Hier können Sie alle Versionen des Dokuments anzeigen.

## Anzeigen und Verwalten von Details für eine frühere Dokumentversion

1. Klicken Sie oben auf der Seite &quot;Dokumentdetails&quot;auf das Dropdown-Menü neben dem Namen und klicken Sie dann auf den Namen der Version, die Sie anzeigen und verwalten möchten.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Neben der Anzeige der Details der Version können Sie Änderungen an der Version vornehmen, z. B. ihren Namen, Metadaten und Testversandeinstellungen (sofern es sich um einen Dokumentversand handelt).

## Herunterladen einer einzelnen Dokumentversion

1. Klicken Sie in der Zusammenfassung unter &quot;**Versionen**&quot;auf das Menü &quot;Mehr&quot;![](assets/more-icon.png) rechts neben der Version und klicken Sie dann in der angezeigten Dropdownliste auf &quot;**Download**&quot;.

   ![](assets/more-versions-350x143.png)

## Alle Versionen eines Dokuments herunterladen

1. Klicken Sie auf **Dokumentdetails** und wählen Sie dann im linken Bereich **Alle Versionen** aus.

1. Klicken Sie oben in der Liste auf **Alle herunterladen** .

## Dokumentversion löschen

Wenn Sie versehentlich eine Version eines Dokuments hochladen oder eine Version nicht mehr benötigt wird, können Sie die Version löschen und das Originaldokument beibehalten.

>[!IMPORTANT]
>
>Sie können eine Dokumentversion, die Sie löschen, nicht einzeln wiederherstellen.

Beachten Sie Folgendes, wenn Sie erwägen, eine Dokumentversion zu löschen:

* Es kann jeweils nur eine Version gelöscht werden. Wenn eine Version gelöscht wird, wird diese Aktion im Dokument unter **Aktualisierungen** angezeigt.
* Wenn Sie eine neue Version hochladen, nachdem Sie eine Version gelöscht haben, erhält die neue Version die nächste sequenzielle Nummer. Wenn es beispielsweise 3 Versionen eines Dokuments gibt und Sie Version 3 löschen, lautet das nächste hochgeladene Dokument Version 4.
* Systemaktualisierungen und Kommentare zu einer Version werden nach dem Löschen der Version in Workfront beibehalten.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

So löschen Sie eine Dokumentversion:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus. Suchen Sie das gewünschte Dokument.
1. Klicken Sie im Bereich **Version** in der Zusammenfassung auf die Version und klicken Sie dann in der angezeigten Dropdownliste auf **Löschen** . Die Option **Löschen** ist nur sichtbar, wenn mindestens zwei Versionen vorhanden sind.

   Wenn das Dokument mit einer externen Quelle verknüpft ist, wird dieser Link gelöscht und der Zugriff auf das Dokument ist über Workfront nicht mehr möglich.

   ![](assets/more-versions-350x143.png)
