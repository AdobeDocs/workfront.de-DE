---
title: Einträge duplizieren
description: Sie können einen vorhandenen Datensatz in der Tabellenansicht duplizieren. Der Seite „Datensatztyp“ wird eine identische Kopie des vorhandenen Datensatzes hinzugefügt.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Doppelte Einträge

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning ist ein Datensatz eine Instanz eines Datensatztyps.

Sie können einen vorhandenen Datensatz in der Tabellenansicht duplizieren. Der Seite „Datensatztyp“ wird eine identische Kopie des vorhandenen Datensatzes hinzugefügt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


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

   * Bewegen Sie den Mauszeiger über den Namen eines Datensatzes und klicken Sie dann auf das Menü **Mehr** inline mit dem Datensatznamen. Klicken Sie dann auf das **Duplizieren**-Symbol ![Duplizieren-Symbol grau](assets/duplicate-icon-gray.png) .

     ![Menü Mehr aus Datensatz in der Tabellenansicht](assets/more-menu-from-record-in-table-view.png)

   * Wählen Sie einen Datensatz aus und klicken Sie dann auf **Symbol &quot;** Duplizieren![ Symbol „Duplizieren](assets/duplicate-icon-white-and-blue.png) in der Symbolleiste am unteren Seitenrand.

     ![Symbol „Duplizieren“ in der Symbolleiste in der Tabellenansicht](assets/duplicate-icon-in-toolbar-in-table-view.png)

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
