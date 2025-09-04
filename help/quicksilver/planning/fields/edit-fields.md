---
title: Feldeinstellungen bearbeiten
description: In Adobe Workfront Planning können Sie die Feldeinstellungen für Felder bearbeiten, die bereits erstellt wurden. Dieser Artikel beschreibt, wie Sie die Einstellungen für Workfront Planning-Felder bearbeiten können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---


# Bearbeiten von Feldeinstellungen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können die Einstellungen bestehender Felder in Adobe Workfront Planning bearbeiten.

Informationen zum Erstellen von Adobe Workfront Planning-Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

Dieser Artikel beschreibt, wie Sie die Einstellungen für Workfront Planning-Felder bearbeiten können. Informationen zum Bearbeiten von Feldwerten für Datensätze finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

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
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p></td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Überlegungen zum Bearbeiten von Feldeinstellungen

Bevor Sie die Konfiguration eines Felds ändern, müssen Sie Folgendes beachten:

* Feldeinstellungen können nur über die Tabelle vom Typ Datensatz bearbeitet werden.
* Die Einstellungen eines Feldes können nicht auf der Datensatzseite oder in einer anderen Ansicht außerhalb der Tabellenansicht bearbeitet werden.
* Nach dem Speichern des Felds ist keine Bearbeitung des Feldtyps möglich.
* Sie können die Auswahl der Einstellung Negative Zahlen zulassen , die zuvor für ein Feld vom Typ Zahl, Prozentsatz oder Währung ausgewählt wurde, nicht aufheben, wenn bereits negative Werte für die Datensätze gespeichert sind, an die sie angehängt ist.
* Sie können die Konfiguration der folgenden Feldelemente bearbeiten, nachdem Sie das Feld gespeichert haben:

   * Der Name oder die Beschreibung eines beliebigen Felds
   * Die Optionen eines Einzelauswahl- oder Mehrfachauswahl-Felds.
   * Der Ausdruck eines Formelfelds.

  >[!WARNING]
  >
  >Wenn Formelausdrücke geändert werden oder Optionen einem Feld vom Typ Auswahl hinzugefügt oder daraus entfernt werden, gehen Daten für die Datensätze verloren, die bereits Informationen in den Feldern enthalten, deren Konfiguration geändert wird.
  >
  >Es gibt keine Warnung oder Anzeige dafür, dass dieser Datenverlust auftreten könnte, wenn Sie die Konfiguration von Feldern ändern.
  >
  >Andere Benutzer werden nicht darüber informiert, dass sich die Feldkonfiguration geändert hat.

* Sie können vorhandene Suchfelder aus verbundenen Datensätzen bearbeiten.
* Zusätzlich zur Bearbeitung des Felds, wie im Abschnitt [Feldeinstellungen bearbeiten](#edit-field-settings-1) in diesem Artikel beschrieben, <span class="preview">Sie die Auswahl eines Felds mit einer oder mehreren Auswahlmöglichkeiten bearbeiten, wenn Sie einen Datensatz in der Tabellenansicht bearbeiten, während Sie die Feldwerte aktualisieren. Weitere Informationen finden Sie [ Abschnitt „Hinzufügen neuer Auswahlmöglichkeiten zu einem vorhandenen Auswahlfeld beim Bearbeiten von Datensätzen in der ](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view)&quot; in diesem Artikel.</span>

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Bearbeiten von Feldeinstellungen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatzfelder Sie bearbeiten möchten.

   Der Arbeitsbereich wird geöffnet und alle Datensatztypen im Arbeitsbereich werden auf Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps.

   Dadurch wird die Seite des Datensatztyps geöffnet.

1. (Bedingt) Klicken Sie auf die Registerkarte einer **Tabellenansicht**.

   Alle vorhandenen Datensätze, die mit dem Datensatztyp verknüpft sind, werden in den Zeilen der Tabellenansicht angezeigt.
1. Bewegen Sie den Mauszeiger über die Spaltenüberschrift eines Felds, das Sie bearbeiten möchten, klicken Sie dann auf den nach unten zeigenden Pfeil nach dem Feldnamen und dann auf **Feld bearbeiten**

   Oder

   Doppelklicken Sie auf die Spaltenüberschrift für das Feld.

   ![Pfeilmenü nach dem Feldnamen in der Tabellenkopfzeile hervorgehoben](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Aktualisieren Sie die Informationen zum Feld und klicken Sie auf **Speichern**.

   Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Sie können den Feldtyp nach dem Speichern des Felds nicht mehr aktualisieren.
   >
   >* Wenn Sie Feldkonfigurationen ändern (Feldoptionen oder Formelausdrücke), werden die Werte von Datensätzen, die bereits Informationen in den geänderten Feldern enthalten, in Echtzeit aktualisiert. Es gibt keine Warnung und kein Administratorprotokoll für die Wertänderungen, die durch Änderungen der Feldkonfiguration ausgelöst werden. Alle Benutzer, die die Felder anzeigen, sehen sofort die neuen Werte mit den Änderungen.

   Die Feldinformationen werden für alle Benutzer aktualisiert, die Zugriff auf den Arbeitsbereich haben.

1. (Bedingt) Klicken Sie bei verbundenen Datensatzfeldern auf **Suchfelder bearbeiten** und fügen Sie Suchfelder zum verbundenen Datensatztyp hinzu oder entfernen Sie diese.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).


<div class="preview">

## Hinzufügen neuer Auswahlmöglichkeiten zu einem vorhandenen Auswahlfeld beim Bearbeiten von Datensätzen in der Tabellenansicht

<!--some of this information is also available in Edit records article - update both when necessary-->

Sie können einem vorhandenen Einzel- oder Mehrfachauswahlfeld beim Bearbeiten von Datensätzen in der Tabellenansicht neue Auswahlmöglichkeiten hinzufügen.

>[!IMPORTANT]
>
>Die in diesem Abschnitt beschriebene Funktion ist nur in der Tabellenansicht verfügbar. Sie ist nicht in anderen Bereichen verfügbar, in denen Einzel- oder Mehrfachauswahlfelder angezeigt werden.

**BEISPIEL**

Möglicherweise verfügen Sie über ein Feld mit einer einzigen Auswahl namens Status , in dem die Optionen Neu und Geschlossen verfügbar sind, und Sie möchten eine Auswahl für einen Status In Bearbeitung hinzufügen. Sie können die Auswahl hinzufügen, indem Sie einen der folgenden Schritte ausführen:

* Bearbeiten des Felds. Weitere Informationen finden Sie im Abschnitt [Bearbeiten von ](#edit-field-settings-1)) in diesem Artikel.
* Hinzufügen einer neuen Option beim Bearbeiten des Datensatzes in der Tabellenansicht, wie unten beschrieben.

So fügen Sie beim Bearbeiten eines Datensatzes einem vorhandenen Auswahlfeld eine neue Auswahl hinzu:

1. Wechseln Sie zu einer Seite vom Typ Datensatz und öffnen Sie die Tabellenansicht.
1. Fügen Sie das Einzel- oder Mehrfachauswahlfeld, dem Sie eine Auswahl hinzufügen möchten, in der Tabellenansicht als neue Spalte hinzu. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
1. Beginnen Sie mit der Inline-Bearbeitung des Felds, indem Sie auf die Zelle für das Feld doppelklicken.
1. Geben Sie den Namen der Auswahl ein, die Sie hinzufügen möchten, und klicken Sie dann auf **Auswahl hinzufügen**.

   ![Auswahl im Einzelauswahlfeld in der Tabellenansicht hinzufügen](assets/add-choice-in-table-view-for-single-select-field.png)

   Die neue Auswahl wird sofort zum Feld für die Einzelauswahl hinzugefügt.

</div>