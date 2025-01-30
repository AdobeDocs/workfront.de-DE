---
title: Erstellen von Workfront-Objekten aus Workfront Planning
description: Sie können Workfront-Objekttypen erstellen, während Sie sie aus anderen Datensätzen in Workfront Planning verbinden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Erstellen von Workfront-Objekten aus Workfront Planning


<!-- remove preview and production at release time-->

<span class="preview">Die auf dieser Seite hervorgehobenen Informationen beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können die folgenden Typen von Workfront-Objekten aus Workfront Planning erstellen:

* Projekte
* Portfolios

Sie können in Workfront Planning Workfront-Projekte und -Portfolios erstellen, wenn Sie einen Workfront Planning-Datensatz mit einem Projekt oder Portfolio verbinden.

>[!IMPORTANT]
>
>* Sie können nur Projekte und Portfolios in Workfront erstellen, wenn Sie sie über einen Datensatz verbinden.
>
>* Sie können keine Programme, Gruppen oder Unternehmen erstellen, wenn Sie sie über einen Datensatz in Workfront Planning verbinden.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

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
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>. </p> 
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

* Datensatztypen, die mit Workfront-Projekten oder -Portfolios verbunden sind Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Einträge. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Die richtigen Zugriffsberechtigungen in Workfront Planning und Workfront, wie im Abschnitt [Zugriffsanforderungen“ in ](#access-requirements) Artikel beschrieben.

## Erstellen von Projekten, wenn diese mit Datensätzen aus Workfront Planning verbunden werden

So erstellen Sie Projekte, während Sie sie mit anderen Datensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Projekten, wie im Artikel [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md) beschrieben.

   Sie können Projekte über ein Verbindungsfeld in den folgenden Bereichen von Workfront Planning verbinden:

   * Die Tabellenansicht eines Datensatztyps
   * Die Detailseite oder das Vorschaufeld eines Datensatzes

1. (Bedingt) Wenn Sie ein Projekt beim Versuch, es über das verbundene Datensatzfeld eines anderen Datensatzes hinzuzufügen, nicht finden können, fügen Sie einen Namen hinzu und klicken Sie dann auf **+ Hinzufügen**. Auf die Schaltfläche Hinzufügen folgt der von Ihnen eingegebene Projektname.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click +Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">Das Feld **Projekt erstellen** wird geöffnet.</span>

1. <span class="preview">(Optional) Aktualisieren Sie den **Projektnamen**. Standardmäßig wird das Projekt nach dem benannt, was Sie beim Verbinden aus dem Datensatz als Suchelement hinzugefügt haben. </span>
1. <span class="preview">(Optional) Wählen Sie eine **Projektvorlage** aus. Wenn Sie keine Vorlage auswählen, erstellt Workfront ein leeres Projekt ohne Aufgaben. </span>
1. <span class="preview">Klicken Sie **Erstellen**. </span>
1. <span class="preview">(Bedingt) Wenn Sie ausgewählt haben, ein Projekt aus einer Vorlage zu erstellen, befolgen Sie die Schritte im Artikel [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) , um das Hinzufügen des Projekts abzuschließen.</span>

   Das neue Projekt wird erstellt und dem verbundenen Feld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Projekts, um die Projektseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Projekt vorzunehmen.

## Erstellen von Portfolios, wenn diese mit Datensätzen aus Workfront Planning verbunden werden

So erstellen Sie Portfolios, während Sie sie mit anderen Datensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Portfolios, wie im Artikel [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md) beschrieben.

   Portfolios können über ein Verbindungsfeld in folgenden Bereichen von Workfront Planning verknüpft werden:

   * Die Tabellenansicht eines Datensatztyps
   * Die Detailseite oder das Vorschaufeld eines Datensatzes

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Bedingt) Wenn Sie ein Portfolio beim Versuch, es über das verbundene Datensatzfeld eines anderen Datensatzes hinzuzufügen, nicht finden können, fügen Sie einen Namen hinzu und klicken Sie dann auf **+ Portfolio hinzufügen**. Auf die Schaltfläche Hinzufügen folgt auch der von Ihnen eingegebene Portfolioname.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Das Portfolio wird erstellt und zum Verbindungsfeld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Portfolios, um die Portfolioseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Portfolio vorzunehmen.

<!--

<div class="preview">

## Create programs when connecting them with records from Workfront Planning

To create programs as you are connecting them from other records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    You can connect programs from a connection field in following areas of Workfront Planning:

    * The table view of a record type
    * The details page or preview box of a record

    ********at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."***********
    
1. (Conditional) If you cannot find a program when trying to add it from the connected record field of another record, add a name, then click **+ Add**. The Add button is followed by the program name you typed. 

    ![](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->