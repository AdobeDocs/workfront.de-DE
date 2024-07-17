---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Dokumentordner freigeben
description: Sie können einen Ordner und dessen Inhalt im Bereich "Dokumente"freigeben.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Dokumentordner freigeben

Sie können einen Ordner und dessen Inhalt im Bereich &quot;Dokumente&quot;freigeben.

>[!NOTE]
>
>* Der Ordner muss sich auf den fünf obersten Ebenen einer Ordnerhierarchie eines Objekts befinden. Jeder Ordner auf der sechsten Ebene oder darunter übernimmt seine Freigabekonfigurationen direkt über dem Ordner.
>
>  Informationen zum Hinzufügen von Unterordnern zum Erstellen einer Ordnerhierarchie finden Sie im Abschnitt [Erstellen von Ordnern und Unterordnern](../../documents/organizing-documents/create-documents-folder.md#creating-folders) im Artikel [Erstellen von Dokumentordnern](../../documents/organizing-documents/create-documents-folder.md).
>
>* Smart-Ordner können nicht freigegeben werden.
>* Wenn Sie Freigabeoptionen für einen Dokumentordner in einer Vorlage konfigurieren und dann ein Projekt aus dieser Vorlage erstellt wird, werden Ihre Freigabekonfigurationen nicht in den Dokumentordner im neuen Projekt übertragen.
>* Wenn Sie Freigabeoptionen für einen Dokumentordner innerhalb eines Arbeitselements konfigurieren und dann das Arbeitselement kopieren, werden Ihre Freigabekonfigurationen nicht in den Dokumentordner im neuen Arbeitselement übertragen.
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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf ein Objekt anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Ordner freigeben

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Dokumente**.![](assets/main-menu-icon.png)

   Oder

   Klicken Sie bei geöffnetem Workfront-Objekt im linken Bereich auf **Dokumente** .

1. Wählen Sie den Ordner aus und klicken Sie dann in der Symbolleiste auf das Symbol Freigabe ![](assets/share-icon.png) .

   Der Ordner muss sich auf den fünf obersten Ebenen einer Ordnerhierarchie eines Objekts befinden und darf kein Smart-Ordner sein.

1. Geben Sie in dem angezeigten Feld unter **Ordnerzugriff gewähren auf** den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/das Sie den Ordner freigeben möchten, und drücken Sie dann bei der Anzeige des Namens die Eingabetaste **3}.**
1. Um den Zugriff auf den soeben hinzugefügten Benutzer, das Team, die Rolle, die Gruppe oder das Unternehmen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und konfigurieren Sie dann eine der folgenden verfügbaren Optionen und eine der erweiterten Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Möglichkeit, Ordner und Inhalt anzuzeigen.</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um festzulegen, ob Folgendes zulässig sein soll:</p> 
       <ul> 
        <li><strong>Download</strong>: Möglichkeit, den Ordner und dessen Inhalt als ZIP-Datei herunterzuladen</li> 
        <li> <p><strong>Freigabe</strong>: Möglichkeit, den Ordner für andere im System freizugeben</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Möglichkeit, Ordner und Inhalt anzuzeigen und zu bearbeiten</p> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob Sie Benutzern Folgendes erlauben möchten:</p> 
       <ul> 
        <li><strong>Löschen</strong>: Löschen Sie den Ordner und dessen Inhalt aus dem System.</li> 
        <li><b>Herunterladen</b>: Laden Sie den Ordner und seinen Inhalt als ZIP-Datei herunter.</li> 
        <li><strong>Freigabe</strong>: Geben Sie den Ordner und dessen Inhalt für andere Benutzer im System frei.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die Schritte 3 bis 4, um weitere Namen zur Liste hinzuzufügen und deren Optionen zu konfigurieren.
1. (Optional) Wenn Sie möchten, dass alle Benutzer im System den Ordner und dessen Inhalt anzeigen können, klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und klicken Sie dann auf **Dieses Bild systemweit anzeigen**.

   Wenn Sie Ihre Meinung ändern, können Sie auf **Systemweiten Zugriff entfernen** klicken (Standardoption).

## So greifen Benutzer auf den Inhalt eines Ordners zu, der für sie freigegeben wurde

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Wenn Sie derzeit einen Ordner freigeben, sehen Ihre Empfänger den Ordner nicht im Bereich &quot;Dokumente&quot;. Sie können jedoch auf ihre Dokumente zugreifen, indem sie einen Dokumentbericht ausführen.

Informationen zum Ausführen eines Berichts finden Sie im Abschnitt [Objektbericht anzeigen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Siehe auch [Benutzerspezifischen Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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

## Vererbte Berechtigungen beim Freigeben eines Objekts, das einen Ordner enthält

Wenn Sie ein Objekt freigeben, das einen Dokumentordner enthält, erhalten Ihre Empfänger auch Zugriff auf den Ordner:

* Wenn Sie Ihren Empfängern Zugriff auf das übergeordnete Objekt gewähren Ansichtszugriff gewähren, haben sie Zugriff auf den Ordner.
* Wenn Sie Ihren Empfängern Contribute oder Verwalten Zugriff auf das übergeordnete Objekt gewähren, haben sie Zugriff auf den Ordner .
* Wenn Sie dem übergeordneten Objekt einen Zugriff vom Typ (Ansicht, Contribute oder Verwalten) und dem Ordner einen anderen Typ gewähren, haben Ihre Empfänger den höchsten dieser beiden Arten von Zugriff auf Dokumente im Ordner

  Wenn Sie beispielsweise das übergeordnete Objekt mit Zugriff auf Ansicht und den Ordner mit Zugriff auf Verwalten freigeben, haben Ihre Empfänger die Option Verwalten für die Dokumente im Ordner.

  >[!NOTE]
  >
  >Ein angehängtes Dokument erbt die Berechtigungen nur von dem Objekt, an das es angehängt wurde. Wenn Sie einen Ordner für das Objekt erstellen und das Dokument in den Ordner verschieben, erbt es die Berechtigungen des Ordners. Wenn Sie jedoch einen Ordner für ein übergeordnetes oder übergeordnetes Objekt erstellen und das Dokument in diesen Ordner verschieben, erbt es nicht die Berechtigungen dieses Ordners.

* Wenn die Option &quot;Dokumentzugriff nie von Projekten, Aufgaben, Problemen usw. übernehmen&quot;auf der Zugriffsebene des Empfängers aktiviert ist, erben diese keine Berechtigungen für Dokumente in einem Ordner, den Sie für sie freigeben. Um ihnen Zugriff auf ein Dokument im Ordner zu gewähren, müssen Sie das Dokument freigeben.

  Weitere Informationen zur Option &quot;Niemals übernehmen&quot;finden Sie unter [Zugriff auf Adobe Workfront konfigurieren](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  Informationen zum Freigeben eines Dokuments finden Sie unter [Freigeben eines Dokuments](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
