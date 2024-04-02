---
title: Verbesserungen für Administratoren im zweiten Quartal 2024
description: Verbesserungen für Administratoren im zweiten Quartal 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 30a10e240b0f418f7ba49cd2e70e6f3d33956cd6
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Verbesserungen für Administratoren im zweiten Quartal 2024

Auf dieser Seite werden alle Administratorverbesserungen beschrieben, die mit der Version vom zweiten Quartal 2024 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im Versionszyklus des zweiten Quartals 2024 verfügbar sind, finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Logik und Logik zum Überspringen sind jetzt im Vorschaumodus des Formulardesigners verfügbar

>[!NOTE]
>
>Vorschau-Version: 28. März 2024; Produktion für alle Kunden: 24.4 (April 2024)

Mit dem benutzerdefinierten Beta-Formularentwickler können Sie jetzt Ihre Anzeigelogik testen und die Logik im Vorschaumodus überspringen. Zuvor wurden alle Felder auch bei Anwendung der Logik in der Vorschau angezeigt.

Weitere Informationen zur Vorschau eines benutzerdefinierten Formulars im Formularentwickler finden Sie unter [Organisieren und Anzeigen einer Vorschau eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Unternehmen und Benutzer unterstützen jetzt erweiterte benutzerdefinierte Formularfelder

>[!NOTE]
>
>Vorschau-Version: 14. März 2024; Produktion für alle Kunden: 24.4 (April 2024)

Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind jetzt verfügbar, wenn Sie ein benutzerdefiniertes Formular an ein Unternehmen oder einen Benutzer anhängen. Die erweiterten Funktionen sind auf den Seiten &quot;Firmendetails&quot;und &quot;Benutzerdetails&quot;verfügbar, nicht in den Dialogfeldern &quot;Unternehmen bearbeiten&quot;und &quot;Benutzer bearbeiten&quot;. Das benutzerdefinierte Formular muss im neuen Formularentwickler erstellt werden, um diese Feldtypen nutzen zu können.

Weitere Informationen zu benutzerdefinierten Formularfeldern finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## JumpSeat-Integration jetzt für neue Pakettypen verfügbar

>[!NOTE]
>
>Vorschau-Version: 26. Februar 2024; Produktion für schnelle Veröffentlichung: Mit Version 24.3 (14. März 2024); Produktion für alle Kunden: 24.4 (April 2024)

Die vorhandene JumpSeat-Integration ist jetzt für Konten verfügbar, die einen der neuen Pakettypen verwenden (d. h. Select, Prime oder Ultimate). Sie müssen weiterhin über ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.

Weitere Informationen zur JumpSeat-Integration finden Sie unter [Konfigurieren der JumpSeat-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Native Workfront-Felder sind in der Beta-Version des Formulardesigners verfügbar.

>[!NOTE]
>
>Vorschau-Version: 29. Februar 2024; Produktion für schnelle Veröffentlichung: Mit Version 24.3 (14. März 2024); Produktion für alle Kunden: 24.4 (April 2024)

In Workfront native Felder können jetzt zu benutzerdefinierten Formularen hinzugefügt werden. Mit diesem neuen Feldtyp können Sie Daten logisch organisieren und darstellen, ohne vorhandene Daten in benutzerdefinierten Feldern neu erstellen zu müssen.

Nachdem Sie in der Liste der benutzerdefinierten Formularfelder die Option &quot;Natives Feld&quot;ausgewählt haben, um das Feld zum Formularentwickler hinzuzufügen, können Sie ein beliebiges natives Feld für die Formularobjekte auswählen. Wenn beispielsweise in der Liste &quot;Objekttypen&quot;oben im Formularentwickler &quot;Projekt&quot;angezeigt wird, können Sie native Felder für Projekte auswählen, jedoch nicht für Aufgabenfelder.

Wenn das benutzerdefinierte Formular an ein Objekt angehängt wird, wird das Feld aus den Objektdaten ausgefüllt. Beispielsweise ruft das Feld Beschreibung in einem benutzerdefinierten Formular, das an ein Projekt angehängt ist, die Projektbeschreibung ab. (Wenn keine Daten verfügbar sind, kann im Feld &quot;K. A.&quot;angezeigt werden.)

Native Felder, die in benutzerdefinierten Formularen verwendet werden, stehen in der Feldbibliothek im Designer zur Wiederverwendung zur Verfügung. Sie sind auch im Bereich Einrichtung > Benutzerdefinierte Forms > Felder sichtbar, damit Sie sehen können, in welchen Formularen sie verwendet werden.

Diese Funktion ist nur in der Beta-Version des Formulardesigners verfügbar, nicht aber in der Legacy-Form-Builder.

Weitere Informationen finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Die Attributzuordnung ist jetzt für Organisationen verfügbar, die zu Adobe IMS migriert haben

>[!NOTE]
>
>Vorschau-Version: 22. Februar 2024; Produktion für alle Kunden: 22. Februar 2024

Workfront-Systemadministratoren können jetzt die Zuordnung von Benutzerattributen für Organisationen einrichten, die zu Adobe IMS migriert wurden. Auf diese Weise können Benutzerinformationen vom SSO-Provider (Single Sign-on) des Unternehmens an Workfront weitergegeben werden, sodass die Benutzerdaten nicht sowohl in Workfront als auch im SSO-Provider eingegeben werden müssen.

Bisher war diese Funktion nur für Organisationen verfügbar, die noch nicht in Adobe IMS integriert waren.

Anweisungen zum Konfigurieren der Zuordnung von Attributen finden Sie unter [Zuordnen von Benutzerattributen zum einheitlichen Adobe-Erlebnis](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) im Artikel **Benutzerattribute zuordnen und neue Benutzer automatisch bereitstellen**.

## Logik und Anzeigenlogik überspringen sind jetzt in der Beta-Version des Formulardesigners verfügbar

>[!NOTE]
>
>Vorschau-Version: 8. Februar 2024; Produktion für schnelle Veröffentlichung: Mit Version 24.2 (15. Februar 2024); Produktion für alle Kunden: TBD

Sie können jetzt die vorhandene Anzeige bearbeiten und die Logik überspringen und benutzerdefinierte Formulare in der Beta-Version des Formulardesigners um eine neue Logik erweitern. Mit einem benutzerfreundlichen Logikaufbau können Sie festlegen, welche Felder je nach Auswahl im Formular angezeigt oder übersprungen werden sollen.

Symbole auf einem Feld auf der Arbeitsfläche des Formularentwurfs zeigen an, dass die Logik für dieses Feld konfiguriert ist oder dass das Feld in Logikregeln verwendet wird, die für andere Felder konfiguriert sind.

Weitere Informationen finden Sie unter [Fügen Sie die Anzeigenlogik hinzu und überspringen Sie die Logik mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
