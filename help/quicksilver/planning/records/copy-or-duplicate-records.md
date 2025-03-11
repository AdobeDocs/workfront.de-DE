---
title: Einträge duplizieren
description: Sie können einen vorhandenen Datensatz in der Tabellenansicht duplizieren. Der Seite „Datensatztyp“ wird eine identische Kopie des vorhandenen Datensatzes hinzugefügt.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Doppelte Einträge

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning ist ein Datensatz eine Instanz eines Datensatztyps.

Sie können einen vorhandenen Datensatz in der Tabellenansicht duplizieren. Der Seite „Datensatztyp“ wird eine identische Kopie des vorhandenen Datensatzes hinzugefügt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
   <td>   <p>Mitwirken an oder höhere Berechtigungen für eine Workspace-<!--<span class="preview">and record type</span>--></a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Duplizieren einer <!--in a record type table (I don't think you can create them elsewhere right now)-->

Sie können Datensätze in der Tabellenansicht einer Datensatztypseite durch Duplizieren einer vorhandenen Seite erstellen. Ein mit dem vorhandenen identischer Datensatz wird erstellt und unter dem ursprünglichen Datensatz hinzugefügt.


{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.
Alle Datensätze des ausgewählten Typs werden in der Ansicht angezeigt.

1. (Bedingt) Tabellenansicht auswählen.

1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über den Namen eines Datensatzes und klicken Sie dann auf das **Mehr**-Menü inline mit dem Datensatznamen. Klicken Sie dann auf das **Duplizieren**-Symbol ![](assets/duplicate-icon-gray.png) .

     ![](assets/more-menu-from-record-in-table-view.png)

   * Wählen Sie einen Datensatz aus und klicken Sie dann auf **Symbol** Duplizieren![](assets/duplicate-icon-white-and-blue.png) unten auf der Seite in der Symbolleiste.

     ![](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Unterhalb des ursprünglichen Datensatzes wird ein identischer Datensatz mit identischem Namen erstellt. Alle Felder des neuen Datensatzes werden mit denselben Informationen wie im ursprünglichen Datensatz ausgefüllt.

1. (Optional) Starten Sie die Aktualisierung der Informationen zum neuen Datensatz in den Feldern, die in der Tabellenansicht verfügbar sind, oder klicken Sie auf den Datensatz und aktualisieren Sie die Informationen in der Datensatzvorschau oder -seite.

   >[!NOTE]
   >
   >  * Es gibt keine Pflichtfelder für Datensätze. Es wird jedoch empfohlen, Informationen für das Primärfeld eines Datensatzes hinzuzufügen, da es hilfreich ist, Datensätze zu identifizieren, wenn Datensätze miteinander verknüpft werden. Weitere Informationen zu Primärfeldern finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md) und [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Felder, die auf andere Datensatztypen oder berechnete Felder verweisen, sind schreibgeschützt.

   Weitere Informationen zum Bearbeiten von Datensätzen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Hinzufügen neuer Datensätze oder deren Informationen rückgängig zu machen oder wiederherzustellen, wenn Sie sie in der Tabellenansicht hinzufügen:

   * STRG + Z (⌘ + Z für Mac), um eine Änderung rückgängig zu machen
   * Strg+Umsch+Z (⌘+Umschalt+Z für Mac), um eine Änderung wiederherzustellen.
