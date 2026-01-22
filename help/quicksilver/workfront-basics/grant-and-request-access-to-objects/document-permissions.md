---
title: Eine Dokument freigeben
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Systems Workfront-Administrator gewährt Benutzern Zugriff auf Ansicht oder bearbeitete Dokumente, wenn sie Zugriffsebenen zuweisen, wie unter Zugriff auf Dokumente gewähren erläutert.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 5%

---

# Dokument freigeben

Der Workfront-Administrator steuert, wer Dokumente im Bereich „Zugriffsebenen“ im Setup anzeigen oder bearbeiten kann. Weitere Informationen finden Sie unter [Zugriff auf Dokumente gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Benutzer können auch Dokumente teilen, die sie hochgeladen haben oder auf die sie Zugriff haben, und anderen Berechtigung geben, sie zu Ansicht oder zu managen.

* Berechtigungen gelten für Kontakt Elemente und definieren, welche Aktionen ausgeführt werden können.
* Die Person, die eine Dokument hochlädt, erhält automatisch die volle Kontrolle (Berechtigungen verwalten).
* Informationen zum Freigeben eines gesamten Ordners finden Sie unter [Freigeben eines Dokument Ordners](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

>[!NOTE]
>
>Wenn Ihr Workfront Instanz Adobe Systems Enterprise-Datenspeicherung verwendet, können Sie Kontakt Dokumente nicht freigeben. Stattdessen gewähren Sie den Zugriff auf Projektebene. Denken Sie daran, dass die Freigabe des Projekts je nach gewählter Berechtigung Zugriff auf sensible Projektinformationen liken Finanzen gewähren kann.



## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Ansichtszugriff oder höher auf die Objekte, die Sie freigeben möchten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekt Berechtigungen</td> 
   <td> <p>Ansicht mindestens Berechtigungen für die Objekte ein, die Sie freigeben möchten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Eine Dokument freigeben

Der User, der eine Dokument in Workfront hochlädt, verfügt standardmäßig über Verwaltungsberechtigungen.

{{step1-to-documents}}

1. Bewegen Sie den Mauszeiger auf der **Dokumente** Seite über die Dokument, die Sie freigeben möchten, und klicken Sie auf das **angezeigte Dokument Details verknüpfen** . Der **Seite Dokumentdetails** wird geöffnet.

   ![Dokument Details verknüpfen](assets/document-details-link.png)

1. Klicken Sie auf das **Mehr** Symbol ![Mehr rechts](assets/more-icon.png) neben dem Namen der Dokument und dann auf **&quot;Teilen**&quot;. Das **Dialogfeld &quot;Dokumentnamen[ freigeben]**&quot; wird geöffnet.

   ![Eine Dokument freigeben](assets/share-a-document-350x160.png)

1. Beginnen Sie im **Feld &quot;Zugriff Dokument gewähren** &quot; mit der Eingabe des Namens des User, des Team, des Rolle, Gruppe oder der Firma, für die Sie die Dokument freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können eine Dokument nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Dropdownliste Wer hat Zugriff** und dann die Zugriffsebene des Dokument aus:

   * **Nur eingeladene Personen können darauf zugreifen:** Nur Benutzer, die zum Dokument eingeladen wurden, können darauf zugreifen (Standardmäßig).
   * **Jeder im System kann Ansicht**: Alle Benutzer im System können die Dokument ohne Einladung Ansicht.

1. (Optional) Um die Dokument öffentlich zu machen, klicken Sie auf das Zahnradsymbol ![Wählen Sie das Zahnradsymbol](assets/gear-icon.png) aus und klicken Sie dann auf das Kästchen neben Für externe Benutzer **öffentlich machen**. Die **Button Kopie öffentlichen verknüpfen** wird am unteren Rand des Dialogfelds angezeigt.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen der User und wählen Sie die Berechtigung Ebene für diese Dokument aus:

   * **Ansicht**: Benutzer können die Dokument überprüfen und freigeben.
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf die Dokument ohne Administratorrechte, die auf der Zugriffsebene gewährt werden (umfasst auch alle Ansicht Berechtigungen).

1. (Optional) Klicken Sie auf das Symbol &quot;Erweiterte Optionen&quot; neben der Berechtigung-Stufe, die Sie erteilt haben, um bestimmte Berechtigungen für die Dokument zu konfigurieren.

   ![Erweiterte Berechtigung Optionen konfiguriert](assets/advanced-options-icon.png)

1. (Optional) Um geerbte Berechtigungen für die untergeordneten Objekte des Dokument zu deaktivieren, klicken Sie auf Inline-Berechtigungen **deaktivieren** mit **geerbten Berechtigungen**.

1. (Bedingt) Klicken Sie zum Kopieren der öffentlichen verknüpfen, die es Ihnen ermöglicht, die Dokument für externe Benutzer freizugeben, auf Kopie **öffentliche verknüpfen**.

   >[!CAUTION]
   >
   >Gehen Sie bei der Freigabe von Dokument mit vertrauliche Informationen für externe Benutzer vorsichtig vor. Auf diese Weise können sie Informationen Ansicht, ohne ein Workfront-User oder Teil Ihrer Organisation zu sein.

1. Klicken Sie auf **Speichern**.

## Dokumente in Massen freigeben

{{step1-to-documents}}

1. Halten Sie auf der Registerkarte **Alle Dokumente** auf der Seite **Dokumente** die **Befehl** (Mac) oder **Strg** (Windows) gedrückt und klicken Sie auf jedes Dokument, das Sie freigeben möchten.

1. Klicken Sie oben auf der Seite auf das Symbol **Freigeben** (Symbol ![Freigeben](assets/share-icon.png). Das Modal „Freigeben“ wird geöffnet.

   ![Teilen-Symbol](assets/share-documents-in-bulk.png)

1. Beginnen Sie im **Feld &quot;Zugriff Dokument gewähren** &quot; mit der Eingabe des Namens des User, der Team, des Rolle, des Gruppe oder der Firma, für die Sie die Dokumente freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können Dokumente nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Dropdown-Liste &quot;Wer hat Zugriff** &quot; aus, und wählen Sie die Zugriffsebene der Dokumente aus:

   * **Nur eingeladene Personen können darauf zugreifen:** Nur Benutzer, die zum Dokumente eingeladen wurden, können darauf zugreifen (Standardmäßig).
   * **Jeder im System kann Ansicht**: Alle Benutzer im System können die Dokumente ohne Einladung Ansicht.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen der User und wählen Sie die Berechtigung Ebene für die Dokumente aus:

   * **Ansicht**: Benutzer können die Dokumente überprüfen und freigeben.
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf die Dokumente ohne Administratorrechte, die auf der Zugriffsebene gewährt werden (umfasst auch alle Ansicht Berechtigungen).

1. (Optional) Klicken Sie auf das Symbol &quot;Erweiterte Optionen&quot; neben der Berechtigung Ebene, die Sie erteilt haben, um bestimmte Berechtigungen für die Dokumente zu konfigurieren.

   ![Erweiterte Berechtigung Optionen konfiguriert](assets/advanced-options-icon.png)

1. Klicken Sie auf **Speichern**.

## Gemeinsame Nutzung Adobe Systems Dokuments mit  Datenspeicherung

Workfront stellt auf die Adobe Systems Enterprise-Datenspeicherung-Lösung um, bestellen eine bessere Konnektivität mit Adobe Creative Cloud Produkten zu bieten. Bestehende Kunden werden in Phasen in das neue Modell verschoben. Weitere Informationen zu den Vorteilen Adobe Systems Enterprise-Datenspeicherung finden Sie Visit [Adobe Systems](/help/quicksilver/review-and-approve-work/esm-overview.md) Enterprise Datenspeicherung Übersicht.

Wenn Ihre Workfront-Instanz Adobe Enterprise Storage verwendet, können Sie einzelne Dokumente nicht direkt freigeben. Stattdessen müssen Sie Zugriff auf Projektebene gewähren.

>[!IMPORTANT]
>
>Durch die Freigabe eines Projekts können Benutzer auch Zugriff auf vertrauliche Projektinformationen, wie z. B. Finanzen, erhalten, je nachdem, welche Berechtigung Ebene Sie auswählen.
>
>Lesen Sie Berechtigung Einstellungen sorgfältig durch, bevor Sie sie freigeben.

## Berechtigungen für Dokumente

Berechtigungen gelten nur für ein Element in Workfront und definieren, welche Aktionen für dieses Element ausgeführt werden können. Weitere Informationen zu Objektberechtigungen finden Sie unter [Übersicht über die Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern erteilen können, wenn Sie ihnen erlauben, Dokumente zu Ansicht oder zu managen:

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
   <td scope="row">Kasse</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">hinzufügen Genehmigende Personen</td> 
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
   <td scope="row">Benutzerdefinierte Felder Bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verschieben zu (Objekt)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Senden an (Integration)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aktualisierungen/ Kommentare</td> 
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
   <td scope="row">Dokument(e) Ansicht</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Vorschau</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Beweis**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Testversand generieren**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Entfernen Test**</td> 
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
   <td scope="row">hinzufügen/ Entfernen</td> 
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

&#42; Aktion wird sowohl von Dokumenten als auch von Dokumentordnern verwendet.

&#42;&#42; Sie müssen über eine separate Proofing-Lizenz für Ihr Workfront-Konto verfügen, um Dokumente prüfen zu können. Wenden Sie sich an Ihren Account Manager, um eine Proofing-Lizenz zu erwerben. Weitere Informationen zum Korrekturlesen in Workfront finden Sie unter [Korrekturlesen](../../review-and-approve-work/proofing/proofing.md).

## Überlegungen zum Freigeben von Dokumente

Zusätzlich zu den folgenden Überlegungen finden Sie auch unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann Berechtigungen für alle Elemente im System für alle Benutzer hinzufügen oder entfernen, ohne der Verantwortlicher dieser Elemente zu sein.

* Die Freigabe einer Dokument ist ähnlich wie die Freigabe anderer Objekte in Workfront. Weitere Informationen zum Freigeben von Dokumente in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können Dokumente die folgenden Berechtigungen erteilen:

   * Ansicht
   * Verwalten

* Sie können ein Dokument auch öffentlich oder systemweit freigeben.

  >[!CAUTION]
  >
  >Es wird empfohlen, bei der Freigabe eines Objekts, das vertrauliche Informationen enthält, für externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen Ansicht, ohne ein Workfront-User oder Teil Ihrer Organisation zu sein.

* Sie können eine Dokument für eine Person freigeben, die nicht über eine Workfront-Konto verfügt, indem Sie deren E-Mail-Adresse in das Feld Dokument Zugriff geben auf hinzufügen.
* Wenn Sie eine Dokument freigeben, haben Benutzer denselben Zugriff auf alle Dokument Versionen und alle Dokument Testsendungen.\
  Weitere Informationen zum Korrekturlesen in Workfront finden Sie im [Abschnitt Korrekturlesen](../../review-and-approve-work/proofing/proofing.md) .

* Sie können Berechtigungen für Dokumente von den Objekten vererben, mit denen sie verknüpft sind. Ihr Workfront-Administrator kann die Vererbung von Berechtigungen für Dokumente in Ihrer Zugriffsebene einschränken.

  Weitere Informationen zum Beschränken von geerbten Berechtigungen für Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Sie können geerbte Berechtigungen für Dokumente manuell entfernen. Weitere Informationen finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* Ein angehängtes Dokument erbt nur Berechtigungen von dem Objekt, an das es angehängt wurde. Wenn Sie einen Ordner für das Objekt erstellen und das Dokument in den Ordner verschieben, übernimmt es die Berechtigungen des Ordners. Wenn Sie jedoch einen Ordner auf einem übergeordneten oder übergeordneten Objekt erstellen und das Dokument in diesen Ordner verschieben, werden die Berechtigungen dieses Ordners nicht übernommen.