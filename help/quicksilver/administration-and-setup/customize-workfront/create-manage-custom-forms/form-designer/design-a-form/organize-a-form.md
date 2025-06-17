---
title: Organisieren und Vorschau eines Formulars
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Sie können ein benutzerdefiniertes Formular mit dem Formular-Designer organisieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 7373ee9f31e4b7561735920f3ff02cbd4fdce44a
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Organisieren und Vorschau eines Formulars

Sie können ein benutzerdefiniertes Formular mit dem Formular-Designer organisieren und eine Vorschau davon anzeigen, um zu überprüfen, ob es korrekt eingerichtet ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Abschnittsumbruch hinzufügen

Sie können die benutzerdefinierten Felder und Widgets in einem benutzerdefinierten Formular in Abschnitten mit Überschriften gruppieren. Dies ist nützlich, um Benutzenden, die das Formular ausfüllen, ein organisiertes Erlebnis zu präsentieren. Wenn Sie den Zugriff auf bestimmte benutzerdefinierte Felder und Widgets auf bestimmte Benutzer beschränken müssen, können Sie diese in einem Abschnitt platzieren und dann den Zugriff auf den Abschnitt nur diesen Benutzern gewähren.

Wenn Sie beispielsweise sensible Informationen verfolgen müssen, die nur Systemadministratoren anzeigen oder bearbeiten können sollen, können Sie einen Abschnittsumbruch mit Nur-Admin-Berechtigungen erstellen und die sensiblen Felder in diesem Abschnitt platzieren.

Die Zugriffseinstellungen, die Sie für einen Abschnitt auswählen, sind direkt an die Berechtigungen gebunden, die Benutzende für das Workfront-Objekt haben, an das das benutzerdefinierte Formular angehängt ist. Sie können einen Abschnitt je nachdem, ob der Benutzer Zugriff zum Anzeigen, Mitwirken oder Verwalten dieses Objekts hat, aus- oder einblenden. Alternativ können Sie einen Abschnitt auf Nur Admin festlegen, sodass nur Benutzer mit der Zugriffsebene „Systemadministrator“ darauf zugreifen können.

Informationen zu Berechtigungen für Objekte finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Informationen zu benutzerdefinierten Feldern und Widgets in benutzerdefinierten Formularen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Erstellen und Konfigurieren des Zugriffs für einen Abschnitt in einem benutzerdefinierten Formular

1. Beginnen Sie mit dem Erstellen oder Bearbeiten eines benutzerdefinierten Formulars und dem Hinzufügen von Feldern, wie in [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Klicken Sie **Abschnittsumbruch** und ziehen Sie ihn an die gewünschte Position auf der Arbeitsfläche.

1. Konfigurieren Sie im rechten Bedienfeld die gewünschten Optionen für den Abschnitt:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Erforderlich) Geben Sie einen beschreibenden Titel ein, der über dem Abschnitt angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Verwenden Sie in dieser Kennzeichnung keine Sonderzeichen. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie einen Text ein, wenn Sie den Benutzern erklären möchten, wozu der Abschnitt dient. Dies wird unter der Beschriftung des Abschnitts im benutzerdefinierten Formular angezeigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Zugriff erteilen</p> </td> 
      <td> <p> Wählen Sie die Berechtigungen aus, die Benutzer für ein Objekt benötigen, an das das benutzerdefinierte Formular angehängt ist, um diesen Abschnitt anzuzeigen und seine Feldwerte zu bearbeiten. 
       <p>Die folgenden Berechtigungen sind unter verfügbar <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte anzeigen</b>:</p> 
         <ul>
          <li><strong>Anzeigen</strong>: Anzeigen von Berechtigungen für das Objekt</li>
          <li><p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
          <p>Ermöglicht Benutzern, zum Objekt beizutragen, wenn es sich um ein Projekt, eine Aufgabe oder ein Problem handelt.</p>
          <p>Ermöglicht Benutzern das Bearbeiten des Profils oder das Besitzen der Profilberechtigung für das Objekt, wenn es ein Benutzer ist.</p></li> 
          <li><b>Bearbeiten</b>: Verwalten von Berechtigungen für das Objekt </li> 
          <li><b>Nur Admin</b>: Zugriffsebene des Systemadministrators</li> 
         </ul> </li> 
        <p>Die folgenden Berechtigungen sind unter verfügbar <b>Benutzer mit diesem Zugriff auf das Objekt können Feldwerte bearbeiten</b>: </p> 
         <ul> 
          <li> <p><b>Eingeschränkte Bearbeitung</b>: (Nur verfügbar, wenn das Objekt ein Projekt, eine Aufgabe, ein Problem oder ein Benutzer ist):</p> 
           <p>Wenn das Objekt ein Projekt, eine Aufgabe oder ein Problem ist, ermöglicht diese Berechtigung Benutzern, zum Objekt beizutragen</p>
          <p>Wenn das Objekt ein Benutzer ist, ermöglicht diese Berechtigung Benutzern das Bearbeiten des Profils oder das Besitzen der Profilberechtigung für das Objekt.</p> 
          <li><b>Bearbeiten</b>: Verwalten von Berechtigungen für das Objekt </li> 
          <li><b>Nur Admin</b>: Zugriffsebene des Systemadministrators</li> 
         </ul> </li> 
       </ul> 
       <p>Informationen zu Berechtigungen für Objekte finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Übersicht über Freigabeberechtigungen für Objekte</a>.</p> 
       <p><b>HINWEIS</b>:  
       <ul> 
       <li> <p>Benutzende ohne die hier angegebenen Berechtigungen können die benutzerdefinierten Felder und Widgets im Abschnitt nicht sehen. </p> <p>Dies gilt auch, wenn Sie die Werte der Felder in Berichten anzeigen oder in berechneten Feldern im Textmodus-Reporting verwenden.</p> </li> 
       <li><p>Für Anfrage-/Problem-benutzerdefinierte Formulare: Wenn der Ansichtszugriff erforderlich ist, um die Felder im Abschnittsumbruch anzuzeigen, aber zum Bearbeiten der Felder Administratorzugriff benötigt wird, sind der Abschnitt und alle zugehörigen Felder für Nicht-Admins nicht sichtbar, wenn sie das Formular ausfüllen. Nachdem die Anfrage erstellt wurde, können die Benutzer mit Ansichtszugriff die Felder im Abschnitt anzeigen.</p></li>
       <li> <p>Wenn Sie dem Formular mehrere Objekttypen zuordnen, können sich die in diesen Schritten verfügbaren Anzeige- und Bearbeitungsberechtigungen ändern. Weitere Informationen finden Sie unter <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Wie mehrere Objekttypen sich auf Abschnittsumbruchberechtigungen in einem benutzerdefinierten Formular auswirken können</a> in diesem Artikel.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Logik hinzufügen</p></td> 
      <td><p>Verwenden Sie Anzeigelogik , um anzugeben, ob der Abschnitt basierend auf den Auswahlen, die Benutzer in benutzerdefinierten Feldern mit Mehrfachauswahl treffen, wenn sie das Formular ausfüllen, im Formular angezeigt werden soll.</p><p><strong>HINWEIS</strong> Wenn auf alle einzelnen Felder unter einem Abschnittsumbruch eine Anzeigelogik angewendet wurde und sie infolge der Logik alle ausgeblendet sind, wird der gesamte Abschnitt im benutzerdefinierten Formular ausgeblendet. Dies geschieht auch dann, wenn die Anzeigelogik nicht auf den Abschnittsumbruch angewendet wird.</p><p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Anzeigelogik hinzufügen und Logik mit dem Formular-Designer überspringen</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Ziehen Sie mindestens ein benutzerdefiniertes Feld oder Widget in den neuen Abschnitt oder fügen Sie es hinzu. Dies ist vor dem Speichern des Abschnitts erforderlich.

1. Klicken Sie **Fertig**.

   >[!TIP]
   >
   >Sie können jederzeit auf **Anwenden** klicken, während Sie ein benutzerdefiniertes Formular erstellen, um Ihre Änderungen zu speichern und das Formular offen zu halten.

### Wie sich mehrere Objekttypen auf Berechtigungen für Abschnittsumbrüche auswirken können {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Die Berechtigung zum eingeschränkten Bearbeiten für Abschnittsumbrüche in benutzerdefinierten Formularen ist nur für die Objekttypen „Projekt“, „Aufgabe“, „Problem“ und „Benutzer“ verfügbar.

In einem benutzerdefinierten Formular mit einem Abschnittsumbruch, der mit der Berechtigung „Eingeschränkte Bearbeitung“ konfiguriert wurde, werden Sie beim Hinzufügen eines der anderen Objekttypen zum Formular (Portfolio, Programm, Dokument, Unternehmen, Rechnungsnachweis, Iteration, Ausgabe oder Gruppe) aufgefordert, zur Berechtigung „Bearbeiten“ zu wechseln, die sowohl mit diesem Objekttyp als auch mit den vorhandenen Objekttypen im Formular kompatibel ist.

>[!INFO]
>
>**Beispiel** In einem benutzerdefinierten Formular, das mit dem Projektobjekttyp verknüpft ist, wird ein Abschnittsumbruch mit der Berechtigung „Eingeschränkte Bearbeitung“ konfiguriert.
>
>Sie fügen dem Formular den Portfolio-Objekttyp hinzu, was bedeutet, dass die Option zur eingeschränkten Bearbeitung für den Abschnittsumbruch im Formular nicht mehr verfügbar ist.
>
>Eine Meldung auf dem Bildschirm fordert Sie auf, zur Bearbeitungsberechtigung zu wechseln. Dies ist die niedrigste Berechtigungsstufe, die sowohl mit dem Projektobjekttyp als auch mit dem Portfolio-Objekttyp kompatibel ist.


## Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular


1. Beginnen Sie mit der Erstellung oder Bearbeitung eines benutzerdefinierten Formulars, wie in [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Um benutzerdefinierte Felder und Widgets in derselben Zeile zu positionieren, ziehen Sie eines neben das andere, bis eine Linie zwischen ihnen angezeigt wird.

   >[!NOTE]
   >
   >* Sie können die Schaltfläche **Vorschau** in der oberen rechten Ecke verwenden, um einen Eindruck davon zu gewinnen, wie die benutzerdefinierten Felder und Widgets im Formular angezeigt werden.
   >* Benutzerdefinierte Felder und Widgets werden möglicherweise nicht immer auf die gleiche Weise im Formular angezeigt, je nachdem, wie viel Platz auf dem Bildschirm verfügbar ist, wenn ein Benutzer es anzeigt. Beispielsweise kann das dritte Feld in einer Reihe von Feldern in die nächste Zeile umgebrochen werden, wenn der horizontale Abstand begrenzt ist.

1. (Optional) Um ein benutzerdefiniertes Feld oder Widget über oder unter einem anderen zu positionieren, ziehen Sie es über oder unter, bis zwischen den Elementen eine horizontale blaue Linie angezeigt wird.

1. Um ein benutzerdefiniertes Feld in einen anderen Abschnitt im Formular zu verschieben, können Sie es per Drag-and-Drop an die gewünschte Position verschieben oder auf das **Verschieben nach**-Symbol auf dem Feld klicken und den Abschnitt auswählen, in den das Feld verschoben werden soll.

   ![Feld in einen Abschnitt verschieben](assets/move-field-to-section.png)

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen**

   oder

   Klicken Sie **Speichern und schließen**.

## Vorschau eines benutzerdefinierten Formulars

1. Beginnen Sie mit dem Erstellen oder Bearbeiten eines benutzerdefinierten Formulars und dem Hinzufügen von Feldern, wie in [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

1. Klicken Sie **oben** auf „Vorschau“, um die Darstellung des Formulars bei Verwendung zu überprüfen, und dann auf **Vorschau beenden**, um zur Bearbeitung des Formulars zurückzukehren.

   >[!NOTE]
   >
   >Erweiterte Logik wird im Vorschaumodus des Formular-Designers nicht unterstützt.


