---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopieren einer Projektvorlage
description: Sie können eine Projektvorlage nicht nur von Grund auf neu erstellen, sondern auch kopieren und ändern.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 3%

---

# Kopieren einer Projektvorlage

<!--Audited: 5/2025-->

Sie können eine Projektvorlage nicht nur von Grund auf neu erstellen, sondern auch kopieren und in Adobe Workfront ändern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

Sie benötigen den folgenden Zugriff.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für eine Vorlage</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zum Kopieren von Vorlagen

Die folgenden Elemente werden immer von einer vorhandenen Vorlage in eine neue kopiert:

* Vorlagenaufgaben
* Standardinformationen zu Vorlagenaufgaben (Standardgenehmigungsprozess für Aufgaben, Standardaufgabe für benutzerdefinierte Forms)
* Benutzerdefinierte Formulare
* Risiken
* Informationen zur Warteschlangeneinrichtung
* Portfolio und Programm
* Genehmigungen
* Dokumente
* Die Tage der ursprünglichen Vorlagenaufgaben werden auf die neue Vorlage übertragen. Sie müssen das Anfangs- oder Fertigstellungstag der Vorlage (je nach Planungsmodus) ändern, um die Tage in den Vorlagenaufgaben bei Bedarf zu aktualisieren.

Die folgenden Elemente werden niemals aus einer vorhandenen Vorlage in eine neue kopiert:

* Abrechnungssätze
* Benutzerkommentare

## Kopieren einer Vorlage

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Wechseln Sie zu der Vorlage, die Sie kopieren möchten.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) rechts neben dem Vorlagennamen in der Kopfzeile und klicken Sie dann auf **Kopieren**.

   Das Feld **Vorlage kopieren** wird geöffnet.

   ![Feld „Vorlage kopieren“](assets/copy-template-box.png)

1. Geben Sie einen Namen für die Vorlage im Feld **Neuer Vorlagenname** an.

   Standardmäßig legt Workfront den neuen Namen in diesem Format fest: `Copy of Original template name`.

1. Wählen Sie die Option **Benutzerzuweisungen für Aufgaben und Vorlagen beibehalten**, wenn Sie alle Aufgaben- und Vorlagenzuweisungen von der ursprünglichen Vorlage in die neue Vorlage übernehmen möchten. Vorlagenaufgabenzuweisungen und der Vorlagenbesitzer sowie der Sponsor werden zur kopierten Vorlage übertragen.
1. Klicken Sie **Speichern**, um eine Kopie der Vorlage zu erstellen.

   Die neue Vorlage wird in der Vorlagenliste im Vorlagenbereich von Workfront angezeigt.
