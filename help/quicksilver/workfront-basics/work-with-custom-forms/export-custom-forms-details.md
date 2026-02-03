---
title: Benutzerdefinierte Forms- und Objektdetails exportieren
description: Sie können die Übersicht und die benutzerdefinierten Formularinformationen aus dem Abschnitt Details eines Objekts in eine PDF-Datei exportieren. Anschließend können Sie die PDF drucken oder für andere Benutzer freigeben.
author: Alina
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 4%

---

# Exportieren benutzerdefinierter Formulare und Objektdetails

<!--Audited: 10/2025-->

Sie können die Übersicht und die benutzerdefinierten Formularinformationen aus dem Abschnitt Details eines Objekts in eine PDF-Datei exportieren. Anschließend können Sie die PDF drucken oder für andere Benutzer freigeben.

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

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Lizenz</p> </td> 
   <td><p>Für Probleme:</p>
   <ul><li><p>Mitwirkender oder höher</p></li>
   <li><p>Antragsteller oder höher</p> </li></ul>
   <p>Für Projekte und Aufgaben:</p>
   <ul><li><p>Licht oder höher</p></li>
   <li><p>Reviewer oder höher</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder höher für Projekte, Aufgaben und Probleme</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>Zeigen Sie oder höhere Berechtigungen für das Projekt, die Aufgabe oder das Problem an, dessen Formular Sie exportieren möchten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

Bevor Sie beginnen, benötigen Sie Folgendes:

1. Erstellen Sie ein benutzerdefiniertes Formular für ein bestimmtes Objekt, aus dem Sie es exportieren möchten.
1. Benutzerdefiniertes Formular an das Objekt anhängen lassen

   ODER

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

   ![Schaltfläche für benutzerdefiniertes Formular exportieren](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Die folgenden Szenarien sind möglich:
   >
   >   * Wenn Ihre Gruppe oder der Workfront-Administrator alle Felder im Bereich Übersicht aufhebt und an das Objekt benutzerdefinierte Formulare angehängt sind, wird der Abschnitt Übersicht nicht angezeigt.
   >   * Wenn Ihre Gruppe oder der Workfront-Administrator alle Felder im Bereich Übersicht abwählt und an das Objekt keine benutzerdefinierten Formulare angehängt sind, ist das Dropdown-Menü „Export“ nicht sichtbar.
   >   * Wenn an das Objekt keine benutzerdefinierten Formulare angehängt sind, können Sie nur den Bereich Überblick exportieren.
   >   * Benutzerdefinierte Felder, die sich hinter einer Logik befinden und im Formular nicht sichtbar sind, werden nicht exportiert. Informationen zum Hinzufügen von Logik zu einem benutzerdefinierten Formular finden Sie unter [Hinzufügen von Logikregeln zu benutzerdefinierten Formularen und Feldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

   Es wird eine PDF-Datei erstellt und auf den Computer heruntergeladen. Die PDF-Datei enthält die folgenden Informationen:

   * Der Name des Objekts, an das das Formular angehängt ist
   * Der Name des Benutzers, der die PDF exportiert hat
   * Datum und Uhrzeit der Erstellung des PDFS
   * Der Name der exportierten Formulare
   * Informationen aus den im Formular ausgefüllten Feldern
