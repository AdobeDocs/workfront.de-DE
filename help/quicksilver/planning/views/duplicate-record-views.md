---
title: Doppelte Datensatzansichten
description: Wenn Sie mehrere Versionen einer Ansicht beibehalten und geringfügige Änderungen zwischen den Versionen vornehmen möchten, können Sie eine Ansicht in Adobe Workfront Planning duplizieren. In diesem Artikel wird beschrieben, wie Sie eine Ansicht duplizieren können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Doppelte Datensatzansichten

<!--remove preview and production references-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Wenn Sie mehrere Versionen einer Ansicht beibehalten und geringfügige Änderungen zwischen den Versionen vornehmen möchten, können Sie eine Ansicht in Adobe Workfront Planning duplizieren.

Beim Duplizieren einer Ansicht werden identische Kopien einer vorhandenen Ansicht erstellt.

Die Freigabeberechtigungen der ursprünglichen Ansicht werden nicht in die duplizierte Ansicht übertragen.

Das Duplizieren von Ansichten ist für alle Ansichtstypen in Workfront Planning identisch.

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
   <td>   <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Anzeigeberechtigungen für eine Ansicht, um die Anzeigeeinstellungen vorübergehend zu ändern oder zu duplizieren.</p> </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it.</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Duplizieren einer Datensatzansicht

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Führen Sie je nach verwendeter Umgebung die folgenden Schritte aus:

   * Bewegen Sie in der Produktionsumgebung den Mauszeiger auf der Registerkarte Ansicht über einen der Namen der Ansicht und klicken Sie dann auf **Mehr** ![Mehr &#x200B;](assets/more-menu.png) links neben dem Ansichtsnamen und klicken Sie dann auf **Duplizieren**.
   * <span class="preview">Klicken Sie in der Vorschau-Umgebung auf das Dropdown-Symbol ![Dropdown-Symbol](assets/drop-down-icon.png) neben dem Namen der aktuellen Ansicht, bewegen Sie den Mauszeiger über den Namen einer Ansicht, klicken Sie auf **Mehr** und dann auf **Duplizieren**.</span>

     ![Menü „Mehr“ in der Ansicht mit Optionen](assets/more-menu-for-views-expanded-with-delete-option.png)

     Die Ansicht wird dupliziert und der Name der neuen Ansicht folgt dem folgenden Muster: `Original view's name (Copy)`. Die neue Ansichtsregisterkarte wird am Ende aller Ansichtsregisterkarten angezeigt.
