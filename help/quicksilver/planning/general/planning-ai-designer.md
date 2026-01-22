---
title: Erste Schritte mit Adobe Workfront Planning Designer
description: Mit der Adobe Planning-Designer können Sie einen neuen Arbeitsbereich erstellen, Datensatztypen und -felder in Workfront Planning hinzufügen, Objekte zu einem Arbeitsbereich hinzufügen oder einen Änderungsverlauf für Datensätze anzeigen.
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 866b237db5d109b0a435145119a6412e41d960ab
workflow-type: tm+mt
source-wordcount: '1020'
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


## Zugriffsanforderungen

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

<!--edit this Or create a new article under Beta programs?? -->

Derzeit können Sie die Teilnahme am Closed Beta-Programm für Planning Designer anfordern.

## Überlegungen zum Planning Designer

* Um Planning Designer verwenden zu können, muss Ihr Unternehmen die Anforderungen für die Verwendung des Workfront AI Assistant erfüllen.

  Weitere Informationen finden Sie unter [Voraussetzungen für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

* Um Planning Designer verwenden zu können, muss es von einem Systemadministrator im Bereich „Systemeinstellungen“ des Setups aktiviert werden.

* Sie können Eingabeaufforderungen verwenden, um Planning-Objekte entweder mithilfe des Workfront-KI-Assistenten aus dem Bereich Planning oder mithilfe der Planning-Designer zu erstellen.

* Die vom KI-Assistenten im Bereich Planung durchgeführten Aktionen bzw. die vom Planning Designer ausgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die von Planning Designer im Auftrag des Benutzers vorgenommen werden, werden im Verlaufsfenster des Datensatzes erfasst.

* Sie können Befehle verwenden, um Ihre Aktionen rückgängig zu machen. Sie können beispielsweise „Letzte Änderung rückgängig machen“ eingeben, um Ihre Änderung rückgängig zu machen.

* Beim Erstellen, Aktualisieren oder Löschen eines Objekts über die Planning-Designer werden die beabsichtigten Aktionen angezeigt und zur Bestätigung aufgefordert. Anschließend können Sie die Aktionen bestätigen oder abbrechen.

* Beim Erstellen von Arbeitsbereichen und Datensatztypen mit der Planning-Designer werden auch Ansichten und Felder automatisch erstellt.

## Derzeit verfügbare Funktionen für Planning Designer

Sie können entweder den Planning-Designer oder den KI-Assistenten verwenden, um eine der folgenden Aktionen durchzuführen:

* Erstellen und Konfigurieren von Arbeitsbereichen

* Datensatztypen erstellen

* Design-Felder oder Formelfelder

* Erstellen, Löschen, Duplizieren und Wiederherstellen von Datensätzen

* Bearbeiten, Aktualisieren und Anhängen eines Felds in einem Datensatz

* Datensätze mit anderen Datensätzen verknüpfen

* Zugriff auf den Änderungsverlauf des Datensatzes

* Erstellen benutzerdefinierter Ansichten

* Erstellen Sie Datensätze durch Importieren eines Dokuments.

  Das Erstellen von Datensätzen aus einem importierten Dokument ist nur in der Planning-Designer verfügbar und nicht im KI-Assistenten.

  Informationen zu den akzeptierten Dateitypen und -größen finden Sie im Abschnitt „Leitplanken für Dokumente“ im Artikel [Verwenden Sie das Ausfüllen von Formularen mit künstlicher Intelligenz, um eine Anfrage mithilfe von Eingabeaufforderungen oder Dokumenten auszufüllen](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Aktivieren der Planungs-Designer für Ihr Unternehmen

Als Workfront-Administrator müssen Sie zunächst die Planning Designer für Ihr Unternehmen aktivieren.

<!--add steps here-->

1. Melden Sie sich bei Workfront als Systemadministrator an.
1. Klicken Sie **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-shell.png) in der oberen linken Ecke des Bildschirms und dann auf **Setup**.
1. Klicken Sie **linken Bereich auf** System“ > und gehen Sie dann in den Bereich **KI-Voreinstellungen**.
1. Schalten Sie die folgenden Einstellungen ein:
   * **KI aktivieren**
   * **Opt-in für KI-Beta-Versionen**
   * **Planen von Designer**

   ![Planen der Designer-Einstellung in den Systemvoreinstellungen](assets/planning-designer-toggle-in-system-preferences.png)
1. Klicken Sie auf **Speichern**.

   Alle Benutzer des Systems, die über eine Standardlizenz verfügen, sehen jetzt die Schaltfläche **Design with AI** auf der Hauptseite „Arbeitsbereiche“ im Bereich Planung . <!--check screen shot-->

   ![Schaltfläche „Design mit KI“ auf der Seite „Arbeitsbereiche“](assets/design-with-ai-button-on-workspaces-page.png)

   Alle Benutzer können jetzt Planning Designer verwenden, um Workfront Planning-Objekte zu erstellen und zu aktualisieren.

## Erstellen oder Aktualisieren von Objekten mit der Planning-Designer

Sie können Objekte in Workfront Planning entweder mithilfe der Planning-Designer oder des KI-Assistenten erstellen oder aktualisieren, sofern nicht anders angegeben.

1. Melden Sie sich bei Workfront an und klicken Sie dann oben links auf **&#x200B;**&#x200B;Hauptmenü![Symbol &quot;](assets/lines-main-menu.png)&quot;.

1. Klicken Sie **Planung**. Der Bereich Planung wird geöffnet.

1. Klicken Sie **Design mit KI**.

   Das **Planning Designer** wird geöffnet.

   ![Fenster &quot;Designer planen“](assets/planning-designer-window.png)

1. Beginnen Sie in dem dafür vorgesehenen Feld mit der Eingabe von Befehlen für den KI-Assistenten und klicken Sie abschließend auf die Eingabetaste .

   <!--add screen shot-->

   Sie können beispielsweise eine Anfrage ähnlich der folgenden eingeben:

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

   Im Vorschaubereich rechts neben der Eingabeaufforderung können Sie Arbeitsbereiche, Datensatztypen, Felder, Ansichten und Datensätze überprüfen.
1. (Optional) Geben Sie zusätzliche Eingabeaufforderungen ein, um Ihre Objekte weiter zu bearbeiten.
1. (Optional) Klicken Sie auf das Symbol **Umschalten des KI-Arbeitsbereich**-Vorschaubildschirms![&#x200B; Symbol „Vorschau anzeigen“ &#x200B;](assets/hide-show-preview-screen-in-planning-designer.png), um den Vorschaubildschirm auf der rechten Seite zu öffnen oder zu schließen.
1. Klicken Sie auf **Symbol „Arbeitsbereich in neuer Registerkarte öffnen** Symbol ![Arbeitsbereich in neuer Registerkarte öffnen](assets/open-workspace-on-new-tab-icon.png), um den Arbeitsbereich, den Sie aktualisieren, in einer neuen Registerkarte zu öffnen.
1. Klicken Sie auf das **Schließen**-Symbol **X**, um Planning Designer zu schließen und den Arbeitsbereich zu öffnen.
1. Öffnen Sie den bearbeiteten Arbeitsbereich mit der Planning-Designer und nehmen Sie weitere Änderungen an den Objekten vor.




