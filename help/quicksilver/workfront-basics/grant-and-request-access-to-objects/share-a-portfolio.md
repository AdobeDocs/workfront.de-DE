---
title: Portfolio freigeben
description: Sie können ein Portfolio für andere Benutzer freigeben, wenn Sie über die Berechtigung zum Zugriff darauf verfügen.
author: Courtney
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 3%

---

# Portfolio freigeben

Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Portfolios gewähren. Sie müssen über eine Plan-Lizenz verfügen, um Zugriff zum Bearbeiten eines Portfolios zu erhalten. Weitere Informationen finden Sie unter [Zugriff auf Portfolios gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Neben der Ihnen gewährten Zugriffsebene können Sie auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Portfolios von Benutzern erhalten, die diese für Sie freigeben können. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Funktionsweise von Zugriffsebenen und Berechtigungen](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen Benutzende für dieses Element ausführen können.


## Zugriffsanforderungen

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
   <td> <p>Standard</p> 
   <p>Work oder höher</p> 
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

## Überlegungen zur Freigabe von Portfolios

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

* Der Ersteller eines Portfolios hat standardmäßig Verwaltungsberechtigungen dafür.
* Sie können ein Portfolio einzeln freigeben oder mehrere Portfolios gleichzeitig freigeben. Die Freigabe eines Portfolios ist mit der Freigabe anderer Objekte in Workfront identisch. Weitere Informationen finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Sie können nur Anzeigen- oder Verwaltungsberechtigungen für Portfolios erteilen.
</span>
* Wenn Sie ein Portfolio gemeinsam nutzen, erben Benutzer standardmäßig dieselben Berechtigungen für alle untergeordneten Objekte, die mit dem Portfolio verknüpft sind.

Weitere Informationen zur Objekthierarchie in Workfront finden Sie unter [Grundlegendes zu Objekten in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Sie können geerbte Berechtigungen aus der Portfolio entfernen. Weitere Informationen zum Entfernen von Berechtigungen aus Objekten finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Portfolio freigeben

{{step1-to-portfolios}}

1. Wählen Sie auf **Seite** das Portfolio aus, das Sie freigeben möchten. Die Portfolioseite wird geöffnet.

1. Klicken Sie rechts neben dem Portfolionamen auf &quot;**&quot;**. Das **Freigeben von [Portfolio-]**&quot; wird geöffnet.

   ![Schaltfläche „Portfolio freigeben“](assets/share-portfolio-button.png)

1. Beginnen Sie im Feld **Portfoliozugriff gewähren auf** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, für den bzw. die Sie das Portfolio freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können ein Portfolio nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Wer hat Zugriff** Dropdown-Liste und wählen Sie die Zugriffsebene des Portfolios:

   * **Nur eingeladene Personen können darauf zugreifen:** Nur Benutzer, die zum Portfolio eingeladen sind, können darauf zugreifen (Standard).
   * **Alle im System können anzeigen**: Alle Benutzer im System können das Portfolio ohne Einladung anzeigen.

1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie seine Berechtigungsstufe für dieses Portfolio aus:

   * **Anzeigen**: Der Benutzer kann das Portfolio überprüfen und freigeben.
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf das Portfolio ohne Administratorrechte, die auf Zugriffsebene gewährt werden (umfasst auch alle Anzeigeberechtigungen).

1. (Optional) Klicken Sie auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe, die Sie gewährt haben, um bestimmte Berechtigungen für das Portfolio zu konfigurieren.

   ![Erweiterte Berechtigungsoptionen konfiguriert](assets/advanced-options-icon.png)

1. (Optional) Um das Portfolio mithilfe eines Links schnell freizugeben, klicken Sie auf **Link kopieren** und leiten Sie es dann an den Empfänger weiter.

1. Klicken Sie auf **Speichern**.

## Portfolios in Massen teilen

{{step1-to-portfolios}}

1. Aktivieren **auf** Seite „Portfolios“ das Kontrollkästchen links neben jedem Portfolio, das Sie freigeben möchten, und klicken Sie dann oben auf der Seite auf **Freigeben**-Symbol ![Freigeben](assets/share-icon.png). Das Modal „Freigeben“ wird geöffnet.

   ![Massenfreigabe-Portfolios](assets/bulk-share-portfolios.png)

1. Beginnen Sie im Feld **Zugriff auf Portfolios gewähren** mit der Eingabe des Namens des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens, für den bzw. die Sie die Portfolios freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können Portfolios nur für aktive Benutzer, Teams, Rollen oder Unternehmen freigeben.


1. (Optional) Wählen Sie die **Wer hat Zugriff** Dropdown-Liste und wählen Sie die Zugriffsebene des Portfolios:

   * **Nur eingeladene Personen können zugreifen:** Nur Benutzer, die zu den Portfolios eingeladen sind, können darauf zugreifen (Standard).
   * **Alle im System können anzeigen**: Alle Benutzer im System können die Portfolios ohne Einladung anzeigen.


1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen des Benutzers und wählen Sie seine Berechtigungsstufe für die Portfolios aus:

   * **Anzeigen**: Der Benutzer kann die Portfolios überprüfen und freigeben.
   * **Verwalten**: Der Benutzer hat vollen Zugriff auf die Portfolios ohne Administratorrechte, die auf Zugriffsebene gewährt werden (umfasst auch alle Anzeigeberechtigungen).

1. (Optional) Klicken Sie auf das Symbol Erweiterte Optionen neben der Berechtigungsstufe, die Sie gewährt haben, um bestimmte Berechtigungen für die Portfolios zu konfigurieren.

   ![Erweiterte Berechtigungsoptionen konfiguriert](assets/advanced-options-icon.png)

1. Klicken Sie auf **Speichern**.


## Portfolio-Berechtigungen

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern erteilen können, wenn sie eine Portfolio anzeigen oder verwalten möchten:

| **Aktionen** | **Verwalten** | **Anzeigen** |
|---|---|---|
| Portfolio-Details bearbeiten | ✓ |   |
| Anzeigen einer Portfolio | ✓ | ✓ |
| Löschen einer Portfolio | ✓ |   |
| Benutzerdefiniertes Formular anhängen | ✓ |   |
| Benutzerdefiniertes Feld bearbeiten | ✓ |   |
| Ein Programm hinzufügen oder entfernen&#42; | ✓ |   |
| Ein Projekt hinzufügen oder entfernen&#42; | ✓ |   |
| Genehmigen eines Projekts | ✓ |   |
| Portfolio-Optimierung&#42; | ✓ |   |
| Dokumentenordner hinzufügen&#42; | ✓ | ✓ |
| Dokument hinzufügen | ✓ | ✓ |
| Aktualisierungen/Kommentare | ✓ | ✓ |
| Freigeben | ✓ | ✓ |
| Systemweit freigeben |   | ✓ |

*Diese Berechtigungen werden durch die Zugriffsebene und Berechtigungen für andere Objekte wie Projekte, Programme und Dokumente gesteuert.
