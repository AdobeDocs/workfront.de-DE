---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Verwenden von Adobe Cloud Drive
description: Arbeiten Sie mit Ihren Adobe-Cloud-Speicherprojekten direkt über den Finder oder den Datei-Explorer mit Adobe Cloud Drive. Dateien in jeder Anwendung öffnen und bearbeiten, offline arbeiten und Konflikte lösen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
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
