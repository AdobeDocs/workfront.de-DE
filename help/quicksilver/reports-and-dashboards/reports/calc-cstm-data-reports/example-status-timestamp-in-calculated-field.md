---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular'
description: Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Beispiel für ein berechnetes benutzerdefiniertes Feld: Anzeigen eines Status-Zeitstempels in einem benutzerdefinierten Formular

Das folgende berechnete Feld zeigt das Datum an, an dem der Objektstatus als In Bearbeitung (INP) markiert ist. Sie können dieselben Informationen für berechnete benutzerdefinierte Felder für Probleme, Aufgaben oder Projekte verwenden.

>[!NOTE]
>
>Wenn sich der Status des Objekts in INP ändert, dann ändert er sich in einen anderen Status und dann zurück in INP, erfasst Adobe Workfront nur den Zeitstempel der ersten Änderung an INP.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.</p> 
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
   <td> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Konfigurationen der Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff zum Erstellen von Berichten, Dashboards und Kalendern bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>Verwalten Sie die Berechtigungen für das Objekt, an das das Formular angehängt ist</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.<br>Weitere Informationen zu Berechtigungen für Dashboards finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Freigeben von Berichten, Dashboards und Kalendern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
