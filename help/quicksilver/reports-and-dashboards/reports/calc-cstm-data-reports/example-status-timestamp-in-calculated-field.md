---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Beispiel für ein berechnetes benutzerdefiniertes Feld: einen Status-Zeitstempel in einem benutzerdefinierten Formular anzeigen'
description: Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.
author: Courtney
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OsYpPu9dAsSEQE6BBkvGovNR5E6I7k0BC2n48R7psLg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 343
ht-degree: 13%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.

>[!NOTE]
>
>Wenn sich der Status des Objekts in INP ändert, dann ändert er sich in einen anderen Status und dann zurück in INP, erfasst Adobe Workfront nur den Zeitstempel der ersten Änderung an INP.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
      <p>Abo</p></td>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

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
