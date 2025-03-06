---
title: Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 279238689e132490b2d67ae64e8ef2c50a8fc604
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 1%

---

# Erstellen von Datensatztypen durch Importieren von Informationen aus einer CSV- oder Excel-Datei

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens erforderlichen Arbeitselemente veranschaulichen, indem Sie Informationen aus einer CSV- oder Excel-Datei importieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

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
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
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
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Importieren von Datensatztypen mithilfe einer Excel- oder CSV-Datei

* Jedes Blatt der Excel-Datei wird zu einem Datensatztyp. Der Name des Blatts wird zum Namen des Datensatztyps.
* Wenn nur ein Blatt vorhanden ist oder Sie eine CSV-Datei importieren, wird der Name der Datei zum Namen des Datensatztyps.
* Die Spaltenüberschriften in jedem Blatt werden zu den Feldern, die mit jedem Datensatztyp verknüpft sind.
* Felder sind für die jeweiligen Datensatztypen eindeutig.
* Jede Zeile in jedem Blatt wird zu einem eindeutigen Datensatz, der mit seinem jeweiligen Datensatztyp verknüpft ist.
* Jedes Blatt der Excel-Datei sollte Folgendes nicht überschreiten:
   * 25.000 Zeilen
   * 500 Spalten
* Die Datei sollte nicht größer als 5 MB sein.
* Leere Blätter werden nicht unterstützt.

So importieren Sie Datensatztypen mithilfe einer Excel- oder CSV-Datei:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensatztypen erstellen möchten,

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie **Datensatztyp hinzufügen**.
1. Klicken Sie auf **Aus Datei**.
1. Ziehen Sie eine zuvor auf Ihrem Computer gespeicherte Excel- oder CSV-Datei per Drag-and-Drop oder klicken Sie **CSV- oder Excel-Datei auswählen** um eine Datei zu suchen.
1. Klicken Sie auf **Vorschau und Bearbeitung**.

   Das **„Vorschau und**&quot; wird mit den folgenden Informationen angezeigt:

   * Die Namen der Tabellen oder der zukünftigen Datensatztypen werden im linken Bereich angezeigt. Workfront Planning wählt standardmäßig ein Symbol und eine Farbe für jeden neuen Datensatztyp aus.
   * Das erste Blatt oder der erste Datensatztyp wird ausgewählt, und die Namen der mit ihm verknüpften Felder werden als Spaltenüberschriften angezeigt. Der Typ jedes Felds ist standardmäßig ausgewählt.
   * Jede Zeile stellt einen neuen Datensatz dar. Nur die ersten 10 Datensätze werden im Vorschau- und Bearbeitungsfeld angezeigt.

   ![Vorschau und Bearbeitungsfeld](assets/preview-and-edit-box.png)

1. (Optional) Klicken Sie auf den Namen der einzelnen Blätter im linken Bereich, um die darin enthaltenen Informationen zu überprüfen.

   >[!NOTE]
   >
   >Leere Blätter werden nicht unterstützt und sind abgeblendet.

1. (Optional) Deaktivieren Sie im linken Bereich die Auswahl der Blätter, die Sie nicht importieren möchten.

   ![Dropdown-Liste Zu importierende Tabellen auswählen mit nicht ausgewählter Option](assets/select-sheets-to-import-drop-down-with-unselected.png)

   Blättert, wenn Sie die Auswahl aufgehoben haben, wird die Anzeige mit grauem Hintergrund angezeigt.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben der Spaltenüberschrift, um eine der folgenden Aktionen durchzuführen:

   * Eines der Felder umbenennen
   * Ändern des **Feldtyps**
   * Aktualisieren Sie das Feld **Beschreibung**

1. (Bedingt) Klicken Sie nach dem Aktualisieren der Feldinformationen auf **Speichern**.

1. Klicken Sie **Importieren** wenn Sie bereit sind, Ihre Datei zu importieren.

   Die folgenden Informationen werden in Workfront Planning importiert:

   * Neue Datensatztypen
   * Neue Felder, die mit jedem Datensatztyp verknüpft sind
   * Neue Datensätze, die mit jedem Datensatztyp verknüpft sind

   Sie können mit der Verwaltung von Feldern und Datensätzen auf den Datensatztypseiten beginnen.

   Alle Personen mit Zugriff auf Workfront Planning und den Arbeitsbereich können jetzt die importierten Datensatztypen und deren Informationen anzeigen und bearbeiten.
