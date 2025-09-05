---
title: Erste Schritte mit der Workfront Planning and GenStudio for Performance Marketing Integration
description: Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat. Erfahren Sie mehr über die Grundlagen, wie Sie Ihre Workflows mithilfe dieser Integration optimieren können.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4745b93e02c9de087afbee752e0303280e52d688
workflow-type: tm+mt
source-wordcount: '1765'
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

Unternehmen, die sowohl Adobe Workfront Planning als auch Adobe GenStudio for Performance Marketing verwenden, definieren Marketing-Konzepte wie Kampagnen, Produkte und Personas häufig detaillierter als das, was GenStudio standardmäßig unterstützt.

GenStudio for Performance Marketing und Workfront Planning sind nativ integriert. Diese Integration ermöglicht es Benutzenden, in Workfront Planning, Kampagnen, Produkte, Personas, Aktivierungen, Kanäle und Regionen zu verwalten, die in GenStudio verwendet werden. Außerdem können sie GenStudio so konfigurieren, dass in Workfront Planning auf bestehende Datensatztypen verwiesen wird, und so einen besser vernetzten und konsistenteren Marketing-Workflow erstellen.

Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat.

## Integrationsvorteile

Durch die Integration von Workfront Planning mit GenStudio for Performance Marketing können Sie:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Anzeigen von GenStudio Workspace in Workfront Planning.
* Ändern Sie Ihre Kampagnen in GenStudio und führen Sie Echtzeitaktualisierungen derselben Informationen in Workfront Planning durch.
* Ändern Sie Ihre Kampagnen in Workfront Planning und erhalten Sie in GenStudio Echtzeit Aktualisierungen derselben Informationen.
* Doppelte Dateneingabe vermeiden.
* Beibehaltung der Ausrichtung bei allen Planungs- und Aktivierungsmaßnahmen.

## Integrationsanforderungen

Ihr Unternehmen muss die folgenden Anforderungen erfüllen, damit die Integration zwischen Workfront Planning und GenStudio for Performance Marketing vorhanden ist:

* Workfront und GenStudio for Performance Marketing müssen für dieselbe Organisation aktiviert sein.

  Weitere Informationen zu GenStudio finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Ihre Workfront-Instanz ist Teil des einheitlichen Adobe-Erlebnisses, einschließlich der Verwendung des Identity Management-Systems (IMS).

  Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Benutzer, die sowohl Planning als auch GenStudio verwenden, dürfen nur zu einer Workfront-Instanz in der IMS-Organisation gehören.

  Benutzende, die nur Workfront nutzen, können den GenStudio-Arbeitsbereich nicht sehen, selbst wenn er in Workfront verfügbar ist.

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
   <li>GenStudio System Manager für den Zugriff auf Aktivierungen und Ereignisse</li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Verwalten Sie Berechtigungen für den GenStudio-Arbeitsbereich, um die Architektur des Arbeitsbereichs, die Datensatztypen und Felder zu ändern</p></li>
   <li><p>Berechtigungen für den GenStudio-Arbeitsbereich hinzufügen, um Datensätze im GenStudio-Datensatzbereich hinzuzufügen, zu aktualisieren oder zu löschen</p> </li>  
   </ul>
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


## Überblick über die Funktionen zur Integration von Workfront Planning und GenStudio

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
<p>In Workfront Planning gibt es einen GenStudio-Arbeitsbereich</p>
<p>Alle Benutzenden mit Zugriff auf GenStudio und Workfront Planning verfügen über Verwaltungsberechtigungen für den GenStudio Workspace</p> 
</td> </tr>
   <tr> 
<td> 
   <p> Mehrere Instanzen von Workfront</p> </td> 
   <td> 
   <p>In jeder Workfront Planning-Instanz gibt es einen GenStudio-Arbeitsbereich</p>
<p>Alle Benutzenden mit Zugriff auf GenStudio und Workfront Planning haben Beitragsberechtigungen für den GenStudio-Arbeitsbereich jeder Instanz</p> </td> 
  </tr>

</tbody> 
</table>

Informationen zu Workfront-Planungsberechtigungen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

In den folgenden Abschnitten werden die folgenden Themen beschrieben:

* Funktionen zum Aktualisieren von Workfront-Planungsinformationen aus GenStudio
* Funktionen zum Aktualisieren von GenStudio-Informationen aus Workfront Planning
* Einschränkungen für das, was Sie in einem GenStudio-Arbeitsbereich in Workfront Planning verwalten können und was nicht.

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Der GenStudio-Arbeitsbereich

* Wenn Sie GenStudio Workspace in GenStudio aktualisieren, werden die Änderungen in GenStudio Workspace in Planning angezeigt.
* Der GenStudio-Arbeitsbereich zeigt in Workfront Planning einen visuellen Indikator an, um ihn als solchen zu identifizieren.

  ![GenStudio-Karte in Planung](assets/genstudio-card-with-tag-highlighted.png)

  Weitere Informationen finden Sie unter [Verwalten des GenStudio-Arbeitsbereichs in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie:

   * Aktualisieren des GenStudio-Arbeitsbereichs in Planning (Name, Beschreibung, Symbol)
   * Erstellen von Abschnitten
   * Datensatztypen hinzufügen
   * Für andere freigeben

     Sie können den GenStudio-Arbeitsbereich für andere freigeben, die kein GenStudio-Konto haben. Sie können sie nur für Benutzende freigeben, die im Identity Management-System (IMS) Ihres Unternehmens verfügbar sind. <!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie den Arbeitsbereich nicht in Planning ändern.

### Datensatztypen im GenStudio Workspace

* Wenn Sie die GenStudio-Datensatztypen in GenStudio bearbeiten, werden die Änderungen in Planning im GenStudio-Arbeitsbereich angezeigt.
* Datensatztypen, die sowohl in GenStudio als auch in Planning sichtbar sind, haben in Workfront Planning einen GenStudio-Indikator.

  ![Karte vom Typ &quot;GenStudio-Datensatz“ in Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:
   * Bearbeiten von Informationen zu GenStudio-Datensatztypen (ihr Erscheinungsbild, erweiterte Einstellungen).
   * GenStudio-Datensatztypen für andere freigeben.
   * Datensatztypen erstellen. Diese Datensatztypen verbleiben nur in Workfront Planning. Sie werden in GenStudio nicht angezeigt.
* Wenn Sie über die Berechtigung Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie die GenStudio-Datensatztypen in Planning nicht ändern.

### Datensätze im GenStudio Workspace

* Wenn Sie GenStudio-Datensätze in GenStudio bearbeiten, sind die Änderungen in allen GenStudio-Arbeitsbereichen in allen Instanzen von Workfront sichtbar.
* Sie können keine Aktivierungsdatensätze aus Workfront Planning erstellen oder löschen.
* Wenn Sie über die Berechtigung Verwalten oder Beitragen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes tun:
   * Wenn Sie Datensätze hinzufügen oder löschen, werden diese in GenStudio sichtbar (oder daraus entfernt).

     Gelöschte Datensätze aus Workfront Planning oder GenStudio werden 30 Tage lang in den Workfront Planning-Container verschoben. GenStudio hat keine kürzlich gelöschte Bin.
   * Stellen Sie einen Datensatz aus dem kürzlich gelöschten Bin wieder her. Wenn gelöschte Datensätze wiederhergestellt werden, werden sie wieder in Workfront Planning und GenStudio platziert.
   * Fügen Sie Datensätze wie folgt hinzu:

      * Manuell, von Grund auf, aus jeder Ansicht mithilfe der Schaltfläche Neuer Datensatz
      * Durch Importieren mithilfe einer CSV- oder Excel-Datei in die Tabellenansicht
      * Manuell, in jeder Ansicht in Workfront Planning
      * Durch Senden einer Anfrage an ein Anfrageformular für einen Datensatztyp in Workfront.

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Sie können Datensatzinformationen für alle Datensätze im Arbeitsbereich von GenStudio in Workfront Planning bearbeiten.

  Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

### Felder von Datensatztypen im GenStudio Workspace

* GenStudio-Datensatzfelder werden standardmäßig in Workfront Planning importiert.
* Datensatztypen in GenStudio können keine Felder hinzugefügt werden.
* Wenn Sie über Verwaltungsberechtigungen für den GenStudio-Arbeitsbereich in Planning verfügen, können Sie in Workfront Planning Folgendes ausführen:

   * Bearbeiten der GenStudio-Feldeinstellungen.
   * Erstellen Sie Felder für GenStudio-Datensatztypen, wenn Sie Verwaltungszugriff in Gen Studio haben.

     Wenn Sie in Planning Felder für GenStudio-Datensatztypen erstellen, sind diese in den folgenden Bereichen sichtbar:

      * Workfront-Planungsansichten
      * Detailseiten für Workfront-Planungsdatensätze
      * Detailseiten für GenStudio-Einträge

     >[!TIP]
     >
     >In Workfront Planning erstellte Felder sind in der GenStudio-Listenansicht nicht sichtbar.

   * Felder in der Tabellenansicht eines GenStudio-Datensatztyps in Planning ausblenden.
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

### Datensatzansichten im GenStudio-Arbeitsbereich

>[!NOTE]
>
>Die GenStudio-Datensatztypen werden in der aus GenStudio importierten Standardtabellenansicht angezeigt.
>
>Sie können die ursprüngliche Tabellenansicht, die standardmäßig aus GenStudio importiert wurde, nicht löschen.

* Sie können in GenStudio nicht mehrere Ansichten erstellen.

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

