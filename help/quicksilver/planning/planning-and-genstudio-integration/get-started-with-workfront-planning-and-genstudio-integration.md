---
title: Erste Schritte mit der Workfront Planning and GenStudio for Performance Marketing Integration
description: Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat. Erfahren Sie mehr über die Grundlagen, wie Sie Ihre Workflows mithilfe dieser Integration optimieren können.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '1475'
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

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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

* Workfront und GenStudio for Performance Marketing müssen für dieselbe Organisation aktiviert sein.

  Weitere Informationen zu GenStudio finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).

* GenStudio ist in Workfront Planning nicht verfügbar, wenn Ihr Unternehmen mehrere Workfront-Instanzen hat. <!--this will change-->

* Die Workfront-Instanz ist Teil von Adobe Unified Experience, einschließlich der Verwendung des Identity Management Systems (IMS).

  Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Benutzende, die sowohl Planning als auch GenStudio verwenden, können zu nur einer Workfront-Instanz in der IMS-Organisation gehören.

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
<p>Beliebiges Adobe Workfront-Workflow-Paket</p>
<p>Beliebiges Adobe Workfront-Planungspaket</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio-Paket</p></td> 
   <td> 
<p>??? VERFÜGT GEN GEN STUDIO ÜBER EIN PAKET, DAS DIES UNTERSTÜTZT???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio-Lizenz</p></td> 
   <td><p> ??? BENÖTIGT GEN STUDIO EINE SPEZIELLE LIZENZ, DIE DIES UNTERSTÜTZT???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>  
   <p>Konfiguration für GenStudio: ???WAS IST DIE ZUGRIFFSEBENE, DIE GENS BENÖTIGT???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen*</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p> </li> 
   <li><p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p></li>
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Alle Berechtigungen in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Erstellen von Berechtigungen in Adobe GenStudio for Performance Marketing zum Erstellen von Elementen</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
*Weitere Informationen zu Adobe GenStudio for Performance Marketing finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).


## Übersicht über die Integration von Workfront Planning und GenStudio

In den folgenden Abschnitten werden die folgenden Themen beschrieben:

* Funktionen zum Aktualisieren von Workfront-Planungsinformationen aus GenStudio
* Funktionen zum Aktualisieren von GenStudio-Informationen aus Workfront Planning
* Einschränkungen für das, was Sie in einem GenStudio-Arbeitsbereich in Workfront Planning verwalten können und was nicht.

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Der GenStudio-Arbeitsbereich in Workfront Planning

* Wenn Ihr Unternehmen über mehrere Workfront-Instanzen verfügt, ist der GenStudio-Arbeitsbereich in keiner Ihrer Workfront-Instanzen sichtbar. <!-- this might change-->
* Der GenStudio-Arbeitsbereich zeigt einen visuellen Indikator an, der deutlich macht, dass er aus GenStudio importiert wurde. Weitere Informationen finden Sie unter [Verwalten des GenStudio-Arbeitsbereichs in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).
* Alle Benutzenden, die sowohl Zugriff auf GenStudio als auch auf Workfront Planning haben, können auch den GenStudio-Arbeitsbereich in Workfront Planning anzeigen.
* Workfront Planning-Benutzer müssen über das Adobe Identity Management System (IMS) verwaltet werden, damit sie den GenStudio Workspace von Workfront aus anzeigen und verwenden können.

  Benutzende, die nur Workfront nutzen, können den GenStudio-Arbeitsbereich nicht sehen, selbst wenn er in Workfront verfügbar ist.

  Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


### Datensatztypen

* Sie können Informationen zu GenStudio-Datensatztypen (z. B. deren Erscheinungsbild) in Workfront Planning bearbeiten.
* Sie können GenStudio-Datensatztypen in Planning für andere freigeben.
* Datensatztypen können im Arbeitsbereich von GenStudio unter „Planung“ erstellt werden. Diese Datensatztypen verbleiben nur in Planning. Sie werden in GenStudio nicht angezeigt.
* Datensatztypen, die mit GenStudio synchronisiert werden, zeigen in Workfront Planning einen visuellen Indikator an, der deutlich macht, dass die Datensatztypen aus GenStudio importiert wurden.

### Einträge

Datensätze, die zu GenStudio-Datensatztypen gehören und sowohl in GenStudio als auch in Workfront Planning angezeigt werden, können wie folgt konfiguriert werden:

* Sie können Datensätze in GenStudio hinzufügen oder löschen, damit sie in Workfront Planning sichtbar werden (oder daraus entfernt werden).
* Sie können Datensätze in Workfront Planning hinzufügen oder löschen, damit sie in GenStudio sichtbar werden (oder daraus entfernt werden).
* Wenn Sie Datensätze aus Workfront Planning oder GenStudio löschen, werden sie 30 Tage lang in das Bin für kürzlich gelöschte Workfront Planning verschoben. GenStudio hat keine kürzlich gelöschte Bin.
* Wenn Sie einen Datensatz aus dem kürzlich gelöschten Bin wiederherstellen, wird er wieder in Workfront Planning und GenStudio platziert.
* Sie können Datensätze aus Workfront Planning wie folgt hinzufügen:

   * Manuell, von Grund auf, aus jeder Ansicht mithilfe der Schaltfläche Neuer Datensatz
   * Durch Importieren mithilfe einer CSV- oder Excel-Datei
   * Manuell, inline, in der Tabellenansicht
   * Manuell, direkt in der Zeitleisten- oder Kalenderansicht <!--ensure the calendar is released when this releases-->

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Sie können keine Aktivierungsdatensätze aus Workfront Planning erstellen oder löschen.
* Sie können Datensatzinformationen für alle Datensätze im Arbeitsbereich von GenStudio in Planning in jedem der sichtbaren Felder von Workfront Planning bearbeiten.

  Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Felder

* Datensatzfelder werden aus GenStudio importiert. Sie können GenStudio-Feldeinstellungen über Workfront Planning bearbeiten.
* In Workfront Planning können Sie Felder für GenStudio-Datensatztypen erstellen, wenn Sie in Gen Studio über Verwaltungszugriff verfügen.
* Wenn Sie in Planning Felder für GenStudio-Datensatztypen erstellen, sind diese in den folgenden Bereichen sichtbar:
   * Planungsansichten
   * Detailseiten für Planungsdatensätze
   * Detailseiten für GenStudio-Einträge

  >[!TIP]
  >
  >In Workfront Planning erstellte Felder sind in der GenStudio-Listenansicht nicht sichtbar.

* Sie können Felder in der Tabellenansicht eines GenStudio-Datensatztyps in Planning ausblenden.
* Aus GenStudio importierte Felder können nicht aus Workfront Planning gelöscht werden.
* Sie können Felder, die in Workfront Planning für GenStudio-Datensatztypen erstellt wurden, aus Workfront Planning löschen.

### Die Felder Erstellt von und Genehmigt von

* Sie können die Felder Erstellt von und Genehmigt von für die GenStudio-Datensatztypen in Workfront Planning aus Workfront Planning hinzufügen.
* Die Datensätze, die in den Datensatztypen „Kanal“ und „Region“ angezeigt werden, zeigen „System“ als vom Benutzer erstellt an. Diese Datensätze werden automatisch erstellt, wenn der GenStudio-Arbeitsbereich in Workfront Planning erstellt wird.
* Die Datensätze, die in GenStudio erstellt wurden, nachdem der Arbeitsbereich in Workfront Planning verfügbar gemacht wurde, zeigen den Namen des IMS-Benutzers an, der den Datensatz im Feld Erstellt von erstellt hat, auch wenn der Benutzer die Datensätze in GenStudio erstellt hat und kein Workfront-Benutzer ist.
* Das Feld Genehmigt von zeigt den Namen der genehmigenden Person an, wenn ein Anfrageformular gesendet wird, um in Workfront Planning einen Datensatz vom Typ &quot;GenStudio-Datensatz“ zu erstellen.

### Ansichten 

* Sie können Ansichten für GenStudio-Datensatztypen erstellen.

  Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

* Die Freigabe der Ansicht eines GenStudio-Datensatztyps ist identisch mit der Freigabe einer Ansicht für einen Planning-Datensatztyp.
* Sie können in GenStudio nicht mehrere Ansichten erstellen.

### Verbindungen

* Sie können in Workfront Planning die folgenden Verbindungen zwischen GenStudio-Datensatztypen und anderen Datensatz- oder Objekttypen herstellen:

   * Zwei GenStudio-Datensatztypen
   * Einen GenStudio-Datensatztyp und einen Planning-Datensatztyp aus demselben Arbeitsbereich
   * Einen GenStudio-Datensatztyp und einen Planning-Datensatztyp aus einem anderen Arbeitsbereich, wenn die Datensatztypen für die Verbindung aus einem anderen Arbeitsbereich konfiguriert sind.
   * Ein GenStudio-Datensatztyp und ein Workfront-Objekttyp (Projekte, Portfolios, Programme, Unternehmen, Gruppen)
   * Einen GenStudio-Datensatztyp und einen AEM Assets-Objekttyp.

### Anforderungsformulare und Automatisierungen

* Sie können in Workfront Planning Anfrageformulare zu einem GenStudio-Datensatztyp hinzufügen.
* Sie können Automatisierungen für einen GenStudio-Datensatztyp in Workfront Planning konfigurieren.

### Die Vorschau-Umgebung

* Der GenStudio-Arbeitsbereich, auf den Sie über Ihre Produktionsumgebung zugreifen können, wird auch in Ihrer Vorschau-Umgebung angezeigt.
* Sie können alle in diesem Artikel beschriebenen Aktivitäten im GenStudio-Arbeitsbereich in Workfront Planning in Ihrer Vorschau-Umgebung ausführen. Diese Änderungen werden jedoch nicht auf GenStudio übertragen.
Nur Änderungen, die Sie an Elementen in der Produktionsumgebung vornehmen, werden zwischen Workfront Planning und GenStudio synchronisiert.
GenStudio hat keine Vorschau-Umgebung.

