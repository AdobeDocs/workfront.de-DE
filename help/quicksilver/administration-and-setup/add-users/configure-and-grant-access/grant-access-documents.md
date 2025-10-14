---
title: Zugriff auf Dokumente gewähren
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Dokumente in Workfront zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 1%

---

# Zugriff auf Dokumente gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf Dokumente zu definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Dieser Zugriff gilt auch für Dokumentordner.

Informationen zur Verwendung benutzerdefinierter Zugriffsebenen zur Verwaltung des Benutzerzugriffs auf andere Objekttypen in Workfront finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.&gt;.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Konfigurieren des Benutzerzugriffs auf Dokumente mithilfe einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der **Ansicht** oder **Bearbeiten** rechts neben Dokumente und wählen Sie dann die Funktionen aus, die Sie unter **Einstellungen optimieren** gewähren möchten.

   ![document_access.png](assets/document-access.png)

   Sie können Benutzern die folgenden Aktionen für Projekte, Aufgaben und Probleme ermöglichen, auf die sie Zugriff haben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Erstellen</td> 
      <td>Dokumente hochladen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen</td> 
      <td> <p>Hochgeladene Dokumente entfernen.</p> <p>Die <b>Erstellen</b>-Option wird automatisch aktiviert, wenn diese Option aktiviert ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigeben</td> 
      <td>Freigeben von Dokumenten für bestimmte Benutzer, Aufgabengebiete und Teams</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente öffentlich teilen</td> 
      <td>Dokumente für externe Benutzer freigeben (ohne Workfront-Lizenz).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Systemweit teilen</td> 
      <td> <p>Machen Sie Dokumente für alle Personen in Ihrer Workfront-Instanz verfügbar.</p> <p>Jeder im System kann ein auf diese Weise freigegebenes Dokument sehen, wenn:</p> 
       <ul> 
        <li> <p>Sie senden ihnen einen Link zur Seite „Dokumente“, auf die sie hochgeladen werden.</p> </li> 
        <li> <p>Sie suchen danach in Workfront</p> </li> 
       </ul> <p>Die <b>Freigabe</b>-Option wird automatisch aktiviert, wenn diese Option aktiviert ist.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn Sie eine Zugriffsebenen-Einstellung für einen bestimmten Objekttyp konfigurieren, hat diese Konfiguration keine Auswirkungen auf den Zugriff der Benutzer auf Objekte mit einem niedrigeren Rang. Sie können beispielsweise Benutzerinnen und Benutzer daran hindern, Projekte in ihrer Zugriffsebene zu löschen, was sie jedoch nicht daran hindert, Dokumente zu löschen, die schlechter rangieren als Projekte. Weitere Informationen zur Hierarchie von Objekten finden Sie im Abschnitt [Interdependenz und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Grundlegendes zu Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optional) Um geerbte Berechtigungen für Dokumente von Objekten mit höherem Rang einzuschränken, klicken Sie auf **Zusätzliche Einschränkungen festlegen** und wählen Sie dann **Dokumentzugriff nie von Projekten, Aufgaben, Problemen erben usw**.
1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Dokumente nach Lizenztyp

Weitere Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Dokumenten tun können, finden Sie im Abschnitt [Dokumente](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Dokumente

Nachdem Sie ein Dokument in Workfront hochgeladen haben, können Sie es für andere Benutzende freigeben, indem Sie ihnen die entsprechenden Berechtigungen erteilen, wie unter [Dokument freigeben](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md) beschrieben.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers durch eine Kombination zweier Dinge bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt erteilen
* Die Zugriffsebenen-Einstellungen des Empfängers für den Objekttyp
