---
product-area: documents
navigation-topic: manage-documents
title: Dokumentversionen verwalten
description: Sie können mehrere Versionen eines Dokuments in Workfront verwalten.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Dokumentversionen verwalten

Sie können mehrere Versionen eines Dokuments in Workfront verwalten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf das Dokument</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

* In diesem Artikel wird davon ausgegangen, dass das Dokument mehrere Versionen aufweist.

  Informationen zum Hochladen neuer Versionen eines Dokuments in Workfront finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md).

## Anzeigen einer Liste aller Versionen eines Dokuments

1. Scrollen Sie in der Zusammenfassung zum Abschnitt **Alle Versionen**. Hier können Sie alle Versionen des Dokuments anzeigen.

## Anzeigen und Verwalten von Details für eine frühere Dokumentversion

1. Klicken Sie oben auf der Seite Dokumentdetails auf das Dropdown-Menü neben dem Namen und dann auf den Namen der Version, die Sie anzeigen und verwalten möchten.

   ![Versions-Dropdown in den Dokumentdetails](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Neben der Anzeige der Versionsdetails können Sie Änderungen an der Version vornehmen, z. B. an ihrem Namen, ihren Metadaten und den Proofing-Einstellungen (wenn es sich um einen Dokument-Korrekturabzug handelt).

## Einzelne Dokumentversion herunterladen

1. Klicken Sie in der Zusammenfassung unter **Versionen** auf das Menü Mehr ![Mehr](assets/more-icon.png) rechts neben der Version und klicken Sie dann in der angezeigten Dropdown-Liste auf **Herunterladen**.

   ![Ein einzelnes Dokument herunterladen](assets/more-versions-350x143.png)

## Herunterladen aller Versionen eines Dokuments

1. Klicken Sie **Dokumentdetails** und wählen Sie dann **Alle Versionen** im linken Bereich aus.

1. Klicken **oben in** Liste auf „Alle herunterladen“.

## Dokumentversion löschen

Wenn Sie versehentlich eine Version eines Dokuments hochladen oder eine Version nicht mehr benötigt wird, können Sie die Version löschen und das Originaldokument beibehalten.

>[!IMPORTANT]
>
>Sie können eine Dokumentversion, die Sie einzeln löschen, nicht wiederherstellen.

Beachten Sie beim Löschen einer Dokumentversion Folgendes:

* Es kann jeweils nur eine Version gelöscht werden. Wenn eine Version gelöscht wird, wird diese Aktion in der Datei **Updates** im Dokument angezeigt.
* Wenn Sie nach dem Löschen einer Version eine neue Version hochladen, erhält die neue Version die nächste sequenzielle Nummer. Wenn es beispielsweise drei Versionen eines Dokuments gibt und Sie Version 3 löschen, wird als nächstes Dokument Version 4 hochgeladen.
* Systemaktualisierungen und Kommentare zu einer Version werden nach dem Löschen der Version in Workfront beibehalten.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Löschen einer Dokumentversion:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie **Dokumente**. Suchen Sie das gewünschte Dokument.
1. Klicken Sie im Bereich **Version** in der Zusammenfassung auf die Version und klicken Sie dann in **angezeigten Dropdown** Liste auf „Löschen“. Die **Löschen**-Option ist nur sichtbar, wenn mindestens zwei Versionen vorhanden sind.

   Wenn das Dokument mit einer externen Quelle verknüpft ist, wird dieser Link gelöscht und das Dokument ist nicht mehr über Workfront zugänglich.

   ![Dokumentversion löschen](assets/more-versions-350x143.png)
