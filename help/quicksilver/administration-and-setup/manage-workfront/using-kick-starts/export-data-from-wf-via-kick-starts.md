---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Exportieren von Daten aus Adobe Workfront über Kick-Starts
description: Als Adobe Workfront-Administrator können Sie den Kick-Starts-Datenexporteur verwenden, um Daten aus Workfront zu exportieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 48c9bb06dff1e8f1260b331ace7843b204b3139e
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 8%

---

# Exportieren von Daten aus Adobe Workfront über Kick-Starts

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-Administrator können Sie den Kick-Starts-Datenexporteur verwenden, um Daten aus Workfront zu exportieren. Sie können sie nach dem Export in anderen Anwendungen verwenden.

Der Datenexport über Kick-Starts ist auch hilfreich, um zu verstehen, welche Felder mit den einzelnen Objekten verknüpft sind, wie diese Felder codiert werden und wie die Werte dieser Felder in der Datenbank formatiert sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vorteile und Nachteile der Verwendung von Schnellstarts zum Exportieren von Daten

Es gibt zwei Möglichkeiten, Daten in Workfront zu exportieren:

* Daten aus einem Bericht oder einer Liste exportieren

  Weitere Informationen zum Exportieren von Daten aus einem Bericht oder einer Liste finden Sie unter [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exportieren von Daten über Schnellstarts

Die folgende Tabelle zeigt die Vor- und Nachteile jeder Methode:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Exportierte Daten enthalten Objekt- und Feldwerte</p> </th> 
   <th> <p>Möglichkeit zum gleichzeitigen Export von Daten für mehrere Objekttypen</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportieren von Daten aus einer Listenansicht</strong> </p> <p>Weitere Informationen zum Exportieren von Daten aus einer Liste finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Daten exportieren</a></p> </td> 
   <td> <p>Ja</p> <p>Sowohl native Workfront-Felder als auch benutzerdefinierte Felder, die mit den Objekten verknüpft sind, werden exportiert.</p> </td> 
   <td> <p>Nein</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportieren von Daten über Schnellstarts</strong> </p> </td> 
   <td> <p>Ja (begrenzt)</p> <p>Die meisten nativen Workfront-Felder, die mit Objekten verknüpft sind, werden exportiert, einige jedoch nicht. Beispielsweise können Sie die Felder "Zeitplan", "Projekteigentümer"oder "Projektsponsor"nicht über einen Projekt-Kick-Start-Export exportieren.</p> <p>In einem Projekt, an das ein benutzerdefiniertes Formular angehängt ist, werden die in die Felder des Formulars eingegebenen Daten nicht exportiert.</p> <p>Sie können jedoch ein benutzerdefiniertes Formular exportieren. Die resultierende Datei listet die im Formular konfigurierten Felder auf, z. B. Textfelder und Optionsfelder.</p> </td> 
   <td> <p>Ja</p> <p>Durch die Verwendung von Kick-Starts zum Exportieren von Workfront-Daten können Sie Daten exportieren, die sich auf mehrere Objekttypen beziehen. Sie können beispielsweise Aufgaben, Probleme und Projekte in einen einzigen Export einbeziehen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ausfuhrbeschränkungen

Beim Datenexport über Kick-Start (Daten werden im Excel-Dateiformat exportiert) bestehen die folgenden Einschränkungen:

* **50.000 Zeilen:** Die zulässige Anzahl von Zeilen in der Datei.
* **65.530 Hyperlinks:** Dies ist eine Beschränkung, die Excel für Dokumente mit mehr als 65.530 Hyperlinks vorschreibt. Diese Dokumente können nach dem Export nicht mehr geöffnet werden. Beachten Sie, dass ein Excel-Dokument möglicherweise nur 200 Datenzeilen enthält. Wenn jedoch mehr als 65.530 Links innerhalb des Dokuments vorhanden sind, wird das Dokument nicht geöffnet.

## Daten über Kick-Start exportieren

{{step-1-to-setup}}

1. Klicks **System** > **Kick-Starts,** Klicken Sie dann auf **Daten exportieren.**

1. Wählen Sie das Objekt aus, das Sie exportieren möchten. Standardmäßig werden die folgenden Objekte unter **Was soll eingeschlossen werden?**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objekt</strong> </p> </th> 
      <th> <p><strong>Exportierte Tabellen der Excel-Datei</strong> </p> </th> 
      <th> <p> <strong>Exportformat</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Dashboard</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Bericht<br>Tab-Bereich "Portal"<br>Dashboard<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Bericht</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Bericht<br>Voreinstellungen</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Genehmigung</p> </td> 
      <td scope="col" valign="top"> <p>Schritt-Genehmiger<br>Validierungsschritt<br>Validierung<br>Validierungsprozess<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Benutzerdefinierte Daten</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Ausgabentyp</p> </td> 
      <td valign="top"> <p>Ausgabentyp<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Stundentyp</p> </td> 
      <td valign="top"> <p>Stündentyp<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Team Member<br>Team<br>Voreinstellungen </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Benutzerin oder Benutzer</p> </td> 
      <td valign="top"> <p>Benutzer<br>Voreinstellungen</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Weitere Optionen** um die vollständige Liste der Objekte anzuzeigen.

   Alle hier aufgelisteten Objekte können auch zum Importieren von Daten in Workfront verwendet werden.

   Die einzige Ausnahme ist die **Zugriffsebenen** -Objekt. Das Datenblatt Zugriffsebenen , das in einem Export enthalten ist, dient nur zu Referenzzwecken. Damit können Sie einem neuen Benutzerkonto anhand der Kennung eine Zugriffsstufe zuweisen.

   Weitere Informationen zum Importieren von Daten in Workfront über Schnellstarts finden Sie unter [Daten mithilfe einer Kick-Start-Vorlage in Adobe Workfront importieren](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Im Folgenden finden Sie eine Liste aller Objekte, die über Kick-Start exportiert werden können:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objekt</p> </th> 
      <th> <p>Exportierte Tabellen der Excel-Datei</p> </th> 
      <th> <p>Exportformat</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Zugriffsebene</td> 
      <td scope="col" valign="top">Zugriffsstufe<br>Voreinstellungen</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Zuweisung</td> 
      <td scope="col" valign="top">Zuweisung<br>Voreinstellungen</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Firma</td> 
      <td scope="col" valign="top"> Firma<br>Voreinstellungen </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E-Mail-Vorlage</td> 
      <td scope="col" valign="top"> E-Mail-Vorlage<br>Voreinstellungen </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Ausgabe</td> 
      <td valign="top"> Ausgaben<br>Voreinstellungen </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Externe Seite</td> 
      <td valign="top"> Externe Seite<br>Voreinstellungen </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> Filter<br>Voreinstellungen </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppe</td> 
      <td valign="top"> Gruppe<br>Voreinstellungen  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppierung</td> 
      <td valign="top"> Gruppierung<br>Voreinstellungen </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Stunde</td> 
      <td valign="top"> Stunde<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problem</td> 
      <td valign="top"> Problem<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Aufgabengebiet</td> 
      <td valign="top"> Auftragsrolle<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Meilensteinpfad</td> 
      <td valign="top"> Milestone<br>Milestone-Pfad<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Notiz</td> 
      <td valign="top"> Hinweis<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfolio</td> 
      <td valign="top"> Portfolio<br>Voreinstellungen  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projekt</td> 
      <td valign="top"> Warteschlange<br>Projekt<br>Routing-Regel<br>Warteschlangenthema<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ressourcenkalkulation</td> 
      <td valign="top"> Ressourcenschätzung<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ressourcenpool</td> 
      <td valign="top"> Ressourcenpool<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risiko</td> 
      <td valign="top"> Risiko<br>Voreinstellungen  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risikotyp</td> 
      <td valign="top"> Risikotyp<br>Voreinstellungen  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Scorecard-Fragen<br>Scorecard-Option<br>Scorecard<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Aufgabe</td> 
      <td valign="top"> Aufgabe<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlage</td> 
      <td valign="top"> Warteschlange<br>Vorlage<br>Routing-Regel<br>Warteschlangenthema<br>Voreinstellungen </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlagenzuweisung</td> 
      <td valign="top"> Vorlagenzuweisung<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlagenaufgabe</td> 
      <td valign="top"> Vorlagenaufgabe<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Arbeitszeittabelle</td> 
      <td valign="top"> Datenblatt-Profil<br>Datenblatt<br>Voreinstellungen </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Anzeigen </td> 
      <td valign="top"> Ansicht<br>Voreinstellungen  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicks **Herunterladen.**

   Die exportierte Schnellstartdatei wird entweder als Excel-Datei oder als heruntergeladen. ZIP-Datei mit mehreren Excel- und Eigenschaftendateien. Jede Excel-Datei ist eine Zusammenstellung von Arbeitsblättern, wobei jedes Blatt ein Feld darstellt, das mit dem ausgewählten Objekt verknüpft ist. Es gibt eine **Eigenschaften** mit jedem Export verknüpftes Blatt.

   Die **Dashboard** und **Bericht** können Sie bestimmte Dashboards und Berichte auswählen, die in den Download aufgenommen werden sollen. Sie können nur Dashboards exportieren, die systemweit freigegeben sind.

   Matrix-Berichte können nicht exportiert werden. Weitere Informationen zu Matrix-Berichten finden Sie unter [Erstellen eines Matrix-Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Sie können bis zu 100 Dashboards und 100 Berichte in einem Export auswählen.

   ![](assets/kickstart-export-350x381.png)

   Sie können mehrere Objekte gleichzeitig exportieren.



1. (Empfohlen) Analysieren Sie die exportierten Daten, um sicherzustellen, dass alle erwarteten Informationen exportiert wurden.

   Bei umfangreichen Exporten erzeugt Workfront im Hintergrund die Excel-Datei und erzeugt eine Warnmeldung über die Verzögerung. Die Kick-Start-Datei wird Ihnen per E-Mail zugeschickt, wenn der Download abgeschlossen ist.

   ![](assets/large-kick-start-file-warning-350x65.png)
