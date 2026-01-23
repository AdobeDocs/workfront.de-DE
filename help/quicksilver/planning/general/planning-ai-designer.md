---
title: Erste Schritte mit Adobe Workfront Planning Designer
description: Mit der Adobe Planning-Designer können Sie einen neuen Arbeitsbereich erstellen, Datensatztypen und -felder in Workfront Planning hinzufügen, Objekte zu einem Arbeitsbereich hinzufügen oder einen Änderungsverlauf für Datensätze anzeigen.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bd3dde54d986416af847b2f3b2a1e8570d5ce3f2
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# Erste Schritte mit Adobe Workfront Planning Designer

{{planning-important-intro}}

Sie können den Adobe Planning Designer mit KI verwenden, um einen neuen Arbeitsbereich zu generieren, Objekte zu einem Arbeitsbereich hinzuzufügen (Datensatztypen, Datensätze, Ansichten oder Felder) oder einen Änderungsverlauf für Datensätze anzuzeigen.

>[!IMPORTANT]
>
>Planning Designer ist derzeit nur für Benutzende verfügbar, die am Closed Beta-Programm teilnehmen.

Weitere Informationen zu Workfront Planning finden Sie in den folgenden Artikeln:

* [Allgemeine Informationen zu Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md)
* [Erste Schritte mit Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Zugriffsübersicht für Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)


## &#x200B;<!--edit theses??--> der Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Beliebiges Workfront- und Planungspaket</p>
<p>Beliebiges Workflow- und Planungspaket</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Registrierung für das Closed Beta-Programm von Planning Designer

Derzeit können Sie sich für das Closed Beta-Programm für Planning Designer bewerben, indem Sie uns eine E-Mail an sargism@adobe.com senden.

Nachdem wir die E-Mail erhalten haben, aktiviert unser Engineering-Team Planning Designer in Ihrer Workfront-Instanz.

>[!IMPORTANT]
>
>Ihr Unternehmen muss zunächst die Vereinbarung über den KI-Assistenten akzeptieren, bevor die Planning Designer in Ihrem System verfügbar ist.

## Überlegungen zum Planning Designer

* Um Planning Designer verwenden zu können, müssen Sie zunächst den KI-Assistenten für Ihr Unternehmen aktivieren. Folgendes muss vorhanden sein, damit der KI-Assistent für alle Personen in Ihrer Organisation verfügbar ist:

   * Workfront muss den KI-Assistenten für Ihr Unternehmen verfügbar machen.

     Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).
   * Nachdem Workfront den KI-Assistenten für Ihr Unternehmen zur Verfügung gestellt hat, kann der Workfront-Hauptadministrator darauf zugreifen.

     Weitere Informationen finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).
   * Der Workfront-Administrator muss die KI-Assistentenvereinbarung akzeptieren und dann den KI-Assistenten für alle anderen Benutzenden aktivieren.

     Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).
* Nachdem Ihr Systemadministrator den KI-Assistenten für Ihre Organisation aktiviert hat, ist der Planungsassistent standardmäßig für alle Benutzer verfügbar, sofern er für Ihre Organisation zur Verfügung gestellt wurde.
* Von Planning Designer durchgeführte Aktionen können auch vom KI-Assistenten ausgeführt werden, wenn Sie ihn im Planungsbereich verwenden.
* Die vom KI-Assistenten im Bereich Planung durchgeführten Aktionen bzw. die vom Planning Designer ausgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die im Auftrag des Benutzers vom KI-Assistenten oder vom Planning Designer vorgenommen werden, werden im Verlaufsfenster des Datensatzes erfasst.

* Die von Planning Designer durchgeführten Aktionen sind dauerhaft und könnten unumkehrbar sein. Das Löschen eines Felds kann beispielsweise nicht rückgängig gemacht werden. Überprüfen Sie alle von Designer vorgeschlagenen Aktionen, bevor Sie sie akzeptieren.

  >[!IMPORTANT]
  >
  >Beim Erstellen, Aktualisieren oder Löschen eines Objekts über die Planning-Designer werden Sie in der Eingabeaufforderung nur für die Aktionen zur Bestätigung aufgefordert, die irreversibel sind. Das Löschen eines Datensatztyps oder eines Arbeitsbereichs kann beispielsweise nicht rückgängig gemacht werden. Löschen eines Datensatzes ist nicht möglich. Die Planning Designer fordert nur dann zur Bestätigung auf, wenn versucht wird, einen Datensatztyp oder einen Arbeitsbereich zu löschen.

* Beim Erstellen von Arbeitsbereichen und Datensatztypen mit der Planning-Designer werden auch Ansichten und Felder automatisch erstellt.

## Derzeit verfügbare Funktionen für Planning Designer

Sie können entweder den Planning-Designer oder den KI-Assistenten verwenden, um eine der folgenden Aktionen durchzuführen:

* Erstellen und Konfigurieren von Arbeitsbereichen

* Erstellen von Datensatztypen, einschließlich Definieren und Hinzufügen globaler Datensatztypen zu Arbeitsbereichen

* Design-Felder oder Formelfelder

* Erstellen, Löschen, Duplizieren und Wiederherstellen von Datensätzen

* Bearbeiten, Aktualisieren und Anhängen eines Felds in einem Datensatz

* Datensätze mit anderen Datensätzen verknüpfen

* Zugriff auf den Änderungsverlauf des Datensatzes

* Erstellen benutzerdefinierter Ansichten

* Erstellen von Datensätzen durch Importieren eines Dokuments

  Sie können beispielsweise ein Bild eines Organigramms in Ihr Unternehmen hochladen, und die Planning Designer kann auf dieser Grundlage einen Arbeitsbereich erstellen.

  Das Erstellen von Objekten aus einem importierten Dokument ist nur in der Planning-Designer und nicht im KI-Assistenten verfügbar.

  >[!IMPORTANT]
  >
  >Obwohl wir .XLSX- und .CSV-Dateitypen unterstützen, können diese nicht für den groß angelegten Datensatzimport über die Planning Designer verwendet werden.
  >Wenn Sie derzeit eine erhebliche Anzahl von Datensätzen importieren müssen, empfehlen wir, hierzu die in Planning verfügbaren manuellen Funktionen zu verwenden.
  >
  >Weitere Informationen finden Sie unter [Erstellen von Datensätzen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/records/import-file-to-create-records.md).
  >Informationen zu Dateitypbeschränkungen finden Sie im Abschnitt „Abrufen von Vorschlägen basierend auf einem Dokument, das Sie hochladen“ im Abschnitt &quot;[&#x200B; von Formularausfüllen mit KI zum Ausfüllen einer Anfrage mithilfe von Eingabeaufforderungen oder Dokumenten](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Erstellen oder Aktualisieren von Objekten mit der Planning-Designer

Sie können Objekte in Workfront Planning entweder mithilfe der Planning-Designer oder des KI-Assistenten erstellen oder aktualisieren, sofern nicht anders angegeben.

1. Melden Sie sich bei Workfront an und klicken Sie dann oben links auf **&#x200B;**-Symbol ![Hauptmenü „Zeilen](assets/lines-main-menu.png) und dann auf **Planung**.

   Der Bereich **Planung** wird geöffnet.

   ![Design mit KI-Schaltfläche auf der Seite „Arbeitsbereiche“](assets/design-with-ai-button-on-workspaces-page.png)

1. Klicken Sie **Design mit KI**.

   Das **Planning Designer** wird geöffnet.

   ![Fenster &quot;Designer planen“](assets/planning-designer-window.png)

1. Beginnen Sie im bereitgestellten Feld mit der Eingabe von Eingabeaufforderungen für den KI-Assistenten und klicken Sie dann auf die Eingabetaste , wenn Sie fertig sind.

   <!--add screen shot-->

   Sie können beispielsweise Eingabeaufforderungen ähnlich den folgenden eingeben:

   * Erstellen und konfigurieren Sie einen Arbeitsbereich mit fünf Datensatztypen zur Verwaltung von Kampagnen

   * Marketing-Kampagnen für jeden Monat des aktuellen Jahres erstellen

   * Hinzufügen eines Kampagnenfelds für den Status des Arbeitsbereichs Marketing-Design

   * Löschen Sie alle Datensätze mit dem Status Veraltet

   * Alle Planning-Kampagnen auf den Status „Aktiv“ aktualisieren

   * Verbinden von Kampagnen mit Personas im Arbeitsbereich Marketing-Design

   * Änderungshistorie der Kampagne „Valentinstag“ anzeigen

   * Erstellen einer Zeitleisten -Ansicht für Kampagnen im Arbeitsbereich Marketing-Design

   * Erstellen Sie Datensätze durch Importieren eines Dokuments. Das Erstellen von Datensätzen aus einem importierten Dokument ist nur in der Planning-Designer verfügbar und nicht im KI-Assistenten.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

1. Folgen Sie nach Erhalt einer erfolgreichen Antwort den Links im Eingabeaufforderungsbereich, um das Objekt Ihrer Anfrage zu erstellen, zu aktualisieren oder zu überprüfen.

   Wenn Sie mit der Erstellung Ihrer Objekte einverstanden sind, werden Ihre Änderungen rechts neben dem Eingabeaufforderungsbereich angezeigt.

   Rechts neben der Eingabeaufforderung können Sie Workspaces, Datensatztypen, Felder, Ansichten und Datensätze im Vorschaubereich anzeigen.

   >[!TIP]
   >
   >Einige Objekte werden sofort erstellt, ohne dass eine Bestätigung erforderlich ist.

1. (Optional) Geben Sie zusätzliche Eingabeaufforderungen ein, um Ihre Objekte weiter zu bearbeiten.
1. (Optional) Klicken Sie auf das Symbol **Vorschaufenster anzeigen oder ausblenden** Symbol ![Vorschaufenster ein- oder &#x200B;](assets/hide-show-preview-screen-in-planning-designer.png) anzeigen), um den Vorschaufenster auf der rechten Seite zu öffnen oder zu schließen.
1. Klicken Sie auf **Symbol „Arbeitsbereich in neuer Registerkarte öffnen** Symbol ![Arbeitsbereich in neuer Registerkarte öffnen](assets/open-workspace-on-new-tab-icon.png), um den Arbeitsbereich, den Sie aktualisieren, in einer neuen Registerkarte zu öffnen.
1. Klicken Sie auf das **Schließen**-Symbol **X**, um Planning Designer zu schließen und den Arbeitsbereich zu öffnen.
1. Öffnen Sie den bearbeiteten Arbeitsbereich mit der Planning-Designer und nehmen Sie weitere Änderungen an den Objekten vor.

## Deaktivieren von Planning Designer für Ihr Unternehmen

Nachdem Ihr Workfront-Administrator die KI-Assistentenvereinbarung akzeptiert hat, ist die Planungs-Designer standardmäßig für alle Personen in Ihrem Unternehmen aktiviert.

So deaktivieren Sie sie:

1. Melden Sie sich bei Workfront als Systemadministrator an.
1. Klicken Sie **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-shell.png) in der oberen linken Ecke des Bildschirms und dann auf **Setup**.
1. Klicken Sie **linken Bereich auf** System“ > und gehen Sie dann in den Bereich **KI-Voreinstellungen**.
1. Deaktivieren Sie die Einstellung **Planning Designer**. <!--add new screen shot with info icon-->

   ![Planen der Designer-Einstellung in den Systemvoreinstellungen](assets/planning-designer-toggle-in-system-preferences.png)
1. Klicken Sie auf **Speichern**.

   Dadurch wird die Planning-Designer für alle Benutzenden im System entfernt.






