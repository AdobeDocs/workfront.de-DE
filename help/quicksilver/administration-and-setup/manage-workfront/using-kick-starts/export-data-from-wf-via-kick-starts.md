---
user-type: administrator
product-area: system-administration
keywords: Kickstart,Kickstart,Kickstarts,Kickstarts
navigation-topic: use-kick-starts
title: Exportieren von Daten aus Workfront über Kickstarts
description: Als Adobe Workfront-Administrator können Sie den Kickstart-Datenexporteur verwenden, um Daten aus Workfront zu exportieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 7b9989b73f7be46690073f323203ae2d9ca1a4b5
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 7%

---

# Exportieren von Daten aus Workfront über Kickstarts

<!-- Audited: 2/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

Als Adobe Workfront-Administrator können Sie den Kickstart-Datenexporteur verwenden, um Daten aus Workfront zu exportieren. Sie können sie in anderen Anwendungen verwenden, nachdem Sie sie exportiert haben.

Der Export von Daten über Kickstarts ist auch hilfreich, um zu verstehen, welche Felder mit den einzelnen Objekten verknüpft sind, wie diese Felder kodiert werden und wie die Werte dieser Felder in der Datenbank formatiert sind.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vor- und Nachteile der Verwendung von Kickstarts zum Datenexport

Es gibt zwei Möglichkeiten, Daten in Workfront zu exportieren:

* Exportieren von Daten aus einem Bericht oder einer Liste

  Weitere Informationen zum Exportieren von Daten aus einem Bericht oder einer Liste finden Sie unter [Exportieren von Daten](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Datenexport über Kickstarts

Die folgende Tabelle zeigt die Vor- und Nachteile jeder Methode:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Die exportierten Daten enthalten Objekt- und Feldwerte</p> </th> 
   <th> <p>Fähigkeit, Daten um mehrere Objekttypen gleichzeitig zu exportieren</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportieren von Daten aus einer Listenansicht</strong> </p> <p>Weitere Informationen zum Exportieren von Daten aus einer Liste finden Sie unter <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportieren von Daten</a></p> </td> 
   <td> <p>Ja</p> <p>Sowohl native Workfront-Felder als auch benutzerdefinierte Felder, die mit den -Objekten verknüpft sind, werden exportiert.</p> </td> 
   <td> <p>Nein</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportieren von Daten über Kickstarts</strong> </p> </td> 
   <td> <p>Ja (begrenzt)</p> <p>Die meisten nativen Workfront-Felder, die mit -Objekten verknüpft sind, werden exportiert, einige jedoch nicht. Beispielsweise können Sie die Felder „Zeitplan“, „Projektbesitzer“ oder „Projektsponsor“ nicht über einen Projekt-Kickstart-Export exportieren.</p> <p>In einem Projekt, an das ein benutzerdefiniertes Formular angehängt ist, werden alle Daten, die in die Felder des Formulars eingegeben werden, nicht exportiert.</p> <p>Sie können jedoch auch ein benutzerdefiniertes Formular exportieren. Die resultierende Datei listet die im Formular konfigurierten Felder auf, z. B. Textfelder und Optionsfelder.</p> </td> 
   <td> <p>Ja</p> <p>Durch Kickstarts zum Exportieren von Workfront-Daten können Sie Daten, die sich auf mehrere Objekttypen beziehen, in einen einzigen Export exportieren. Sie können beispielsweise Aufgaben, Probleme und Projekte in einen einzigen Export einbeziehen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exportbeschränkungen

Beim Exportieren von Daten über Kickstarts (Daten werden im Excel-Dateiformat exportiert) bestehen die folgenden Einschränkungen:

* **50.000 Zeilen:** Die Anzahl der Zeilen, die in der Datei zulässig sind.
* **65.530 Hyperlinks:** Dies ist eine von Excel auferlegte Grenze für Dokumente, die mehr als 65.530 Hyperlinks enthalten. Diese Dokumente können nach dem Export nicht mehr geöffnet werden. Beachten Sie, dass ein Excel-Dokument möglicherweise nur 200 Datenzeilen enthält. Wenn das Dokument jedoch mehr als 65.530 Links enthält, wird es nicht geöffnet.

## Exportieren von Daten über Kickstarts

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kickstarts** und dann auf **Daten exportieren.**

1. Wählen Sie das Objekt aus, das Sie exportieren möchten. Standardmäßig werden die folgenden Objekte unter „Was **einschließen** angezeigt:

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
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Bericht<br>Portalregisterkartenabschnitt<br>dashboard<br>preferences</p> </td> 
      <td scope="col" valign="top"> PLZ</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Bericht</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Bericht<br>Voreinstellungen</td> 
      <td scope="col" valign="top"> PLZ </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Genehmigung</p> </td> 
      <td scope="col" valign="top"> <p>Schritt Genehmiger<br>Genehmigungsschritt<br>Genehmigung<br>Genehmigungsprozess<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Benutzerdefinierte Daten</p> </td> 
      <td scope="col" valign="top"> <p>Parameter<br>Parameteroption<br>Parametergruppe<br>Kategorieparameter<br>Kategorie<br>Voreinstellungen</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Ausgabentyp</p> </td> 
      <td valign="top"> <p>Ausgabentyp/<br></p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Stundentyp</p> </td> 
      <td valign="top"> <p>Stundentyp/<br></p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Team</p> </td> 
      <td valign="top"> Teammitglied<br>Team<br>preferences </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Benutzerin oder Benutzer</p> </td> 
      <td valign="top"> <p><br></p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Weitere Optionen**, um die vollständige Liste der Objekte anzuzeigen.

   Alle hier aufgeführten Objekte können auch zum Importieren von Daten in Workfront verwendet werden.

   Die einzige Ausnahme ist das **Zugriffsebenen**-Objekt. Das Datenblatt Zugriffsebenen , das in einem Export enthalten ist, wird nur zu Referenzzwecken bereitgestellt. Damit können Sie einem neuen Benutzerkonto eine Zugriffsebene anhand der ID zuweisen.

   Weitere Informationen zum Importieren von Daten in Workfront über Kickstarts finden Sie unter [Importieren von Daten in Adobe Workfront mithilfe einer Kickstart-Vorlage](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Im Folgenden finden Sie eine Liste aller Objekte, die über Kickstarts exportiert werden können:

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
      <td scope="col" valign="top">Zugriffsebene<br>Einstellungen</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Zuweisung</td> 
      <td scope="col" valign="top">assignment<br>preferences</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Firma</td> 
      <td scope="col" valign="top"> company<br>preferences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">E-Mail-Vorlage</td> 
      <td scope="col" valign="top"> Email template<br>preferences </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Ausgabe</td> 
      <td valign="top"> <br> </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Externe Seite</td> 
      <td valign="top"> Externe Seite<br>Voreinstellungen </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filter</td> 
      <td valign="top"> <br> </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppe</td> 
      <td valign="top"> <br>  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Gruppierung</td> 
      <td valign="top"> grouping.<br> </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Stunde</td> 
      <td valign="top"> <br> </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problem</td> 
      <td valign="top"> Anfrage<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Aufgabengebiet</td> 
      <td valign="top"> Aufgabengebiet/<br> </td> 
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
      <td valign="top"> Portfolios <br>preferences  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projekt</td> 
      <td valign="top"> queue<br>project<br>routing rule<br>queue topic<br>preferences </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ressourcenkalkulation</td> 
      <td valign="top"> Ressourcenkalkulation/<br> </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Ressourcen-Pool</td> 
      <td valign="top"> Ressourcenpool<br>Voreinstellungen </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risiko</td> 
      <td valign="top"> <br>  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risikotyp</td> 
      <td valign="top"> Risikotyp/<br>  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Scorecard-Fragen<br>Scorecard-Option<br>Scorecard<br>Voreinstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Aufgabe</td> 
      <td valign="top"> <br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlage</td> 
      <td valign="top"> queue<br>template<br>routing rule<br>queueTopic<br>preferences </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlagenzuweisung</td> 
      <td valign="top"> Vorlagenzuweisung<br>Einstellungen </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Vorlagenaufgabe</td> 
      <td valign="top"> Vorlagenaufgabe/<br> </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Arbeitszeittabelle</td> 
      <td valign="top"> Arbeitszeittabellen-Profil<br>Arbeitszeittabelle<br>Voreinstellungen </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Anzeigen </td> 
      <td valign="top"> <br>  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Herunterladen.**

   Die exportierte Kickstart-Datei wird entweder als Excel-Datei oder als heruntergeladen. komprimierte Datei, die mehrere Excel- und Eigenschaftendateien enthält. Jede Excel-Datei ist eine Sammlung von Blättern, wobei jedes Blatt ein Feld darstellt, das mit dem ausgewählten Objekt verknüpft ist. Jedem Export ist **Blatt** Eigenschaften“ zugeordnet.

   Mit den **Dashboard** und **Report** können Sie bestimmte Dashboards und Berichte auswählen, die in den Download aufgenommen werden sollen. Sie können nur Dashboards exportieren, die systemweit freigegeben sind.

   Matrixberichte können nicht exportiert werden. Weitere Informationen zu Matrixberichten finden Sie unter [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   Kickstarts unterstützen keine Textmodusfilter oder Gruppierungen. Für einen erfolgreichen Export müssen die Berichtsfilter und Gruppierungen in den Standardmodus umgeschaltet werden.

   Sie können in einem Export bis zu 100 Dashboards und 100 Berichte auswählen.

   <span class="preview">Beispielbild in der Vorschau-Umgebung:</span>
   ![Kickstart-Export](assets/kickstart-export-spreadsheet-options.png)

   Beispielbild in der Produktionsumgebung:
   ![Kickstart-Export](assets/kickstart-export-350x381.png)

   Sie können mehrere Objekte gleichzeitig exportieren.

1. (Empfohlen) Analysieren Sie die exportierten Daten, um sicherzustellen, dass alle erwarteten Informationen exportiert wurden.

   Bei großen Exporten arbeitet Workfront im Hintergrund, um die Excel-Datei zu erstellen, und gibt Ihnen eine Warnmeldung über die Verzögerung. Die Kickstart-Datei wird Ihnen nach Abschluss des Downloads per E-Mail zugeschickt.

