---
title: Verbesserungen für Administratoren im dritten Quartal 2026
description: Verbesserungen für Administratoren im dritten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: a9688886f32cd41dd7d53dbf0a918f25fdd04a0b
workflow-type: tm+mt
source-wordcount: '1328'
ht-degree: 5%

---

# Verbesserungen für Administratoren im dritten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom dritten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

<!--

## Change tracking for unified review and approval

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The Change History page in Workfront now captures activity across unified review and approval workflows, giving administrators a complete governance trail for review and document lifecycle events.

Approval, stage, and participant actions are now tracked. These actions may include:

* Making an approval decision in the Frame.io viewer
* Creating or deleting an approval
* Updating a document such as renaming, moving, or deleting it

Each entry includes the standard tracked fields: date and time, operation, user name (or "system generated"), and object name. Frame.io viewer comments are not included.

This phase of change tracking does not include MCP events. Those will be part of a future release.

For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

-->

## Internes Lookup-Feld, das den Typ Typeahead ersetzt

>[!NOTE]
>
>Vorschau: 7. Juli 2026Produktions-Schnellveröffentlichung: 15. Juli 2026Produktion für alle: 16. Juli 2026

Der neue Feldtyp **Interne Suche** in benutzerdefinierten Formularen bietet dynamische Filterung. Es ähnelt dem Feldtyp mit automatischer Textvervollständigung und ermöglicht es Benutzenden, vorhandene Workfront-Objekte zu suchen und auszuwählen, indem sie einen Teil des Namens eingeben. Der Filter für die interne Suche kann auf den Wert in einem anderen Feld im Formular verweisen, was mit Typeahead nicht möglich ist.

Die Mehrfachauswahl wird bei internen Suchen unterstützt, und dieser Feldtyp bietet auch eine verbesserte Leistung für große Datensätze. Die folgenden nativen Workfront-Objekte werden bei der internen Suche unterstützt: Projekt, Unternehmen, Gruppe, Aufgabengebiet, Portfolio, Programm, Team, Vorlage, Benutzer, Aufgabe, Problem, Dokument und Standort.

Der Feldtyp Interne Suche ersetzt den Feldtyp mit automatischer Textvervollständigung . Sie können vorhandene Felder mit automatischer Textvervollständigung schnell in interne Suchen konvertieren, indem Sie auf die Schaltfläche in den Feldoptionen auf der rechten Seite klicken. Bei der Konvertierung bleiben historische Daten im Feld und werden in Berichten auf die gleiche Weise verwendet.

>[!IMPORTANT]
>
>Externe Integrationen wie Workfront Fusion-Szenarien oder API-basierte Automatisierungen können auf veraltete Feldstrukturen verweisen und erfordern nach der Konvertierung Aktualisierungen. Sie sollten alle Integrationen überprüfen, bevor Sie Typeahead-Felder in interne Lookup-Felder konvertieren.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Von nativen Referenzfeldern unterstützte Standardwertlogik

>[!NOTE]
>
>Vorschau: 7. Juli 2026Produktions-Schnellveröffentlichung: 15. Juli 2026Produktion für alle: 16. Juli 2026
>
>Diese Funktion ist nur für Organisationen mit den Workflow-Paketen Prime oder Ultimate verfügbar.

In benutzerdefinierten Formularen können Sie jetzt mit nativen Referenzfeldern eine Standardwertlogik hinzufügen.

Dieser Logiktyp in nativen Referenzfeldern ist nur in der Benutzeroberfläche und nicht in der Workfront-API verfügbar.

Weitere Informationen finden Sie unter [Hinzufügen von Standardwertlogik zu einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) im Artikel [Hinzufügen von Logikregeln zu benutzerdefinierten Formularen und Feldern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Aktualisierungen der nativen Feldfilterung in benutzerdefinierten Formularen

>[!NOTE]
>
>Vorschau: 7. Juli 2026Produktions-Schnellveröffentlichung: 15. Juli 2026Produktion für alle: 16. Juli 2026

Systemfilter, die in nativen Feldern vorhanden sind, werden jetzt auf die Felder in benutzerdefinierten Formularen angewendet und sind für Administratoren sichtbar.

Wenn Sie ein natives Referenzfeld hinzufügen, auf das ein Systemfilter angewendet wurde, können Sie denselben Filter auf das Feld im benutzerdefinierten Formular anwenden und den Filter bei Bedarf im Textfeld Textmodus ändern.

Wenn Sie dem Feld einen eigenen benutzerdefinierten Filter hinzufügen, wird der Systemfilter für das Feld überschrieben. Wenn Sie keinen benutzerdefinierten Filter eingeben, wird der Systemfilter standardmäßig angewendet.

Außerdem ist jetzt dynamische Filterung für native Referenzfelder verfügbar. Mit einem dynamischen Filter können Sie die Liste der Elemente basierend auf dem Wert eines anderen Felds eingrenzen.

Wenn Sie beispielsweise `?portfolioID={portfolio}.{ID}` in einem Projektfeldfilter verwenden und sich im benutzerdefinierten Formular ein natives Portfolio-Feld befindet, werden im Projektfeld nur Projekte angezeigt, die sich im ausgewählten Portfolio befinden. Wenn das Feld Portfolio leer gelassen wird, sind alle Projekte im Feld Projekt verfügbar.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Schützen von Feldnamen vor versehentlichem Umbenennen

>[!NOTE]
>
>Vorschau: 7. Juli 2026Produktions-Schnellveröffentlichung: 15. Juli 2026Produktion für alle: 16. Juli 2026

Zum Schutz von Integrationen und Datenintegrität haben wir aktualisiert, wie Feldnamen im Bedienfeld Feldeinstellungen eines benutzerdefinierten Formulars bearbeitet werden können.

Feldnamen im Bedienfeld Feldeinstellungen sind jetzt standardmäßig schreibgeschützt. Sie können den Feldnamen weiterhin bearbeiten, für die Umbenennung ist jedoch ein expliziter Bestätigungsschritt erforderlich. Das Feld **Name** wurde ebenfalls in &quot;**&quot;**, um seine technische Bedeutung besser widerzuspiegeln. Das Feld **label** bleibt bearbeitbar.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

## Anzeigen des Änderungsverlaufs für Workfront-Objekte

>[!NOTE]
>
>Vorschau: 11. Juni 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Um Ihnen die Anzeige der in einer zentralen Liste aufgetretenen Änderungen zu erleichtern, haben wir die Liste „Änderungsverlauf“ erstellt. Diese Liste zeigt Informationen wie das Objekt, den Vorgang und die Quelle der Änderung (z. B. einen Benutzer oder das Workfront-System) an.

Zuvor waren Auditprotokolle verfügbar, die jedoch keine Objekte abdeckten.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des &#x200B;](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

## Neue Systemvoreinstellung zum Konvertieren veralteter Speicherportfolios in Adobe Cloud-Speicher

>[!NOTE]
>
>Vorschau: 11. Juni 2026Produktion für alle: 11. Juni 2026

Workfront-Administratoren können jetzt ältere Speicherportfolios direkt aus den Systemeinstellungen in Adobe Cloud-Speicher konvertieren. Um Portfolios zu konvertieren, wählen Sie sie im neuen Feld Portfolios zum Konvertieren in Unternehmensspeicher auswählen aus und speichern Sie die Seite.

Wenn ein Portfolio in Adobe Cloud-Speicher konvertiert wird:

* Sie können in dieses Portfolio keine Projekte mehr verschieben, die Legacy-Workfront-Speicher verwenden
* Alle in diesem Portfolio neu erstellten Projekte verwenden Cloud-Speicherplatz von Adobe
* Frame.io ist der Viewer für Dokumente, die Adobe Cloud Storage verwenden
* Untergeordnete Objekte, die Legacy-Workfront-Speicher verwenden, verbleiben im Legacy-Speicher

Durch Hinzufügen eines Adobe-Cloud-Speicherprojekts zu einem Legacy-Speicherportfolio wurde das Portfolio zuvor automatisch in Adobe Cloud-Speicher konvertiert.

Weitere Informationen finden Sie unter [Systemvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Rich Text ersetzt Text durch Schrift im Feld „Formatierung“

>[!NOTE]
>
>Vorschau: 28. Mai 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Der neue **Rich-Text**-Feldtyp in benutzerdefinierten Formularen ist ein robuster Texteditor mit Formatierungsoptionen wie Hochgestellt und Tiefgestellt, Überschriften und Tabellen sowie den herkömmlichen Optionen Fett, Kursiv, Unterstrichen, Aufzählungszeichen, Nummerierung, Hyperlinks und Blockanführungszeichen. Die Zeichenbeschränkung bleibt bei 15.000.

Der Rich-Text-Feldtyp ersetzt den Text durch den Feldtyp Formatierung . Sie können vorhandenen Text mit Formatierungsfeldern schnell in Rich-Text konvertieren, indem Sie auf die Schaltfläche in den Feldoptionen rechts klicken. Bei der Konvertierung bleiben historische Daten im Feld und werden in Berichten auf die gleiche Weise verwendet.

>[!IMPORTANT]
>
>Externe Integrationen wie Workfront Fusion-Szenarien oder API-basierte Automatisierungen können auf veraltete Feldstrukturen verweisen und erfordern nach der Konvertierung Aktualisierungen. Sie sollten alle Integrationen überprüfen, bevor Sie Felder in Rich-Text konvertieren.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Native Finanzfelder, die in benutzerdefinierten Formularen unterstützt werden

>[!NOTE]
>
>Vorschau: 28. Mai 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Sie können jetzt native Finanzfelder von Workfront in benutzerdefinierte Formulare einbeziehen. Zuvor wurden die Finanzfelder nicht unterstützt.

Die verfügbaren Finanzfelder, auf die Sie verweisen können, hängen vom Typ des Formulars ab.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-workfront-native-fields).

## Benutzerdefinierte Formulare können systemweit freigegeben werden, mit der Möglichkeit, Anlagen hinzuzufügen

>[!NOTE]
>
>Vorschau: 28. Mai 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Die neue Freigabeoption „Jeder im System kann anzeigen und anhängen“ wurde zu benutzerdefinierten Formularen hinzugefügt. Wenn Sie diese Option auswählen, können alle Benutzer systemweit das Formular an andere Objekte anhängen.

Durch die systemweite Freigabe entfällt die Notwendigkeit, Formulare manuell freizugeben und Berechtigungen über Gruppen oder Agenturen hinweg zu aktualisieren, wenn neue Gruppen hinzugefügt werden.

Weitere Informationen finden Sie unter [Freigeben eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Neue Systemvoreinstellung zum Erzwingen erforderlicher Felder bei der Massenbearbeitung

>[!NOTE]
>
>Vorschau: 28. Mai 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Derzeit werden bei der Massenbearbeitung von Objekten erforderliche Felder nur erzwungen, wenn ein Benutzer das Feld ändert. Wenn ein Feld nicht geändert wird, wird es als optional behandelt und nicht validiert.

Mit einer neuen Systemvoreinstellung können Sie jetzt erforderliche Felder in der Massenbearbeitung erzwingen. Um das Speichern von Massenbearbeitungsobjekten nur zu ermöglichen, wenn alle erforderlichen Felder Werte aufweisen, wählen Sie die Option **Erforderliche Felder bei der Massenbearbeitung immer erzwingen** auf der Seite Setup > System > Voreinstellungen aus.

Weitere Informationen finden Sie unter [Systemvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).
