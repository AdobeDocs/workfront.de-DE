---
title: Erstellen von Datensatztypen
description: Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten Arbeitselemente illustrieren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 1%

---


<!--this is linked to the UI in an empty workspace screen-->

# Erstellen von Datensatztypen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten arbeitsbezogenen Elemente veranschaulichen.

Weitere Informationen zu Datensatztypen finden Sie unter [Übersicht über Datensatztypen](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Überlegungen zum Erstellen von Datensatztypen

* Sie können Datensatztypen in einem Arbeitsbereich wie folgt erstellen:

   * Automatisch:
      * Wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

      * <span class="preview">Wenn Sie sie mit einer Excel- oder CSV-Datei importieren. </span>

     >[!TIP]
     >
     ><span class="preview">Beim Import eines Datensatztyps aus einer Excel- oder CSV-Datei können auch Datensätze und Felder importiert werden.</span>

   * Manuell:

      * Von Grund auf neu.

        In diesem Artikel wird beschrieben, wie Sie neue Datensatztypen erstellen.

* Sie können Datensatztypen innerhalb eines Abschnitts und von einem Abschnitt eines Arbeitsbereichs in einen anderen verschieben. Es ist nicht möglich, Datensatztypen von einem Arbeitsbereich in einen anderen zu verschieben.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Sie können Datensatztypen automatisch erstellen, wenn Sie einen Arbeitsbereich mithilfe einer Workfront-Planungsvorlage erstellen. Jede Vorlage enthält Beispieldatensatztypen.

Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, sind die Datensatztypen in den folgenden Abschnitten gruppiert:

* Betriebsdatentypen
* Taxonomien

Sie können Datensatztypen manuell sowohl in den Abschnitten &quot;Operative Datensatztypen&quot;als auch &quot;Taxonomien&quot;hinzufügen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Informationen dazu, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Workspace-Vorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

## Erstellen eines neuen Datensatztyps

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie einen Datensatztyp erstellen möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Abschnitt hinzufügen** , um einen neuen Abschnitt zum Arbeitsbereich hinzuzufügen.
1. Klicken Sie auf **Record Type hinzufügen** und dann auf <span class="preview">**New**</span>.

   Das Feld Datensatztyp hinzufügen wird geöffnet.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen:

   * Ersetzen Sie &quot;Untitled record type&quot;durch den Namen Ihres künftigen Datensatztyps. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschreibung**: Fügen Sie weitere Informationen zum Datensatztyp hinzu.
   * Wählen Sie eine Farbe und Form für das dem Datensatztyp zugeordnete Symbol aus. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um Ihren neuen Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp. Graustufen ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. Klicken Sie auf **Erstellen**.

   Die Karte vom Typ Datensatz wird dem ausgewählten Bereich und Arbeitsbereich hinzugefügt.
Die Beschreibung des Datensatztyps wird auf der Karte angezeigt.

   ![](assets/record-type-card-with-description.png)

1. (Optional) Bewegen Sie den Mauszeiger über die Karte des Datensatztyps, klicken Sie oben rechts auf das Symbol **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Bearbeiten** , um Informationen zum Datensatztyp zu ändern.
1. (Optional) Klicken Sie auf die Karte vom Typ Datensatz , um die Seite vom Typ Datensatz zu öffnen.

   ![](assets/operational-record-type-blank.png)

   Die Seite vom Typ Datensatz wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operationellen Datensatztyps angezeigt:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf das Symbol **Mehr** ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten** , um ihn umzubenennen oder die Informationen darüber zu ändern. Weitere Informationen finden Sie unter [Bearbeiten von Datensatztypen](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Klicken Sie auf **+ Neuer Datensatz** , um Datensätze des ausgewählten Datensatztyps hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md).
1. (Optional) Klicken Sie oben rechts in der Tabelle auf das Symbol **+** , um dem Datensatztyp weitere Felder hinzuzufügen.

   Weitere Informationen zum Erstellen von Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

1. (Optional) Klicken Sie in der Kopfzeile auf den nach links zeigenden Pfeil neben dem Namen des Datensatztyps, um zum ausgewählten Arbeitsbereich zurückzukehren.

1. (Optional) Klicken Sie im Arbeitsbereich auf eine Karte vom Typ Datensatz, um den Datensatztyp per Drag-and-Drop an eine gewünschte Stelle zu ziehen oder in einen anderen Bereich zu verschieben.

   Die Änderungen werden automatisch gespeichert.

   Weitere Informationen zum Hinzufügen von Datensätzen, zum Löschen oder Bearbeiten von Datensatztypen oder zum Aktualisieren der Ansicht auf der Seite mit dem Datensatztyp finden Sie in den folgenden Artikeln:

   * [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md)
   * [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md)

<div class="preview">

## Erstellen von Datensatztypen durch Importieren einer Excel- oder CSV-Datei

Beachten Sie beim Importieren von Datensatztypen mit einer Excel- oder CSV-Datei Folgendes:

* Jedes Blatt der Excel-Datei wird zu einem Datensatztyp. Der Name des Blattes wird zum Namen des Datensatztyps.
* Wenn es nur ein Blatt gibt oder Sie eine CSV-Datei importieren, wird der Name der Datei zum Namen des Datensatztyps.
* Die Spaltenüberschriften der einzelnen Blätter werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für ihre jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit dem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei darf nicht größer sein als:
   * 10.000 Zeilen
   * 500 Spalten
* Die Excel-Datei sollte nicht größer als 5 MB sein.
* Leere Arbeitsblätter werden nicht unterstützt.

So importieren Sie Datensatztypen mit einer Excel- oder CSV-Datei:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensatztypen erstellen möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf **Hinzufügen des Datensatztyps**.
1. Klicken Sie auf **Aus Datei**.
1. Ziehen Sie eine zuvor gespeicherte Excel- oder CSV-Datei in den Arbeitsbereich oder klicken Sie auf **Wählen Sie eine CSV- oder Excel-Datei aus**, um nach einer Datei zu suchen.
1. Klicken Sie auf **Vorschau anzeigen und bearbeiten**.

   Das Feld **Vorschau und Bearbeitung** wird mit den folgenden Informationen angezeigt:

   * Die Namen der Blätter oder der künftigen Datensatztypen werden im linken Bereich angezeigt. Workfront Planning wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
   * Die erste Tabelle oder der erste Datensatztyp wird ausgewählt und die Namen der Felder, die mit ihr verknüpft sind, werden als Spaltenüberschriften angezeigt. Der Feldtyp wird standardmäßig ausgewählt.
   * Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten zehn Datensätze werden im Feld Vorschau und Bearbeitung angezeigt.

   ![](assets/preview-and-edit-box.png)

1. (Optional) Klicken Sie im linken Bereich auf den Namen der einzelnen Blätter, um die darin enthaltenen Informationen zu überprüfen.

   >[!NOTE]
   >
   >Leere Blätter werden nicht unterstützt und sind abgeblendet.

1. (Optional) Deaktivieren Sie im linken Bereich die Tabellen, die Sie nicht importieren möchten.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Sie können die Auswahl der Anzeige mit grauem Hintergrund deaktivieren.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben der Spaltenüberschrift, um einen der folgenden Schritte auszuführen:

   * Umbenennen eines der Felder
   * Ändern des **Feldtyps**
   * Aktualisieren Sie das Feld **Beschreibung**

1. (Bedingt) Klicken Sie nach dem Aktualisieren der Informationen zum Feld auf **Speichern**.

1. Klicken Sie auf **Importieren** , wenn Sie zum Importieren Ihrer Datei bereit sind.

   Die folgenden Informationen werden in die Workfront-Planung importiert:

   * Neue Datensatztypen
   * Neue Felder, die jedem Datensatztyp zugeordnet sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Seiten mit den Datensatztypen beginnen.

   Jeder, der Zugriff auf Workfront Planning hat, kann jetzt die importierten Datensatztypen und ihre Informationen anzeigen und bearbeiten.

</div>

