---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Stapelweises Bearbeiten von Dokumenten
description: Sie können mehrere Dokumente gleichzeitig im Bereich "Dokumente"bearbeiten.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c1f829eb29d8cd13524814d98ed353add15e881
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---


# Stapelweises Bearbeiten von Dokumenten

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Sandbox-Umgebung verfügbar.</span>

Sie können die Beschreibung bearbeiten, benutzerdefinierte Formulare hinzufügen und benutzerdefinierte Formulare in mehreren Dokumenten gleichzeitig bearbeiten.

## Überlegungen beim Bearbeiten benutzerdefinierter Formulare

Beachten Sie Folgendes beim Bearbeiten von benutzerdefinierten Formularen für Dokumente in großen Mengen:

* Die Informationen, die Sie in allen ausgewählten Dokumenten ändern, überschreiben die vorhandenen Informationen in den einzelnen Dokumenten.
* Wenn Sie Dokumente mit unterschiedlichen Werten für dasselbe Feld auswählen, wird im Feld die Anzeige &quot;Mehrere Werte&quot;angezeigt. Felder, bei denen es sich um Kontrollkästchen, Optionsfelder und Umschalter handelt, weisen neben ihnen die Anzeige &quot;Mehrere Werte&quot;auf.
* Wenn Sie eine Option in einem Feld mit mehreren Optionen aktualisieren (z. B. ein Feld, das als Satz von Umschaltern oder Kontrollkästchen angezeigt wird), müssen alle anderen Optionen zwischen den ausgewählten Dokumenten übereinstimmen.

>[!BEGINSHADEBOX]

**Beispiel**
Möglicherweise verfügen Sie über ein benutzerdefiniertes Formular mit einem Kontrollkästchen mit drei Kontrollkästchen (Option1, Option 2 und Option 3) und Option 1 ist für alle ausgewählten Dokumente deaktiviert und Option 2 und 3 für einige und deaktiviert für andere Dokumente, die Sie ausgewählt haben. Wenn Sie Option 1 für alle Dokumente aktivieren möchten, müssen Sie auch Option 2 und 3 für alle ausgewählten Projekte abgleichen, bevor Sie Ihre Änderungen speichern können. Sie müssen sie also entweder auswählen oder die Auswahl aufheben, damit sie für alle ausgewählten Projekte übereinstimmen können. Wenn Sie keine der Optionen ändern, können Sie das Feld unverändert speichern und die Dokumente behalten ihre aktuelle Auswahl für alle Optionen bei.

>[!ENDSHADEBOX]

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td><p> Neu: Mitarbeiter oder höher</p> 
   <p> Aktuell: Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Dokument verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Stapelweises Bearbeiten von Dokumenten

So bearbeiten Sie Dokumente stapelweise:

1. Navigieren Sie im Hauptmenü zur Registerkarte Dokumente eines Projekts oder zum Bereich Dokumente .
1. Drücken Sie die Strg- oder Befehlstaste auf der Tastatur und wählen Sie die Dokumente aus, die Sie bearbeiten möchten.
1. Klicken Sie auf das Bearbeitungssymbol ![Bearbeitungssymbol](assets/edit-icon.png).
   ![Bearbeitungs-Symbolposition auf Seite](assets/edit-multiple-documents.png)
1. (Optional) Fügen Sie die **Beschreibung** hinzu oder bearbeiten Sie sie. Wenn die Beschreibung in den einzelnen Dokumenten unterschiedlich ist, wird im Beschreibungsfeld _Mehrere Werte_ angezeigt. Sie können dieselbe Beschreibung für alle Dokumente hinzufügen, aber Sie können einzelne Dokumentbeschreibungen nicht bearbeiten, wenn Sie sie stapelweise bearbeiten.
1. Nehmen Sie die folgenden Änderungen mit benutzerdefinierten Formularen vor:

   <table>
    <tr>
    <td><strong>Formulare hinzufügen</strong></td>
    <td>Im Feld <strong>Benutzerdefiniertes Formular hinzufügen</strong> können Sie aus den hinzugefügten Formularen und Formularen auswählen. Die angehängten Formulare beziehen sich auf einige der ausgewählten Dokumente, jedoch nicht auf alle. Ein Formular, das an das gesamte ausgewählte Dokument angehängt ist, wird automatisch im Bearbeitungsfenster angezeigt.  </td>
    </tr>
    <tr>
    <td><strong>Formulare bearbeiten</strong></td>
    <td>Bearbeiten Sie alle angehängten benutzerdefinierten Formulare. Die Informationen, die Sie ändern, überschreiben die vorhandenen Informationen zu einzelnen Dokumenten. Felder mit unterschiedlichen Werten für verschiedene Dokumente werden als "Mehrere Werte"angezeigt. </td>
    </tr>
    <tr>
    <td><strong>Formulare neu anordnen</strong></td>
    <td>Klicken Sie auf das benutzerdefinierte Formular und ziehen Sie es, um es neu anzuordnen.</td>
    </tr>
    </table>
1. Klicken Sie auf **Speichern**.


