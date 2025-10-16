---
title: Freigeben einer Aufgabe
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen Zugriff zum Anzeigen oder Bearbeiten von Aufgaben gewähren, wenn er Zugriffsebenen zuweist. Weitere Informationen zum Gewähren des Zugriffs auf Aufgaben finden Sie unter Gewähren des Zugriffs auf Aufgaben.
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 6%

---

# Freigeben einer Aufgabe

Ihr Adobe Workfront-Administrator kann Ihnen Zugriff zum Anzeigen oder Bearbeiten von Aufgaben gewähren, wenn er Zugriffsebenen zuweist. Weitere Informationen zum Gewähren des Zugriffs auf Aufgaben finden Sie unter [Zugriff auf Aufgaben gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen, Mitwirken oder Verwalten bestimmter Aufgaben erteilen, auf die Sie Zugriff haben.

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <td> <p>Standard</p> 
   <p>Arbeit oder höher</p> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe einer Aufgabe

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Der Ersteller einer Aufgabe hat standardmäßig Verwaltungsberechtigungen dafür.
* Sie können Aufgaben einzeln oder gemeinsam mit mehreren gleichzeitig ausführen.\
  Die Freigabe von Aufgaben ist mit der Freigabe anderer Objekte identisch. Weitere Informationen zum Freigeben von Elementen in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Sie können einer Aufgabe die folgenden Berechtigungen erteilen: 

   * Ansicht
   * Verwalten
   * Mitwirken
* Wenn Sie eine Aufgabe freigeben, erben Benutzer standardmäßig dieselben Berechtigungen für alle untergeordneten Objekte, die mit der Aufgabe verknüpft sind. Beispielsweise erben sie dieselben Berechtigungen für die untergeordneten Aufgaben, Probleme und Dokumente, die an die Aufgabe angehängt sind.\
  Weitere Informationen zur Hierarchie von Objekten in Workfront finden Sie unter  [Verstehen von Objekten in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Der Workfront-Administrator kann angeben, ob Dokumente Berechtigungen von höheren Objekten auf der Zugriffsebene der Benutzenden erben sollen. Weitere Informationen zum Beschränken von geerbten Berechtigungen für Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Sie können geerbte Berechtigungen aus einer Aufgabe entfernen.\
  Weitere Informationen zum Entfernen geerbter Berechtigungen von Objekten finden Sie unter  [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Möglichkeiten zum Freigeben einer Aufgabe

Sie können eine Aufgabe wie folgt freigeben:

* Manuell, entweder einzeln oder stapelweise.

* Gehen Sie wie folgt automatisch vor:

   * Geben Sie die Berechtigungen für eines der übergeordneten Objekte der Aufgabe an: Projekt, Programm oder Portfolio. Aufgaben erben die Berechtigungen von ihren übergeordneten Objekten. Weitere Informationen zum Anzeigen geerbter Berechtigungen für Objekte finden Sie unter [Anzeigen geerbter Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Entitäten zur Projektfreigabe hinzufügen, die auf einer Vorlage basieren, mit der das Projekt erstellt wurde, für das die Aufgabe ausgeführt wird. Informationen zum Freigeben von Projekten aus Vorlagen finden Sie unter [Freigeben einer Vorlage](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Geben Sie die Berechtigungen für alle Aufgaben in einem Projekt an, wenn Sie das Projekt bearbeiten. Informationen zur Verwaltung des Zugriffs auf Aufgaben im Projekt auf der Grundlage der Berechtigungen, die ein Benutzer für das Projekt erhält, finden Sie im [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) Abschnitt im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Wenn Sie nicht angeben, welche Aufgabenberechtigungen Benutzerinnen und Benutzer haben sollen, wenn sie den Aufgaben im Projekt zugewiesen werden, erhalten sie standardmäßig dieselben Berechtigungen wie für das Projekt.

## Freigeben einer Aufgabe

1. Navigieren Sie zu der Aufgabe, die Sie freigeben möchten.

1. Klicken Sie rechts neben dem Aufgabennamen auf &quot;**&quot;**. Das **Freigeben [Aufgabenname]** wird geöffnet.

   ![Schaltfläche „Aufgabe freigeben“](assets/share-task-button.png)

1. Beginnen Sie im Feld **Zugriff auf Aufgabe gewähren** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, für den/die Sie die Aufgabe freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können eine Aufgabe nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Wer hat Zugriff** aus und wählen Sie die Zugriffsebene der Aufgabe aus:

   * **Nur eingeladene Personen können darauf zugreifen:** Nur Benutzer, die zur Aufgabe eingeladen sind, können darauf zugreifen (Standard).
   * **Alle im System können anzeigen**: Alle Benutzer im System können die Aufgabe ohne Einladung anzeigen.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie seine Berechtigungsstufe für diese Aufgabe aus:

   * **Anzeigen**: Der Benutzer kann die Aufgabe überprüfen und freigeben.
   * **Beitragen**: Benutzende können Aktualisierungen vornehmen, Informationen protokollieren, kleinere Änderungen vornehmen und die Aufgabe freigeben (einschließlich aller Anzeigeberechtigungen).
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf die Aufgabe ohne Administratorrechte, die auf Zugriffsebene gewährt werden (umfasst auch alle Anzeigen- und Beitragsberechtigungen).

1. (Optional) Klicken Sie auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe, die Sie gewährt haben, um bestimmte Berechtigungen für die Aufgabe zu konfigurieren.

   ![Erweiterte Berechtigungsoptionen konfiguriert](assets/advanced-permission-options.png)

1. (Optional) Um geerbte Berechtigungen für die untergeordneten Objekte der Aufgabe zu deaktivieren, klicken Sie auf **Deaktivieren** inline mit **Geerbte Berechtigungen**.

1. (Optional) Um die Aufgabe mithilfe eines Links schnell freizugeben, klicken Sie auf **Link kopieren** und leiten Sie sie dann an den Empfänger weiter.

1. Klicken Sie auf **Speichern**.


## Aufgaben stapelweise freigeben

1. Navigieren Sie zu dem Projekt, das die Aufgaben enthält, die Sie freigeben möchten.

1. Wählen **auf der** „Aufgaben“ links neben jeder Aufgabe, die Sie freigeben möchten, das Kästchen aus und klicken Sie dann oben auf der Seite auf **Freigeben**-Symbol ![Freigeben](assets/share-icon.png). Das Modal „Freigeben“ wird geöffnet.

   ![Massenfreigabe-Aufgaben](assets/bulk-share-tasks.png)

1. Beginnen Sie im Feld **Zugriff auf Aufgabe gewähren** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, für den bzw. die Sie die Aufgaben freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können Aufgaben nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Wer hat Zugriff** aus und wählen Sie die Zugriffsebene der Aufgaben aus:

   * **Nur eingeladene Personen können zugreifen:** Nur Benutzer, die zu den Aufgaben eingeladen sind, können darauf zugreifen (Standard).
   * **Alle im System können anzeigen**: Alle Benutzer im System können die Aufgaben ohne Einladung anzeigen.


1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie seine Berechtigungsstufe für die Aufgaben aus:

   * **Anzeigen**: Der Benutzer kann die Aufgaben überprüfen und freigeben.
   * **Beitragen**: Benutzende können Aktualisierungen vornehmen, Informationen protokollieren, kleinere Änderungen vornehmen und die Aufgaben freigeben (einschließlich aller Anzeigeberechtigungen).
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf die Aufgaben ohne Administratorrechte, die auf Zugriffsebene gewährt werden (umfasst auch alle Anzeigen- und Beitragsberechtigungen).

1. (Optional) Klicken Sie auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe, die Sie gewährt haben, um bestimmte Berechtigungen für die Aufgaben zu konfigurieren.

   ![Erweiterte Berechtigungsoptionen konfiguriert](assets/advanced-permission-options.png)

1. Klicken Sie auf **Speichern**.

## Aufgabenberechtigungen

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern erteilen können, wenn Sie ihnen das Anzeigen, Mitwirken oder Verwalten einer Aufgabe ermöglichen:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong> </th> 
   <th><strong>Verwalten</strong> </th> 
   <th><strong>Beitragen</strong> </th> 
   <th><strong>Anzeigen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Aufgabe(n) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Vorgänger hinzufügen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Anfrage(n) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe löschen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Allgemeine Aufgabenbearbeitung<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabenstatus ändern</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabenbeschränkung bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dokument(e) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe kopieren*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe verschieben*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Stunden protokollieren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Geplante Daten ändern</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Zuweisung akzeptieren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Zuweisung vornehmen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefiniertes Formular anfügen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefinierte Felder bearbeiten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Erstellen eines Genehmigungsprozesses</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe genehmigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Finanzen bearbeiten*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Kosten hinzufügen/bearbeiten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Finanzen anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aktualisierungen/Kommentare</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Freigeben</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Systemweit teilen</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wird von der Zugriffsebene und den Berechtigungen für das Projekt gesteuert.
