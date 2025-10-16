---
content-type: reference
product-area: reporting
keywords: Audit, Protokoll, benutzerdefiniert, Feld
navigation-topic: calculate-custom-data-reports
title: 'Beispiel für berechnete benutzerdefinierte Felder: Anzeigen des Bearbeitungsverlaufs eines Felds'
description: Wenn Benutzer benutzerdefinierte Felder regelmäßig aktualisieren und Sie ein Protokoll aller an einem Feld vorgenommenen Änderungen sowie ein Datum, an dem die Änderungen vorgenommen werden, erfassen möchten, können Sie diese Informationen in einem berechneten benutzerdefinierten Feld erfassen.
author: Jenny
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Beispiel für berechnete benutzerdefinierte Felder: Anzeigen des Bearbeitungsverlaufs eines Felds

Wenn Benutzer benutzerdefinierte Felder regelmäßig aktualisieren und Sie ein Protokoll aller an einem Feld vorgenommenen Änderungen sowie ein Datum, an dem die Änderungen vorgenommen werden, erfassen möchten, können Sie diese Informationen in einem berechneten benutzerdefinierten Feld erfassen.

Das folgende Beispiel zeigt, wie Sie das berechnete Feld Bearbeitungsverlauf für Anweisungen erstellen, um alle Änderungen an einem einzeiligen Textfeld namens Anweisungen zu erfassen.

>[!TIP]
>
>Diesem Beispiel können Sie für alle Arten von benutzerdefinierten Feldern folgen, nicht nur für einzeilige Textfelder.

Dies geschieht folgendermaßen:

* Beschränkt das Feld Anleitung Bearbeitungsverlauf auf die letzten 2.000 Zeichen, um innerhalb des Workfront-Datenbanklimits zu bleiben.
* Überprüft, ob der aktuelle Wert des Felds Anweisungen mit dem vorderen Wert des Wertes für Bearbeitungsverlauf für Anweisungen übereinstimmt. Es wird davon ausgegangen, dass er leer ist. Ist dies nicht der Fall, wird Folgendes ausgeführt:

   * Wenn sie übereinstimmen, bleiben die Anweisungen zum Bearbeiten des Verlaufs unverändert.
   * Wenn sie nicht übereinstimmen, wird der Bearbeitungsverlauf der Anweisungen durch den neuesten Wert im Feld Anweisungen ersetzt, gefolgt vom aktuellen Datum in Klammern, einem vertikalen Balken und dem Bearbeitungsverlauf der vorherigen Anweisungen, wodurch der/die vorherige(n) Wert(e) und das Datum/die Datumsangaben beibehalten werden.

## Zugriffsanforderungen

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Paket</p> </td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Konfigurationen der Zugriffsebene</p></td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Forms</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Verwalten der Berechtigungen für die benutzerdefinierten Formulare</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Um einem benutzerdefinierten Formular ein berechnetes Feld hinzuzufügen, das den Bearbeitungsverlauf eines Felds anzeigt, müssen Sie zunächst Folgendes tun:

* Erstellen eines benutzerdefinierten Formulars
* Fügen Sie das Feld, dessen Verlauf Sie erfassen möchten, zum benutzerdefinierten Formular hinzu

## Anzeigen des Bearbeitungsverlaufs eines Felds

1. Wechseln Sie zu einem benutzerdefinierten Formular, in dem Sie das berechnete Feld hinzufügen möchten.

1. Um beispielsweise das benutzerdefinierte Feld Einzeiliger Text zu erstellen, gehen Sie wie folgt vor:

   1. Klicken Sie **Einzeiliger Text**.
   1. Geben Sie einen **Titel** für das benutzerdefinierte Feld an. Sie können ihr beispielsweise den Namen „Anweisungen“ geben.
   1. Klicken Sie auf **Übernehmen**.

1. Klicken Sie **Berechnet**, um dem Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.
1. Geben Sie einen **Titel** für das berechnete benutzerdefinierte Feld an. Sie können ihr beispielsweise den Namen „Anweisungen - Bearbeitungsverlauf“ geben.

   Dies ist das Feld, das alle Änderungen erfasst, die am ersten von Ihnen erstellten Feld vorgenommen wurden („Anweisungen„).

1. Klicken Sie **Speichern und schließen**.
1. Klicken Sie auf den Namen des Formulars, dem Sie jetzt zwei Felder hinzugefügt haben, um es erneut zu öffnen.
1. Klicken Sie auf das berechnete benutzerdefinierte Feld **Anweisungen Bearbeitungsverlauf**, kopieren Sie Folgendes und fügen Sie es in das Feld **Berechnung** ein:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Empfohlen) Fügen Sie dieselbe Berechnung in das Feld **Anweisungen** im berechneten Feld im Formular ein.
1. Stellen Sie sicher **dass** Text) im Feld **Format** ausgewählt ist, um das berechnete benutzerdefinierte Feld als Text zu formatieren.

   Dies ist der Standardwert.

1. Klicken Sie **Speichern und schließen**.

   Wenn Sie nun das benutzerdefinierte Formular an ein Objekt anhängen und dann jemand die Informationen im Feld **Anweisungen** ändert, zeigt das Feld **Anweisungen - Bearbeitungsverlauf** den neuesten Wert an, gefolgt vom aktuellen Datum in Klammern und einem vertikalen Balken. Wenn weitere Änderungen vorgenommen werden, werden sie auf die gleiche Weise zu diesen Informationen hinzugefügt.

   Bei der obigen Berechnung können Sie *Anweisungen* durch den genauen Namen Ihres einzeiligen Textfelds, dessen Verlauf Sie verfolgen möchten, und **Anweisungen - Verlauf bearbeiten** durch den genauen Namen Ihres berechneten Felds ersetzen.
