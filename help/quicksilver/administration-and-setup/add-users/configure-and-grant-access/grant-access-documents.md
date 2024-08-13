---
title: Zugriff auf Dokumente gewähren
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf Dokumente in Workfront zu definieren.
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

Als Adobe Workfront-Administrator können Sie eine Zugriffsstufe verwenden, um den Zugriff eines Benutzers auf Dokumente zu definieren, wie unter [Überblick über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Dieser Zugriff gilt auch für Dokumentordner.

Informationen zur Verwendung benutzerdefinierter Zugriffsebenen zur Verwaltung des Benutzerzugriffs auf andere Objekttypen in Workfront finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.&gt;.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzerzugriff auf Dokumente mit einer benutzerdefinierten Zugriffsebene konfigurieren

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche **Ansicht** oder **Bearbeiten** rechts neben &quot;Dokumente&quot;und wählen Sie dann die Fähigkeiten aus, die Sie unter **Feinabstimmung Ihrer Einstellungen** gewähren möchten.

   ![document_access.png](assets/document-access.png)

   Sie können Benutzern Folgendes erlauben, um Projekte, Aufgaben und Probleme zu bearbeiten, auf die sie Zugriff haben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Erstellen</td> 
      <td>Hochladen von Dokumenten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen</td> 
      <td> <p>Entfernen hochgeladener Dokumente</p> <p>Die Option <b>Erstellen</b> wird automatisch aktiviert, wenn diese Option aktiviert ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigeben</td> 
      <td>Freigeben von Dokumenten für bestimmte Benutzer, Aufgabenrollen und Teams.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente öffentlich teilen</td> 
      <td>Freigeben von Dokumenten für externe Benutzer (ohne Workfront-Lizenz).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Systemweit teilen</td> 
      <td> <p>Bereitstellen von Dokumenten für alle Benutzer in Ihrer Workfront-Instanz.</p> <p>Jeder im System kann ein auf diese Weise freigegebenes Dokument sehen, wenn:</p> 
       <ul> 
        <li> <p>Sie senden ihnen einen Link zur Seite "Dokumente", auf die sie hochgeladen wurden.</p> </li> 
        <li> <p>Sie suchen nach Workfront</p> </li> 
       </ul> <p>Die Option <b>Freigabe</b> wird automatisch aktiviert, wenn diese Option aktiviert ist.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn Sie eine Einstellung auf Zugriffsebene für einen bestimmten Objekttyp konfigurieren, wirkt sich diese Konfiguration nicht auf den Zugriff der Benutzer auf Objekte mit niedrigerem Rang aus. Sie können beispielsweise Benutzer daran hindern, Projekte auf ihrer Zugriffsebene zu löschen. Dies schränkt jedoch nicht das Löschen von Dokumenten ein, die im Vergleich zu Projekten untergeordneter sind. Weitere Informationen zur Objekthierarchie finden Sie im Abschnitt [Interdependenz und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Optional) Um die geerbten Berechtigungen für Dokumente aus hochrangigen Objekten einzuschränken, klicken Sie auf **Zusätzliche Einschränkungen festlegen** und wählen Sie dann **Erben Sie den Dokumentzugriff nie von Projekten, Aufgaben, Problemen usw.**.
1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugang zu Dokumenten nach Lizenztyp

Weitere Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Dokumenten tun können, finden Sie im Abschnitt [Dokumente](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugriff auf freigegebene Dokumente

Nachdem Sie ein Dokument in Workfront hochgeladen haben, können Sie es für andere Benutzer freigeben, indem Sie ihnen Berechtigungen erteilen, wie unter [Freigeben eines Dokuments](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md) beschrieben.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp
