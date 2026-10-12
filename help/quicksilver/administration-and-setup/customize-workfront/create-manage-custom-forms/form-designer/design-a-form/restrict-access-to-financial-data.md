---
title: Beschränken des Zugriffs auf Finanzdaten in benutzerdefinierten Feldern
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn Sie ein benutzerdefiniertes Feld erstellen, können Sie optionale Einstellungen definieren, um den Zugriff auf Finanzdaten zu beschränken.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 77be87f54c8745b1cdab219d9d0c5f4ea48d86e4
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 8%
---
# Beschränken des Zugriffs auf Finanzdaten in benutzerdefinierten Feldern

Wenn Sie ein benutzerdefiniertes Feld erstellen, können Sie optionale Einstellungen definieren, um den Zugriff auf Finanzdaten zu beschränken. Auf diese Weise können Benutzende, deren Zugriffsebenen bestimmte Berechtigungen haben, die Daten sehen, und sie können keine Finanzdaten sehen, auf die sie keinen Zugriff haben sollten.

Informationen zum Erstellen eines benutzerdefinierten Felds finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Informationen zur Definition des Zugriffs auf Finanzdaten über Zugriffsebenen und -berechtigungen finden Sie unter [Zugriff auf Finanzdaten gewähren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) und [Finanzberechtigungen für ein Objekt freigeben](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf benutzerdefinierte Formulare</td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beschränken des Zugriffs auf Finanzdaten in einem benutzerdefinierten Feld

1. Ein neues benutzerdefiniertes Formular erstellen oder ein vorhandenes Formular öffnen.

   Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Fügen Sie dem Formular ein benutzerdefiniertes Feld hinzu oder wählen Sie ein vorhandenes Feld aus.

   Diese Feldtypen können je nach Zugriff auf Finanzdaten eingeschränkt werden:

   * Einzeiliger Text
   * Absatz
   * Einfachauswahl-Dropdown
   * Mehrfachauswahl-Dropdown
   * Kontrollkästchen-Gruppe
   * Optionsfelder
   * Externer Lookup
   * Externe Suche mit Mehrfachauswahl
   * Berechnet

1. Wählen Sie im Feld **Format** die Option **Währung** aus.

   >[!NOTE]
   >
   >Für berechnete Felder ist jedes Format zulässig. Alle anderen Feldtypen müssen das **Währung**-Format verwenden, da sonst das Feld **Finanzberechtigungstyp** nicht verfügbar ist.

1. (Optional) Aktivieren Sie nur für berechnete Felder die Option **Automatische Berechtigung**, damit die Finanzberechtigungen automatisch aus den Feldern in der Formel erstellt werden können.

1. Wählen Sie eine Option für den **Finanzberechtigungstyp**.

   Diese Einstellung definiert den Zugriffstyp und die Berechtigungen, die Benutzer haben müssen, bevor sie dieses benutzerdefinierte Feld im Formular anzeigen oder bearbeiten können.

   * **Keine Berechtigungen erforderlich:** Alle Benutzer können das Feld sehen, unabhängig von ihrer Zugriffsebene und den Objektberechtigungen.
   * **Allgemein:** Benutzer müssen über eine dieser Optionen verfügen, um das Feld sehen zu können:

     * Ihre Zugriffsebene umfasst die Anzeige oder Bearbeitung des Zugriffs auf Finanzdaten mit aktiviertem Zugriff für General Finance.
     * Ihre Berechtigungen für das Objekt, an das das benutzerdefinierte Formular angehängt ist, umfassen das Anzeigen oder Bearbeiten von General Finance.

   * **Bill:** Benutzer müssen eine dieser Optionen haben, um das Feld sehen zu können:

     * Ihre Zugriffsebene umfasst den Zugriff auf „Anzeigen“ oder „Bearbeiten“ von Finanzdaten, wobei der Zugriff für Abrechnungssätze aktiviert ist.
     * Zu den Berechtigungen für das Objekt, an das das benutzerdefinierte Formular angehängt ist, gehört das Anzeigen oder Bearbeiten von Abrechnungssätzen.

   * **Kosten:** Benutzer müssen über eine dieser Optionen verfügen, um das Feld sehen zu können:

     * Ihre Zugriffsebene umfasst den Zugriff auf „Anzeigen“ oder „Bearbeiten“ von Finanzdaten, wobei der Zugriff für Kostensätze aktiviert ist.
     * Zu den Berechtigungen für das Objekt, an das das benutzerdefinierte Formular angehängt ist, gehören das Anzeigen oder Bearbeiten von Kostensätzen.

   Für berechnete Felder:

   * Das Feld **Finanzberechtigungstyp** ist nicht für das manuelle Festlegen von Berechtigungen verfügbar, wenn das Feld **Automatische Berechtigung** aktiviert ist.
   * Die in der Formel verwendeten Felder bestimmen, ob das Berechtigungsfeld aktiv ist. Wenn das Berechtigungsfeld leer ist (und die automatischen Berechtigungen nicht aktiviert sind), unterstützen die Felder in der Formel die Finanzberechtigungen nicht.
   * Zugriff ist für alle Felder in der Formel erforderlich. Wenn beispielsweise zwei Felder in einem berechneten Feld verwendet werden und auf eines davon die Berechtigung Abrechnung angewendet wurde und auf das zweite die Berechtigung Kosten angewendet wurde, muss der Benutzer über die Berechtigung verfügen, sowohl Abrechnungs- als auch Kostensätze anzuzeigen, um den berechneten Wert anzuzeigen.

1. Um Ihre Änderungen zu speichern, klicken Sie auf **Übernehmen** und setzen Sie den Aufbau des Formulars fort.

   Oder

   Klicken Sie auf **Speichern und schließen**.

## Beispiel

Zwei Projekte werden für einen Benutzer freigegeben:

* Der Benutzer ist berechtigt, beim ersten Projekt alle Finanzierungsoptionen zu bearbeiten
* Der Benutzer ist berechtigt, Abrechnungssätze und allgemeine Finanzdaten für das zweite Projekt anzuzeigen

Wenn der/die Benutzende das erste Projekt bearbeitet, können alle Finanzfelder im benutzerdefinierten Formular bearbeitet werden. Wenn der/die Benutzende das zweite Projekt bearbeitet, sind die auf **Rechnung** oder **Allgemein** gesetzten Felder schreibgeschützt und die auf **Kosten** gesetzten Felder sind nicht sichtbar.

Wenn der/die Benutzende die Projekte in einer Liste oder einem Bericht anzeigt:

* Finanzfelder können gemäß den Berechtigungen und den Berichtseinstellungen angezeigt oder bearbeitet werden
* Finanzfelder sind leer, wenn der Benutzer nicht berechtigt ist, sie anzuzeigen

Beim Exportieren von Projektdetails werden dieselben Finanzfeldwerte (oder leere Felder) wie in der Liste angezeigt.

Bei der Massenbearbeitung beider Projekte werden die Felder „Abrechnung“ und „Allgemeine Finanzen“ als schreibgeschützt angezeigt und die Kostenfelder zeigen „Nicht zutreffend“ an.
