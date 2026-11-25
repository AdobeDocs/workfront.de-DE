---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Verwenden von Adobe Cloud Drive
description: Arbeiten Sie mit Ihren Adobe-Cloud-Speicherprojekten direkt über den Finder oder den Datei-Explorer mit Adobe Cloud Drive. Dateien in jeder Anwendung öffnen und bearbeiten, offline arbeiten und Konflikte lösen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: c16dc2b8b508f71767999aec7029664f5d31f23f
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 2%
---
# Verwenden von Adobe Cloud Drive

Nach der Installation von Adobe Cloud Drive können Sie direkt im Finder oder im Datei-Explorer mit Ihren Adobe-Cloud-Speicherprojekten arbeiten. Sie können Dateien in jeder Anwendung öffnen und bearbeiten, offline arbeiten und Ihre Änderungen mit Adobe Cloud Drive synchronisieren lassen.

Informationen zum Installieren von Adobe Cloud Drive finden Sie unter [Installieren von Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Version</td> 
   <td>Workflow-Ultimate mit aktiviertem Adobe-Cloud-Speicher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>
      <p>Anzeigen des Zugriffs auf ein Projekt, um es in Adobe Cloud Drive anzuzeigen</p>
      <p>Bearbeiten des Zugriffs auf ein Projekt zum Hinzufügen, Bearbeiten oder Löschen von Dateien</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Zugreifen auf Ihre Projekte

1. Öffnen Sie den Finder (Mac) oder den Datei-Explorer (Windows).
1. Navigieren Sie zu **Adobe Cloud Drive**.
1. Durchsuchen Sie die Liste der Projekte, auf die Sie in Workfront Zugriff haben. Öffnen Sie einen beliebigen Projektordner, um dessen Dateien und Unterordner anzuzeigen.

   >[!NOTE]
   >
   >* Projektordner sind auf der obersten Ebene schreibgeschützt. Sie können Projektordner nicht selbst umbenennen, löschen oder verschieben.
   >* Sie können mit Dateien und Ordnern in einem Projektordner arbeiten - öffnen, bearbeiten, erstellen, löschen usw.
   >* Ältere Workfront-Projekte werden nicht in Adobe Cloud Drive angezeigt. Es sind nur Projekte verfügbar, die im Adobe-Cloud-Speicher gespeichert sind.

## Dateistatusindikatoren

Adobe Cloud Drive verwendet visuelle Indikatoren, um den Dateisynchronisierungsstatus anzuzeigen. Die Symbole in Windows und Mac sind unterschiedlich.

### Dateistatusanzeigen unter Windows

| Symbol | Status | Dateibedeutung | Bedeutung des Ordners |
| --- | --- | --- | --- |
| ![Nur Online-Symbol](assets/acd-windows-online-only.png) | Nur Online | Die Datei ist synchronisiert, aber nur online verfügbar. | Alle Dateien darin sind online verfügbar. |
| ![Synchronisierungssymbol](assets/acd-windows-syncing.png) | Synchronisieren | Die neuesten Dateiaktualisierungen werden mit dem lokalen Cache oder mit dem Adobe-Cloud-Speicher synchronisiert. | Mindestens eine Datei im Ordner wird synchronisiert. |
| ![Symbol „Offline verfügbar“](assets/acd-windows-available-offline.png) | Offline verfügbar | Die Datei ist synchronisiert und offline verfügbar. | Mindestens eine Datei im Ordner ist offline verfügbar. |
| ![Angeheftetes Symbol](assets/acd-windows-pinned.png) | angeheftet (immer auf dem Gerät) | Die Datei wird synchronisiert und immer offline gehalten. Adobe Cloud Drive löscht angeheftete Inhalte nicht automatisch. | Alle Dateien im Ordner befinden sich im lokalen Cache und sind offline verfügbar. |
| ![Schreibgeschütztes Symbol](assets/acd-windows-read-only.png) | Schreibgeschützt | Die Datei ist schreibgeschützt. | Ordner ist schreibgeschützt. |
| ![Sync error icon](assets/acd-windows-sync-error.png) | Synchronisierungsfehler | Datei kann nicht synchronisiert werden. Bewegen Sie den Mauszeiger über das Symbol, um Details anzuzeigen. | Ordner kann nicht synchronisiert werden. Bewegen Sie den Mauszeiger über das Symbol, um Details anzuzeigen. |
| ![Symbol „Ausgeschlossen synchronisieren“](assets/acd-windows-sync-excluded.png) | Synchronisierung ausgeschlossen | Datei kann wegen eines nicht unterstützten Typs oder Namens nicht synchronisiert werden. | Ordner kann wegen eines nicht unterstützten Namens nicht synchronisiert werden. |

### Dateistatusanzeigen in Mac

| Symbol | Status | Dateibedeutung | Bedeutung des Ordners |
| --- | --- | --- | --- |
| (Kein Symbol) | Offline verfügbar | Die Datei ist synchronisiert und offline verfügbar. | Alle Dateien sind offline verfügbar. |
| ![Nur Online-Symbol](assets/acd-mac-online-only.png) | Nur Online | Die Datei ist synchronisiert und nur online verfügbar. | Mindestens eine Datei im Ordner ist nur online. |
| ![Synchronisierungssymbol](assets/acd-mac-syncing.png) | Synchronisieren | Die neuesten Dateiaktualisierungen werden mit dem lokalen Cache oder mit dem Adobe-Cloud-Speicher synchronisiert. | Ordnerinhalt wird synchronisiert. |
| ![Sync error icon](assets/acd-windows-sync-error.png) | Synchronisierungsfehler | Datei kann nicht aktualisiert oder synchronisiert werden. Bewegen Sie den Mauszeiger über das Symbol, um Details anzuzeigen. | Ordner kann nicht aktualisiert oder synchronisiert werden. Bewegen Sie den Mauszeiger über das Symbol, um Details anzuzeigen. |
| ![Symbol „Ausgeschlossen synchronisieren“](assets/acd-windows-sync-excluded.png) | Synchronisierung ausgeschlossen | Die Datei ist von der Synchronisierung ausgeschlossen. | Ordner ist von der Synchronisierung ausgeschlossen. |
| ![Schreibgeschütztes Symbol](assets/acd-mac-read-only.png) | Schreibgeschützt | Die Datei ist schreibgeschützt. | Ordner ist schreibgeschützt. |
| ![Angeheftetes Symbol](assets/acd-windows-pinned.png) | angeheftet (immer auf dem Gerät) | Die Datei ist angeheftet, um offline verfügbar zu sein. Adobe Cloud Drive löscht angeheftete Inhalte nicht automatisch. | Der Ordner ist angeheftet, um offline verfügbar zu sein. |

### Fehler-Tooltips

Wenn ein Synchronisierungsfehler oder -problem auftritt, bewegen Sie den Mauszeiger über das Datei- oder Ordnersymbol, um eine QuickInfo anzuzeigen, die das Problem beschreibt.

| Fehlerkategorie | QuickInfos | Bedeutung |
|---|---|---|
| Synchronisierung ausgeschlossen | Nicht unterstützter Dateityp | Der Dateityp wird von Adobe Cloud Drive nicht unterstützt. |
| Synchronisierung ausgeschlossen | Nicht unterstützter Dateiname | Der Dateiname wird von Adobe Cloud Drive nicht unterstützt. |
| Synchronisierung ausgeschlossen | Übergeordnetes Projekt gelöscht | Das übergeordnete Workfront-Projekt wurde gelöscht. |
| Synchronisierung unterbrochen | Dateiinhalt wird nicht unterstützt | Der Dateiinhalt kann nicht synchronisiert werden (z. B. ein Sicherheitsproblem wurde erkannt). |
| Synchronisierung unterbrochen | Ungültige Zeichen im Dateinamen | Der Dateiname enthält ungültige Zeichen. |
| Synchronisierung unterbrochen | Vollständiger Pfad zu lang | Der Dateipfad überschreitet die maximal zulässige Länge. |
| Synchronisierung unterbrochen | Keine Schreibberechtigung | Ihr Schreibzugriff auf diese Datei oder dieses Projekt wurde widerrufen. |
| Synchronisierungsfehler | Authentifizierungsproblem | Es gibt ein Problem mit Ihren Anmeldedaten. |
| Synchronisierungsfehler | Cloud-Speicher nicht verfügbar | Adobe Cloud Services sind vorübergehend nicht verfügbar. |
| Synchronisierungsfehler | Cloud-Speicher voll | Ihr Cloud-Speicherkontingent ist voll. |
| Synchronisierungsfehler | Lokale Festplatte voll | Auf der lokalen Festplatte ist nicht genügend freier Speicherplatz vorhanden. |
| Synchronisierungsfehler | Keine Internetverbindung | Ihr Gerät ist nicht mit dem Internet verbunden. |
| Synchronisierungsfehler | Unerwarteter Fehler | Unerwarteter Fehler bei der Synchronisierung. |
| Synchronisierungsfehler | Konto gesperrt | Ihr Konto wurde vom Dienst gesperrt. |

>[!NOTE]
>
>Fehler auf Systemebene, wie z. B. getrennte Verbindung, Authentifizierungsfehler, Netzwerkausfall, Volle lokale Festplatte oder voller Cloud-Speicher, werden in der Taskleiste (Windows) oder Menüleiste (Mac) angezeigt, nicht in Einzeldateien.

### Ausschlussliste synchronisieren

Adobe Cloud Drive schließt bestimmte systemgenerierte, temporäre und Sperrdateien von der Synchronisierung aus. Die folgenden Dateitypen und -muster sind ausgeschlossen:

| Kategorie | Dateitypen/-muster | Beschreibung |
|---|---|---|
| Systemdateien | `.DS_Store`, `Thumbs.db` | Cache-Dateien für Betriebssystemmetadaten und Miniaturansichten |
| System- und virtuelle Speicherdateien | `*.sys` (z. B. `hiberfil.sys`, `pagefile.sys`, `swapfile.sys`) | Große Systemdateien, die für virtuellen Speicher, Ruhezustand oder andere Betriebssystemfunktionen verwendet werden. |
| macOS-Indizierungsdateien | `.Spotlight-V100`, `.fseventsd` | macOS Spotlight-Indizierungs- und Dateisystem-Ereignisverfolgungsdateien. |
| Temporäre und Backup-Dateien | `*.tmp`, `*.swp`, `*~`, `*.bak` | Von Anwendungen generierte temporäre, vorübergehende oder Backup-Dateien. |

## Datei öffnen

1. Navigieren Sie in Adobe Cloud Drive zur -Datei.
1. Doppelklicken Sie auf die Datei .

   Die Datei wird in der Standardanwendung geöffnet.

Adobe Cloud Drive unterstützt alle Dateitypen, die eine auf Ihrem Computer installierte Anwendung öffnen kann, darunter:

* Adobe Creative Cloud-Formate (PSD, AI, INDD, PRPROJ, AEP usw.)
* Microsoft Office-Dokumente (DOCX, XLSX, PPTX)
* Bilder (JPG, PNG, GIF usw.)
* Videodateien (MP4, MOV usw.)

>[!NOTE]
>
>Cloud-Dokumentenformate (PSDC, AIDC usw.) werden als Standardäquivalente (PSD, AI usw.) geöffnet, wenn Sie über Adobe Cloud Drive darauf zugreifen.

## Bearbeiten und Speichern einer Datei

1. Öffnen Sie eine Datei aus Adobe Cloud Drive.
1. Nehmen Sie Ihre Änderungen im Programm vor.
1. Speichern Sie die Datei, indem Sie **Datei** > **Speichern** auswählen oder Strg+S (Windows) bzw. Befehl+S (Mac) drücken.

   Ihre Änderungen werden automatisch mit dem Adobe Cloud-Speicher synchronisiert.

>[!IMPORTANT]
>
>Speichern Sie die Dateien über **Datei** > **Speichern** oder den Tastaturbefehl. Vermeiden Sie die Verwendung **Speichern unter** zum Erstellen von Kopien, da dadurch doppelte Dateien im Laufwerk erzeugt werden.

## Erstellen oder Hinzufügen einer neuen Datei

Sie können eine neue Datei direkt in einem Projekt erstellen oder eine vorhandene Datei aus Ihrem lokalen Speicher hinzufügen.

### Erstellen einer neuen Datei aus einer Anwendung

1. Öffnen Sie das Programm, das Sie zum Erstellen der Datei verwenden möchten.
1. Erstellen Sie die Datei wie gewohnt.
1. Wählen Sie beim Speichern einen Speicherort in einem Adobe Cloud Drive-Projektordner aus.

   Die Datei wird in Adobe Cloud Drive angezeigt und mit dem Adobe Cloud-Speicher synchronisiert.

### Hinzufügen einer vorhandenen Datei zu einem Projekt

1. Öffnen Sie im Finder (Mac) oder im Datei-Explorer (Windows) den Projektordner in Adobe Cloud Drive.
1. Ziehen Sie Dateien aus dem lokalen Speicher in den Projektordner.

   Die Dateien werden automatisch mit dem Adobe Cloud-Speicher synchronisiert.

## Dateien und Ordner offline verfügbar machen

Wenn eine Datei oder ein Ordner offline verfügbar ist, können Sie sie oder ihn ohne Internetverbindung öffnen und bearbeiten. Offline-Dateien verwenden lokalen Speicherplatz.

### Datei oder Ordner auf dem Gerät behalten

1. Klicken Sie mit der rechten Maustaste auf die Datei oder den Ordner in Adobe Cloud Drive.
1. Wählen Sie **Immer auf diesem Gerät**.

   Die Datei oder der Ordner wird in Ihren lokalen Cache heruntergeladen, und Sie können damit arbeiten, auch wenn Sie offline sind.

### Offline-Zugriff entfernen, um Speicherplatz freizugeben

1. Klicken Sie mit der rechten Maustaste auf die Offlinedatei oder den Ordner.
1. Wählen Sie **Speicherplatz freigeben**.

   Die Datei bzw. der Ordner verbleibt im Cloud-Speicher, wird jedoch aus dem lokalen Cache entfernt.

>[!NOTE]
>
>Offline-Dateien und -Ordner nutzen lokalen Speicherplatz. Entfernen Sie den Offline-Zugriff für Dateien und Ordner, für die Sie keinen Speicherplatz mehr freigeben müssen.

## Kopieren einer Datei in den lokalen Speicher

Sie können eine Datei aus Adobe Cloud Drive auf Ihr lokales Laufwerk kopieren. Das Original verbleibt in Adobe Cloud Drive, und die Kopie wird zu einer unabhängigen lokalen Datei.

1. Klicken Sie mit der rechten Maustaste auf die Datei in Adobe Cloud Drive.
1. Klicken Sie **Kopieren** und fügen Sie die Datei an der gewünschten Stelle auf dem lokalen Laufwerk ein.

   Die Datei wird in das Ziel kopiert. Das Original verbleibt in Adobe Cloud Drive.

>[!NOTE]
>
>Dateien, die in Ihren lokalen Speicher kopiert werden, sind unabhängige Kopien. Änderungen, die Sie an einer lokalen Kopie vornehmen, werden nicht wieder mit dem Adobe Cloud-Speicher synchronisiert.

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## Dateien in die Cloud hochladen (direkter Upload) {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

Der direkte Upload sendet Dateien von Ihrem Computer direkt an den Adobe Cloud-Speicher, ohne sie zuerst in den Adobe Cloud Drive-Ordner zu kopieren.

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### Dateien hochladen

1. Klicken Sie im Finder (Mac) oder im Datei-Explorer (Windows) mit der rechten Maustaste auf eine Datei.
1. Wählen **In Cloud hochladen** aus.
1. Wählen Sie in der Zielauswahl einen Speicherort in einem der Projekte in Adobe Cloud Drive aus und klicken Sie dann auf **Hier hochladen**.
1. Überwachen Sie den Fortschritt **Abschnitt** Direkter Upload“ im Fenster „Aktivität synchronisieren“.

### Wissenswertes über Direct Upload

* „Direkter Upload“ kopiert das Element in die Cloud. Das ursprüngliche Element bleibt an seinem aktuellen Speicherort.
* Sie können mehrere Elemente auswählen, die gleichzeitig hochgeladen werden sollen.
* Im Abschnitt Direkter Upload werden nur einzelne Dateien bis zu maximal 500 aufgelistet.
* Sie können Elemente aus Ihrem Benutzerverzeichnis oder von einem beliebigen angeschlossenen externen Laufwerk hochladen. Andere Cloud-Speicherorte wie iCloud Drive oder `~/Library/CloudStorage` werden nicht unterstützt.
* Sie müssen mit einem berechtigten Adobe-Konto angemeldet sein. Sie benötigen keine Internetverbindung, um einen Upload zu starten. Ohne Verbindung bleiben Uploads in der Warteschlange.
* Durch das Anhalten der Synchronisierung werden laufende Uploads abgebrochen. Uploads in der Warteschlange werden automatisch fortgesetzt, wenn die Synchronisierung fortgesetzt wird.
* Wenn Sie Adobe Cloud Drive während eines Uploads beenden, werden laufende Uploads als abgebrochen markiert. Uploads in der Warteschlange werden beim Neustart der App automatisch fortgesetzt.
* Ausgeblendete Dateien, symbolische Links und Aliase werden nicht unterstützt.
* Adobe Cloud Drive steuert, wie viele Uploads gleichzeitig ausgeführt werden. Die verbleibenden Uploads bleiben in der Warteschlange, bis ein Slot verfügbar wird.
* Eine Live-Anzahl von Uploads, einschließlich fehlgeschlagener Uploads, wird angezeigt, z. B. „3 Dateien werden hochgeladen“. Wenn alle Uploads erfolgreich abgeschlossen wurden, ändert sich die Anzahl in eine Zusammenfassung, z. B. „3 Dateien hochgeladen“. Wählen Sie **Verwerfen** aus, um sie zu entfernen.

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### Upload-Status

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| Symbol | Status | Beschreibung | Verfügbare Aktionen |
| --- | --- | --- | --- |
| ![Symbol „In Warteschlange“](assets/acd-upload-status-queued.png) | In Warteschlange | Der Upload wartet auf den Start. | **Abbrechen** hebt dieses Element auf. |
| ![Upload-Symbol](assets/acd-upload-status-uploading.png) | Upload läuft | Upload läuft. | **Abbrechen** hebt dieses Element auf. |
| ![Symbol „Abgeschlossen“](assets/acd-upload-status-completed.png) | Abgeschlossen | Upload erfolgreich abgeschlossen. | **In Workfront öffnen** öffnet das Asset in der Workfront-Web-Oberfläche. |
| ![Symbol „Fehlgeschlagen](assets/acd-upload-status-failed.png) | Fehlgeschlagen | Der Upload konnte nicht abgeschlossen werden. | **Quelldatei anzeigen** zeigt die Originaldatei an. **Wiederholen** versucht den Upload erneut. Ein erneuter Versuch ist nur bei bestimmten Fehlern verfügbar. |
| ![Symbol „Abgebrochen“](assets/acd-upload-status-cancelled.png) | Storniert | Der Upload wurde entweder von Ihnen oder vom System angehalten. | Kein. Abgebrochene Uploads werden nicht wiederholt. Sie müssen einen neuen Upload starten. |

Um den Grund für einen Fehler anzuzeigen, bewegen Sie den Mauszeiger über das fehlgeschlagene Element.

### Verwalten der Upload-Liste

Jede Aktion ist nur verfügbar, wenn sie anwendbar ist.

* **Alle Uploads abbrechen:** Verfügbar, wenn Uploads in die Warteschlange gestellt werden oder in Bearbeitung sind. Hebt alle auf.
* **Fehlgeschlagene Uploads wiederholen:** verfügbar, wenn fehlgeschlagene Uploads, die erneut versucht werden können, vorhanden sind. Wiederholt alle. Uploads, für die kein erneuter Versuch unternommen werden kann, bleiben unverändert.
* **Löschen:** verfügbar, wenn keine Uploads in die Warteschlange gestellt sind oder in Bearbeitung sind. Entfernt alle abgeschlossenen, fehlgeschlagenen und abgebrochenen Elemente. Bereits hochgeladene lokale Dateien und Inhalte sind davon nicht betroffen.
* **Automatisches Löschen** Abgeschlossene, fehlgeschlagene und abgebrochene Elemente werden 24 Stunden nach dem letzten Update automatisch entfernt. In die Warteschlange gestellte und in Bearbeitung befindliche Elemente werden nie automatisch entfernt.

## Synchronisierung anhalten und fortsetzen {#pause-resume-sync}

Sie können Adobe Cloud Drive anhalten, wenn Sie nicht möchten, dass Dateien hochgeladen oder heruntergeladen werden, z. B. bei einer langsamen oder getakteten Internetverbindung. Während die Synchronisierung angehalten wird, werden Ihre Änderungen nicht an die Cloud gesendet und Änderungen aus der Cloud werden nicht auf Ihren Computer heruntergeladen. Die Synchronisierung bleibt angehalten, bis Sie sie fortsetzen.

### Synchronisierung anhalten

1. Klicken Sie auf das Symbol Adobe Cloud Drive in der Taskleiste (Windows) oder in der Menüleiste (Mac).
1. Klicken Sie auf **Menü**-Symbol (≡) oben rechts im Fenster &quot;Adobe Cloud Drive“.
1. Wählen Sie **Synchronisierung anhalten** aus.

   >[!TIP]
   >
   >Wenn das Fenster &quot;Adobe Cloud Drive“ geöffnet ist, können Sie auch Strg+P (Windows) oder Befehl+P (Mac) drücken.

   Das Fenster Adobe Cloud Drive zeigt **Synchronisierung wurde angehalten** und die Meldung **Dateien werden erst synchronisiert, wenn Sie fortfahren**. Wenn Sie den Mauszeiger über das Symbol für das Adobe Cloud Drive bewegen, wird **Adobe Cloud Drive (angehalten)** angezeigt.

>[!NOTE]
>
>Synchronisierung anhalten ist nur verfügbar, wenn Sie angemeldet sind und Adobe Cloud Drive verbunden ist.

### Synchronisierung fortsetzen

1. Klicken Sie auf das Symbol Adobe Cloud Drive in der Taskleiste (Windows) oder in der Menüleiste (Mac).
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie **Fortsetzen**.
   * Klicken Sie auf das **Menü**-Symbol (≡) und wählen Sie dann **Synchronisierung fortsetzen** aus. Drücken Sie bei geöffnetem Fenster auch Strg+R (Windows) oder Befehl+R (Mac).

   Adobe Cloud Drive beginnt wieder mit der Synchronisierung, einschließlich aller Änderungen, die Sie während der Synchronisierung vorgenommen haben.

## Versionsverlauf anzeigen und verwalten {#version-history}

Sie können den Versionsverlauf in Adobe Cloud Drive verwenden, um gespeicherte Cloud-Versionen einer unterstützten Datei zu durchsuchen, Versionsdetails und Miniaturansichten anzuzeigen und zu einer früheren Version zurückzukehren. Sie können auch den Namen und die Beschreibung einer Version bearbeiten, wenn Sie über die erforderlichen Berechtigungen verfügen.

### Versionsverlauf anzeigen

1. Navigieren Sie zu Ihrem Adobe Cloud Drive-Ordner im Finder oder Datei-Explorer.
1. Eine unterstützte Datei auswählen.
1. Klicken Sie mit der rechten Maustaste auf die Datei und wählen Sie **Versionsverlauf**.
1. Wählen Sie eine Version aus, um die verfügbaren Details und Miniaturansichten anzuzeigen.

   Wenn die Datei keine früheren Versionen enthält, **„Keine früheren**&quot; angezeigt. Miniaturansichten sind möglicherweise nicht für jede Datei oder Version verfügbar.

### Versionsinformationen bearbeiten

1. Öffnen Sie den Versionsverlauf für die Datei.
1. Wählen Sie die Version aus, die Sie aktualisieren möchten.
1. Öffnen Sie das Optionsmenü der Version und wählen Sie **Versionsinformationen bearbeiten** aus.
1. Geben Sie einen **Versionsnamen“** &quot;**&quot;**.
1. Wählen Sie **Speichern** aus.

   Die aktualisierten Informationen werden gespeichert und angezeigt, wenn Sie den Versionsverlauf erneut öffnen.

### Auf eine frühere Version zurücksetzen

1. Öffnen Sie den Versionsverlauf für die Datei.
1. Wählen Sie die Version aus, die Sie wiederherstellen möchten.
1. Wählen Sie **Auf diese Version zurücksetzen**, falls verfügbar.
1. Warten Sie, bis die Synchronisierung abgeschlossen ist.
1. Öffnen Sie die Datei erneut, um zu überprüfen, ob der Inhalt der ausgewählten Version jetzt aktuell ist.

## Verwalten des lokalen Speichers {#manage-local-storage}

Sie können den lokalen Speicher in Adobe Cloud Drive verwalten verwenden, um die lokale Festplattenauslastung zu überwachen, ein Speicherlimit festzulegen und Dateien anzuzeigen, die als „Immer **diesem Gerät“** sind.

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### Anzeigen der lokalen Speicherverwendung

1. Wählen Sie das Symbol Adobe Cloud Drive aus und öffnen Sie das zugehörige Optionsmenü.
1. Wählen **Lokalen Speicher verwalten**.
1. Überprüfen Sie die aktuelle Speichernutzung und die Liste der Dateien, die als &quot;**auf diesem Gerät“ markiert**.
1. Sortieren Sie die Dateiliste nach **Name** oder **Size**, um bestimmte Dateien zu finden.

### Ändern der lokalen Speicherbegrenzung

1. Öffnen Sie **Lokalen Speicher verwalten** über das Menü Adobe Cloud Drive-Optionen .
1. Geben Sie das gewünschte Speicherlimit ein.
1. Wählen Sie **Speichern**, um die Änderung anzuwenden.

>[!NOTE]
>
>Stellen Sie sicher, dass auf dem Gerät ausreichend freier Speicherplatz verfügbar ist, wenn Sie das Speicherlimit festlegen.

## Anzeigen der Synchronisierungsaktivität {#sync-activity}

Die Aktivität „Synchronisieren“ zeigt die letzte Aktivität zwischen dem Adobe Cloud Drive-Ordner auf Ihrem Computer und dem Adobe Cloud-Speicher an. Überwachen Sie damit Uploads und Downloads, überprüfen Sie abgeschlossene Änderungen und identifizieren Sie Elemente, die nicht synchronisiert werden können.

### Anzeigen der Synchronisierungsaktivität

1. Wählen Sie das Symbol Adobe Cloud Drive in der Menüleiste (Mac) oder in der Taskleiste (Windows) aus.
1. Erweitern Sie den Abschnitt Aktivität synchronisieren mit dem Pfeil neben der Statuszusammenfassung.
1. Überprüfen Sie die aufgelisteten Elemente und deren Statusindikatoren. Bewegen Sie den Mauszeiger über eine Statusanzeige, um den Übertragungsfortschritt, den abgeschlossenen Vorgang oder eine Fehlermeldung anzuzeigen.
1. Wählen Sie das Menü Mehr-Aktionen neben einem Element aus, um die für dieses Element verfügbaren Aktionen anzuzeigen.

### Wissenswertes über Synchronisierungsaktivität

* Die normale Synchronisierung verfolgt Änderungen, die über den Adobe Cloud Drive-Ordner vorgenommen wurden, einschließlich Uploads, Downloads, Erstellungen, Umbenennungen, Verschiebungen und Löschungen.
* Die normale Synchronisierungsliste enthält bis zu 500 aktuelle Einträge. Neue oder aktualisierte Einträge werden oben angezeigt. Ältere Einträge werden möglicherweise entfernt, wenn die Liste ihre Grenze erreicht.
* Ein Eintrag kann zunächst angezeigt **Wird vorbereitet…**, während sein Name oder seine Metadaten aufgelöst werden.
* In der Zusammenfassung wird die Anzahl der derzeit synchronisierten Elemente angezeigt. **Synchronisierung abgeschlossen** bedeutet, dass derzeit keine Elemente aktiv sind. Überprüfen Sie die Liste auf fehlgeschlagene oder ausgeschlossene Elemente, anstatt diese Zusammenfassung als Bestätigung zu behandeln, dass jedes Element erfolgreich war.
* Dateien und Ordner, die von der Synchronisierung ausgeschlossen wurden, werden möglicherweise mit einem Fehler angezeigt, der den nicht unterstützten Namen, den nicht unterstützten Typ oder einen anderen Ausschlussgrund erklärt.
* Aktivität wird beim Abmelden gelöscht. Die Liste ist eine Aktivitätsansicht, kein permanenter Prüfverlauf.

### Synchronisierungsstatus

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| Symbol | Status | Beschreibung | Verfügbare Aktionen |
| --- | --- | --- | --- |
| Warteanzeige | Warten auf Synchronisierung | Das Element wartet darauf, dass seine Operation beginnt. | **Im Finder anzeigen** (Mac) oder **Im Explorer anzeigen** (Windows), falls zutreffend. |
| ![Upload-Symbol](assets/acd-sync-status-uploading.png) | Hochladen/Herunterladen | Dateiinhalt wird übertragen. Bewegen Sie den Mauszeiger über die Anzeige, um die Übertragungsrichtung und den Prozentsatz anzuzeigen, sofern verfügbar. Bei 100 % zeigt die QuickInfo möglicherweise **Wird abgeschlossen…**, bis die Verarbeitung abgeschlossen ist. | **Im Finder anzeigen** oder **Im Explorer anzeigen**, falls zutreffend. |
| ![Symbol „Abgeschlossen“](assets/acd-sync-status-completed.png) | Synchronisierter/abgeschlossener Vorgang | Der Vorgang wurde abgeschlossen. Die QuickInfo kann in der Cloud hochgeladen, heruntergeladen, erstellt, umbenannt, umbenannt, verschoben, gelöscht oder gelöscht identifizieren. | **Im Finder anzeigen** oder **Im Explorer anzeigen** für nicht gelöschte Elemente. **In Workfront öffnen** für geeignete abgeschlossene, nicht gelöschte Elemente. |
| ![Symbol „Fehlgeschlagen](assets/acd-sync-status-failed.png) | Synchronisierung fehlgeschlagen/ausgeschlossen | Das Element konnte nicht synchronisiert werden oder ist von der Synchronisierung ausgeschlossen. Bewegen Sie den Mauszeiger aus dem Grund über die Anzeige. | **Im Finder anzeigen** oder **Im Explorer anzeigen**, falls zutreffend. Beheben Sie das gemeldete Problem, bevor Sie erwarten, dass das Element synchronisiert wird. |

Gelöschte Elemente können nicht lokal angezeigt oder in Workfront aus ihrem Aktivitätseintrag geöffnet werden.

### Verwalten der Aktivitätenliste

| Aktion | Beschreibung |
| --- | --- |
| Erweitern oder reduzieren | Verwenden Sie den Pfeil neben der Synchronisierungszusammenfassung, um einzelne Einträge ein- oder auszublenden. |
| Im Finder anzeigen/Im Explorer anzeigen | Suchen Sie ein nicht gelöschtes Element im Adobe Cloud Drive-Ordner. |
| In Workfront öffnen | Öffnen Sie ein geeignetes abgeschlossenes Element in Workfront in Ihrem Browser. Diese Aktion ist nicht für aktive, fehlgeschlagene oder gelöschte normale Synchronisierungseinträge verfügbar. |
| Löschen | Verfügbar, wenn keine normalen Synchronisierungselemente aktiv sind. Löscht fertige Einträge, einschließlich fehlgeschlagener Einträge, aus der Aktivitätsansicht. Durch Löschen des Verlaufs werden keine lokalen Dateien oder Cloud-Inhalte gelöscht und auch kein Synchronisierungsfehler behoben. |
| Schließen | Nachdem Sie einen abgeschlossenen Batch gelöscht haben, wird möglicherweise eine Zusammenfassung synchronisierter Elemente angezeigt. Klicken Sie auf die Schaltfläche Schließen , um die Zusammenfassung zu schließen. |

>[!NOTE]
>
>Normale Synchronisierungszeilen enthalten nicht die Einzelaktionen **Wiederholen** oder **Abbrechen**, die vom direkten Upload verwendet werden. Weitere Informationen zum direkten Upload finden Sie unter [Dateien in die Cloud hochladen (direkter Upload)](#direct-upload).

## Öffnen eines Elements in Workfront {#open-in-workfront}

In Workfront öffnen führt Sie von einem Element in Adobe Cloud Drive zum entsprechenden Speicherort in Workfront in Ihrem Browser. Verwenden Sie es, um mit dem Cloud-Element in Workfront weiter zu arbeiten, ohne manuell danach zu suchen.

### Öffnen eines Elements im Finder oder Datei-Explorer

1. Öffnen Sie den Ordner &quot;Adobe Cloud Drive“ im Finder (Mac) oder im Datei-Explorer (Windows).
1. Wählen Sie eine einzelne Datei oder einen Ordner aus, der mit einem Workfront-Element verknüpft ist.
1. Klicken Sie mit der rechten Maustaste auf das Element und wählen Sie **In Workfront öffnen**.

   Ihr Browser öffnet den entsprechenden Workfront-Speicherort. Wenn Sie dazu aufgefordert werden, melden Sie sich mit einem Konto an, das Zugriff auf dieses Element hat.

### Öffnen eines Elements aus der Aktivität „Synchronisieren“

1. Wählen Sie das Symbol Adobe Cloud Drive in der Menüleiste (Mac) oder in der Taskleiste (Windows) aus.
1. Erweitern Sie den Abschnitt Aktivität synchronisieren .
1. Öffnen Sie für ein geeignetes abgeschlossenes, nicht gelöschtes Element das Menü Mehr Aktionen und wählen Sie **In Workfront öffnen**.
1. Verwenden Sie für eine Datei, die über den direkten Upload hochgeladen wurde, dieselbe Aktion bei ihrem abgeschlossenen Eintrag im Abschnitt **Direkter Upload**.

### Wissenswertes über Open in Workfront

* Wählen Sie jeweils nur ein Element aus. Das Öffnen mehrerer ausgewählter Elemente in Workfront wird nicht unterstützt.
* Im Datei-Explorer ist der Befehl für Elemente außerhalb des Adobe Cloud Drive-Ordners und für den Laufwerkstamm selbst ausgeblendet. Er ist deaktiviert, wenn mehrere Elemente ausgewählt sind.
* Ein Element muss über einen entsprechenden Workfront-Speicherort verfügen. Einige Ordner oder andere Elemente verfügen möglicherweise nicht über eine Workfront-Zuordnung, auch wenn sie in Adobe Cloud Drive sichtbar sind.
* Ein neues lokales Element, das den Upload noch nicht abgeschlossen hat, hat möglicherweise noch keinen Workfront-Link. Warten Sie, bis der Upload abgeschlossen ist, bevor Sie es erneut versuchen.
* In der normalen Synchronisierungsaktivität wird die Aktion nur für qualifizierte abgeschlossene Einträge angeboten. Sie wird nicht für aktive, fehlgeschlagene oder gelöschte Einträge angeboten.
* Beim direkten Upload wird die Aktion für abgeschlossene Uploads angeboten, nicht für Einträge in der Warteschlange, Uploads, fehlgeschlagene oder abgebrochene.
* Sie müssen bei Adobe Cloud Drive angemeldet sein. Workfront bittet Sie möglicherweise auch, sich separat im Browser anzumelden, wobei Ihre Workfront-Berechtigungen weiterhin gelten.
* Sie benötigen eine Internetverbindung, um einen nicht zwischengespeicherten Link abzurufen und auf Workfront zuzugreifen. Ein zuvor aufgelöster Link bietet keinen Offline-Zugriff auf Workfront.
* Diese Aktion öffnet Workfront in einem Browser. Es öffnet die Datei nicht in seiner Desktop-Anwendung, lädt keine weitere Kopie hoch und ändert auch nicht die lokale Offline-Verfügbarkeit.

### In Workfront öffnen verfügbar

| Element oder Status | Im Workfront-Verhalten öffnen | Erforderliche Schritte |
| --- | --- | --- |
| Einzelnes geeignetes Element in Adobe Cloud Drive | Öffnet den entsprechenden Workfront-Speicherort. | Wählen Sie **In Workfront öffnen** aus. |
| Mehrere ausgewählte Elemente | Das Öffnen mehrerer Elemente wird nicht unterstützt. Der Datei-Explorer deaktiviert den Befehl. | Ein einzelnes Element auswählen. |
| Neues Element wird noch hochgeladen | Der Workfront-Link ist möglicherweise noch nicht verfügbar. | Warten Sie, bis der Upload abgeschlossen ist, und versuchen Sie es dann erneut. |
| Normale Synchronisationseingabe abgeschlossen | Verfügbar, wenn das Element geeignet ist und nicht gelöscht wurde. | Verwenden Sie das Menü Mehr-Aktionen des Eintrags. |
| Vollständiger direkter Upload-Eintrag | Verfügbar nach Abschluss des Uploads. | Verwenden Sie das Menü Mehr-Aktionen des Eintrags. |
| Element ohne Workfront-Zuordnung | Eine Meldung weist darauf hin, dass das Element nicht in Workfront verfügbar ist. | Markieren Sie das Element direkt in Workfront oder wählen Sie ein anderes unterstütztes Element aus. |
| Gelöschter normaler Synchronisierungseintrag | Die Aktion ist nicht verfügbar. | Verwenden Sie Workfront direkt, wenn Sie das gelöschte Element untersuchen müssen. |

## Abmelden von Adobe Cloud Drive

Wenn Sie sich von Adobe Cloud Drive abmelden, bleibt das Laufwerk im Finder oder Datei-Explorer sichtbar. Alle Änderungen, die Sie während der Abmeldung im Laufwerk vornehmen, und alle Änderungen, die vor der Abmeldung nicht synchronisiert wurden, werden nicht mit der Cloud synchronisiert.

Was als Nächstes geschieht, hängt davon ab, mit welchem Konto Sie sich wieder anmelden.

### Melden Sie sich mit demselben Konto wieder an

Adobe Cloud Drive behält den lokalen bereitgestellten Ordner bei, wenn Sie sich abmelden. Wenn Sie sich mit denselben Anmeldeinformationen erneut anmelden:

* Adobe Cloud Drive verwendet die vorhandene Bereitstellung automatisch.
* Alle nicht synchronisierten Änderungen, die Sie vor dem Abmelden vorgenommen haben, werden beibehalten und nach der Wiederherstellung der Verbindung synchronisiert.
* Es ist keine Aktion von Ihnen erforderlich.

### Mit einem anderen Konto anmelden

Wenn Sie sich nach der Abmeldung mit einem anderen Adobe-Konto anmelden:

* Der aktuelle bereitgestellte Ordner wird automatisch umbenannt und gesichert. Der Name des Sicherungsordners hat folgendes Format: `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`.
* Das dem neuen Konto zugeordnete Adobe-Cloud-Laufwerk wird wie gewohnt im Finder oder Datei-Explorer verfügbar sein.
* Sie können nicht synchronisierte Arbeiten manuell aus dem Sicherungsordner wiederherstellen, bevor Sie sie entfernen.

>[!NOTE]
>
>Sicherungsordner werden in `~/Library/CloudStorage` unter Mac und `C:\Users\<user>\` unter Windows gespeichert. Wenn Sie mehrmals zwischen Konten wechseln, werden mehrere Sicherungsordner mit Zeitstempel erstellt. Regelmäßige Überprüfung und Bereinigung von Backups, um Speicherplatz freizugeben.

## Lösen von Dateikonflikten

Konflikte können in jeder der folgenden Situationen auftreten:

* Mehrere Benutzer bearbeiten oder löschen dieselbe Datei gleichzeitig.
* Eine Datei wird geändert, während sie von einem anderen Benutzer geöffnet ist.
* Netzwerkunterbrechungen verursachen Synchronisierungsprobleme.

### Wie Adobe Cloud Drive Konflikte löst

Adobe Cloud Drive verwendet eine Duplizierungsstrategie für Konflikte:

* **Keine Dateisperrung.** Mehrere Benutzer können Dateien gleichzeitig bearbeiten.
* **Automatische Duplizierung.** Wenn Adobe Cloud Drive einen Konflikt erkennt, werden beide Versionen beibehalten.
* **Namen löschen.** Die Konfliktdateien enthalten den Benutzernamen und den Zeitstempel in folgendem Format: `filename (Conflicted copy from username on date_time).extension`. Beispiel: `hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`.

### Konflikt manuell lösen

1. Identifizieren Sie die Konfliktdatei. Konfliktdateien enthalten „Konfliktkopie“ im Dateinamen.
1. Überprüfen Sie beide Versionen, um festzustellen, welche richtig ist.
1. Behalten Sie die richtige Version bei und löschen Sie die andere Version.
1. Geben Sie der gespeicherten Datei einen geeigneten Namen.

>[!TIP]
>
>So minimieren Sie Konflikte:
>
>* Überprüfen Sie den Synchronisierungsstatus, bevor Sie Dateien bearbeiten.
>* Kommunizieren Sie mit Team-Mitgliedern darüber, wer welche Dateien bearbeitet.
>* Speichern Sie häufig, damit Änderungen sofort synchronisiert werden.
>* Schließen Sie die Dateien, wenn Sie die Bearbeitung abgeschlossen haben.
