---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Dokumentenordner freigeben
description: Sie können einen Ordner und seinen Inhalt über den Bereich Dokumente freigeben.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 2%

---

# Dokumentenordner freigeben

Sie können einen Ordner und seinen Inhalt über den Bereich Dokumente freigeben.

>[!NOTE]
>
>* Der Ordner muss sich in den obersten fünf Ebenen einer Ordnerhierarchie für ein Objekt befinden. Jeder Ordner auf der sechsten Ebene oder darunter erbt seine Freigabekonfigurationen von dem Ordner direkt darüber.
>
>  Informationen zum Hinzufügen von Unterordnern zum Erstellen einer Ordnerhierarchie finden Sie im Abschnitt [Erstellen von Ordnern und Unterordnern](../../documents/organizing-documents/create-documents-folder.md#creating-folders) im Artikel [Erstellen von Dokumentordnern](../../documents/organizing-documents/create-documents-folder.md).
>
>* Intelligente Ordner können nicht freigegeben werden.
>* Wenn Sie Freigabeoptionen für einen Dokumentordner in einer Vorlage konfigurieren und jemand dann ein Projekt aus dieser Vorlage erstellt, werden Ihre Freigabekonfigurationen nicht in den Dokumentordner im neuen Projekt übertragen.
>* Wenn Sie Freigabeoptionen für einen Dokumentenordner innerhalb eines Arbeitselements konfigurieren und dann das Arbeitselement kopieren, werden Ihre Freigabekonfigurationen nicht in den Dokumentenordner des neuen Arbeitselements übertragen.
>

## Zugriffsanforderungen

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Licht oder höher</p> 
   <p>Überprüfen oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf ein Objekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Freigeben von Ordnern

{{step1-to-documents}}

ODER

Klicken Sie bei geöffnetem Workfront **Objekt** linken Bereich auf Dokumente .

1. Wählen Sie den Ordner aus und klicken Sie dann auf das Symbol Freigeben ![Freigabesymbol](assets/share-icon.png) in der Symbolleiste.

   Der Ordner muss sich in den obersten fünf Ebenen einer Ordnerhierarchie für ein Objekt befinden und kann kein intelligenter Ordner sein.

1. Geben Sie in das angezeigte Feld unter **Ordnerzugriff erteilen an** den Namen des Benutzers, Teams, Aufgabengebiets, der Gruppe oder des Unternehmens ein, für den bzw. das Sie den Ordner freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.
1. Um den Zugriff für den soeben hinzugefügten Benutzer, das Team, das Aufgabengebiet, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine seiner erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Möglichkeit zum Anzeigen des Ordners und seines Inhalts.</p> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>Download</strong>: Möglichkeit, den Ordner und seinen Inhalt als ZIP-Datei herunterzuladen</li> 
        <li> <p><strong>Freigeben</strong>: Möglichkeit, den Ordner für andere im System freizugeben</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Möglichkeit zum Anzeigen und Bearbeiten des Ordners und seines Inhalts</p> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong>, um anzugeben, ob Sie Benutzenden Folgendes erlauben möchten:</p> 
       <ul> 
        <li><strong>Löschen</strong>: Löschen des Ordners und seines Inhalts aus dem System</li> 
        <li><b>Herunterladen</b>: Laden Sie den Ordner und seinen Inhalt als ZIP-Datei herunter</li> 
        <li><strong>Freigeben</strong>: Freigeben des Ordners und seines Inhalts für andere Benutzer im System</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 3 bis 4, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Wenn alle Systembenutzenden den Ordner und seinen Inhalt anzeigen können sollen, klicken Sie auf das Zahnradsymbol ![Zahnradsymbol mit Pfeil nach unten](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und dann auf **Dies systemweit sichtbar machen.**

   Wenn Sie Ihre Meinung ändern, können Sie auf **Systemweiten Zugriff entfernen** (die Standardoption) klicken.

## Zugriff von Benutzern auf den Inhalt eines Ordners, der für sie freigegeben wurde

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story   <a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Wenn Sie einen Ordner freigeben, sehen Ihre Empfänger den Ordner derzeit nicht in ihrem Dokumentbereich. Sie können jedoch auf die zugehörigen Dokumente zugreifen, indem sie einen Dokumentbericht ausführen.

Informationen zum Ausführen eines Berichts finden Sie im Abschnitt [Berichte zu Objekten](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) im Artikel [Grundlegendes zu Objekten in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Siehe auch [Erstellen eines benutzerdefinierten Berichts](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Vererbte Berechtigungen bei Freigabe eines Objekts, das einen Ordner enthält

Wenn Sie ein Objekt mit einem Dokumentordner freigeben, erhalten Ihre Empfänger ebenfalls Zugriff auf den Ordner:

* Wenn Sie Ihren Empfängerinnen und Empfängern Ansichtszugriff auf das übergeordnete Objekt gewähren, haben sie Ansichtszugriff auf den Ordner.
* Wenn Sie Ihren Empfängern den Zugriff auf das übergeordnete Objekt gewähren (Contribute oder Verwalten), verfügen diese über den Verwaltungszugriff auf den Ordner.
* Wenn Sie einen Zugriffstyp (Anzeigen, Beitragen oder Verwalten) für das übergeordnete Objekt und einen anderen für den Ordner gewähren, haben Ihre Empfänger den höchsten dieser beiden Zugriffstypen auf Dokumente im Ordner

  Wenn Sie beispielsweise das übergeordnete Objekt mit Ansichtszugriff und den Ordner mit Verwaltungszugriff freigeben, können Ihre Empfänger die Dokumente im Ordner verwalten.

  >[!NOTE]
  >
  >Ein angehängtes Dokument erbt nur Berechtigungen von dem Objekt, an das es angehängt wurde. Wenn Sie einen Ordner für das Objekt erstellen und das Dokument in den Ordner verschieben, übernimmt es die Berechtigungen des Ordners. Wenn Sie jedoch einen Ordner auf einem übergeordneten oder übergeordneten Objekt erstellen und das Dokument in diesen Ordner verschieben, werden die Berechtigungen dieses Ordners nicht übernommen.

* Wenn die Option „Dokumentzugriff nie von Projekten, Aufgaben, Problemen usw. erben“ auf der Zugriffsebene der Empfängerin bzw. des Empfängers aktiviert ist, erben diese keine Berechtigungen für Dokumente in einem Ordner, den Sie für sie freigeben. Um ihnen Zugriff auf ein Dokument im Ordner zu gewähren, müssen Sie das Dokument freigeben.

  Informationen zur Option „Nie vererben“ finden Sie unter [Zugriff auf Adobe Workfront konfigurieren](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Informationen zum Freigeben eines Dokuments finden Sie unter [Freigeben eines Dokuments](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
