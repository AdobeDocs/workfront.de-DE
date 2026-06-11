---
title: Verbesserungen für Administratoren im dritten Quartal 2026
description: Verbesserungen für Administratoren im dritten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 34ec779f648db8c3f1a1fe2a76f5b7fda83679a6
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 1%

---

# Verbesserungen für Administratoren im dritten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom dritten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Anzeigen des Änderungsverlaufs für Workfront-Objekte

>[!NOTE]
>
>Vorschau: 11. Juni 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Um Ihnen die Anzeige der in einer zentralen Liste aufgetretenen Änderungen zu erleichtern, haben wir die Liste „Änderungsverlauf“ erstellt. Diese Liste zeigt Informationen wie das Objekt, den Vorgang und die Quelle der Änderung (z. B. einen Benutzer oder das Workfront-System) an.

Zuvor waren Auditprotokolle verfügbar, die jedoch keine Objekte abdeckten.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Neue Systemvoreinstellung zum Konvertieren veralteter Speicherportfolios in Adobe Cloud-Speicher

>[!NOTE]
>
>Vorschau: 11. Juni 2026>Produktion für alle: 11. Juni 2026

Workfront-Administratoren können jetzt ältere Speicherportfolios direkt aus den Systemeinstellungen in Adobe Cloud-Speicher konvertieren. Um Portfolios zu konvertieren, wählen Sie sie im neuen Feld Portfolios zum Konvertieren in Unternehmensspeicher auswählen aus und speichern Sie die Seite.

Wenn ein Portfolio in Adobe Cloud-Speicher konvertiert wird:

* Sie können keine Projekte mehr, die alten Workfront-Speicher verwenden, in dieses Portfolio verschieben
* Alle in diesem Portfolio erstellten neuen Projekte verwenden den Adobe Cloud-Speicher
* Frame.io ist der Viewer für Dokumente, die Adobe Cloud Storage verwenden
* Untergeordnete Objekte, die Legacy-Workfront-Speicher verwenden, verbleiben im Legacy-Speicher

Durch Hinzufügen eines Adobe-Cloud-Speicherprojekts zu einem Legacy-Speicherportfolio wurde das Portfolio zuvor automatisch in Adobe Cloud-Speicher konvertiert.

Weitere Informationen finden Sie unter [Systemvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Rich-Text - Ersetzen von Text durch den Feldtyp Formatierung

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Der neue **Rich-Text**-Feldtyp in benutzerdefinierten Formularen ist ein robuster Texteditor mit Formatierungsoptionen wie Hochgestellt und Tiefgestellt, Überschriften und Tabellen sowie den herkömmlichen Optionen Fett, Kursiv, Unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen. Die Zeichenbeschränkung bleibt bei 15.000.

Der Rich-Text-Feldtyp ersetzt den Text durch den Feldtyp Formatierung . Sie können vorhandenen Text mit Formatierungsfeldern schnell in Rich-Text konvertieren, indem Sie auf die Schaltfläche in den Feldoptionen rechts klicken. Bei der Konvertierung bleiben historische Daten im Feld und werden in Berichten auf die gleiche Weise verwendet.

>[!IMPORTANT]
>
>Externe Integrationen wie Workfront Fusion-Szenarien oder API-basierte Automatisierungen können auf veraltete Feldstrukturen verweisen und erfordern nach der Konvertierung Aktualisierungen. Sie sollten alle Integrationen überprüfen, bevor Sie Felder in Rich-Text konvertieren.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Native Finanzfelder, die in benutzerdefinierten Formularen unterstützt werden

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Sie können jetzt native Finanzfelder von Workfront in benutzerdefinierte Formulare einbeziehen. Zuvor wurden die Finanzfelder nicht unterstützt.

Die verfügbaren Finanzfelder, auf die Sie verweisen können, hängen vom Typ des Formulars ab.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Benutzerdefinierte Formulare können systemweit freigegeben werden und haben Zugriff auf das Anhängen

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Die neue Freigabeoption „Jeder im System kann anzeigen und anhängen“ wurde zu benutzerdefinierten Formularen hinzugefügt. Wenn Sie diese Option auswählen, können alle Benutzer systemweit das Formular an andere Objekte anhängen.

Durch die systemweite Freigabe entfällt die Notwendigkeit, Formulare manuell freizugeben und Berechtigungen über Gruppen oder Agenturen hinweg zu aktualisieren, wenn neue Gruppen hinzugefügt werden.

Weitere Informationen finden Sie unter [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Neue Systemvoreinstellung zum Erzwingen erforderlicher Felder bei der Massenbearbeitung

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Derzeit werden bei der Massenbearbeitung von Objekten erforderliche Felder nur erzwungen, wenn ein Benutzer das Feld ändert. Wenn ein Feld nicht geändert wird, wird es als optional behandelt und nicht validiert.

Mit einer neuen Systemvoreinstellung können Sie jetzt erforderliche Felder in der Massenbearbeitung erzwingen. Um das Speichern von Massenbearbeitungsobjekten nur zu ermöglichen, wenn alle erforderlichen Felder Werte aufweisen, wählen Sie die Option **Erforderliche Felder bei der Massenbearbeitung immer erzwingen** auf der Seite Setup > System > Voreinstellungen aus.

Weitere Informationen finden Sie unter [Systemvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
