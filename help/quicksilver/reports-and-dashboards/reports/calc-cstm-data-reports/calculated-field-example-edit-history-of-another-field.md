---
content-type: reference
product-area: reporting
keywords: audit,trail,custom,field
navigation-topic: calculate-custom-data-reports
title: "Berechnetes benutzerdefiniertes Feldbeispiel: Bearbeitungsverlauf eines Felds anzeigen"
description: Wenn Benutzer benutzerdefinierte Felder regelmäßig aktualisieren und Sie ein Protokoll aller an einem Feld vorgenommenen Änderungen sowie ein Datum, an dem die Änderungen vorgenommen werden, erfassen möchten, können Sie diese Informationen in einem berechneten benutzerdefinierten Feld erfassen.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Berechnetes benutzerdefiniertes Feldbeispiel: Anzeigen des Bearbeitungsverlaufs eines Felds

Wenn Benutzer benutzerdefinierte Felder regelmäßig aktualisieren und Sie ein Protokoll aller an einem Feld vorgenommenen Änderungen sowie ein Datum, an dem die Änderungen vorgenommen werden, erfassen möchten, können Sie diese Informationen in einem berechneten benutzerdefinierten Feld erfassen.

Das folgende Beispiel zeigt, wie Sie die *Anweisungen zum Bearbeiten des Verlaufs* berechnetes Feld, um alle Änderungen zu erfassen, die an einem einzeiligen Textfeld namens *Anweisungen*.

>[!TIP]
>
>In diesem Beispiel können Sie für alle Typen von benutzerdefinierten Feldern folgen, nicht nur für einzeilige Textfelder.

Dies geschieht folgendermaßen: 

* Begrenzt die *Anweisungen zum Bearbeiten des Verlaufs* auf die letzten 2000 Zeichen gesetzt, um innerhalb der Workfront-Datenbankbegrenzung zu bleiben.
* Überprüft, ob der aktuelle Wert der *Anweisungen* -Feld entspricht der Vorderseite der *Anweisungen zum Bearbeiten des Verlaufs* Wert; Es wird davon ausgegangen, dass es leer ist. Ist dies nicht der Fall, wird Folgendes ausgeführt: 

   * Wenn sie übereinstimmen, bleibt die *Anweisungen zum Bearbeiten des Verlaufs* unverändert;
   * Wenn sie nicht übereinstimmen, wird die *Anweisungen zum Bearbeiten des Verlaufs* mit dem neuesten Wert im *Anweisungen* gefolgt vom aktuellen Datum in Klammern, einem vertikalen Balken und dem vorherigen *Anweisungen zum Bearbeiten des Verlaufs*, wodurch der/die vorherige(n) Wert(e) und das Datum(e) der Eingabe beibehalten werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Administratorzugriff auf Custom Forms</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>Berechtigungen für benutzerdefinierte Formulare verwalten </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Um einem benutzerdefinierten Formular ein berechnetes Feld hinzuzufügen, das den Bearbeitungsverlauf eines Felds anzeigt, müssen Sie zunächst:

* Benutzerdefiniertes Formular erstellen
* Fügen Sie dem benutzerdefinierten Formular das Feld hinzu, dessen Verlauf Sie erfassen möchten

## Anzeigen des Bearbeitungsverlaufs eines Felds

1. Gehen Sie zu einem benutzerdefinierten Formular, in das Sie das berechnete Feld einfügen möchten.

1. Gehen Sie wie folgt vor, um das benutzerdefinierte Feld für einzeiligen Text zu erstellen:

   1. Klicken **Einzelzeilentext-Feld**.
   1. Geben Sie eine **Titel** für das benutzerdefinierte Feld, z. B. *Anweisungen*.
   1. Klicken **Applye**.

1. Auswählen **Feld hinzufügen**, wählen Sie **Berechnet** , um dem Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.
1. Geben Sie eine **Titel** für das berechnete benutzerdefinierte Feld, z. B. *Anweisungen zum Bearbeiten des Verlaufs*.

   Dies ist das Feld, das alle Änderungen erfasst, die an dem ersten von Ihnen erstellten Feld (*Anweisungen*).

1. Klicken **Speichern und schließen**.
1. Klicken Sie auf den Namen des Formulars, dem Sie nun zwei Felder hinzugefügt haben, um es erneut zu öffnen.
1. Klicken Sie auf das berechnete benutzerdefinierte Feld *Anweisungen zum Bearbeitungsverlauf,* Kopieren Sie dann Folgendes und fügen Sie es in das Feld Berechnung ein:
1. Im **Berechnung** Geben Sie die folgende Berechnung für Ihr benutzerdefiniertes Feld an:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Empfohlen) Fügen Sie dieselbe Berechnung in die **Anweisungen** im berechneten Feld des Formulars.
1. Stellen Sie sicher, dass  **Text** wird im **Format** -Feld, um das berechnete benutzerdefinierte Feld als Text zu formatieren.

   Dies ist die Standardeinstellung.

1. Klicken **Speichern+Schließen**.

   Wenn Sie jetzt das benutzerdefinierte Formular an ein Objekt anhängen und dann jemand die Informationen im *Anweisungen* im Feld *Anweisungen zum Bearbeiten des Verlaufs&quot;den neuesten Wert, gefolgt vom aktuellen Datum in Klammern und einer vertikalen Leiste. Wenn weitere Änderungen vorgenommen werden, werden sie auf die gleiche Weise zu diesen Informationen hinzugefügt.

   In der obigen Berechnung können Sie *Anweisungen* mit dem genauen Namen Ihres einzeiligen Textfelds, dessen Verlauf Sie verfolgen möchten, und *Anweisungen zum Bearbeiten des Verlaufs* mit dem genauen Namen Ihres berechneten Felds.
