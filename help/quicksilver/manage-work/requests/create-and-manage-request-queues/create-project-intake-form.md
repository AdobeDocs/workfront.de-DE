---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Erstellen von Forms zur Projekterfassung
description: Sie können Formulare zur Projekterfassung verwenden, um das Erstellen von Projekten in Workfront zu vereinfachen
author: Alina
feature: Work Management, Requests
role: User, Admin
hide: true
hidefromtoc: true
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 4%

---

# Erstellen von Projekt-Aufnahmeformularen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Formulare zur Projekterfassung sind eine Art von Anfrageformular, mit dem Benutzer Projekte anfordern können. Die Projekte werden aus dem Formular erstellt, ohne dass ein Projekt aus einer gesendeten Anfrage erstellt werden muss.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neue Lizenz: Standard </p>
   ODER
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein, um Aufnahmeformulare für Projekte erstellen zu können. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere Produkte</td> 
   <td> <p>Ihr Unternehmen muss Workfront Planning erworben haben, um Planungsfunktionen wie Automatisierungen verwenden zu können.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Funktionen und Einschränkungen bei der Projekterfassung in Forms

### Funktionen

Die Formulare für die Projekterfassung umfassen die folgenden Funktionen:

#### Workfront - Automatisierungen

Workfront-Projekterfassungsformulare unterstützen Workfront Planning Automations, um die erstellten projektspezifischen Eigenschaften zu konfigurieren.

Weitere Informationen zu Planungsautomatisierungen finden Sie unter [Konfigurieren von Adobe Workfront-Planungsautomatisierungen](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Genehmigungskonfiguration

Formulare zur Projekterfassung bieten die Möglichkeit, genehmigende Personen für gesendete Anfragen zu konfigurieren.

### Einschränkungen

#### Unterstützte Feldtypen

Der Projekterfassungs-Forms kann Felder aus jedem benutzerdefinierten Formular mit dem Projektobjekttyp enthalten.

Die folgenden Feldtypen werden derzeit in Forms zur Projekterfassung nicht unterstützt:

* Abschnitt
* Formel
* Datenaggregation
* Einzeilige Datenaggregation
* Planungsverbindung
* Native Feldverweise, die auf native Projektfelder verweisen, die schreibgeschützt sind (z. B. `workRequiredExpression`)

#### Erlebnis wird angefordert

Formulare für die Projekterfassung können nur mit dem neuen anfordernden Erlebnis verwendet werden.

Informationen zum neuen anfragenden Erlebnis finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Freigeben

Formulare zur Projekterfassung unterstützen keine öffentliche Freigabe. Zu den Freigabeoptionen gehören:

* **Beliebig**: Jeder im System kann das Formular verwenden, um eine Projektanfrage zu senden.
* **Angegebene Benutzer**: Sie können auswählen, welche Benutzer Zugriff auf das Projektanfrageformular haben.

## Erstellen eines Eingabeformulars für ein Projekt

{{step1-to-requests}}

1. Aktivieren Sie **Einstellung „Zu einem neuen Erlebnis**&quot; in der rechten oberen Ecke des Bildschirms.
1. Klicken **oben rechts** Bildschirm auf „Formulare anfordern“.

   >[!NOTE]
   >
   >Da nur Workfront-Administratoren Aufnahmeformulare erstellen können, ist die Schaltfläche Formulare anfragen nur für Administratoren sichtbar.

   Eine Liste der derzeit verfügbaren Anfrageformulare wird angezeigt. Dazu gehören Anfrageformulare von Workfront Planning.

1. Klicken **oben** auf „Neues Anfrageformular“.
1. Geben Sie einen Namen für das Anfrageformular ein. Standardmäßig lautet der Name des Formulars **Unbenanntes Formular**.
1. Wählen Sie oben **der Dropdown-Liste** Objekttyp (Projekt) aus. Derzeit ist dies der einzige verfügbare Workfront-Projekttyp. Andere Elemente in der Liste gehören zu Workfront Planning.
1. (Optional) Fügen Sie **Anfrageformular eine** Beschreibung“ hinzu.
1. Klicken Sie auf **Erstellen**. Das Anfrageformular für den ausgewählten Datensatztyp wird auf der Registerkarte Formular geöffnet.

   Der Formular-Builder für die Projektaufnahme wird auf der Registerkarte Formular geöffnet.

   Das Aufnahmeformular enthält standardmäßig die folgenden Informationen:

   * **Standardabschnitt**: Dies ist der standardmäßige Abschnittsumbruch, den Workfront auf das Anfrageformular anwendet. Alle Datensatzfelder werden im Bereich **Standard** angezeigt.
   * **Betreff** Feld: Das Feld, das die Anfrage in Workfront identifiziert. Die Konfiguration und der Wert des Felds Betreff können nicht bearbeitet werden.
   * Alle mit Projekten verknüpften Felder.

     Die im Anfrageformular enthaltenen Felder sind für alle sichtbar, die eine Projektanfrage einreichen.

1. Um Felder zum Formular hinzuzufügen, klicken Sie im linken Navigationsbereich auf den Feldtyp und wählen Sie dann das Feld aus.
1. (Optional) Um ein Feld zu entfernen, bewegen Sie den Mauszeiger über das Feld in dem Formular, das Sie entfernen möchten, und klicken Sie dann auf das Symbol **x**, um es zu entfernen.
1. (Optional) Gehen Sie wie **vor, um den Abschnitt** Standard“ aus dem Formular zu entfernen:

   1. Entfernen Sie alle Felder aus dem Standardabschnitt.
   1. Klicken Sie auf **Inhaltselemente** und fügen Sie einen neuen Abschnitt und dann einen Namen für den Abschnitt hinzu.
   1. Fügen Sie Felder zum neuen Abschnitt hinzu.
   1. Klicken Sie auf das **x**-Symbol, um den **Standardabschnitt“** entfernen.
1. Klicken Sie auf ein beliebiges Feld und verwenden Sie dann die Steuerelemente im rechten Bereich im Formular, um ihre Größe oder eine der folgenden Informationen zu definieren:

   * **label**: Dies ist der Name des Felds, wie er im Anfrageformular angezeigt wird. Der Name des Datensatzfelds wird dadurch nicht geändert.
   * **Anweisungen**: Fügen Sie weitere Informationen über das Feld hinzu.
   * **Erforderliches Feld festlegen**: Wenn diese Option aktiviert ist, muss das Feld einen Wert enthalten. Andernfalls kann das Formular nicht gesendet werden.
   * **Logik hinzufügen**: Definieren Sie, welche Bedingungen erfüllt sein müssen, damit das Feld angezeigt oder ausgeblendet wird.

   >[!TIP]
   >
   >   Der Feldtyp der einzelnen Felder wird oben im rechten Bereich angezeigt, nachdem Sie das Feld im Formular ausgewählt haben.
   >     

1. (Optional) Klicken Sie auf **Registerkarte** Inhaltselemente“ auf der linken Seite des Formulars und fügen Sie eines der folgenden Elemente hinzu:

   * **Beschreibender Text**
   * **Abschnittsumbruch**

   Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie auf **Registerkarte** Automatisierungen“ auf der linken Seite des Formulars und führen Sie dann einen der folgenden Schritte aus:

   * Projektvorlage auswählen
   * Beliebige benutzerdefinierte Formulare anhängen
   * Festlegen eines Projektbesitzers
   * Hinzufügen des Projekts zu einem Portfolio oder Programm

   Alle Auswahlen, die Sie hier vornehmen, werden auf Projekte angewendet, die aus diesem Aufnahmeformular erstellt wurden.

1. (Optional) Klicken Sie auf **Vorschau**, um anzuzeigen, wie das Formular für andere Benutzer angezeigt wird, wenn diese es zum Senden eines neuen Datensatzes verwenden werden.

1. (Optional) Klicken Sie auf die **Konfiguration** und fügen Sie dann mindestens einen Benutzer oder ein Team&lt; zum Feld **Genehmiger** hinzu, um neue Anfragen für dieses Aufnahmeformular zu genehmigen.

   * Wenn Sie ein Aufnahmeformular mit genehmigenden Personen verknüpfen, müssen alle neuen Anforderungen zunächst von allen genehmigenden Personen genehmigt werden, bevor ein Projekt generiert wird.
   * Sie können einem Aufnahmeformular eine oder mehrere genehmigende Personen hinzufügen.
   * Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und das Projekt nicht erstellt.
   * Alle genehmigenden Personen müssen eine Entscheidung treffen, bevor ein Projekt genehmigt oder abgelehnt wird.
   * Wenn ein Team als genehmigende Person festgelegt ist, ist nur eine Entscheidung vom Team erforderlich.

     Weitere Informationen zum Hinzufügen von Genehmigungen zu Anfrageformularen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Optional) Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Formulars in der Kopfzeile und klicken Sie dann auf **Bearbeiten**, um den Namen des Formulars zu aktualisieren.

1. Klicken Sie auf **Veröffentlichen**, um das Formular zu veröffentlichen und einen eindeutigen Link für es zu erhalten.

   Folgendes geschieht:

   * Die Schaltfläche **Veröffentlichen** wird entfernt.
   * Die **Veröffentlichung aufheben** wird dem Formular hinzugefügt. Wenn Sie darauf klicken, ist der Zugriff auf das Formular nicht möglich.
   * Eine **Freigeben**-Schaltfläche wird dem Formular hinzugefügt.
   * Das Formular wird im Bereich Anfragen des Hauptmenüs in Workfront verfügbar.

1. Klicken Sie **Freigeben**, um das Formular für andere freizugeben.
1. Klicken Sie auf den nach links zeigenden Pfeil links neben dem Namen des Formulars in der Kopfzeile, um das Formular zu schließen.

   Die **Formulare anfordern** Tabellenansicht wird geöffnet und das Formular wird ihr hinzugefügt.

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Anfrageformulars in der Tabellenansicht, klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Formularnamen und klicken Sie auf eine der folgenden Optionen:

   * **Formular bearbeiten**: Klicken Sie hier, um weitere Informationen zum Formular zu bearbeiten.
   * **Veröffentlichung aufheben**: Klicken Sie hierauf, um die Veröffentlichung des Formulars aufzuheben. Dadurch wird es aus dem Bereich „Anfragen“ in Workfront entfernt.
   * **Freigeben**: Klicken Sie hier, um zu ändern, wer Zugriff auf das Formular hat.
   * **Link kopieren**: Klicken Sie hier, um den Link des Anfrageformulars schnell zu kopieren, ohne das Formular zu öffnen.
   * **Löschen**: Klicken Sie hier, um das Formular zu löschen. Alle über das Formular hinzugefügten Anfragen und Datensätze werden nicht gelöscht. Das Formular kann nicht wiederhergestellt werden.

   >[!NOTE]
   >
   >Sie können Formulare für die Projekterfassung in der Tabellenansicht identifizieren, da sie in der Spalte „Objekttyp“ „Projekt“ anzeigen.

1. Klicken Sie auf den nach links zeigenden Pfeil links neben **Anfrageformulare** in der Kopfzeile, um die Tabelle mit den Anfrageformularen zu schließen.

