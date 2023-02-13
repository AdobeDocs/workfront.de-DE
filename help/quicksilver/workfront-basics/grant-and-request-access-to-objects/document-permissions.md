---
title: Freigeben eines Dokuments
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie unter Zugriff auf Dokumente gewähren beschrieben.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# Freigeben eines Dokuments

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie hier beschrieben: [Zugriff auf Dokumente gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Die Zugriffsebene, die der Workfront-Administrator Benutzern gewährt, ermöglicht es ihnen, Dokumente anzuzeigen oder zu bearbeiten. Darüber hinaus können andere Benutzer anderen Benutzern auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dokumente erteilen, die sie selbst hochgeladen haben oder auf die sie Zugriff haben.

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können. Weitere Informationen zu Objektberechtigungen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Der Benutzer, der ein Dokument in Workfront hochlädt, hat standardmäßig die Berechtigung &quot;Verwalten&quot;.

Informationen zum Freigeben eines gesamten Dokumentordners finden Sie unter [Dokumentordner freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Überlegungen zum Freigeben von Dokumenten

Zusätzlich zu den unten stehenden Überlegungen siehe [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

* Das Freigeben eines Dokuments ähnelt dem Freigeben anderer Objekte in Workfront. Informationen zum Freigeben von Dokumenten in Workfront finden Sie unter [Objekt freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können Dokumenten die folgenden Berechtigungen erteilen:

   * Anzeigen
   * Verwalten

* Sie können ein Dokument auch öffentlich oder systemweit freigeben.

   >[!CAUTION]
   >
   >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen für externe Benutzer Vorsicht walten zu lassen. Dadurch können sie Informationen anzeigen, ohne Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

* Sie können ein Dokument für eine Person freigeben, die kein Workfront-Konto hat, indem Sie deren E-Mail-Adresse im Feld Dokumentzugriff gewähren hinzufügen.
* Wenn Sie ein Dokument freigeben, haben Benutzer denselben Zugriff auf alle Dokumentversionen und alle Dokumentsendungen.\
   Weitere Informationen zum Testen in Workfront finden Sie unter [Testversand](../../review-and-approve-work/proofing/proofing.md) Abschnitt.

* Sie können Berechtigungen für Dokumente von den Objekten erben, mit denen sie verknüpft sind. Ihr Workfront-Administrator kann die Vererbung von Berechtigungen für Dokumente auf Ihrer Zugriffsebene beschränken.

   Weitere Informationen zum Einschränken von geerbten Berechtigungen auf Dokumente finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   Sie können geerbte Berechtigungen für Dokumente manuell entfernen. Weitere Informationen finden Sie unter [Berechtigungen aus Objekten entfernen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Ein angehängtes Dokument erbt die Berechtigungen nur von dem Objekt, an das es angehängt wurde. Wenn Sie einen Ordner für das Objekt erstellen und das Dokument in den Ordner verschieben, erbt es die Berechtigungen des Ordners. Wenn Sie jedoch einen Ordner für ein übergeordnetes oder übergeordnetes Objekt erstellen und das Dokument in diesen Ordner verschieben, erbt es nicht die Berechtigungen dieses Ordners.

## Dokumentberechtigungen

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern gewähren können, wenn sie es ihnen ermöglichen, Dokumente anzuzeigen oder zu verwalten:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktion</strong> </p> </th> 
   <th> <p><strong>Verwalten</strong> </p> </th> 
   <th> <p><strong>Anzeigen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Erstellen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dokumentdetails bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Löschen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Herunterladen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Checkout</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Hinzufügen von Genehmigern</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dokument genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefiniertes Formular anfügen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefinierte Felder bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verschieben nach (Objekt)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Senden an (Integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aktualisierungen/Kommentare</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Neue Version hochladen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Version löschen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dokument(e) anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Vorschau</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Korrekturabzug**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Korrekturabzug generieren**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Korrekturabzug entfernen**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Freigeben*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Systemweit freigeben*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Dokumente öffentlich freigeben*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Freigeben mit einer externen E-Mail-Adresse</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Hinzufügen/Entfernen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Umbenennen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Link (mit Integration)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Verknüpfung aufheben (mit Integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Die Aktion wird sowohl von Dokumenten als auch von Dokumentordnern gemeinsam verwendet.

&#42;&#42; Sie müssen über eine separate Testlizenz verfügen, die mit Ihrem Workfront-Konto verknüpft ist, um Dokumente testen zu können. Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie eine Testlizenz erwerben möchten. Weitere Informationen zum Testen in Workfront finden Sie unter [Testversand](../../review-and-approve-work/proofing/proofing.md).
