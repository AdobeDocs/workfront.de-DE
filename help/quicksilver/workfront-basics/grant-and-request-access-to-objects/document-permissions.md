---
title: Dokument freigeben
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie in Gewähren des Zugriffs auf Dokumente beschrieben.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%

---

# Dokument freigeben

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Dokumenten, wenn sie Zugriffsebenen zuweisen, wie in [Zugriff auf Dokumente gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md) beschrieben.

Die Zugriffsebene, die der Workfront-Administrator den Benutzenden gewährt, ermöglicht ihnen das Anzeigen oder Bearbeiten von Dokumenten. Darüber hinaus können andere Benutzer anderen Benutzern auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Dokumente erteilen, die sie selbst hochgeladen haben oder auf die sie Zugriff zum Freigeben haben.

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann. Informationen zu Objektberechtigungen finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Der Benutzer, der ein Dokument in Workfront hochlädt, hat standardmäßig Verwaltungsberechtigungen dafür.

Informationen zum Freigeben eines gesamten Dokumentordners finden Sie unter [Freigeben eines Dokumentordners](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um Objekte freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p> 
   Oder
   <p>Aktuell: Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Ansichtszugriff oder höher auf die Objekte, die Sie freigeben möchten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigung zum Anzeigen oder höher für die Objekte, die Sie freigeben möchten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Dokumenten

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

* Die Freigabe eines Dokuments ähnelt der Freigabe jedes anderen Objekts in Workfront. Informationen zum Freigeben von Dokumenten in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können die folgenden Berechtigungen für Dokumente gewähren:

   * Anzeigen
   * Verwalten

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

## Dokument freigeben

{{step1-to-documents}}

1. Bewegen Sie auf der **Dokumente** den Mauszeiger über das Dokument, das Sie freigeben möchten, und klicken Sie auf den **Dokumentdetails** Link, der angezeigt wird. Die **„Dokumentdetails** wird geöffnet.

   ![Link „Dokumentdetails“](assets/document-details-link.png)

1. Klicken Sie auf **Mehr**-Symbol ![Mehr](assets/more-icon.png) rechts neben dem Dokumentnamen und dann auf **Freigeben**. Das **Freigeben [Dokumentname]** wird geöffnet.

   ![Dokument freigeben](assets/share-a-document-350x160.png)

1. Beginnen Sie im Feld **Dokumentzugriff gewähren auf** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, für den bzw. die Sie das Dokument freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können ein Dokument nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Wer hat Zugriff** aus und wählen Sie die Zugriffsebene des Dokuments aus:

   * **Nur eingeladene Personen können darauf zugreifen:** Nur Benutzer, die zum Dokument eingeladen sind, können darauf zugreifen (Standard).
   * **Alle im System können anzeigen**: Alle Benutzer im System können das Dokument ohne Einladung anzeigen.

1. (Optional) Um das Dokument öffentlich zu machen, klicken Sie auf das Zahnradsymbol ![Zahnradsymbol auswählen](assets/gear-icon.png) und klicken Sie dann auf das Feld, das sich in der Reihe **Für externe Benutzer öffentlich machen** befindet. Die **Öffentlichen Link kopieren** wird am unteren Rand des Dialogfelds angezeigt.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie seine Berechtigungsstufe für dieses Dokument aus:

   * **Anzeigen**: Der Benutzer kann das Dokument überprüfen und freigeben.
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf das Programm ohne Administratorrechte, die auf Zugriffsebene gewährt werden (umfasst auch alle Anzeigeberechtigungen).

1. (Optional) Klicken Sie auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe, die Sie gewährt haben, um bestimmte Berechtigungen für das Programm zu konfigurieren.

   ![Erweiterte Berechtigungsoptionen konfiguriert](assets/advanced-options-icon.png)

1. (Optional) Um geerbte Berechtigungen für die untergeordneten Objekte des Dokuments zu deaktivieren, klicken Sie auf **Deaktivieren** Inline mit **Geerbte Berechtigungen**.

1. (Bedingt) Um den öffentlichen Link zu kopieren, über den Sie das Dokument für externe Benutzer freigeben können, klicken Sie auf **Öffentlichen Link kopieren**.

   >[!CAUTION]
   >
   >Es wird empfohlen, beim Freigeben eines Dokuments mit vertraulichen Informationen an externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne ein Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

1. Klicken Sie auf **Speichern**.


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
