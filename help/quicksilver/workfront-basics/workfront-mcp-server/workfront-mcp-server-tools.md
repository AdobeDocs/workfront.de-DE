---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP-Server-Tools
description: Referenzliste der über den Adobe Workfront MCP-Server verfügbaren Tools, gruppiert nach Workfront-Bereich.
author: Courtney
feature: Get Started with Workfront
source-git-commit: f4f73cf44107850573e1a6966568645b9537b757
workflow-type: tm+mt
source-wordcount: '1615'
ht-degree: 6%

---


# Adobe Workfront MCP-Server-Tools

In diesem Artikel werden die Tools aufgelistet, die der [!DNL Adobe Workfront] MCP-Server für eine verbundene KI-Agentenplattform bereitstellt. Die -Plattform ruft diese Tools in Ihrem Namen auf, wenn Sie sie zum Suchen, Erstellen, Aktualisieren oder Löschen von Workfront-Elementen auffordern.

Informationen zur Verwendung dieser Tools über eine KI-Agentenplattform finden Sie unter [Verwenden des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Informationen zum Einrichten der Verbindung finden Sie unter [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>Die KI-Agentenplattform agiert in Workfront unter Verwendung Ihres Workfront-Kontos, Ihrer Zugriffsebene und Ihrer Objektberechtigungen. Ein Tool funktioniert nur, wenn Sie den entsprechenden Zugriff in Workfront haben. Adobe übernimmt keine Verantwortung für Änderungen, die die KI-Agentenplattform an Ihren Workfront-Daten vornimmt.


## Lese- und Schreibaktionen

Jedes Tool in den folgenden Tabellen wird in der Spalte Aktion entweder als Lese- oder Schreibaktion klassifiziert:

* **Lesen**: Ruft Informationen aus Workfront ab, ohne die Daten zu ändern. Zum Beispiel, um ein Projekt zu finden, Dokumente aufzulisten oder die Details eines Datensatzes abzurufen.
* **Write**: Erstellt, aktualisiert oder löscht Workfront-Daten. Beispielsweise beim Erstellen eines Projekts, Aktualisieren eines Datensatzes oder Löschen einer Ansicht.

Ihr Workfront-Administrator steuert über zwei Umschalter in den Systemeinstellungen, welche Toolkategorien die KI-Agentenplattform verwenden kann:

* **Schreibgeschützte MCP-Tools** (standardmäßig aktiviert)
* **MCP-Tools schreiben** (standardmäßig deaktiviert)

Wenn die KI-Agentenplattform Workfront-Elemente finden, diese jedoch nicht erstellen, aktualisieren oder löschen kann, bitten Sie Ihren Workfront-Administrator, Schreibaktionen zu aktivieren. Weitere Informationen finden Sie unter [Administratorvoraussetzungen](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites) in *Konfigurieren des Adobe Workfront MCP-Servers*.

## Validierungs-Tools

### Dokumente

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Dokumentversion nach Namen suchen | `approvals_find_document_version_by_name` | Sucht die aktuelle Versions-ID eines Dokuments nach Dateinamen. Unterstützt Teilübereinstimmungen. | Lesen |
| Dokument nach Versions-ID abrufen | `approvals_get_document_by_version_id` | Ruft Dokumentdetails (Name, Größe, Upload-Datum, Uploader) für eine bekannte Dokumentversions-ID ab. | Lesen |
| Dokumente nach Projekt abrufen | `approvals_get_documents_by_project` | Listet Dokumente innerhalb eines Workfront-Projekts mit der aktuellen Versions-ID jedes Dokuments auf. | Lesen |
| Dokumentbereich auflösen | `approvals_resolve_document_scope` | Erweitert ein Projekt oder einen Ordner in die Liste der darin enthaltenen Dokumentversions-IDs. Unterstützt Bereiche mit Projekt-, Ordner- und Ordnernamen. | Lesen |
| Auflisten von mit AEM verknüpften Ordnern | `approvals_list_aem_linked_folders` | Listet Workfront-Dokumentordner auf, die mit Adobe Experience Manager verknüpft sind. | Lesen |
| Dokumente an AEM-Ordner senden | `approvals_send_documents_to_aem_folder` | Verschiebt ein oder mehrere Workfront-Dokumente in einen mit AEM verknüpften Ordner. | Schreiben |

### Genehmigungs-Workflows

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Informationen zum Genehmigungs-Workflow abrufen | `approvals_get_approval_info` | Gibt den aktuellen Genehmigungs-Workflow (Phasen, Teilnehmer, Status) für eine Dokumentversion aus. | Lesen |
| Genehmigungs-Workflow erstellen oder aktualisieren | `approvals_create_or_update_approval_workflow` | Erstellt oder aktualisiert die Genehmigungs-Workflow-Phasen für eine Dokumentversion. Unterstützt lineare und parallele (Graph-)Stufenabhängigkeiten. | Schreiben |
| Genehmigung aus Vorlage erstellen | `approvals_create_approval_from_template` | Erstellt einen Genehmigungs-Workflow für ein Dokument unter Verwendung einer vorhandenen Vorlage. | Schreiben |
| Dokumentgenehmigung anfordern | `approvals_request_document_approval` | Öffnet ein geführtes Formular zum Anfordern von Genehmigungen für eine Dokumentversion (Titel, genehmigende Personen/Prüfer, optionales Fälligkeitsdatum und Meldung). | Schreiben |
| Genehmigungsphase löschen | `approvals_delete_approval_stage` | Löscht eine einzelne Phase aus einem Genehmigungs-Workflow nach Name oder Position. Nur nicht gestartete Stadien können gelöscht werden. | Schreiben |

### Reminders

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Erinnerung an Teilnehmer senden | `approvals_send_reminder_to_participants` | Sendet Erinnerungs-E-Mails an bestimmte Teilnehmer in einer Genehmigungsphase. Funktioniert nur bei gestarteten, nicht abgeschlossenen, nicht gesperrten Phasen. | Schreiben |
| Erinnerung an unentschlossene Teilnehmer senden | `approvals_send_reminder_to_undecided` | Sendet Erinnerungs-E-Mails an alle unentschlossenen Teilnehmer (benachrichtigt, geöffnet oder kommentiert) in einer Genehmigungsphase. | Schreiben |

### Genehmigungsvorlagen

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Genehmigungsvorlagen auflisten | `approvals_list_templates` | Listet die in dieser Workfront-Instanz verfügbaren Validierungsvorlagen auf. Unterstützt das Filtern nach Ersteller, Teilnehmer und das Sortieren nach Verwendung. | Lesen |
| Vorlage nach Namen suchen | `approvals_search_template_by_name` | Sucht Validierungsvorlagen nach Namen (Teilübereinstimmung ohne Berücksichtigung der Groß-/Kleinschreibung). | Lesen |
| Erstellen einer Validierungsvorlage | `approvals_create_template` | Erstellt eine neue Validierungsvorlage mit linearen oder diagrammbasierten Stufenabhängigkeiten. | Schreiben |
| Genehmigungsvorlage aktualisieren | `approvals_update_template` | Aktualisiert eine vorhandene Vorlage mit strukturierten Änderungen (Teilnehmer hinzufügen oder entfernen, Stadien umbenennen, Fristen festlegen usw.) | Schreiben |

### Suchen und Benutzer

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Aktuellen Benutzer abrufen | `approvals_get_current_user` | Gibt die Workfront-Identität des aufrufenden Benutzers zurück, einschließlich Name, Benutzer-ID, Name des Home-Teams und ID des Home-Teams. | Lesen |
| Benutzer nach Namen suchen | `approvals_find_user_by_name` | Sucht die ID eines Workfront-Benutzers nach Namen (unscharf oder teilweise Übereinstimmung). Gibt Namen, ID, E-Mail, Titel und Avatar-URL zurück. | Lesen |
| Team nach Namen suchen | `approvals_find_team_by_name` | Sucht die ID eines Workfront-Teams nach Namen (unscharf oder teilweise Übereinstimmung). | Lesen |
| Projekt nach Namen suchen | `approvals_find_project_by_name` | Sucht Workfront-Projekte nach einer teilweisen Namensübereinstimmung im gesamten System. | Lesen |
| Projekte nach Besitzer abrufen | `approvals_get_projects_by_owner` | Listet Workfront-Projekte auf, deren Besitzer der aufrufende Benutzer ist. | Lesen |
| Adobe-Region abrufen | `approvals_get_adobe_region` | Gibt den Adobe-Namen einer Cloud-Anbieter-Region zurück. | Lesen |

## Planungstools

### Arbeitsbereiche

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Arbeitsbereich abrufen | `planning_get_workspace` | Ruft vollständige Details eines Arbeitsbereichs nach ID oder Alias ab. | Lesen |
| Arbeitsbereichsliste abrufen | `planning_get_workspace_list` | Listet alle verfügbaren Arbeitsbereiche mit Cursor-basierter Paginierung auf. | Lesen |
| Arbeitsbereich erstellen | `planning_create_workspace` | Erstellt einen neuen leeren Arbeitsbereich zum Organisieren von Datensatztypen, Feldern und Daten. | Schreiben |
| Arbeitsbereich aus Vorlage erstellen | `planning_create_workspace_from_template` | Erstellt einen neuen Workspace, der mit einer vorhandenen Vorlage vorausgefüllt wurde. | Schreiben |
| Arbeitsbereich aktualisieren | `planning_update_workspace` | Aktualisiert teilweise einen Arbeitsbereich - Name, Beschreibung, Symbol, Abschnitte oder Eigentümer. | Schreiben |
| Arbeitsbereich löschen | `planning_delete_workspace` | Löscht dauerhaft einen Arbeitsbereich und alle zugehörigen Daten. | Schreiben |
| Arbeitsbereich in Vorlage konvertieren | `planning_convert_workspace_to_template` | Speichert einen vorhandenen Arbeitsbereich als wiederverwendbare Vorlage (Administrator erforderlich). | Schreiben |
| Workspace-Freigabe abrufen | `planning_get_workspace_sharing` | Gibt die aktuelle Freigabe- und Berechtigungskonfiguration für einen Arbeitsbereich aus. | Lesen |
| Workspace-Freigabe ändern | `planning_modify_workspace_sharing` | Aktualisiert, wer Zugriff auf einen Arbeitsbereich hat und auf welcher Berechtigungsebene. | Schreiben |

### Eintragstypen

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Datensatztyp abrufen | `planning_get_record_type` | Ruft alle Details eines Datensatztyps ab, einschließlich der Felder und Ansichten. | Lesen |
| Erstellen von Eintragstypen | `planning_create_record_types` | Erstellt einen oder mehrere Datensatztypen in einem Workspace-Abschnitt. | Schreiben |
| Eintragstyp aktualisieren | `planning_update_record_type` | Aktualisiert teilweise den Namen, die Beschreibung, das Symbol oder die Farbe eines Datensatztyps. | Schreiben |
| Eintragstyp löschen | `planning_delete_record_type` | Löscht einen Datensatztyp und alle zugehörigen Datensätze, Felder und Ansichten dauerhaft. | Schreiben |
| Auflisten globaler Datensatztypen | `planning_list_global_record_types` | Listet alle zentral definierten (globalen) Datensatztypen auf, die für den aktuellen Benutzer sichtbar sind. | Lesen |
| Auflisten der hinzuzufügenden globalen Datensatztypen | `planning_list_addable_global_record_types` | Listet globale Datensatztypen auf, die einem bestimmten Arbeitsbereich hinzugefügt werden können. | Lesen |
| Globalen Datensatztyp zu Arbeitsbereich hinzufügen | `planning_add_global_record_type_to_workspace` | Verknüpft einen globalen Datensatztyp mit einem angegebenen Arbeitsbereich. | Schreiben |
| Globalen Eintragstyp aus Arbeitsbereich entfernen | `planning_remove_global_record_type_from_workspace` | Hebt die Verknüpfung eines globalen Datensatztyps mit einem Arbeitsbereich auf und löscht alle Datensätze in diesem Arbeitsbereich. | Schreiben |
| Abrufen von externen Datensatzarbeitsbereichen | `planning_get_external_record_workspaces` | Findet heraus, welche Arbeitsbereiche und Datensatztypen mit einem bestimmten externen Datensatz verbunden sind. | Lesen |
| Datensatztyp-Freigabe abrufen | `planning_get_record_type_sharing` | Gibt die Freigabe und Berechtigungen für einen bestimmten Datensatztyp aus. | Lesen |
| Freigabe des Datensatztyps ändern | `planning_modify_record_type_sharing` | Aktualisiert, wer auf welchen Datensatztyp und welche Berechtigungsstufe zugreifen darf. | Schreiben |

### Einträge

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Datensatz abrufen | `planning_get_record` | Ruft alle Details eines einzelnen Datensatzes nach ID ab. | Lesen |
| Datensätze suchen | `planning_search_records` | Durchsucht und filtert Datensätze innerhalb eines Datensatztyps. | Lesen |
| Masseneintragsaktionen | `planning_bulk_record_actions` | Erstellt, aktualisiert, löscht oder stellt mehrere Datensätze in einer Anfrage wieder her. | Schreiben |
| Verbindungsdatensatz erstellen | `planning_create_connection_record` | Erstellt einen neuen Datensatz in einem verbundenen externen System (z. B. einem Workfront-Projekt). | Schreiben |
| Reihenfolge der Einträge aktualisieren | `planning_update_records_order` | Ändert die Anzeigereihenfolge der Datensätze innerhalb eines Datensatztyps. | Schreiben |
| Datensatz-Änderungsprotokoll abrufen | `planning_get_record_change_log` | Gibt den Bearbeitungsverlauf auf Feldebene für einen Datensatz zurück. | Lesen |
| Datensatzfreigabe abrufen | `planning_get_record_sharing` | Gibt die Freigabekonfiguration für einen bestimmten Datensatz aus. | Lesen |
| Freigabe von Datensätzen ändern | `planning_modify_records_sharing` | Aktualisiert, wer auf einen oder mehrere Datensätze zugreifen kann und auf welcher Berechtigungsebene. | Schreiben |

### Felder

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Feld abrufen | `planning_get_field` | Ruft vollständige Details und Schemawerte für ein Feld nach ID ab. | Lesen |
| Erstellen von Feldern | `planning_create_fields` | Fügt einem Datensatztyp mindestens ein Feld (Spalten) hinzu. | Schreiben |
| Feld aktualisieren | `planning_update_field` | Aktualisiert teilweise den Namen, die Beschreibung, die Optionen oder die Konfiguration eines Felds. | Schreiben |
| Feld löschen | `planning_delete_field` | Entfernt ein Feld und alle zugehörigen Daten dauerhaft aus einem Datensatztyp. | Schreiben |

### Ansichten

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Ansicht abrufen | `planning_get_view` | Gibt vollständige Details einer Ansicht nach ID zurück. | Lesen |
| Ansicht erstellen | `planning_create_view` | Erstellt eine neue Tabelle, Timeline oder Kalenderansicht für einen Datensatztyp. | Schreiben |
| Ansicht aktualisieren | `planning_update_view` | Aktualisiert teilweise die Konfiguration, Filter oder Sortierung einer vorhandenen Ansicht. | Schreiben |
| Ansicht löschen | `planning_delete_view` | Löscht eine Ansicht dauerhaft (Datensätze sind nicht betroffen). | Schreiben |
| Ansicht freigeben | `planning_get_view_sharing` | Gibt die Freigabekonfiguration für eine bestimmte Ansicht aus. | Lesen |
| Ansichtsfreigabe ändern | `planning_modify_view_sharing` | Aktualisiert, wer auf welche Berechtigungsstufe Zugriff auf eine Ansicht hat. | Schreiben |

### Vorlagen

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Vorlagenliste abrufen | `planning_get_template_list` | Listet alle verfügbaren Arbeitsbereichsvorlagen mit Zusammenfassungsinformationen auf. | Lesen |
| Vorlage abrufen | `planning_get_template` | Ruft alle Details einer bestimmten Vorlage nach ID ab. | Lesen |

### Suche und Dienstprogramme

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Ressourcen durchsuchen | `planning_search_resources` | Sucht nach Arbeitsbereichen, Datensatztypen und Ansichten nach Namen. | Lesen |
| Daten zur Suchfreigabe | `planning_search_sharing_data` | Sucht Benutzende, Gruppen, Teams, Rollen und Unternehmen nach Namen für Freigabe und Berechtigungen. | Lesen |
| Benutzende suchen | `planning_search_users` | Sucht nach Benutzern mit Paginierungsunterstützung. | Lesen |

## Workflow-Tools

Workflow-Tools sind allgemeine Aktionen, die die KI-Agentenplattform für die Arbeit mit beliebigen Workfront-Objekten verwendet - Projekten, Aufgaben, Problemen, Stunden, Zuweisungen, Programmen, Portfolios usw.

| Titel | Tool-Name | Funktion | Aktion |
|---|---|---|---|
| Objekte suchen | `workflow_search_any_object` | Sucht nach Workfront-Objekten mit flexiblen Filterparametern, Sortierung und Paginierung. | Lesen |
| Objekt erstellen | `workflow_create_any_object` | Erstellt ein neues Workfront-Objekt wie ein Projekt, eine Aufgabe, ein Problem, eine Stunde, eine Zuweisung, ein Programm oder ein Portfolio. | Schreiben |
| Objekt aktualisieren | `workflow_update_any_object` | Aktualisiert Felder eines bestehenden Workfront-Objekts. | Schreiben |
| Objekt löschen | `workflow_delete_any_object` | Löscht ein Workfront-Objekt nach ID. Erfordert eine explizite Benutzerbestätigung, bevor die Aktion ausgeführt wird. | Schreiben |
| Auflösen von Feldnamen | `workflow_resolve_field_names_any_object` | Konvertiert von Benutzenden bereitgestellte Feldnamen oder Kennzeichnungen in die zugrunde liegenden Workfront-API-Feldnamen, damit die KI-Agentenplattform genaue Anfragen erstellen kann. | Lesen |

## So werden Tools aktualisiert

Wenn Adobe eine neue Version des Workfront MCP-Servers veröffentlicht, verwendet die KI-Agentenplattform automatisch den aktualisierten Toolsatz. Sie müssen nichts auf Ihrer Seite neu verbinden oder ändern.



## Weitere Tools in Kürze verfügbar

Wir arbeiten daran, dem Workfront MCP-Server in Zukunft die folgenden Tools hinzuzufügen:

* Kommentare
* Pinnwand