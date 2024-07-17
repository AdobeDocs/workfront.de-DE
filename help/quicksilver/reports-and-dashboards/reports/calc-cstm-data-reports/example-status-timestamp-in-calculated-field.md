---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Berechnetes benutzerdefiniertes Feldbeispiel: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular"
description: Das folgende berechnete Feld zeigt das Datum, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

Das folgende berechnete Feld zeigt das Datum, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.

>[!NOTE]
>
>Wenn sich der Status des Objekts in INP ändert, dann zu einem anderen Status und dann zurück zu INP, erfasst Adobe Workfront nur den Zeitstempel der ersten Änderung zu INP.

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
   <td> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf "Berichte erstellen", "Dashboards"und "Kalender"bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>Berechtigungen für das Objekt verwalten, an das das Formular angehängt ist</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.<br>Weitere Informationen zu Berechtigungen für Dashboards finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Berichte, Dashboards und Kalender freigeben </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzung

Um einem benutzerdefinierten Formular ein berechnetes Feld hinzuzufügen, das den Bearbeitungsverlauf eines Felds anzeigt, müssen Sie zunächst das benutzerdefinierte Formular erstellen.

## Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

1. Gehen Sie zu einem benutzerdefinierten Formular, in das Sie das Feld einfügen möchten.
1. Klicken Sie auf **Berechnet** , um dem Formular ein berechnetes benutzerdefiniertes Feld hinzuzufügen.
1. Geben Sie eine **Beschriftung** für das benutzerdefinierte Feld ein, z. B. *Status Timestamp Custom Field*.
1. Klicken Sie auf **Fertig** und dann auf **Speichern+Schließen**.
1. Öffnen Sie das benutzerdefinierte Formular erneut und wählen Sie dann das neue Feld **Status-Zeitstempel für benutzerdefiniertes Feld** im Formular aus.
1. Kopieren Sie in das Feld **Berechnung** die folgende Berechnung für Ihr benutzerdefiniertes Feld und fügen Sie sie ein:

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >Diese Berechnung ist für alle Objekte und für alle Status identisch. Sie müssen in dieser Berechnung immer die Drei-Buchstaben-Taste und nicht den Statusnamen für den Objektstatus verwenden.
   >
   >Weitere Informationen zu den Schlüsseln für Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicken Sie auf **Speichern+Schließen**.

   Sie können jetzt Berichte über das benutzerdefinierte Feld Status-Zeitstempel erstellen oder es in anderen Berechnungen, in Berichten oder in benutzerdefinierten Feldern verwenden.
