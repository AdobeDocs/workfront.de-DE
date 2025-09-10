---
title: Erste Schritte mit der Workfront Planning and GenStudio for Performance Marketing Integration
description: Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat. Erfahren Sie mehr über die Grundlagen, wie Sie Ihre Workflows mithilfe dieser Integration optimieren können.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1906'
ht-degree: 0%

---

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->


# Erste Schritte mit der Integration von Adobe Workfront Planning und Adobe GenStudio for Performance Marketing

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Unternehmen, die sowohl Adobe Workfront Planning als auch Adobe GenStudio for Performance Marketing verwenden, definieren Marketing-Konzepte wie Kampagnen, Produkte, Aktivierungen und Personas häufig detaillierter als das, was GenStudio standardmäßig unterstützt.

GenStudio for Performance Marketing und Workfront Planning sind nativ integriert. Diese Integration ermöglicht es Benutzenden, in Workfront Planning, Kampagnen, Produkte, Personas, Aktivierungen, Kanäle und Regionen zu verwalten, die in GenStudio verwendet werden. Außerdem können sie GenStudio so konfigurieren, dass in Workfront Planning auf bestehende Datensatztypen verwiesen wird, und so einen besser vernetzten und konsistenteren Marketing-Workflow erstellen.

Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat.

## Integrationsvorteile

Durch die Integration von Workfront Planning mit GenStudio for Performance Marketing können Sie:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Anzeigen von GenStudio Workspace in Workfront Planning.
* Ändern Sie Ihre Kampagnen, Produkte, Personas und Aktivierungen in GenStudio for Performance Marketing und erhalten Sie Echtzeit-Aktualisierungen derselben Informationen in Workfront Planning.
* Ändern Sie Ihre Kampagnen, Produkte, Personas und Aktivierungen in Workfront Planning und erhalten Sie Echtzeit-Aktualisierungen derselben Informationen in GenStudio for Performance Marketing.
* Doppelte Dateneingabe vermeiden.
* Beibehaltung der Ausrichtung bei allen Planungs- und Aktivierungsmaßnahmen.

## Integrationsanforderungen

Ihr Unternehmen muss die folgenden Anforderungen erfüllen, damit die Integration zwischen Workfront Planning und GenStudio for Performance Marketing vorhanden ist:

* Workfront und GenStudio for Performance Marketing müssen für dieselbe Organisation aktiviert sein.

  Weitere Informationen zu GenStudio finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Ihre Workfront-Instanz ist Teil des einheitlichen Adobe-Erlebnisses, einschließlich der Verwendung des Identity Management-Systems (IMS).

  Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Benutzende, die sowohl Workfront Planning als auch GenStudio for Performance Marketing verwenden, dürfen nur zu einer Workfront-Instanz in der IMS-Organisation gehören.

  Benutzende, die nur Workfront verwenden, können den GenStudio-Arbeitsbereich anzeigen, auch wenn sie keine GenStudio for Performance Marketing-Benutzenden sind.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Zugriffsanforderungen

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront-Paket</p>
<p>Beliebiges Planungspaket</p>

</td> </tr>
   <tr> 
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-Benutzerrollen</p></td> 
   <td><p><ul><li>Jede GenStudio-Benutzerrolle für den Zugriff auf Kampagnen, Produkte und Personas</li>
   <li>GenStudio System Manager für den Zugriff auf Aktivierungen <!--and Events--></li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Verwalten Sie Berechtigungen für den GenStudio-Arbeitsbereich, um dem GenStudio-Arbeitsbereich neue Felder oder Datensatztypen hinzuzufügen</p></li>
   <li><p>Mitwirken an Berechtigungen für den GenStudio-Arbeitsbereich zum Hinzufügen, Aktualisieren oder Löschen von Datensätzen im GenStudio-Arbeitsbereich</p> </li>  
   </ul>
   <p>Benutzende können in Workfront Planning keine GenStudio for Performance Marketing-Datensatztypen oder -Felder aus dem GenStudio-Arbeitsbereich entfernen</p>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alle Berechtigungen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Erstellen von Berechtigungen in Adobe GenStudio for Performance Marketing zum Erstellen von Elementen</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

Informationen zum Adobe Workfront Planning-Zugriff finden Sie unter [Übersicht über den Adobe Workfront Planning-Zugriff](/help/quicksilver/planning/access/access-overview.md).

Weitere Informationen zu Adobe GenStudio for Performance Marketing finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).


## Überblick über die Funktionen zur Integration von Workfront Planning und GenStudio for Performance Marketing

Je nachdem, über wie viele Workfront-Instanzen Ihr Unternehmen verfügt, haben Sie automatisch die folgenden Berechtigungen für den GenStudio-Arbeitsbereich in Planning:

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Eine Instanz von Workfront</p></td> 
   <td> 
<p>Der GenStudio-Arbeitsbereich ist in Ihrer Instanz von Workfront Planning sichtbar</p>
<p>Alle Benutzenden, einschließlich Workfront-Administratoren, haben standardmäßig Beitragszugriff auf den GenStudio-Arbeitsbereich in Planning</p>
<p>Workfront-Admins können für den GenStudio-Arbeitsbereich für jeden Benutzer Berechtigungen zum Verwalten ändern und erteilen</p>
</td> </tr>
   <tr> 
<td> 
   <p> Mehrere Instanzen von Workfront</p> </td> 
   <td> 
   <p>Der GenStudio Workspace ist in allen Workfront-Instanzen sichtbar</p>
<p>Alle Benutzenden mit Zugriff auf GenStudio for Performance Marketing und Workfront Planning haben standardmäßig Beitragsberechtigungen für GenStudio in Planning</p> 
<p>Workfront-Admins können niemandem Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich erteilen</p>

</td> 
  </tr>
   </tbody> 
</table>

Informationen zu Workfront-Planungsberechtigungen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

In den folgenden Abschnitten werden die folgenden Themen beschrieben:

* Funktionen zum Aktualisieren von Workfront-Planungsinformationen aus GenStudio for Performance Marketing
* Funktionen zum Aktualisieren von GenStudio for Performance Marketing-Informationen aus Workfront Planning
* Einschränkungen für das, was Sie in einem GenStudio-Arbeitsbereich in Workfront Planning verwalten können und was nicht.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Der GenStudio-Arbeitsbereich in Workfront Planning

* Der GenStudio-Arbeitsbereich zeigt in Workfront einen visuellen Indikator an, um ihn als den GenStudio for Performance Marketing-Arbeitsbereich darzustellen.

  ![GenStudio-Karte in Planung](assets/genstudio-card-with-tag-highlighted.png)

  Weitere Informationen finden Sie unter [Verwalten des GenStudio-Arbeitsbereichs in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie:

   * Aktualisieren des GenStudio-Arbeitsbereichs in Planning (Name, Beschreibung, Symbol)
   * Erstellen von Abschnitten
   * Datensatztypen hinzufügen
   * Für andere freigeben

     Sie können den GenStudio-Arbeitsbereich für andere freigeben, die kein GenStudio-Konto haben. Sie können sie nur für Benutzende freigeben, die im Identity Management-System (IMS) Ihres Unternehmens verfügbar sind. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie den Arbeitsbereich nicht in Workfront Planning ändern.

### Datensatztypen im GenStudio Workspace

* Datensatztypen, die sowohl in GenStudio for Performance Marketing als auch in Planning sichtbar sind, haben in Workfront Planning einen GenStudio-Indikator.

  ![Karte vom Typ &quot;GenStudio-Datensatz“ in Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:
   * Bearbeiten von Informationen zu GenStudio-Datensatztypen (ihr Erscheinungsbild, erweiterte Einstellungen).
   * GenStudio-Datensatztypen für andere freigeben.
   * Datensatztypen erstellen. Diese Datensatztypen verbleiben nur in Workfront Planning. Sie werden in GenStudio nicht angezeigt.
   * Aktivieren von Datensätzen aus GenStudio Workspace, um eine Verbindung von anderen Workspaces herzustellen.
   * Aktivieren Sie das Hinzufügen von Datensätzen aus dem GenStudio-Arbeitsbereich zu anderen Arbeitsbereichen.
* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie die GenStudio-Datensatztypen in Planning nicht ändern.

### Datensätze im GenStudio Workspace

* Wenn Sie GenStudio-Datensätze über GenStudio for Performance Marketing bearbeiten, sind die Änderungen im Arbeitsbereich &quot;GenStudio&quot; in allen Instanzen von Workfront sichtbar.
* Sie können in Workfront Planning keine Aktivierungsdatensätze aus dem GenStudio-Arbeitsbereich erstellen oder löschen.
* Wenn Sie über die Berechtigung Verwalten oder Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes tun:
   * Wenn Sie Datensätze hinzufügen oder löschen, werden diese in GenStudio for Performance Marketing sichtbar (oder daraus entfernt).

     Gelöschte Datensätze aus Workfront Planning oder GenStudio for Performance Marketing werden 30 Tage lang in den Workfront Planning-Container verschoben. GenStudio for Performance Marketing hat keine kürzlich gelöschte Bin.
   * Stellen Sie einen Datensatz aus dem kürzlich gelöschten Bin wieder her. Wenn gelöschte Datensätze wiederhergestellt werden, werden sie wieder in Workfront Planning und GenStudio for Performance Marketing platziert.
   * Fügen Sie Datensätze wie folgt hinzu:

      * Manuell, von Grund auf, aus jeder Ansicht mithilfe der Schaltfläche Neuer Datensatz
      * Durch Importieren mithilfe einer CSV- oder Excel-Datei in die Tabellenansicht
      * Manuell, in jeder Ansicht in Workfront Planning
      * Durch Senden einer Anfrage an ein Anfrageformular für einen Datensatztyp in Workfront.

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Sie können Datensatzinformationen für alle Datensätze im Arbeitsbereich von GenStudio in Workfront Planning bearbeiten.

  Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

### Datensatztypfelder im GenStudio-Arbeitsbereich

* Datensatztypfelder werden standardmäßig aus GenStudio for Performance Marketing in Workfront Planning importiert.
* Sie können keine Felder aus GenStudio for Performance Marketing zu Datensatztypen hinzufügen.
<!--Iskuhi said this is not possible but I can add fields: * You cannot create or delete Activation records' fields from the GenStudio workspace in Workfront Planning. -->
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:

   * Bearbeiten der GenStudio-Feldeinstellungen.
   * Erstellen Sie Felder für GenStudio-Datensatztypen, wenn Sie im Gen Studio-Arbeitsbereich über Verwaltungszugriff verfügen.

     Wenn Sie in Planning Felder für GenStudio-Datensatztypen erstellen, sind diese in den folgenden Bereichen sichtbar:

      * Workfront-Planungsansichten
      * Detailseiten für Workfront-Planungsdatensätze
      * Detailseiten für GenStudio-Einträge

     >[!TIP]
     >
     >In Workfront Planning erstellte Felder sind in der GenStudio-Listenansicht nicht sichtbar.

   * Felder in der Tabellenansicht eines GenStudio-Datensatztyps in Workfront Planning ausblenden.
&lt;!—* Löschen Sie in Workfront Planning für GenStudio erstellte Felder aus Workfront Planning. — dies ist nicht möglich, per Iskuhi; der Link ist vorhanden, aber er wird einen Fehler erzeugen—>

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen:

   * Sie können in Workfront Planning keine Feldeinstellungen bearbeiten, Felder aus dem GenStudio-Arbeitsbereich löschen oder hinzufügen.
   * Sie können Felder in Workfront Planning aus der Tabellenansicht ausblenden.

#### Die Felder Erstellt von und Genehmigt von

* Sie können die Felder Erstellt von und Genehmigt von für die GenStudio-Datensatztypen in Workfront Planning aus Workfront Planning hinzufügen.
* Die Datensätze, die in den Datensatztypen „Kanal“ und „Region“ angezeigt werden, zeigen „System“ als vom Benutzer erstellt an. Diese Datensätze werden automatisch erstellt, wenn der GenStudio-Arbeitsbereich in Workfront Planning erstellt wird.
* Die Datensätze, die in GenStudio erstellt wurden, nachdem der Arbeitsbereich in Workfront Planning verfügbar gemacht wurde, zeigen den Namen des IMS-Benutzers an, der den Datensatz im Feld Erstellt von erstellt hat, auch wenn der Benutzer die Datensätze in GenStudio erstellt hat und kein Workfront-Benutzer ist.
* Das Feld Genehmigt von zeigt den Namen der genehmigenden Person an, wenn ein Anfrageformular gesendet wird, um in Workfront Planning einen Datensatz vom Typ &quot;GenStudio-Datensatz“ zu erstellen.
* Die Felder Erstellt von und Genehmigt von werden in den Details der Datensätze in GenStudio for Performance Marketing angezeigt. Sie werden nicht in der Listenansicht angezeigt.

### Datensatzansichten im GenStudio-Arbeitsbereich

>[!NOTE]
>
>Die GenStudio-Datensatztypen werden in der aus der GenStudio for Performance Marketing-Listenansicht importierten Standardtabellenansicht angezeigt.
>
>Sie können die ursprüngliche Tabellenansicht, die standardmäßig aus GenStudio for Performance Marketing importiert wurde, nicht löschen.

* Sie können in GenStudio for Performance Marketing nicht mehrere Ansichten erstellen.

* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:

   * Erstellen Sie Ansichten für GenStudio-Datensatztypen.

     Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

   * Umbenennen, Freigeben, Exportieren, Duplizieren oder Löschen benutzerdefinierter Ansichten aus den GenStudio-Datensatztypen.

* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:

   * Erstellen Sie Ansichten für GenStudio-Datensatztypen.

     Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

   * Umbenennen, Exportieren, Duplizieren oder Löschen benutzerdefinierter Ansichten aus den GenStudio-Datensatztypen.

     Sie können in Workfront Planning keine Ansichten aus dem GenStudio-Arbeitsbereich freigeben

### Aufzeichnen von Verbindungen im GenStudio Workspace

Sie können in GenStudio-Arbeitsbereichen, für die Sie über Verwaltungsberechtigungen verfügen, Verbindungen zwischen Datensatztypen erstellen.

Sie können in Workfront Planning die folgenden Verbindungen zwischen GenStudio-Datensatztypen und anderen Datensatz- oder Objekttypen herstellen:

* Zwei GenStudio-Datensatztypen
* Einen GenStudio-Datensatztyp und einen Planning-Datensatztyp aus demselben Arbeitsbereich
* Einen GenStudio-Datensatztyp und einen Planning-Datensatztyp aus einem anderen Arbeitsbereich, wenn die Datensatztypen für die Verbindung aus einem anderen Arbeitsbereich konfiguriert sind.
* Ein GenStudio-Datensatztyp und ein Workfront-Objekttyp (Projekte, Portfolios, Programme, Unternehmen, Gruppen)
* Einen GenStudio-Datensatztyp und einen AEM Assets-Objekttyp.

### Anforderungsformulare und Automatisierungen im Datensatztyp GenStudio

* Sie können in Workfront Planning Anfrageformulare zu einem GenStudio-Datensatztyp hinzufügen.

  Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Sie können Automatisierungen für einen GenStudio-Datensatztyp in Workfront Planning konfigurieren.

  Weitere Informationen finden Sie unter [Konfigurieren von Adobe Workfront Planning Automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

## Die Vorschau-Umgebung

* Der GenStudio-Arbeitsbereich, auf den Sie über Ihre Produktionsumgebung zugreifen können, wird auch in Ihrer Vorschau-Umgebung derselben Workfront-Instanz angezeigt.
* Sie können alle in diesem Artikel beschriebenen Aktivitäten im GenStudio-Arbeitsbereich in Workfront Planning in Ihrer Vorschau-Umgebung ausführen. Diese Änderungen werden jedoch nicht in GenStudio angezeigt.

  Nur Änderungen, die Sie an Elementen in der Produktionsumgebung vornehmen, werden zwischen Workfront Planning und GenStudio synchronisiert.

  GenStudio hat keine Vorschau-Umgebung.

