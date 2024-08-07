---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopieren einer Projektvorlage
description: Anstatt eine neue Projektvorlage von Grund auf neu zu erstellen, können Sie eine vorhandene Vorlage kopieren und bei Bedarf Änderungen daran vornehmen.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

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
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für eine Vorlage</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.


## Überlegungen zum Kopieren von Vorlagen

Die folgenden Elemente werden immer aus einem vorhandenen Projekt in ein neues kopiert:

* Vorlagenaufgaben
* Standardinformationen für Vorlagenaufgaben (Prozess für die Standardgenehmigung für Aufgaben, Standardbenutzerdefinierter Forms für Aufgaben)
* Benutzerdefinierte Formulare
* Risiken
* Informationen zur Warteschlangeneinrichtung
* Portfolio und Programm
* Genehmigungen
* Dokumente
* Die Tage der ursprünglichen Vorlagenaufgaben werden auf die neue Vorlage übertragen. Sie müssen den Start- oder Fertigstag der Vorlage ändern (je nach Planungsmodus), um bei Bedarf die Tage für die Vorlagenaufgaben zu aktualisieren.

Die folgenden Elemente werden nie aus einem vorhandenen Projekt in ein neues kopiert:

* Abrechnungssätze
* Benutzerkommentare

## Eine Vorlage kopieren

1. Markieren Sie die Vorlage, die Sie kopieren möchten.
1. Klicken Sie auf das Menü **Mehr** ![](assets/qs-more-icon-on-an-object.png) und dann auf **Kopieren**.
1. Geben Sie im Feld **Neuer Vorlagenname** einen Namen für die Vorlage an.

   Standardmäßig lautet der neue Name **Kopie von `<original template name>`.**

1. Wählen Sie aus, ob Sie **Benutzerzuweisungen für Aufgaben und Vorlagen beibehalten** möchten: Wählen Sie diese Option aus, um alle Aufgaben- und Vorlagenzuweisungen aus der ursprünglichen Vorlage in die neue Vorlage zu übertragen.
1. Klicken Sie auf **Speichern** , um eine Kopie der Vorlage zu erstellen.
