---
title: Erste Schritte mit der Workfront Planning and GenStudio for Performance Marketing Integration
description: Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat. Erfahren Sie mehr über die Grundlagen, wie Sie Ihre Workflows mithilfe dieser Integration optimieren können.
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b366841f3994468624a0c9b07d9de6f2f274cbe0
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 1%

---

# Erste Schritte mit der Integration von Workfront Planning und GenStudio for Performance Marketing

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

Unternehmen, die sowohl Adobe Workfront Planning als auch Adobe GenStudio for Performance Marketing verwenden, definieren Marketing-Konzepte wie Kampagnen, Produkte und Personas häufig detaillierter als das, was GenStudio standardmäßig unterstützt.

GenStudio for Performance Marketing und Workfront Planning sind nativ integriert. Diese Integration ermöglicht es Benutzenden, in Workfront Planning, Kampagnen, Produkte, Personas, Aktivierungen, Kanäle und Regionen zu verwalten, die in GenStudio verwendet werden. Außerdem können sie GenStudio so konfigurieren, dass in Workfront Planning auf bestehende Datensatztypen verwiesen wird, und so einen besser vernetzten und konsistenteren Marketing-Workflow erstellen.

Diese Integration hilft Ihnen, doppelte Dateneingabe zu vermeiden, die Abstimmung über Planungs- und Aktivierungsmaßnahmen hinweg aufrechtzuerhalten und Ihr Marketing-Aufzeichnungssystem zu unterstützen.

Der GenStudio for Performance Marketing-Arbeitsbereich ist in Adobe Workfront Planning verfügbar, wenn Ihr Unternehmen beide Produkte gekauft hat.

Durch die Integration von Workfront Planning mit GenStudio for Performance Marketing können Sie:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* Anzeigen von GenStudio Workspace in Workfront Planning.
* Ändern Sie Ihre Kampagnen in GenStudio und führen Sie Echtzeitaktualisierungen derselben Informationen in Workfront Planning durch.
* Ändern Sie Ihre Kampagnen in Workfront Planning und erhalten Sie in GenStudio Echtzeit Aktualisierungen derselben Informationen.

## Zugriffsanforderungen

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
   <li><p> Adobe Workfront-Planung<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront-Planungspaket</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront Account Manager. </p> 
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
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p> Systemadministrator</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Integrationsanforderungen

* Workfront und GenStudio for Performance Marketing müssen für dieselbe Organisation aktiviert sein.
* GenStudio ist in Workfront Planning nicht verfügbar, wenn Ihr Unternehmen mehrere Workfront-Instanzen hat. <!--this will change-->

* Die Workfront-Instanz ist Teil von Adobe Unified Experience, einschließlich der Verwendung des Identity Management Systems (IMS).

  Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Benutzende, die sowohl Planning als auch GenStudio verwenden, können zu nur einer Workfront-Instanz in der IMS-Organisation gehören.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->


## Überlegungen zum Verwalten eines GenStudio-Arbeitsbereichs in Workfront Planning

* Ihr Unternehmen muss Adobe GenStudio for Performance Marketing erwerben, bevor Sie einen GenStudio-Arbeitsbereich in Workfront Planning anzeigen können.

  Weitere Informationen zu GenStudio finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).

  Weitere Informationen zur Integration von GenStudio und Workfront Planning finden Sie unter [Erste Schritte mit der Integration von Workfront Planning und GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)

* Workfront-Benutzende müssen Zugriff auf GenStudio haben, damit sie den GenStudio-Arbeitsbereich in Workfront Planning sehen können.


* In den folgenden Abschnitten wird beschrieben, welche Einschränkungen es gibt, was Sie in einem GenStudio-Arbeitsbereich in Workfront Planning verwalten können und was nicht.

### Der GenStudio-Arbeitsbereich in Workfront Planning

* Wenn Ihr Unternehmen über mehrere Workfront-Instanzen verfügt, kann nur eine Instanz von Workfront Ihren GenStudio-Arbeitsbereich anzeigen.
* Der GenStudio-Arbeitsbereich zeigt einen visuellen Indikator an, der deutlich macht, dass er aus GenStudio importiert wurde.

### Datensatztypen

* Datensatztypen können in Workfront Planning nicht über GenStudio bearbeitet werden.
* Datensatztypen aus GenStudio können nicht für andere Benutzer freigegeben werden. Workfront-Administratoren können den GenStudio-Arbeitsbereich in ihrem Planungsbereich anzeigen.
* Datensatztypen, die mit GenStudio synchronisiert werden, zeigen einen visuellen Indikator an, der deutlich macht, dass die Datensatztypen aus GenStudio importiert wurden.
* Benutzer, die den GenStudio-Arbeitsbereich in Planning anzeigen, können seine Datensatztypen für andere freigeben.

### Einträge

* Sie können Datensätze in GenStudio hinzufügen oder löschen, damit sie in Workfront Planning sichtbar werden (oder daraus entfernt werden).
Sie können Datensätze in Workfront Planning hinzufügen oder löschen, damit sie in GenStudio sichtbar werden (oder daraus entfernt werden).
* Sie können Datensätze aus Workfront Planning wie folgt hinzufügen:

   * Manuell, von Grund auf
   * Durch Importieren mithilfe einer CSV- oder Excel-Datei

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Sie können keine Aktivierungsdatensätze aus Workfront Planning erstellen oder löschen.
* Sie können Datensatzinformationen für alle Datensätze im Arbeitsbereich von GenStudio in jedem der sichtbaren Felder von Workfront Planning bearbeiten.

  Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

### Felder

* Alle Datensatzfelder werden aus GenStudio importiert und die Feldeinstellungen können nicht bearbeitet werden.
* Sie können in Workfront Planning nur dann Felder für GenStudio-Datensatztypen erstellen, wenn Sie Systemadministratorzugriff in GenStudio haben.
* In Planning können Sie Felder für GenStudio-Datensatztypen erstellen. Diese Felder sind in den folgenden Bereichen sichtbar:
   * Planungsansichten
   * Detailseiten für Planungsdatensätze
   * Detailseiten für GenStudio-Einträge

  >[!TIP]
  >
  >In Workfront Planning erstellte Felder sind in der GenStudio-Listenansicht nicht sichtbar.

* Sie können Felder in der Tabellenansicht eines GenStudio-Datensatztyps in Planning ausblenden, aber Sie können keine Felder aus Workfront Planning löschen.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Ansichten

* Sie können Ansichten für GenStudio-Datensatztypen erstellen. Sie können Ansichten, die automatisch aus GenStudio importiert wurden, nicht bearbeiten, aber Sie können die Ansichtselemente für die GenStudio-Tabellenansicht ändern. Sie können beispielsweise die Filter, die Sortierung, die Gruppierungen, die Zeilenfarben und die Zeilenhöhe in der Tabellenansicht ändern.

  Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

* Sie können die Ansicht eines GenStudio-Datensatztyps wie folgt freigeben:

   * Ansichts-Link kopieren
   * Ansicht in eine Datei exportieren (nur für die Tabellenansicht verfügbar)

### Verbindungen

* Es ist nicht möglich, in Planning andere Datensatz- oder Objekttypen aus GenStudio-Datensatztypen zu verbinden.
* Sie können in Planning von anderen Datensatztypen aus eine Verbindung zu GenStudio-Datensatztypen herstellen.
