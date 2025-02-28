---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopieren einer Projektvorlage
description: Anstatt eine neue Projektvorlage von Grund auf neu zu erstellen, können Sie eine vorhandene Vorlage kopieren und bei Bedarf Änderungen daran vornehmen.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 2%

---

# Kopieren einer Projektvorlage

Anstatt eine neue Projektvorlage von Grund auf neu zu erstellen, können Sie eine vorhandene Vorlage kopieren und bei Bedarf Änderungen daran vornehmen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für eine Vorlage</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.


## Überlegungen zum Kopieren von Vorlagen

Die folgenden Elemente werden immer aus einem vorhandenen Projekt in ein neues kopiert:

* Vorlagenaufgaben
* Standardinformationen zu Vorlagenaufgaben (Standardgenehmigungsprozess für Aufgaben, Standardaufgabe für benutzerdefinierte Forms)
* Benutzerdefinierte Formulare
* Risiken
* Informationen zur Warteschlangeneinrichtung
* Portfolio und Programm
* Genehmigungen
* Dokumente
* Die Tage der ursprünglichen Vorlagenaufgaben werden auf die neue Vorlage übertragen. Sie müssen das Anfangs- oder Fertigstellungstag der Vorlage (je nach Planungsmodus) ändern, um die Tage in den Vorlagenaufgaben bei Bedarf zu aktualisieren.

Die folgenden Elemente werden niemals aus einem vorhandenen Projekt in ein neues kopiert:

* Abrechnungssätze
* Benutzerkommentare

## Kopieren einer Vorlage

1. Wechseln Sie zu der Vorlage, die Sie kopieren möchten.
1. Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/qs-more-icon-on-an-object.png) und dann auf **Kopieren**.
1. Geben Sie einen Namen für die Vorlage im Feld **Neuer Vorlagenname** an.

   Standardmäßig lautet der neue Name **Kopie von `<original template name>`.**

1. Wählen Sie aus, ob **Benutzerzuweisungen für Aufgaben und Vorlagen beibehalten werden sollen**: Wählen Sie diese Option aus, um alle Aufgaben- und Vorlagenzuweisungen von der ursprünglichen Vorlage auf die neue Vorlage zu übertragen.
1. Klicken Sie **Speichern**, um eine Kopie der Vorlage zu erstellen.
