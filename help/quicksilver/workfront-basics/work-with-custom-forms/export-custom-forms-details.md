---
title: Exportieren benutzerdefinierter Formulare und Objektdetails
description: Exportieren benutzerdefinierter Formulare und Objektdetails
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Exportieren benutzerdefinierter Formulare und Objektdetails

Sie können die Übersicht und die benutzerdefinierten Formularinformationen aus dem Abschnitt Details eines Objekts in eine PDF-Datei exportieren. Sie können die PDF dann ausdrucken oder für andere freigeben.

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
>Die Felder im Abschnitt Details, die Ihr Workfront- oder Gruppen-Administrator mithilfe einer Layout-Vorlage entfernt hat, werden nicht angezeigt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Anfrage oder höher für Probleme</p> <p>Überprüfen oder höher für Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong> </td> 
   <td> <p>Anzeigen oder höher für Projekte, Aufgaben und Probleme</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Zeigen Sie oder höhere Berechtigungen für das Projekt, die Aufgabe oder das Problem an, dessen Formular Sie exportieren möchten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie beginnen, benötigen Sie Folgendes:

1. Erstellen Sie ein benutzerdefiniertes Formular für ein bestimmtes Objekt, aus dem Sie es exportieren möchten.
1. Benutzerdefiniertes Formular an das Objekt anhängen lassen

   Oder

   Sie verfügen über die richtigen Zugriffsrechte, um ein benutzerdefiniertes Formular anzuhängen und die Informationen auf dem Formular zu bearbeiten.

Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Informationen zum Anhängen von Formularen an Objekte finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportieren von Informationen im Abschnitt Details

Der Export von Informationen aus dem Abschnitt Details eines Objekts ist für alle Objekte, in denen es unterstützt wird, identisch.

1. Navigieren Sie zu einem Projekt, einer Aufgabe, einem Portfolio, einem Programm oder einem Problem, für das Sie mindestens über die Berechtigung „Anzeigen“ verfügen.
1. Klicken Sie auf das **„Details** im linken Bereich, z. B **„Aufgabendetails**.
1. (Optional) Wenn kein benutzerdefiniertes Formular an das Objekt angehängt ist, geben Sie den Namen eines benutzerdefinierten Formulars in das Feld **Benutzerdefiniertes Formular hinzufügen** ein und klicken Sie dann auf das Formular, wenn es in der Liste angezeigt wird.

   Sie können bis zu 10 Formulare hinzufügen.

1. (Optional) Aktualisieren Sie die Informationen im Abschnitt Details und klicken Sie dann auf **Änderungen speichern**.
1. Klicken Sie auf **Dropdown** Menü „Exportieren“ in der oberen rechten Ecke, wählen Sie **Übersicht** oder die Formulare aus, die Sie exportieren möchten, und klicken Sie dann auf **Exportieren**.

   Sie können auch **Alle auswählen** auswählen, wenn Sie den Übersichtsbereich und alle benutzerdefinierten Formulare exportieren möchten.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Die folgenden Szenarien sind möglich:
   >
   >   
   >   
   >   * Wenn Ihre Gruppe oder der Workfront-Administrator alle Felder im Bereich Übersicht aufhebt und an das Objekt benutzerdefinierte Formulare angehängt sind, wird der Abschnitt Übersicht nicht angezeigt.
   >   * Wenn Ihre Gruppe oder der Workfront-Administrator alle Felder im Bereich Übersicht abwählt und an das Objekt keine benutzerdefinierten Formulare angehängt sind, ist das Dropdown-Menü „Export“ nicht sichtbar.
   >   * Wenn an das Objekt keine benutzerdefinierten Formulare angehängt sind, können Sie nur den Bereich Überblick exportieren.
   >   * Benutzerdefinierte Felder, die sich hinter einer Logik befinden und im Formular nicht sichtbar sind, werden nicht exportiert. Informationen zum Hinzufügen von Logik zu einem benutzerdefinierten Formular finden Sie unter [Hinzufügen einer Anzeigelogik und Überspringen einer Logik zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
   >   
   >

   Es wird eine PDF-Datei erstellt und auf den Computer heruntergeladen. Die PDF-Datei enthält die folgenden Informationen:

   * Der Name des Objekts, an das das Formular angehängt ist
   * Der Name des Benutzers, der die PDF exportiert hat
   * Datum und Uhrzeit der Produktion der PDF
   * Der Name der exportierten Formulare
   * Informationen aus den im Formular ausgefüllten Feldern
