---
product-area: reporting
navigation-topic: text-mode-reporting
title: Vergleichen von Feldern in bedingter Formatierung
description: Sie können bedingte Formatierung verwenden, um zwei verschiedene Felder in einer Ansicht zu vergleichen und sie hervorzuheben, wenn bestimmte Kriterien zwischen den Feldern erfüllt sind.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# Vergleichen von Feldern in bedingter Formatierung

<!-- Audited: 1/2025 -->

Sie können bedingte Formatierung verwenden, um zwei verschiedene Felder in einer Ansicht zu vergleichen und sie hervorzuheben, wenn bestimmte Kriterien zwischen den Feldern erfüllt sind.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um die Ansicht in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht, um die Ansicht in einem Bericht zu bearbeiten</p> <p>Verwalten der Berechtigungen für eine Ansicht</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beispiel: Tatsächliches Startdatum und Geplantes Startdatum vergleichen

Wenn beispielsweise das tatsächliche Startdatum einer Aufgabe nach dem geplanten Startdatum liegt, können Sie die Spalte Geplantes Startdatum mithilfe einer bedingten Formatierung hervorheben.

So vergleichen Sie das geplante Startdatum und das tatsächliche Startdatum einer Aufgabe mithilfe einer bedingten Formatierung:

1. Gehe zu einer Aufgabenansicht oder einem Bericht.
1. (Bedingt) Wenn Sie mit einem Bericht arbeiten, klicken Sie auf der Registerkarte **Spalten (Ansicht)** im Berichtseditor auf die Kopfzeile der Spalte, die Sie mit Bedingungen formatieren möchten, um sie auszuwählen.\
   Wählen Sie beispielsweise die Spalte **Tatsächliches Startdatum** aus, um ihr die bedingte Formatierung hinzuzufügen, indem Sie die Felder Geplantes Startdatum und Tatsächliches Startdatum vergleichen.

1. Klicken Sie **Erweiterte Optionen** und anschließend auf &quot;**für diese Spalte hinzufügen**.

1. Geben Sie die Vergleichskriterien mithilfe der vorhandenen Werte aus dem Builder ein und geben Sie Ihre bedingte Formatierung an.\
   Beispielsweise möchten wir Aufgaben hervorheben, deren tatsächliches Startdatum nach dem geplanten Startdatum liegt (oder größer ist). Wählen Sie den Modifikator Größer als und danach im Datumsfeld ein tatsächliches Datum aus.

   ![Bedingte Formatierung für tatsächliches Startdatum](assets/cond-format-1-350x84.png)

1. (Optional) Wählen Sie **Auf gesamte Zeile anwenden** aus, wenn Sie die Formatierung auf die gesamte Zeile anwenden möchten.
1. Klicken Sie auf **Speichern**.

1. Wählen Sie die **Tatsächliches Startdatum** aus und klicken Sie dann auf **In Textmodus wechseln**.

1. Klicken Sie **Textmodus bearbeiten** und fügen Sie dann die folgende Textzeile hinzu:

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

   ![Bedingte Formatierung](assets/cond-format-2-350x171.png)

1. Klicken Sie auf **Speichern**.
1. Klicken Sie auf **Speichern + schließen**.

   In der Spalte werden die Felder hervorgehoben, die Ihren Kriterien entsprechen.
