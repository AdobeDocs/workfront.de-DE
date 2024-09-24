---
title: Organisieren und Anzeigen einer Vorschau eines Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Formular Designer organisieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 8d9a9d8356f195d1e1fcbf0ae6c9b08f20ba4bbf
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Formular organisieren und in der Vorschau anzeigen

Sie können ein benutzerdefiniertes Formular mit dem Formularentwickler organisieren und eine Vorschau davon anzeigen, um zu überprüfen, ob es korrekt eingerichtet ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abschnittsumbruch hinzufügen

Sie können die benutzerdefinierten Felder und Widgets in einem benutzerdefinierten Formular in Abschnitte mit Überschriften gruppieren. Dies ist nützlich, um Benutzern, die das Formular ausfüllen, ein organisiertes Erlebnis zu präsentieren. Wenn Sie den Zugriff auf bestimmte benutzerdefinierte Felder und Widgets auf bestimmte Benutzer beschränken müssen, können Sie sie in einem Abschnitt platzieren und dann nur diesen Benutzern Zugriff auf den Abschnitt gewähren.

Wenn Sie beispielsweise sensible Informationen verfolgen müssen, die nur Systemadministratoren anzeigen oder bearbeiten können, können Sie einen Abschnittsumbruch mit Administratorberechtigungen erstellen und die sensiblen Felder in diesen Abschnitt einfügen.

Die Zugriffseinstellungen, die Sie für einen Abschnitt auswählen, sind direkt an die Berechtigungen gebunden, die Benutzer für das Workfront-Objekt haben, an das das benutzerdefinierte Formular angehängt ist. Sie können einen Abschnitt ein- oder ausblenden, je nachdem, ob der Benutzer Zugriff auf das Objekt hat, zu dem er beitragen oder es verwalten kann. Sie können auch einen Abschnitt auf &quot;Nur Administrator&quot;festlegen, damit nur Benutzer mit Systemadministrator-Zugriffsstufe darauf zugreifen können.

Weitere Informationen zu Berechtigungen für Objekte finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Weitere Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Erstellen und Konfigurieren des Zugriffs für einen Abschnitt in einem benutzerdefinierten Formular

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars und dem Hinzufügen von Feldern, wie in [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Klicken Sie auf **Abschnittsumbruch** und ziehen Sie ihn an die gewünschte Position auf der Arbeitsfläche.

1. Konfigurieren Sie im rechten Bereich die gewünschten Optionen für den Abschnitt:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Abschnitt angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie Text ein, wenn Sie Benutzern erklären möchten, wofür der Abschnitt dient. Dies wird unter dem Titel des Abschnitts im benutzerdefinierten Formular angezeigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zugriff erteilen</p> </td> 
      <td> <p> Wählen Sie die Berechtigungen aus, die Benutzer für ein Objekt benötigen, an das das benutzerdefinierte Formular angehängt ist, um diesen Abschnitt anzuzeigen und die Feldwerte zu bearbeiten. 
       <p>Die folgenden Berechtigungen sind unter <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte anzeigen</b>:</p> 
         <ul>
          <li><strong>Ansicht</strong>: Berechtigungen für das Objekt anzeigen</li>
          <li><p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
          <p>Ermöglicht Benutzern, zum Objekt beizutragen, wenn es sich um ein Projekt, eine Aufgabe oder ein Problem handelt.</p>
          <p>Ermöglicht Benutzern, das Profil zu bearbeiten oder Eigentümer der Profilberechtigung für das Objekt zu sein, wenn es ein Benutzer ist.</p></li> 
          <li><b>Bearbeiten</b>: Berechtigungen für das Objekt verwalten </li> 
          <li><b>Nur Administrator</b>: Zugriffsstufe des Systemadministrators</li> 
         </ul> </li> 
        <p>Die folgenden Berechtigungen sind unter <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte bearbeiten</b>: </p> 
         <ul> 
          <li> <p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
           <p>Wenn das Objekt ein Projekt, eine Aufgabe oder ein Problem ist, ermöglicht diese Berechtigung Benutzern, zum Objekt beizutragen</p>
          <p>Wenn das Objekt ein Benutzer ist, können Benutzer mit dieser Berechtigung das Profil bearbeiten oder Inhaber der Profilberechtigung für das Objekt sein.</p> 
          <li><b>Bearbeiten</b>: Berechtigungen für das Objekt verwalten </li> 
          <li><b>Nur Administrator</b>: Zugriffsstufe des Systemadministrators</li> 
         </ul> </li> 
       </ul> 
       <p>Weitere Informationen zu Berechtigungen für Objekte finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Überblick über die Freigabe von Berechtigungen für Objekte</a>.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li> <p>Benutzer ohne die hier angegebenen Berechtigungen können die benutzerdefinierten Felder und Widgets im Abschnitt nicht sehen. </p> <p>Dies gilt auch, wenn Sie die Feldwerte in Berichten anzeigen oder in berechneten Feldern in der Textmodusberichterstellung verwenden.</p> </li> 
       <li><p>Für benutzerdefinierte Formulare mit Anforderung/Problem: Wenn Sie Zugriff auf die Felder in der Abschnittsumfrage anzeigen möchten, aber zum Bearbeiten der Felder Administratorzugriff erforderlich ist, sind der Abschnitt und alle zugehörigen Felder für Benutzer ohne Administratorrechte nicht sichtbar, wenn sie das Formular ausfüllen. Nachdem die Anforderung erstellt wurde, können Benutzer mit Zugriff auf die Ansicht die Felder im Abschnitt anzeigen.</p></li>
       <li> <p>Wenn Sie mehrere Objekttypen mit Ihrem Formular verknüpfen, können sich die in diesen Schritten verfügbaren Anzeige- und Bearbeitungsberechtigungen ändern. Weitere Informationen finden Sie in diesem Artikel unter <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Wie mehrere Objekttypen die Berechtigungen für Abschnittsumbrüche in einem benutzerdefinierten Formular beeinflussen können</a>.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Logik hinzufügen</p></td> 
      <td><p>Verwenden Sie eine Anzeigelogik, um anzugeben, ob der Abschnitt basierend auf der Auswahl im Formular angezeigt werden soll, die Benutzer beim Ausfüllen des Formulars in benutzerdefinierten Feldern mit Mehrfachauswahl treffen.</p><p><strong>HINWEIS:</strong> Wenn auf alle einzelnen Felder unter einem Abschnittsumbruch eine Anzeigereihenfolge angewendet wird und sie alle infolge der Logik ausgeblendet sind, wird der gesamte Abschnitt im benutzerdefinierten Formular ausgeblendet. Dies geschieht auch dann, wenn die Anzeigelogik nicht auf den Abschnittsumbruch angewendet wird.</p><p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Hinzufügen der Anzeigelogik und Überspringen der Logik mit dem Formularentwickler</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ziehen Sie mindestens ein benutzerdefiniertes Feld oder Widget in den neuen Abschnitt oder fügen Sie es hinzu. Dies ist vor dem Speichern des Abschnitts erforderlich.

1. Klicken Sie auf **Fertig**.

   >[!TIP]
   >
   >Sie können jederzeit während der Erstellung eines benutzerdefinierten Formulars auf **Anwenden** klicken, um Ihre Änderungen zu speichern und das Formular offen zu halten.

### Wie sich mehrere Objektarten auf die Genehmigungen von Abschnittsumbrüchen auswirken können {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Die eingeschränkte Berechtigung zum Bearbeiten für benutzerdefinierte Formularabschnitte ist nur für die Objekttypen Projekt, Aufgabe, Problem und Benutzer verfügbar.

Wenn Sie in einem benutzerdefinierten Formular mit einer Abschnittspause, die mit der Berechtigung Eingeschränkte Bearbeitung konfiguriert wurde, einen der anderen Objekttypen zum Formular hinzufügen (Portfolio, Programm, Dokument, Firma, Rechnungsdatensatz, Iteration, Kosten oder Gruppe), werden Sie aufgefordert, zur Berechtigung &quot;Bearbeiten&quot;zu wechseln, die sowohl mit diesem Objekttyp als auch mit den vorhandenen Objekttypen im Formular kompatibel ist.

>[!INFO]
>
>**Beispiel:** In einem benutzerdefinierten Formular, das dem Projektobjekttyp zugeordnet ist, wird ein Abschnittsumbruch mit der Berechtigung &quot;Eingeschränkte Bearbeitung&quot;konfiguriert.
>
>Sie fügen den Objekttyp Portfolio zum Formular hinzu. Das bedeutet, dass die Option Eingeschränkte Bearbeitungsberechtigung für den Abschnittsumbruch im Formular nicht mehr verfügbar ist.
>
>Eine On-Screen-Meldung fordert Sie auf, zur Berechtigung Bearbeiten zu wechseln. Dies ist die geringste Berechtigungsstufe, die sowohl mit dem Projektobjekttyp als auch mit dem Portfolio-Objekttyp kompatibel ist.


## Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular


1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie in [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Um benutzerdefinierte Felder und Widgets in derselben Zeile zu positionieren, ziehen Sie eine neben die andere, bis eine Linie dazwischen angezeigt wird.

   >[!NOTE]
   >
   >* Sie können die Schaltfläche **Vorschau** oben rechts verwenden, um eine Vorstellung davon zu erhalten, wie die benutzerdefinierten Felder und Widgets im Formular angezeigt werden.
   >* Benutzerdefinierte Felder und Widgets werden im Formular möglicherweise nicht immer auf die gleiche Weise angezeigt, je nachdem, wie viel Platz auf dem Bildschirm verfügbar ist, wenn ein Benutzer das Formular anzeigt. Beispielsweise kann das dritte Feld in einer Zeile von Feldern zur nächsten Zeile von Feldern umbrechen, wenn der horizontale Bereich begrenzt ist.

1. (Optional) Um ein benutzerdefiniertes Feld oder Widget über oder unter einem anderen zu positionieren, ziehen Sie es über oder unter, bis eine horizontale blaue Linie zwischen den Elementen angezeigt wird.

1. Klicken Sie zum Speichern Ihrer Änderungen auf **Anwenden** .

   oder

   Klicken Sie auf **Speichern und schließen**.

## Vorschau eines benutzerdefinierten Formulars

1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars und dem Hinzufügen von Feldern, wie in [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Klicken Sie oben rechts auf **Vorschau** , um zu sehen, wie das Formular bei Verwendung aussehen wird, und klicken Sie dann auf **Vorschau beenden** , um zum Bearbeiten des Formulars zurückzukehren.

