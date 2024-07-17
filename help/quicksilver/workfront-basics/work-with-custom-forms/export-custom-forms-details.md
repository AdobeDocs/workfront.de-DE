---
title: Exportieren benutzerdefinierter Formulare und Objektdetails
description: Exportieren benutzerdefinierter Formulare und Objektdetails
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 1%

---

# Exportieren benutzerdefinierter Formulare und Objektdetails

Sie können die Übersicht und die benutzerdefinierten Formulardaten aus dem Bereich &quot;Details&quot;eines Objekts in eine PDF-Datei exportieren. Sie können die PDF dann drucken oder für andere Benutzer freigeben.

Diese Funktion wird für die folgenden Objekte unterstützt:

* Projekte
* Aufgaben
* Probleme
* Portfolio
* Programme

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Die Felder im Bereich Details , die Ihr Workfront- oder Gruppenadministrator mithilfe einer Layoutvorlage entfernt hat, werden nicht angezeigt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Anfrage oder höher für Probleme</p> <p>Prüfungen oder höher für Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Anzeigen oder höher für Projekte, Aufgaben und Probleme</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für das Projekt, die Aufgabe oder das Problem, dessen Formular Sie exportieren möchten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie über Folgendes verfügen:

1. Lassen Sie ein benutzerdefiniertes Formular für ein bestimmtes Objekt erstellen, aus dem Sie es exportieren möchten.
1. Das benutzerdefinierte Formular wird an das Objekt angehängt

   Oder

   Sie benötigen den richtigen Zugriff, um ein benutzerdefiniertes Formular anzuhängen und die Informationen im Formular zu bearbeiten.

Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Weitere Informationen zum Anhängen von Formularen an Objekte finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportieren von Informationen im Bereich Details

Das Exportieren von Informationen aus dem Bereich Details eines Objekts ist für alle Objekte identisch, für die es unterstützt wird.

1. Wechseln Sie zu einem Projekt, einer Aufgabe, einem Portfolio, einem Programm oder einem Problem, für das Sie mindestens über Anzeigeberechtigungen verfügen.
1. Klicken Sie im linken Bereich auf das Element **&quot;Details&quot;**, z. B. **Aufgabendetails**.
1. (Optional) Wenn kein benutzerdefiniertes Formular an das Objekt angehängt ist, geben Sie den Namen eines benutzerdefinierten Formulars in das Feld **Benutzerdefiniertes Formular hinzufügen** ein und klicken Sie dann auf dieses Feld, wenn es in der Liste angezeigt wird.

   Sie können bis zu 10 Formulare hinzufügen.

1. (Optional) Aktualisieren Sie die Informationen im Abschnitt &quot;Details&quot;und klicken Sie dann auf **Änderungen speichern**.
1. Klicken Sie auf das Dropdown-Menü **Exportieren** oben rechts, wählen Sie **Überblick** oder die Formulare, die exportiert werden sollen, und klicken Sie dann auf **Exportieren**.

   Sie können auch &quot;**Alle auswählen**&quot;auswählen, wenn Sie den Übersichtsbereich und alle benutzerdefinierten Formulare exportieren möchten.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Die folgenden Szenarien können vorliegen:
   >
   >   
   >   
   >   * Wenn Ihre Gruppe oder Ihr Workfront-Administrator die Auswahl aller Felder im Bereich Überblick aufhebt und dem Objekt benutzerdefinierte Formulare angehängt sind, wird der Abschnitt Übersicht nicht angezeigt.
   >   * Wenn Ihre Gruppe oder Ihr Workfront-Administrator die Auswahl aller Felder im Bereich Übersicht aufhebt und dem Objekt keine benutzerdefinierten Formulare angehängt sind, ist das Dropdown-Menü Exportieren nicht sichtbar.
   >   * Wenn an das Objekt keine benutzerdefinierten Formulare angehängt sind, können Sie nur den Übersichtsbereich exportieren.
   >   * Benutzerdefinierte Felder, die hinter der Logik liegen und im Formular nicht sichtbar sind, werden nicht exportiert. Weitere Informationen zum Hinzufügen von Logik zu einem benutzerdefinierten Formular finden Sie unter [Hinzufügen der Anzeigerlogik und Überspringen der Logik zu einem benutzerdefinierten Formular](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).
   >   
   >

   Eine PDF-Datei wird erstellt und auf Ihren Computer heruntergeladen. Die PDF-Datei enthält die folgenden Informationen:

   * Der Name des Objekts, an das das Formular angehängt ist
   * Der Name des Benutzers, der die PDF exportiert hat
   * Datum und Uhrzeit der Erstellung der PDF
   * Der Name der exportierten Formulare
   * Informationen aus den auf dem Formular ausgefüllten Feldern
