---
title: Dokument freigeben
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie in Gewähren des Zugriffs auf Dokumente beschrieben.
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: b4e90918c5f499638d0cf5355dc75c3ceca48293
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Dokument freigeben

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie in [Zugriff auf Dokumente gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md) beschrieben.

Die Zugriffsebene, die der Workfront-Administrator den Benutzenden gewährt, ermöglicht ihnen das Anzeigen oder Bearbeiten von Dokumenten. Darüber hinaus können andere Benutzer anderen Benutzern auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dokumente erteilen, die sie selbst hochgeladen haben oder auf die sie Zugriff zum Freigeben haben.

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann. Informationen zu Objektberechtigungen finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Der Benutzer, der ein Dokument in Workfront hochlädt, hat standardmäßig Verwaltungsberechtigungen dafür.

Informationen zum Freigeben eines gesamten Dokumentordners finden Sie unter [Freigeben eines Dokumentordners](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Überlegungen zur Freigabe von Dokumenten

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

* Die Freigabe eines Dokuments ähnelt der Freigabe jedes anderen Objekts in Workfront. Informationen zum Freigeben von Dokumenten in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können die folgenden Berechtigungen für Dokumente gewähren:

   * Anzeigen
   * Verwalten

  <span class="preview">In Vorschau:
  ![](assets/document-permissions.png)
</span>

* Sie können ein Dokument auch öffentlich oder systemweit freigeben.

  >[!CAUTION]
  >
  >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen an externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne ein Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

* Sie können ein Dokument für Personen ohne Workfront-Konto freigeben, indem Sie deren E-Mail-Adresse im Feld Dokumentzugriff erteilen an hinzufügen.
* Wenn Sie ein Dokument freigeben, haben Benutzer denselben Zugriff auf alle Dokumentversionen und alle Korrekturabzüge für Dokumente.\
  Weitere Informationen zu Proofing in Workfront finden Sie im Abschnitt [Proofing](../../review-and-approve-work/proofing/proofing.md).

* Sie können Berechtigungen für Dokumente von den Objekten erben, mit denen sie verknüpft sind. Ihr Workfront-Administrator kann die Vererbung von Berechtigungen für Dokumente auf Ihrer Zugriffsebene einschränken.

  Weitere Informationen zum Beschränken von geerbten Berechtigungen für Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Sie können geerbte Berechtigungen für Dokumente manuell entfernen. Weitere Informationen finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Ein angehängtes Dokument erbt nur Berechtigungen von dem Objekt, an das es angehängt wurde. Wenn Sie einen Ordner für das Objekt erstellen und das Dokument in den Ordner verschieben, übernimmt es die Berechtigungen des Ordners. Wenn Sie jedoch einen Ordner auf einem übergeordneten oder übergeordneten Objekt erstellen und das Dokument in diesen Ordner verschieben, werden die Berechtigungen dieses Ordners nicht übernommen.

## Dokumentberechtigungen

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern erteilen können, wenn sie Dokumente anzeigen oder verwalten können:

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
   <td scope="row">Download</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Checkout</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Genehmigende Personen hinzufügen</td> 
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
   <td scope="row">Korrekturabzug erstellen**</td> 
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
   <td scope="row">Für externe E-Mail-Adressen freigeben</td> 
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
   <td scope="row">Relation (mit Integration)</td> 
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

&#42; Aktion wird sowohl von Dokumenten als auch von Dokumentordnern verwendet.

&#42;&#42; Sie müssen über eine separate Proofing-Lizenz für Ihr Workfront-Konto verfügen, um Dokumente prüfen zu können. Wenden Sie sich an Ihren Account Manager, um eine Proofing-Lizenz zu erwerben. Weitere Informationen zu Proofing in Workfront finden Sie unter [Proofing](../../review-and-approve-work/proofing/proofing.md).
