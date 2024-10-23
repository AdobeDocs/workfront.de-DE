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
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Berechnetes benutzerdefiniertes Feldbeispiel: Bearbeitungsverlauf eines Felds anzeigen

Wenn Benutzer benutzerdefinierte Felder regelmäßig aktualisieren und Sie ein Protokoll aller an einem Feld vorgenommenen Änderungen sowie ein Datum, an dem die Änderungen vorgenommen werden, erfassen möchten, können Sie diese Informationen in einem berechneten benutzerdefinierten Feld erfassen.

Im folgenden Beispiel erfahren Sie, wie Sie das berechnete Feld Anweisungen zum Bearbeiten des Verlauf erstellen, um alle Änderungen an einem einzeiligen Textfeld namens Anweisungen zu erfassen.

>[!TIP]
>
>In diesem Beispiel können Sie für alle Typen von benutzerdefinierten Feldern folgen, nicht nur für einzeilige Textfelder.

Dies geschieht folgendermaßen:

* Beschränkt das Feld Anweisungen zum Bearbeiten des Verlaufs auf die letzten 2000 Zeichen, um innerhalb der Workfront-Datenbankbegrenzung zu bleiben.
* Überprüft, ob der aktuelle Wert des Felds Anweisungen mit dem Vorder-Wert des Werts Bearbeitungsverlauf für Anweisungen übereinstimmt. Es wird davon ausgegangen, dass er leer ist. Ist dies nicht der Fall, wird Folgendes ausgeführt:

   * Wenn sie übereinstimmen, bleiben die Anweisungen Verlauf bearbeiten unverändert.
   * Wenn sie nicht übereinstimmen, wird der Bearbeitungsverlauf für Anweisungen durch den neuesten Wert im Feld Anweisungen ersetzt, gefolgt vom aktuellen Datum in Klammern, einem vertikalen Balken und dem Bearbeitungsverlauf für frühere Anweisungen, in dem die vorherigen Werte und das Datum bzw. die Daten, zu denen sie eingegeben wurden, beibehalten werden.

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
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Administratorzugriff auf Custom Forms</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
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

   1. Klicken Sie auf **Einzelzeilentext**.
   1. Geben Sie eine **Beschriftung** für das benutzerdefinierte Feld an. Sie können ihn beispielsweise &quot;Instructions&quot;nennen.
   1. Klicken Sie auf **Anwenden**.

1. Klicken Sie auf **Berechnet** , um dem Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.
1. Geben Sie eine **Beschriftung** für das berechnete benutzerdefinierte Feld an. Sie können ihn beispielsweise &quot;Anweisungen zum Bearbeiten des Verlaufs&quot;nennen.

   Dies ist das Feld, das alle Änderungen erfasst, die an dem ersten von Ihnen erstellten Feld (&quot;Anweisungen&quot;) vorgenommen wurden.

1. Klicken Sie auf **Speichern und schließen**.
1. Klicken Sie auf den Namen des Formulars, dem Sie nun zwei Felder hinzugefügt haben, um es erneut zu öffnen.
1. Klicken Sie auf das berechnete benutzerdefinierte Feld **Anweisungen zum Bearbeiten des Verlaufs** und kopieren Sie dann Folgendes in das Feld **Berechnung**:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Empfohlen) Fügen Sie dieselbe Berechnung in das Feld **Anweisungen** im berechneten Feld im Formular ein.
1. Stellen Sie sicher, dass **Text** im Feld **Format** ausgewählt ist, um das berechnete benutzerdefinierte Feld als Text zu formatieren.

   Dies ist die Standardeinstellung.

1. Klicken Sie auf **Speichern und schließen**.

   Wenn Sie jetzt das benutzerdefinierte Formular an ein Objekt anhängen und dann die Informationen im Feld **Anweisungen** ändern, zeigt das Feld **Bearbeitungsverlauf für Anweisungen** den neuesten Wert an, gefolgt vom aktuellen Datum in Klammern und einem vertikalen Balken. Wenn weitere Änderungen vorgenommen werden, werden sie auf die gleiche Weise zu diesen Informationen hinzugefügt.

   In der obigen Berechnung können Sie *Anweisungen* durch den genauen Namen Ihres einzeiligen Textfelds ersetzen, dessen Verlauf Sie verfolgen möchten, und **Anweisungen zum Bearbeiten des Verlaufs** durch den genauen Namen Ihres berechneten Felds.
