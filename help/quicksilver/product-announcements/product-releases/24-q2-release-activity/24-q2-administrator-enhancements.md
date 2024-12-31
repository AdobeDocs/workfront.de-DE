---
title: Verbesserungen für Administratoren im zweiten Quartal 2024
description: Verbesserungen für Administratoren im zweiten Quartal 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 0%

---

# Verbesserungen für Administratoren im zweiten Quartal 2024

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit der Version vom zweiten Quartal 2024 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im zweiten Quartal 2024 verfügbar sind, finden Sie unter [Versionsübersicht 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## Anzeigelogik und Überspringen-Logik sind jetzt im Vorschaumodus des Formular-Designers verfügbar

>[!NOTE]
>
>Vorschau-Version: 28. März 2024; Produktion für alle Kunden: 24.4 (11. April 2024)

Mit dem benutzerdefinierten Beta-Formular-Designer können Sie jetzt Ihre Anzeigelogik testen und im Vorschaumodus die Logik überspringen . Zuvor wurden alle Felder in der Vorschau angezeigt, selbst wenn Logik angewendet wurde.

Weitere Informationen zur Vorschau eines benutzerdefinierten Formulars im Formular-Designer finden Sie unter [Organisieren und Vorschau eines Formulars mit dem Formular-Designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Unternehmen und Benutzer unterstützen jetzt erweiterte benutzerdefinierte Formularfelder

>[!NOTE]
>
>Vorschau-Version: 14. März 2024; Produktion für alle Kunden: 24.4 (11. April 2024)

Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind jetzt verfügbar, wenn Sie ein benutzerdefiniertes Formular an ein Unternehmen oder einen Benutzer anhängen. Die erweiterten Funktionen sind auf den Seiten „Firmendetails“ und „Benutzerdetails“ verfügbar, nicht in den Dialogfeldern „Unternehmen bearbeiten“ und „Benutzer bearbeiten“. Das benutzerdefinierte Formular muss im neuen Formular-Designer erstellt werden, um diese Feldtypen nutzen zu können.

Weitere Informationen zu benutzerdefinierten Formularfeldern finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Die JumpSeat-Integration ist jetzt für neue Pakettypen verfügbar

>[!NOTE]
>
>Vorschau-Version: 26. Februar 2024; Produktion für die schnelle Version: Mit der Version 24.3 (14. März 2024); Produktion für alle Kunden: 24.4 (11. April 2024)

Die bestehende JumpSeat-Integration ist jetzt für Konten verfügbar, die einen der neuen Pakettypen verwenden (d. h. Select, Prime oder Ultimate). Sie müssen weiterhin über ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.

Weitere Informationen zur JumpSeat-Integration finden Sie unter [Konfigurieren der JumpSeat-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Native Workfront-Felder sind in der Beta-Version von Form Designer verfügbar

>[!NOTE]
>
>Vorschau-Version: 29. Februar 2024; Produktion für die schnelle Version: Mit der Version 24.3 (14. März 2024); Produktion für alle Kunden: 24.4 (11. April 2024)

Die in Workfront nativen Felder können jetzt zu Ihren benutzerdefinierten Formularen hinzugefügt werden. Mit diesem neuen Feldtyp können Sie Daten logisch organisieren und den Benutzern präsentieren, ohne vorhandene Daten in benutzerdefinierten Feldern neu erstellen zu müssen.

Nachdem Sie in der Liste der benutzerdefinierten Formularfelder das native Feld ausgewählt haben, um das Feld zum Formular-Designer hinzuzufügen, können Sie jedes native Feld für die Objekte des Formulars auswählen. Wenn beispielsweise die Liste Objekttypen oben im Formular-Designer „Projekt“ anzeigt, können Sie native Felder für Projekte auswählen, jedoch keine Felder, die speziell für Aufgaben verwendet werden.

Wenn das benutzerdefinierte Formular an ein Objekt angehängt wird, wird das Feld aus den Objektdaten gefüllt. Beispielsweise ruft das Feld Beschreibung in einem benutzerdefinierten Formular, das an ein Projekt angehängt ist, die Projektbeschreibung ab. (Wenn keine Daten verfügbar sind, kann das Feld „K. A.“ anzeigen.)

Native Felder, die in benutzerdefinierten Formularen verwendet werden, stehen in der Feldbibliothek im Designer zur Wiederverwendung zur Verfügung. Sie sind auch im Bereich Einrichtung > Benutzerdefinierte Forms > Felder sichtbar, sodass Sie sehen können, in welchen Formularen sie verwendet werden.

Diese Funktion ist nur in der Form Designer-Betaversion verfügbar, nicht in Form Builder.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## Attributzuordnung jetzt für Organisationen verfügbar, die zu Adobe IMS migriert haben

>[!NOTE]
>
>Vorschau-Version: 22. Februar 2024; Produktion für alle Kunden: 22. Februar 2024

Workfront-Systemadministratoren können jetzt die Benutzerattributzuordnung für Unternehmen einrichten, die zu Adobe IMS migriert sind. Auf diese Weise können Benutzerinformationen vom SSO-Provider (Single Sign-on) des Unternehmens an Workfront weitergeleitet werden, sodass die Daten des Benutzers nicht sowohl in Workfront als auch beim SSO-Provider eingegeben werden müssen.

Zuvor war diese Funktion nur für Organisationen verfügbar, die noch nicht in Adobe IMS integriert wurden.

Anweisungen zum Konfigurieren der Attributzuordnung finden Sie unter [Zuordnen von Benutzerattributen im einheitlichen Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) im Artikel **Zuordnen von Benutzerattributen und automatische Bereitstellung neuer Benutzer**.

## Logik überspringen und Anzeigelogik sind jetzt in der Beta-Version von Form Designer verfügbar

>[!NOTE]
>
>Vorschau-Version: 8. Februar 2024; Produktion für die schnelle Version: Mit der Version 24.2 (15. Februar 2024); Produktion für alle Kunden: 24.4 (11. April 2024)

Sie können jetzt in der Beta-Version von Form Designer vorhandene Anzeigen- und Überspringen-Logik bearbeiten und benutzerdefinierten Formularen eine neue Logik hinzufügen. Ein benutzerfreundlicher Logik-Builder hilft Ihnen dabei, basierend auf einer Auswahl im Formular zu definieren, welche Felder angezeigt oder übersprungen werden sollen.

Symbole auf einem Feld auf der Arbeitsfläche des Formular-Designers geben an, dass die Logik für dieses Feld konfiguriert ist oder dass das Feld in Logikregeln verwendet wird, die für andere Felder konfiguriert sind.

Weitere Informationen finden Sie unter [Anzeigelogik hinzufügen und Logik mit dem Formular-Designer überspringen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
