---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Fehlerbehebung in Adobe Cloud Drive
description: Überprüfen Sie Einschränkungen, Leistungsaspekte und Lösungen für häufige Probleme mit Adobe Cloud Drive unter Mac und Windows.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Fehlerbehebung in Adobe Cloud Drive

In diesem Artikel werden die Einschränkungen von Adobe Cloud Drive, zu berücksichtigende Leistungsaspekte und Lösungen für häufige Probleme beschrieben, auf die Sie stoßen können.

Informationen zum Arbeiten mit Adobe Cloud Drive finden Sie unter [Verwenden von Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Einschränkungen

### Datei- und Ordnervorgänge

* Projektordner sind auf der obersten Ebene schreibgeschützt. Sie können sie nicht umbenennen, löschen oder von Adobe Cloud Drive verschieben. Verwenden Sie die Workfront-Web-Oberfläche, um ein Projekt zu erstellen, umzubenennen oder zu löschen.
* Datei- und Ordnervorgänge in einem Projektordner werden vollständig unterstützt.

### Datei- und Pfadbeschränkungen

* Dateinamen dürfen auf keiner Plattform mehr als 255 Zeichen enthalten.
* Der vollständige Dateipfad (alle Ordnernamen plus Dateiname) darf 1024 Zeichen nicht überschreiten. Dateien mit Pfaden, die länger als dieses Limit sind, werden in Adobe Cloud Drive nicht angezeigt, selbst wenn sie in der Workfront-Web-Oberfläche sichtbar sind.
* Wenn bei einer Datei der Fehler **Vollständiger Pfad zu lang** angezeigt wird, kürzen Sie die Ordnernamen oder verringern Sie die Ordnerverschachtelungstiefe, um den Pfad in den Grenzwert zu bringen.

### Speicherung

* In Adobe Cloud Drive gespeicherte Dateien verwenden lokal Speicherplatz auf dem Gerät.
* Reine Cloud-Dateien verwenden keinen lokalen Speicher.
* Entfernen Sie den Offline-Zugriff für Dateien, die Sie nicht mehr benötigen. Weitere Informationen finden Sie unter [Offline-Zugriff entfernen, um Speicherplatz freizugeben](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space) in [Verwenden von Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).

## Überlegungen zur Leistung

* **Dateigröße:** Die für die Synchronisierung erforderliche Zeit hängt von der Dateigröße ab. Größere Dateien dauern in der Regel länger.
* **Netzwerkgeschwindigkeit:** Schnellere Verbindungen bieten eine bessere Synchronisierungsleistung. Die Synchronisierung wird nach einer Unterbrechung automatisch fortgesetzt.
* **Erstmaliger Zugriff:** Dateien werden bei Ihrem ersten Zugriff bei Bedarf heruntergeladen. Der nachfolgende Zugriff ist schneller, da die Datei lokal zwischengespeichert wird.

## Häufige Probleme

### Adobe Cloud Drive wird nicht angezeigt

**Mögliche Ursachen:**

* Adobe Cloud Drive ist nicht installiert.
* Installation wurde nicht erfolgreich abgeschlossen.
* Ihr Unternehmen verwendet keine Workfront-Version, die die Adobe-Cloud-Datenspeicherung unterstützt.

**Lösungen:**

* Stellen Sie sicher, dass Adobe Cloud Drive installiert ist. Aktivieren Sie **Programme** (Mac) oder **Programme** (Windows).
* Starten Sie Adobe Cloud Drive manuell.
* Wenden Sie sich an Ihren Workfront-Administrator, um zu bestätigen, dass Ihr Unternehmen eine Version von Workfront verwendet, die die Adobe-Cloud-Datenspeicherung unterstützt.
* Installieren Sie bei Bedarf Adobe Cloud Drive neu. Weitere Informationen finden Sie unter [Installieren von Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md).

### Das Adobe Cloud Drive-Symbol wird nicht in der Menüleiste oder in der Taskleiste angezeigt

**Mögliche Ursachen:**

* Die Menüleiste (Mac) oder die Taskleiste (Windows) verfügt nicht über genügend Platz, um das Symbol anzuzeigen.

**Lösungen:**

* **Mac:** Halten Sie den Befehl und ziehen Sie vorhandene Menüleistensymbole, um sie neu anzuordnen oder zu entfernen, wodurch Platz für das Adobe Cloud Drive-Symbol geschaffen wird.
* **Windows:** Klicken Sie in der Taskleiste auf den Aufwärtspfeil **ausgeblendete Symbole anzeigen**, um das Adobe Cloud Drive-Symbol zu finden, und ziehen Sie es dann in den sichtbaren Bereich.

### Projekte werden nicht angezeigt oder einige Projekte fehlen

**Mögliche Ursachen:**

* Sie haben keinen Zugriff auf Projekte.
* Synchronisierung wurde nicht abgeschlossen.
* Es liegt ein Problem mit der Netzwerkverbindung vor.

**Lösungen:**

* Überprüfen des Projektzugriffs in der Workfront-Web-Oberfläche.
* Überprüfen Sie Ihre Netzwerkverbindung.
* Melden Sie sich von Adobe Cloud Drive ab und melden Sie sich wieder an.

### Dateien werden nicht synchronisiert

**Mögliche Ursachen:**

* Es liegt ein Problem mit der Netzwerkverbindung vor.
* Bei der Synchronisierung von Datei oder Ordner ist ein Fehler aufgetreten.
* Sie verfügen nicht über genügend Speicherplatz.

**Lösungen:**

* Überprüfen Sie Ihre Internetverbindung.
* Stellen Sie sicher, dass genügend Speicherplatz verfügbar ist.
* Überprüfen Sie die Dateistatusanzeigen auf Synchronisierungsfehler. Weitere Informationen finden Sie unter [Dateistatusanzeigen](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators) in [Verwenden von Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md).
* Starten Sie Adobe Cloud Drive neu.
* Überprüfen Sie den Status des Adobe Cloud Drive in der Taskleiste (Windows) oder in der Menüleiste (Mac).

### Es kann keine Datei geöffnet werden

**Mögliche Ursachen:**

* Die Datei ist nur in der Cloud verfügbar und der Download ist fehlgeschlagen.
* Die zum Öffnen der Datei erforderliche Anwendung ist nicht installiert.
* Die Datei ist beschädigt.

**Lösungen:**

* Überprüfen Sie die Statusanzeige der Datei.
* Stellen Sie sicher, dass die gewünschte Anwendung installiert ist.
* Klicken Sie mit der rechten Maustaste auf die Datei, wählen Sie **Auf diesem Gerät immer beibehalten** und versuchen Sie dann erneut, sie zu öffnen.
* Stellen Sie sicher, dass die Datei in der Workfront-Web-Oberfläche nicht beschädigt ist.

### Synchronisierung ist langsam

**Mögliche Ursachen:**

* Die Datei ist groß.
* Ihre Netzwerkverbindung ist langsam.
* Viele Dateien werden gleichzeitig synchronisiert.

**Lösungen:**

* Seien Sie geduldig mit großen Dateien. Die Synchronisierung kann fortgesetzt werden, sodass sie nach einer Unterbrechung an der Stelle fortgesetzt wird, an der sie abgebrochen wurde.
* Überprüfen Sie Ihre Netzwerkgeschwindigkeit.
* Anzahl der gleichzeitigen Dateifunktionen begrenzen.
* Bewahren Sie große Dateien nur in der Cloud auf, es sei denn, Sie benötigen Offline-Zugriff.

### Offline-Dateien beanspruchen zu viel Speicherplatz

**Lösungen:**

* Klicken Sie mit der rechten Maustaste auf Offlinedateien und wählen Sie **Speicherplatz freigeben**.
* Überprüfen Sie regelmäßig den Speicherplatz.
* Bewahren Sie große Dateien auf, auf die Sie im reinen Cloud-Modus nur selten zugreifen.

### Sie können keine Dateien oder Ordner erstellen, bearbeiten oder löschen

**Mögliche Ursachen:**

* Sie versuchen, einen Projektordner zu erstellen, umzubenennen oder zu löschen. Projektordner sind auf der obersten Ebene schreibgeschützt.
* Das Projekt ist schreibgeschützt, sodass Sie keine Dateien oder Ordner darin erstellen, bearbeiten oder löschen können.

**Lösungen:**

* Verwenden Sie die Workfront-Web-Oberfläche, um ein Projekt zu erstellen, umzubenennen oder zu löschen.
* Bitten Sie den Projektbesitzer, das Projekt für Sie mit Bearbeitungszugriff freizugeben.

## Hilfe erhalten

Wenden Sie sich bei Lizenzfragen, Problemen mit dem Projektzugriff oder einer organisationsspezifischen Konfiguration an Ihren Workfront-Administrator.

Um Protokolle für die Adobe-Unterstützung freizugeben, führen Sie die Schritte unter [Ausführen des Adobe-Tool zur Protokollerfassung](https://helpx.adobe.com/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html) aus.

## Best Practices

* **Offline-Arbeit planen.** Laden Sie Dateien herunter, bevor Sie reisen oder in Gebieten mit schlechter Konnektivität arbeiten.
* **Synchronisierungsstatus überwachen.** Überprüfen Sie die Dateiindikatoren, bevor Sie Anwendungen schließen.
* **Befolgen Sie die Ordnerstruktur des Projekts.** Organisieren Sie Dateien in Projektordnern so, wie es der Projektinhaber beabsichtigt.
* **Verwenden Sie beschreibende Dateinamen.** Helfen Sie Ihren Team-Mitgliedern, das zu finden, was sie brauchen.
* **Erstellen von Duplikaten vermeiden.** Machen Sie keine unnötigen Kopien von Dateien.
