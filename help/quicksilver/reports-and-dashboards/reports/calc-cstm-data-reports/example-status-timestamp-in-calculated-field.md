---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular'
description: Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.

>[!NOTE]
>
>Wenn sich der Status des Objekts in INP ändert, dann ändert er sich in einen anderen Status und dann zurück in INP, erfasst Adobe Workfront nur den Zeitstempel der ersten Änderung an INP.

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
   <td> <p>Zugriff zum Erstellen von Berichten, Dashboards und Kalendern bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Verwalten Sie die Berechtigungen für das Objekt, an das das Formular angehängt ist</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzung

Um einem benutzerdefinierten Formular ein berechnetes Feld hinzuzufügen, das den Bearbeitungsverlauf eines Felds anzeigt, müssen Sie zunächst das benutzerdefinierte Formular erstellen.

## Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

1. Wechseln Sie zu einem benutzerdefinierten Formular, in dem Sie das Feld hinzufügen möchten.
1. Klicken Sie **Berechnet**, um dem Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.
1. Geben Sie **benutzerdefinierte Feld** Titel“ ein. Beispiel: „Benutzerdefiniertes Feld für Status-Zeitstempel“.
1. Klicken Sie **Speichern+Schließen**.
1. Öffnen Sie das benutzerdefinierte Formular erneut und wählen Sie dann das neue **Feld Zeitstempel benutzerdefiniert** im Formular aus.
1. Kopieren Sie **Feld** und fügen Sie die folgende Berechnung für Ihr benutzerdefiniertes Feld ein:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Diese Berechnung ist für alle Objekte und für alle Status identisch. Bei dieser Berechnung muss immer der aus drei Buchstaben bestehende Schlüssel und nicht der Statusname für den Objektstatus verwendet werden.
   >
   >Weitere Informationen zu den Schlüsseln für Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicken Sie **Speichern+Schließen**.

   Sie können jetzt Berichte zum benutzerdefinierten Feld Status-Zeitstempel erstellen oder es in anderen Berechnungen, in Berichten oder in benutzerdefinierten Feldern verwenden.
