---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Tarifattribute definieren
description: Tarifattribute erweitern die Tarifkarten- und Tariffunktionalität von Adobe Workfront, indem sie es Ihnen ermöglichen, zusätzliche Dimensionen zu Tarifen hinzuzufügen, die über das Aufgabengebiet hinausgehen. Workfront kann dann automatisch die richtige Rate für Zuweisungen auswählen, um die finanzielle Genauigkeit und Konsistenz über alle Projekte hinweg sicherzustellen.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 8e948d1c90a9d528c7ffd4963e14630ae7577e70
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 2%

---


# Tarifattribute definieren

{{highlighted-preview-article-level}}

Tarifattribute erweitern die Tarifkarten- und Tariffunktionalität von Adobe Workfront, indem sie es Ihnen ermöglichen, zusätzliche Dimensionen zu Tarifen hinzuzufügen, die über das Aufgabengebiet hinausgehen. Dies ist entscheidend für Agenturen und Unternehmen, bei denen die Preise nicht nur nach Aufgabengebiet, sondern auch nach Faktoren wie Agentur, Standort, Marke, Kostenstelle oder anderen variieren.
Durch Kombination dieser Attribute kann Workfront automatisch die richtige Rate für Zuweisungen auswählen und so die finanzielle Genauigkeit und Konsistenz über alle Projekte hinweg sicherstellen.

>[!IMPORTANT]
>
>Tarifattribute sind eine einmalige grundlegende Einrichtung.

Sobald Attribute aktiviert und auf Tarifkarten und -sätze angewendet wurden, kann eine spätere Änderung dieser Attribute die Datenintegrität in Ihrer gesamten Finanzeinrichtung beeinträchtigen.

## Übersicht über Tarifattribute

Tarifattribute werden aus folgenden Gründen als einmalige Einrichtung betrachtet:

* Attribute werden Teil des Finanzdatenmodells, sobald sie aktiviert sind.
* Tarife, Zuweisungen, geplante Werte und Istwerte hängen von den ausgewählten Attributwerten ab.
* Späteres Ändern von Attributen (Umbenennen, Entfernen oder Neuanordnung) kann zu Folgendem führen:

   * Verlust der Verknüpfung zwischen Raten und Attributen
   * Ungültige oder „verwaiste“ Tarife
   * Fehlausrichtung bei Abrechnung und Berichterstellung

Aus diesen Gründen sollten Attribute während Ihrer ersten Workfront-Implementierung sorgfältig entworfen und anschließend unverändert bleiben.

### Objekte, die als Ratenattribute verwendet werden

Workfront unterstützt derzeit drei Systemobjekte, die als Ratenattribute verwendet werden können:

* **Gruppe**: Oft umbenannt in _Agentur_ oder _Geschäftseinheit_.
* **Unternehmen** Kann _Marke_, _Client_ oder _Kunde_ repräsentieren.
* **Standort**: Wird normalerweise als _Markt_, _Region_ oder _Office_ verwendet.

  Der Standort ist hierarchisch bis zu drei Ebenen definiert. (Beispiel: Wenn Sie „Standort“ als Los Angeles definieren, werden Kalifornien und die USA auch in Tarifvergleichen verwendet.)

Jedes Objekt kann entsprechend der Terminologie Ihres Unternehmens umbenannt werden, wenn Sie Ihre Attribute einrichten.
Beispiel:

* Bezeichnung „Agentur“ = Gruppenobjekt-Referenz
* Bezeichnung „Kostenstelle“ = Objektreferenz der Untergruppe
* Bezeichnung „Location“ = Standort-Objektreferenz

Dadurch kann die Einrichtung Ihre Geschäftsstruktur spiegeln und gleichzeitig die Integrität des Datenmodells von Workfront beibehalten werden.

### Hinweise zu Tarifattributen in Workfront

* Workfront unterstützt bis zu 5 Attributebenen. Das System folgt immer der Attributhierarchie und wählt die spezifischste verfügbare Übereinstimmung aus.

   * 0= Allgemeiner Basiszinssatz
   * 1-5 = progressiv spezifischere Raten

* Sie können Attribute entsprechend Ihrem Unternehmen umbenennen (Agentur, Marke, Markt, Kostenstelle usw.).
* Die Einrichtung ist nur einmal: Wenn Sie die Attribute später ändern, riskiert dies, die Integrität der Finanzdaten zu beeinträchtigen.
* Attribute, auf die nirgends im System verwiesen wird, können sicher gelöscht werden.

  Wenn jedoch bereits ein Attribut verwendet wird (auf das in Tarifkarten, Benutzerprofilen, Ressourcen oder Zuweisungen verwiesen wird), wird die Löschung blockiert, um die Datenintegrität zu schützen. In diesen Fällen führt der Versuch, das Attribut zu entfernen, insbesondere über einen API-Aufruf, zu einem Fehler.

* Vor der Live-Schaltung testen: Erstellen Sie eine Pilotpreiskarte und überprüfen Sie, ob die richtigen Raten in Zuweisungen aufgelöst werden.
* Dokumentieren Sie Ihre Einrichtung: Geben Sie Ihre Tarifattribute für Ihre Teams frei, damit diese verstehen, wie die Tarife funktionieren.

### Wo Tarifattribute angewendet werden können

Tarifattribute werden in allen Bereichen unterstützt, in denen in Workfront Tarife gelten:

* Tarifkarten: Definieren Sie Tarife nach Aufgabengebiet plus Attributen.
* Überschreibungen auf Projektebene: Wenden Sie Attribute an, wenn Sie Raten auf Projektebene überschreiben.
* Aufgabengebiete (im Setup): Festlegen der Standardraten für Aufgabengebiete mit Attributen.
* Benutzer (Benutzerprofile): Weisen Sie einzelnen Benutzern native Attribute zu, damit ihre Zuweisungen automatisch auf die richtigen Raten aufgelöst werden.
<!--
* Staffing plan resources
* Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->Aufgabengebiete unterstützen keine Ratenattribute direkt auf Objektebene. Sie sind über die für sie definierten Sätze mit Tarifattributen verbunden.

Wenn Sie Platzhalterzuweisungen erstellen können, die an die richtigen Attributwerte gebunden sind, werden Ihre Tarife entsprechend ausgefüllt.

* Wenn Sie bei Aufgabengebieten den Platzhalter später durch einen echten Benutzer ersetzen, setzt das System die Zuweisungsattribute automatisch auf die im Profil dieses Benutzers definierten Attribute zurück. Zu diesem Zeitpunkt können Attribute nicht mehr auf Zuweisungsebene bearbeitet werden. Sie übernehmen vom Benutzer, um die Konsistenz zu wahren und eine Fehlausrichtung zwischen Benutzerattributen und angewendeten Raten zu verhindern.
  <!--* For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Tarifattribute konfigurieren

Jedes Attribut verfügt über einen Satz konfigurierbarer Optionen, einschließlich allgemeiner Eigenschaften und Filter.
Filter steuern, wie Attributwerte bei der Definition von Raten vorgeschlagen und validiert werden. Sie sind wichtig, um die Attributauswahl konsistent zu halten, Benutzende zu gültigen Optionen zu führen und ungültige Kombinationen zu verhindern.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tarifattribute**.
1. Klicken Sie auf ein Pluszeichen im Diagramm, um ein Attribut hinzuzufügen.

   >[!NOTE]
   >
   >Das Diagramm kann bis zu fünf Attribute enthalten. Die Reihenfolge von oben nach unten definiert die Hierarchie, wie die Attribute angewendet werden. Klicken Sie auf **Drehen**-Symbol ![Drehen](assets/rotate-attribute-view-icon.png), um das Diagramm von links nach rechts anzuzeigen. Sie können das Diagramm auch vergrößern oder verkleinern und an den Bildschirm anpassen.

1. Wählen Sie ein Attribut aus, um den Konfigurationsbereich auf der rechten Seite des Bildschirms zu öffnen.

   ![Tarifattribute konfigurieren](assets/configure-rate-attributes.png)

1. Benennen Sie die Objekte (Gruppe, Unternehmen, Standort) in die für Ihr Unternehmen erforderlichen Begriffe (z. B. Agentur, Standort, Kostenstelle) um.
1. Klicken Sie **jedem** auf „Speichern“, um Ihre Namenskonvention zu speichern.

   Die Namen dieser Attribute werden auf allen Tarifkarten und Tarifen im System angezeigt.

1. Legen Sie die Eigenschaften für die einzelnen Attribute im Konfigurationsbereich fest:

   * **Erforderlich**: Wählen Sie aus, ob das Attribut ein Pflichtfeld für Tarife ist.
   * **Zur Verwendung bei der Umsatzberechnung**: Schließt dieses Attribut in die Abrechnungssatzberechnungen ein.
   * **Für Kostenberechnung verwenden**: Schließt dieses Attribut in die Berechnungen des Kostensatzes ein.

     >[!NOTE]
     >
     >Mindestens eine der Berechnungsoptionen muss ausgewählt sein, damit das Attribut in Finanzberechnungen funktioniert.

   * (Optional) **Hierarchisch**: Ermöglicht dem Attribut, hierarchische Beziehungen zwischen übergeordneten und untergeordneten Elementen zu berücksichtigen, z. B. Stadt > Bundesland > Land.

     Diese Eigenschaft ist nur für das Location-Objekt verfügbar.

### Filter für die Attribute definieren

Für die Attribute stehen zwei Filtertypen zur Verfügung:

* Vorschlagsfilter grenzen die Liste der verfügbaren Optionen basierend auf der Systemlogik oder vorherigen Attributauswahlen ein. Sie machen Dropdown-Menüs kontextorientiert und benutzerfreundlich.

  Beispiel: Agentur > Standort > Kostenstelle

  Bei dieser Einrichtung sollte das Attribut „Kostenstelle“ über einen Vorschlagsfilter verfügen, der sowohl auf die Agentur als auch auf den Standort verweist.

  Wenn Sie beim Hinzufügen eines Tarifs zuerst Agentur = „Stern“ wählen, schlägt die Dropdown-Liste Ort nur Orte vor, die zu „Stern“ gehören.

  Wenn Sie dann im Tarif Standort = Chicago wählen, schlägt die Dropdown-Liste Kostenstelle nur Kostenstellen vor, die mit „Stern“ und Chicago verknüpft sind.

* Beziehungsfilter legen die Abhängigkeitskette zwischen Attributen fest. Sie stellen sicher, dass das System versteht, wie Attribute miteinander in Beziehung stehen, und erzwingen gültige Abhängigkeiten.

  Beispiel: Agentur > Standort > Kostenstelle

  Bei dieser Einrichtung sollte das Agenturattribut über einen Beziehungsfilter verfügen, der es mit gültigen Standorten und Kostenstellen verknüpft.

Filter müssen immer in beide Richtungen konfiguriert werden. Wenn Attribut A über einen Beziehungsfilter mit Attribut B verfügt, sollte Attribut B über einen Vorschlagsfilter zurück zu Attribut A verfügen. Dadurch wird die Datenintegrität und ein sauberes Benutzererlebnis sichergestellt.

1. Wählen Sie Optionen aus, um die Vorschlagsfilter und die Beziehungsfilter für das Attribut im Konfigurationsbereich zu definieren:

   * **Filtertyp**:

      * Ein **Standard**-Filter wendet eine universelle Bedingung auf das Attributobjekt an. Beispiel: Standort > Ist Aktiv = True (nur aktive Standorte werden angezeigt).

        Der Standardfilter wird immer angewendet, unabhängig davon, ob andere Attribute ausgewählt sind.

      * Ein **Attribut**-Filter verknüpft ein Attribut mit einem anderen in der Kette. Beispiel: Standort > Referenz = Agentur (es werden nur Standorte angezeigt, die mit der ausgewählten Agentur verknüpft sind).

        Der Attributfilter wird nur angewendet, wenn das referenzierte Attribut einen Wert aufweist. Wenn beispielsweise die Option Agentur ausgewählt ist, werden nur gültige Standorte vorgeschlagen. Wenn Agentur leer ist, werden alle Standorte angezeigt (kann jedoch durch Standardfilter, die auf den Standort angewendet werden, eingeschränkt werden).

   * **Feld**: Das direkte Feld aus dem Attributobjekt, z. B. Standort-ID oder Aktiv-Flag.
   * **Operator**: Diese Optionen hängen vom ausgewählten Feldtyp ab. Beispiele sind Gleich, nicht Gleich, Ist leer, Wahr/Falsch.
   * (Nur Standardfiltertyp) **Wert**: Zum Beispiel Ist Aktiv = True.
   * (Nur Attributfiltertyp) **Referenz**: Das Attribut, von dem dieser Filter abhängt, z. B. Agentur.
   * (Nur Attributfiltertyp) **Referenzfeld**: Das Feld im referenzierten Attribut, das übereinstimmen muss, z. B. die Agentur-ID.

1. Klicken Sie **jedem Attribut** Speichern“, um die Eigenschaften und Filter zu speichern.


