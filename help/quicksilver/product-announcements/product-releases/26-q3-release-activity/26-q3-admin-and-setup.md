---
title: Verbesserungen für Administratoren im dritten Quartal 2026
description: Verbesserungen für Administratoren im dritten Quartal 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: d83d823426b42202e83cb4db64f85d27d4dca0bb
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 8%

---

# Verbesserungen für Administratoren im dritten Quartal 2026

Auf dieser Seite werden Admin-Verbesserungen beschrieben, die mit der Version vom dritten Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md).

## Änderungsverfolgung zur einheitlichen Überprüfung und Genehmigung

>[!NOTE]
>
>Vorschau: 7. Juli 2026Produktions-Schnellveröffentlichung: 15. Juli 2026Produktion für alle: 16. Juli 2026

Die Seite „Änderungsverlauf“ in Workfront erfasst jetzt Aktivitäten in einheitlichen Prüfungs- und Genehmigungs-Workflows und bietet Admins einen vollständigen Governance-Trail für Prüfungs- und Dokumentenlebenszyklus-Ereignisse.

Genehmigungs-, Staging- und Teilnehmeraktionen werden jetzt verfolgt. Diese Maßnahmen können Folgendes umfassen:

* Treffen einer Genehmigungsentscheidung im Frame.io-Viewer
* Erstellen oder Löschen einer Genehmigung
* Aktualisieren eines Dokuments, z. B. Umbenennen, Verschieben oder Löschen

Jeder Eintrag enthält die getrackten Standardfelder: Datum und Uhrzeit, Vorgang, Benutzername (oder „systemgeneriert„) und Objektname. Frame.io-Viewer-Kommentare sind nicht enthalten.

Diese Phase des Änderungs-Trackings umfasst keine MCP-Ereignisse. Diese werden Teil einer zukünftigen Version sein.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

<!--

## Internal lookup field replacing Typeahead field type

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

The new **Internal lookup** field type in custom forms provides dynamic filtering. It is similar to the Typeahead field type and allows users to search and select existing Workfront objects by typing part of the name. The filter on the internal lookup can reference the value in another field on the form, which is not possible with Typeaheads.

Multi-select is supported on internal lookups, and this field type also provides improved performance for large datasets. The following native Workfront objects are supported in internal lookups: Project, Company, Group, Job Role, Portfolio, Program, Team, Template, User, Task, Issue, Document, and Location.

The Internal lookup field type is replacing the Typeahead field type. You can quickly convert existing Typeahead fields to Internal lookups by clicking the button in the field options on the right. When you convert, historical data remains on the field and it is used the same way in reports.

>[!IMPORTANT]
>
>External integrations such as Workfront Fusion scenarios or API-based automations may reference legacy field structures and require updates after the conversion. You should verify any integrations before converting Typeahead fields to Internal lookup fields.

For more information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Default value logic supported on native reference fields

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026
>
>This feature is only available for organizations on the Workflow Prime or Ultimate packages.

In custom forms, native reference fields now allow you to add default value logic.

This logic type on native reference fields is available only in the user interface and not in the Workfront API.

For information, see [Add default value logic to a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md#add-default-value-logic-to-a-custom-form) in the article [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

-->

<!--

## Updates to native field filtering in custom forms

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

System filters that exist on native fields are now applied to the fields in custom forms and are visible to administrators.

When you add a native reference field that has a system filter applied, you can apply the same filter to the field in the custom form and modify the filter if needed in the Text Mode box.

Adding your own custom filter to the field overrides the system filter for the field. If you do not enter a custom filter, the system filter is applied by default.

Also, dynamic filtering is now available on native reference fields. A dynamic filter allows you to narrow the list of items based on the value of another field.

For example, when you use `?portfolioID={portfolio}.{ID}` in a Project field filter and a Portfolio native field is on the custom form, the Project field shows only projects that are in the selected portfolio. If the Portfolio field is left blank, then all projects are available in the Project field.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

-->

<!--

## Protect field names from accidental renaming

>[!NOTE]
>
>Preview: July 7, 2026
>Production fast release: July 15, 2026
>Production for everyone: July 16, 2026

To protect integrations and data integrity, we've updated how field names can be edited in the field settings panel of a custom form.

Field names in the field settings panel are now read-only by default. You can still edit the field name, but renaming requires an explicit confirmation step. The field previously called **Name** has also been updated to **API Name** to better reflect its technical significance. The **Label** field remains editable.

For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#notes-on-field-names-and-labels).

-->

## Anzeigen des Änderungsverlaufs für Workfront-Objekte

>[!NOTE]
>
>Vorschau: 11. Juni 2026Produktions-Schnellveröffentlichung: 11. Juni 2026Produktion für alle: 16. Juli 2026

Um Ihnen die Anzeige der in einer zentralen Liste aufgetretenen Änderungen zu erleichtern, haben wir die Liste „Änderungsverlauf“ erstellt. Diese Liste zeigt Informationen wie das Objekt, den Vorgang und die Quelle der Änderung (z. B. einen Benutzer oder das Workfront-System) an.

Zuvor waren Auditprotokolle verfügbar, die jedoch keine Objekte abdeckten.

Weitere Informationen finden Sie unter [Anzeigen und Verwalten des ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/view-and-manage-change-history.md).

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
