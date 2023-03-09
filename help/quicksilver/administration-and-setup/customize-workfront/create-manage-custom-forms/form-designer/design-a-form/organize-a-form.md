---
title: Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Form Designer organisieren.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 529de9d31be883325d425dceb286d750397c5d8e
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler

{{highlighted-preview-article-level}}

Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler organisieren.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>
   <p>Aktueller Plan: Standard</p>
   <p>oder</p>
   <p>Veralteter Plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Abschnittsumbruch hinzufügen

Sie können die benutzerdefinierten Felder und Widgets in einem benutzerdefinierten Formular in Abschnitte mit Überschriften gruppieren. Dies ist nützlich, um Benutzern, die das Formular ausfüllen, ein organisiertes Erlebnis zu präsentieren. Wenn Sie den Zugriff auf bestimmte benutzerdefinierte Felder und Widgets auf bestimmte Benutzer beschränken müssen, können Sie sie in einem Abschnitt platzieren und dann nur diesen Benutzern Zugriff auf den Abschnitt gewähren.

Wenn Sie beispielsweise sensible Informationen verfolgen müssen, die nur Systemadministratoren anzeigen oder bearbeiten können, können Sie einen Abschnittsumbruch mit Administratorberechtigungen erstellen und die sensiblen Felder in diesen Abschnitt einfügen.

Die Zugriffseinstellungen, die Sie für einen Abschnitt auswählen, sind direkt an die Berechtigungen gebunden, die Benutzer für das Workfront-Objekt haben, an das das benutzerdefinierte Formular angehängt ist. Sie können einen Abschnitt ein- oder ausblenden, je nachdem, ob der Benutzer Zugriff auf das Objekt hat, zu dem er beitragen oder es verwalten kann. Sie können auch einen Abschnitt auf &quot;Nur Administrator&quot;festlegen, damit nur Benutzer mit Systemadministrator-Zugriffsstufe darauf zugreifen können.

Weitere Informationen zu Berechtigungen für Objekte finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Erstellen und Konfigurieren des Zugriffs für einen Abschnitt in einem benutzerdefinierten Formular

1. Erstellen oder bearbeiten Sie ein benutzerdefiniertes Formular und fügen Sie Felder hinzu, wie beschrieben in [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken **Abschnittsumbruch** und ziehen Sie sie an die gewünschte Position auf der Arbeitsfläche.

1. Konfigurieren Sie im rechten Bereich die gewünschten Optionen für den Abschnitt:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Abschnitt angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie Text ein, wenn Sie Benutzern erklären möchten, wofür der Abschnitt dient. Dies wird unter dem Titel des Abschnitts im benutzerdefinierten Formular angezeigt.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Zugriff erteilen</p> </td> 
      <td> <p> Wählen Sie die Berechtigungen aus, die Benutzer für ein Objekt benötigen, an das das benutzerdefinierte Formular angehängt ist, um diesen Abschnitt anzuzeigen und die Feldwerte zu bearbeiten. 
       <p>Die folgenden Berechtigungen sind unter <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte anzeigen</b>:</p> 
         <ul>  
          <li><p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
          <p>Ermöglicht Benutzern, zum Objekt beizutragen, wenn es sich um ein Projekt, eine Aufgabe oder ein Problem handelt.</p>
          <p>Ermöglicht Benutzern, das Profil zu bearbeiten oder Eigentümer der Profilberechtigung für das Objekt zu sein, wenn es ein Benutzer ist.</p></li> 
          <li><b>Bearbeiten</b>: Berechtigungen für das Objekt verwalten </li> 
          <li><b>Nur Administrator</b>: Zugriffsstufe für Systemadministrator</li> 
         </ul> </li> 
        <p>Die folgenden Berechtigungen sind unter <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte bearbeiten</b>: </p> 
         <ul> 
          <li> <p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
           <p>Wenn das Objekt ein Projekt, eine Aufgabe oder ein Problem ist, ermöglicht diese Berechtigung Benutzern, zum Objekt beizutragen</p>
          <p>Wenn das Objekt ein Benutzer ist, können Benutzer mit dieser Berechtigung das Profil bearbeiten oder Inhaber der Profilberechtigung für das Objekt sein.</p> 
          <li><b>Bearbeiten</b>: Berechtigungen für das Objekt verwalten </li> 
          <li><b>Nur Administrator</b>: Zugriffsstufe für Systemadministrator</li> 
         </ul> </li> 
       </ul> 
       <p>Weitere Informationen zu Berechtigungen für Objekte finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über die Freigabe von Berechtigungen für Objekte</a>.</p> 
       <p><b>NOTIZ</b>:  
       <ul> 
       <li> <p>Benutzer ohne die hier angegebenen Berechtigungen können die benutzerdefinierten Felder und Widgets im Abschnitt nicht sehen. </p> <p>Dies gilt auch, wenn Sie die Feldwerte in Berichten anzeigen oder in berechneten Feldern in der Textmodusberichterstellung verwenden.</p> </li> 
       <li> <p>Wenn Sie mehrere Objekttypen mit Ihrem Formular verknüpfen, können sich die in diesen Schritten verfügbaren Anzeige- und Bearbeitungsberechtigungen ändern. Weitere Informationen finden Sie unter <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Wie sich mehrere Objekttypen auf die Berechtigung zum Umbruch von Abschnitten in einem benutzerdefinierten Formular auswirken können</a> in diesem Artikel.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ziehen Sie mindestens ein benutzerdefiniertes Feld oder Widget in den neuen Abschnitt oder fügen Sie es hinzu. Dies ist vor dem Speichern des Abschnitts erforderlich.

1. Klicken **Fertig**.

   >[!TIP]
   >
   >Sie können auf **Anwenden** Sie können jederzeit ein benutzerdefiniertes Formular erstellen, um Ihre Änderungen zu speichern und das Formular offen zu halten.

### Wie sich mehrere Objektarten auf die Genehmigungen von Abschnittsumbrüchen auswirken können {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Die eingeschränkte Berechtigung zum Bearbeiten für benutzerdefinierte Formularabschnitte ist nur für die Objekttypen Projekt, Aufgabe, Problem und Benutzer verfügbar.

Wenn Sie in einem benutzerdefinierten Formular mit einer Abschnittspause, die mit der Berechtigung Eingeschränkte Bearbeitung konfiguriert wurde, einen der anderen Objekttypen zum Formular hinzufügen (Portfolio, Programm, Dokument, Firma, Rechnungsdatensatz, Iteration, Kosten oder Gruppe), werden Sie aufgefordert, zur Berechtigung &quot;Bearbeiten&quot;zu wechseln, die sowohl mit diesem Objekttyp als auch mit den vorhandenen Objekttypen im Formular kompatibel ist.

>[!INFO]
>
>**Beispiel:** In einem benutzerdefinierten Formular, das mit dem Projektobjekttyp verknüpft ist, wird ein Abschnittsumbruch mit der Berechtigung Eingeschränkte Bearbeitung konfiguriert.
>
>Sie fügen den Objekttyp Portfolio zum Formular hinzu. Das bedeutet, dass die Option Eingeschränkte Bearbeitungsberechtigung für den Abschnittsumbruch im Formular nicht mehr verfügbar ist.
>
>Eine On-Screen-Meldung fordert Sie auf, zur Berechtigung Bearbeiten zu wechseln. Dies ist die geringste Berechtigungsstufe, die sowohl mit dem Projektobjekttyp als auch mit dem Portfolio-Objekttyp kompatibel ist.


## Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular


1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie unter [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Um benutzerdefinierte Felder und Widgets in derselben Zeile zu positionieren, ziehen Sie eine neben die andere, bis eine Linie dazwischen angezeigt wird.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Sie können die **Vorschau** rechts oben, um eine Vorstellung davon zu erhalten, wie die benutzerdefinierten Felder und Widgets im Formular angezeigt werden.
>* Benutzerdefinierte Felder und Widgets werden im Formular möglicherweise nicht immer auf die gleiche Weise angezeigt, je nachdem, wie viel Platz auf dem Bildschirm verfügbar ist, wenn ein Benutzer das Formular anzeigt. Beispielsweise kann das dritte Feld in einer Zeile von Feldern zur nächsten Zeile von Feldern umbrechen, wenn der horizontale Bereich begrenzt ist.


1. (Optional) Um ein benutzerdefiniertes Feld oder Widget über oder unter einem anderen zu positionieren, ziehen Sie es über oder unter, bis eine horizontale blaue Linie zwischen den Elementen angezeigt wird.

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Anwenden**

   oder

   Klicken **Speichern und schließen**.

## Vorschau eines benutzerdefinierten Formulars

1. Erstellen oder bearbeiten Sie ein benutzerdefiniertes Formular und fügen Sie Felder hinzu, wie beschrieben in [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken **Vorschau** in der oberen linken Ecke, um zu sehen, wie das Formular bei Verwendung aussehen wird, und klicken Sie dann auf **Endvorschau** , um zum Bearbeiten des Formulars zurückzukehren.