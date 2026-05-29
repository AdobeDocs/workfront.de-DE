---
title: Verbesserungen für Administratoren im dritten Quartal 2026
description: Verbesserungen für Administratoren im dritten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3d8439efd8a92042098fbf995aacf2fe3add43f2
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 2%

---

# Verbesserungen für Administratoren im dritten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom dritten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

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
