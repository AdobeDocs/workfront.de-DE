---
title: Erste Schritte mit Adobe Workfront Planning Designer
description: Mit der Adobe Planning-Designer können Sie einen neuen Arbeitsbereich erstellen, Datensatztypen und -felder in Workfront Planning hinzufügen, Objekte zu einem Arbeitsbereich hinzufügen oder einen Änderungsverlauf für Datensätze anzeigen.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# Erste Schritte mit Adobe Workfront Planning Designer

{{planning-important-intro}}

Mit der Adobe Planning-Designer können Sie einen neuen Arbeitsbereich erstellen, Datensatztypen und -felder in Workfront Planning hinzufügen, Objekte zu einem Arbeitsbereich hinzufügen oder einen Änderungsverlauf für Datensätze anzeigen.

>[!IMPORTANT]
>
>Planning Designer ist derzeit nur für Benutzende verfügbar, die an der Closed Beta-Phase teilnehmen.

## <!--edit theses--> der Zugriffsanforderungen

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

<!--these are from the AI Assistant - edit these-->

* Um Planning Designer verwenden zu können, müssen Sie zunächst den KI-Assistenten für Ihr Unternehmen aktivieren. Damit der KI-Assistent für alle Personen in Ihrer Organisation verfügbar ist, muss Folgendes aktiviert sein:

   * Der KI-Assistent muss für Ihre Organisation aktiviert sein, damit er für Benutzende in Ihrer Firma verfügbar ist. Weitere Informationen finden Sie unter [Übersicht über den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Nachdem Workfront den KI-Assistenten für Ihr Unternehmen aktiviert hat, ist er für den Workfront-Hauptadministrator verfügbar. Weitere Informationen finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * Der Workfront-Administrator muss den KI-Assistenten für alle anderen Benutzer aktivieren. Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * Der KI-Assistent arbeitet im Kontext jeder Seite. Die Anfragen, die Sie für den KI-Assistenten senden, müssen auf Funktionen verweisen, die auf der geöffneten Seite verfügbar sind.

* Um Planning Designer verwenden zu können, muss es von einem Systemadministrator im Bereich „Systemeinstellungen“ des Setups aktiviert werden.

* Die vom KI-Assistenten im Bereich Planung durchgeführten Aktionen stehen im Kontext Ihrer Workfront-Planungsberechtigungen und Ihrer Workfront-Zugriffsebene. Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Lizenztyp-Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Änderungen, die der KI-Assistent im Auftrag des Benutzers vornimmt, werden im Verlaufsfenster des Datensatzes erfasst.

* Sie können Befehle verwenden, um Ihre Aktionen rückgängig zu machen. Sie können beispielsweise „Letzte Änderung rückgängig machen“ eingeben, um Ihre Änderung rückgängig zu machen.

* Beim Erstellen, Aktualisieren oder Löschen eines Objekts über den KI-Assistenten zeigt der KI-Assistent die beabsichtigten Aktionen an und bittet um Bestätigung. Anschließend können Sie die Aktionen bestätigen oder abbrechen.

—>

## Derzeit verfügbare Funktionen für Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Sie können entweder den Planning-Designer oder den KI-Assistenten verwenden, um eine der folgenden Aktionen durchzuführen:

* Erstellen und Konfigurieren von Arbeitsbereichen

* Datensatztypen erstellen

* Design-Felder oder Formelfelder

* Erstellen, Löschen, Duplizieren und Wiederherstellen von Datensätzen

* Bearbeiten, Aktualisieren und Anhängen eines Felds in einem Datensatz

* Datensätze mit anderen Datensätzen verknüpfen

* Zugriff auf den Änderungsverlauf des Datensatzes

* Erstellen benutzerdefinierter Ansichten

* Erstellen Sie Datensätze durch Importieren eines Dokuments. Das Erstellen von Datensätzen aus einem importierten Dokument ist nur in der Planning-Designer verfügbar und nicht im KI-Assistenten. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Suchen der Planning-Designer in Workfront Planning

Sie können über die Hauptseite von Workfront Planning auf die Planning-Designer zugreifen.

<!--add screen shot-->

Sie können auch den KI-Assistenten verwenden, um dieselben Funktionen zu nutzen, die der Planning Designer bietet.

## Aktivieren der Planungs-Designer für Ihr Unternehmen

Als Workfront-Administrator müssen Sie zunächst die Planning Designer für Ihr Unternehmen aktivieren.

<!--add steps here-->

## Erstellen oder Aktualisieren von Objekten mit der Planning-Designer

Sie können Objekte in Workfront Planning entweder mithilfe der Planning-Designer oder des KI-Assistenten erstellen oder aktualisieren, sofern nicht anders angegeben.

1. Melden Sie sich bei Workfront an und klicken Sie dann auf **Hauptmenü** Symbol ![Punkte-](assets/dots-main-menu.png)) in der rechten oberen Ecke des Bildschirms oder auf das Symbol **Hauptmenü** ![Zeilen-Hauptmenü](assets/lines-main-menu.png) in der linken oberen Ecke, falls verfügbar.

1. Klicken Sie **Planung**. Der Bereich Planung wird geöffnet.

1. Klicken Sie **Design mit KI**.

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

   Eine visuelle Vorschau mit einem Beispiel dafür, was der Assistent erstellen kann.

1. Folgen Sie nach Erhalt einer erfolgreichen Antwort den in der Befehlszeile angegebenen Links, um das Objekt Ihrer Anfrage zu erstellen, zu aktualisieren oder zu überprüfen.




