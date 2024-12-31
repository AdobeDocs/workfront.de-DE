---
product-area: reporting
navigation-topic: text-mode-reporting
title: Vergleichen von Feldern in bedingter Formatierung
description: Sie können bedingte Formatierung verwenden, um zwei verschiedene Felder in einer Ansicht zu vergleichen und sie hervorzuheben, wenn bestimmte Kriterien zwischen den Feldern erfüllt sind.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Vergleichen von Feldern in bedingter Formatierung

Sie können bedingte Formatierung verwenden, um zwei verschiedene Felder in einer Ansicht zu vergleichen und sie hervorzuheben, wenn bestimmte Kriterien zwischen den Feldern erfüllt sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um die Ansicht in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht, um die Ansicht in einem Bericht zu bearbeiten</p> <p>Verwalten der Berechtigungen für eine Ansicht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Beispiel: Tatsächliches Startdatum und Geplantes Startdatum vergleichen

Wenn beispielsweise das tatsächliche Startdatum einer Aufgabe nach dem geplanten Startdatum liegt, können Sie die Spalte Geplantes Startdatum mithilfe einer bedingten Formatierung hervorheben.

So vergleichen Sie das geplante Startdatum und das tatsächliche Startdatum einer Aufgabe mithilfe einer bedingten Formatierung:

1. Gehe zu einer Aufgabenansicht oder einem Bericht.
1. (Bedingt) Wenn Sie mit einem Bericht arbeiten, klicken Sie auf der Registerkarte **Spalten (Ansicht)** auf die Kopfzeile der Spalte, die Sie mit Bedingungen formatieren möchten, um sie auszuwählen.\
   Wählen Sie beispielsweise die Spalte **Tatsächliches Startdatum** aus, um ihr die bedingte Formatierung hinzuzufügen, indem Sie die Felder Geplantes Startdatum und Tatsächliches Startdatum vergleichen.

1. Klicken Sie **Erweiterte Optionen** und anschließend auf &quot;**für diese Spalte hinzufügen**.

1. Geben Sie die Vergleichskriterien mithilfe der vorhandenen Werte aus dem Builder ein und geben Sie Ihre bedingte Formatierung an.\
   Beispielsweise möchten wir Aufgaben hervorheben, deren tatsächliches Startdatum nach dem geplanten Startdatum liegt (oder größer ist). Wählen Sie den Modifikator Größer als und danach im Datumsfeld ein tatsächliches Datum aus.\
     ![](assets/cond-format-1-350x84.png)

1. (Optional) Wählen Sie **Auf gesamte Zeile anwenden** aus, wenn Sie die Formatierung auf die gesamte Zeile anwenden möchten.
1. Klicken Sie **Regel hinzufügen** und dann **Fertig**.

1. Wählen Sie die **Tatsächliches Startdatum** aus und klicken Sie dann auf **In Textmodus wechseln**.

1. **Klicken Sie, um Text zu bearbeiten** und fügen Sie dann die folgende Textzeile hinzu:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   In unserem Beispiel: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Wenn Sie ein natives Workfront-Feld vergleichen, verwenden Sie die Binnenmajuskeln-Syntax für den Feldnamen. Wenn Sie ein benutzerdefiniertes Feld vergleichen, verwenden Sie **DE:Actual Name of the Field** für das Namensfeld, das Sie mit dem ersten Feld vergleichen.\
   >Wenn Sie z. B. das **Tatsächliche Startdatum** mit einem benutzerdefinierten Feld mit der Bezeichnung **Versanddatum** vergleichen, fügen Sie die folgende Anweisung in Ihrem Textmodus-Code hinzu:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Stellen Sie sicher, dass die `righttext` Codezeile mit der Anweisung in der `rightmethod` Codezeile übereinstimmt.

   ![](assets/cond-format-2-350x171.png)

1. Klicken Sie auf **Speichern**.
1. Klicken Sie auf **Speichern + schließen**.

   In der Spalte werden die Felder hervorgehoben, die Ihren Kriterien entsprechen.
