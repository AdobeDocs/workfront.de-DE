---
title: Erstellen von Workfront-Objekten aus Workfront Planning
description: Sie können Workfront-Objekttypen erstellen, während Sie sie aus anderen Datensätzen in Workfront Planning verbinden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 597d8db034269e673dbe46e8c0f4934bf9509e2f
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Erstellen von Workfront-Objekten aus Workfront Planning <!--as you connect them to records-->

<!-- update the title (and all the links to this article) at preview, to be this: Create Workfront objects from Workfront Planning as you connect them to records-->
<!-- remove preview and production at release time-->

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

<!--
You can create Adobe Workfront objects from Workfront Planning in the following ways: 

* As you try to connect Workfront objects from Planning records

    This article describes how to create Workfront objects from Workfront Planning as you try to connect them from Planning records. 
* <span class="preview">When you use automations from a record's page.</span> 

    For information about creating Workfront objects using automations, see [Create objects using Adobe Workfront Planning record automations](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md). 
-->

Sie können die folgenden Typen von Workfront-Objekten aus Workfront Planning erstellen, wenn Sie einen Workfront Planning-Datensatz mit den folgenden Workfront-Objekttypen verbinden:

* Projekte
* Portfolios
  <!--* <span class="preview">Programs</span>-->

>[!IMPORTANT]
>
>* Sie können nur Projekte und Portfolios in Workfront erstellen, wenn Sie sie über einen Datensatz verbinden.
>
>* Sie können keine Programme, Gruppen oder Unternehmen erstellen, wenn Sie sie über einen Datensatz in Workfront Planning verbinden.
>

<!--replace the IMPORTANT above with this when we release programs: 

>[!IMPORTANT]
>
>* You can create only projects, portfolios, and <span class="preview">programs</span> in Workfront when connecting them from a record. 
>
>* You cannot create groups or companies when connecting them from a record in Workfront Planning. 
>
-->

Sie können Projekte und Portfolios <!--<span class="preview"> and programs </span>--> über ein Verbindungsfeld in folgenden Bereichen von Workfront Planning verbinden:

* Die Tabellenansicht eines Datensatztyps
* Die Detailseite oder das Vorschaufeld eines Datensatzes

Informationen zum Verbinden von Planning-Datensätzen mit Workfront-Objekten finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

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
   <td> Standard
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p> 
   <p>Bearbeiten Sie den Zugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte und Portfolios), während Sie die Datensätze mit ihnen verbinden. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie die Berechtigungen für den Arbeitsbereich, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für das Erstellen von Workfront-Objekten beim Verbinden dieser Objekte mit Datensätzen aus Workfront Planning

Sie müssen über Folgendes verfügen, bevor Sie neue Projekte oder Portfolios hinzufügen können, indem Sie sie mit vorhandenen Datensätzen verbinden:

* Datensatztypen, die mit Workfront-Projekten oder -Portfolios <!--or <span class="preview">programs</span>--> verbunden sind. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Einträge. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Die richtigen Zugriffsberechtigungen in Workfront Planning und Workfront, wie im Abschnitt [Zugriffsanforderungen“ in ](#access-requirements) Artikel beschrieben.

## Erstellen Sie Projekte, während Sie sie mit Datensätzen aus Workfront Planning verbinden

So erstellen Sie Projekte, während Sie sie mit anderen Datensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Projekten, wie im Artikel [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md) beschrieben.

1. (Bedingt) <!--<span class="preview">Click **Add project**</span> Or Start typing the name of a project, then click **Add project** if you cannot find it.--> Wenn Sie ein Projekt nicht finden können, wenn Sie versuchen, es über das Feld Verbundener Datensatz eines anderen Datensatzes hinzuzufügen, fügen Sie einen Namen hinzu und klicken Sie dann auf **Projekt hinzufügen**. Auf die Schaltfläche Hinzufügen folgt der von Ihnen eingegebene Projektname.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![Projekt hinzufügen beim Verbinden über ein Verbindungsfeld](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Das Feld **Projekt erstellen** wird geöffnet.</span>

1. <span class="preview">(Optional) Aktualisieren Sie den **Projektnamen**. Standardmäßig wird das Projekt nach dem benannt, was Sie beim Verbinden aus dem Datensatz als Suchelement hinzugefügt haben. </span>
1. <span class="preview">(Optional) Wählen Sie eine **Projektvorlage** aus. Wenn Sie keine Vorlage auswählen, erstellt Workfront ein leeres Projekt ohne Aufgaben. </span>
1. <span class="preview">Klicken Sie **Erstellen**. </span>
1. <span class="preview">(Bedingt) Wenn Sie ausgewählt haben, ein Projekt aus einer Vorlage zu erstellen, befolgen Sie die Schritte im Artikel [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) , um das Hinzufügen des Projekts abzuschließen.</span>

   Das neue Projekt wird erstellt und dem verbundenen Feld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Projekts, um die Projektseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Projekt vorzunehmen.

## Erstellen Sie Portfolios, während Sie sie mit Datensätzen aus Workfront Planning verbinden

So erstellen Sie Portfolios, während Sie sie mit Planungsdatensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Portfolios, wie im Artikel [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md) beschrieben.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Bedingt) <!--<span class="preview">Click **Add portfolio**</span> Or Start typing the name of a portfolio, then click **Add portfolio** if you cannot find it.--> Wenn Sie ein Portfolio beim Versuch, es über das verbundene Datensatzfeld eines anderen Datensatzes hinzuzufügen, nicht finden können, fügen Sie einen Namen hinzu und klicken Sie dann auf **Portfolio hinzufügen**. Auf die Schaltfläche Hinzufügen folgt auch der von Ihnen eingegebene Portfolioname.

   ![Portfolio beim Verbinden über ein Verbindungsfeld hinzufügen](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Das Portfolio wird erstellt und zum Verbindungsfeld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Portfolios, um die Portfolioseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Portfolio vorzunehmen.

<!--

<div class="preview">

## Create programs as you connect them with records from Workfront Planning

To create programs as you are connecting them from Planning records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    ******** at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click Add to add a new program"; take this out too: "The Add button is followed by the program name you typed." ***********
    
1. Click **Add program** 

    Or 
    
    Start typing the name of a program, then click **Add program** if you cannot find it. The Add button is followed by the program name you typed. 

    ![Add Workfront program when connecting it from connection field](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->