---
title: Doppelte Datensatzansichten
description: Wenn Sie mehrere Versionen einer Ansicht beibehalten und geringfügige Änderungen zwischen den Versionen vornehmen möchten, können Sie eine Ansicht in Adobe Workfront Planning duplizieren. In diesem Artikel wird beschrieben, wie Sie eine Ansicht duplizieren können.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

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

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

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
<li>Prime</li> 
<li>Ultimate</li></ul> 
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
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
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
   <td>   <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Anzeigeberechtigungen für eine Ansicht, um die Anzeigeeinstellungen vorübergehend zu ändern oder zu duplizieren.</p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Duplizieren einer Datensatzansicht

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
Standardmäßig werden alle Datensätze des ausgewählten Typs in der Tabellenansicht angezeigt.

1. Führen Sie je nach verwendeter Umgebung die folgenden Schritte aus:

   * Bewegen Sie in der Produktionsumgebung den Mauszeiger auf der Registerkarte Ansicht über einen der Namen der Ansicht und klicken Sie dann auf **Mehr** ![Mehr ](assets/more-menu.png) links neben dem Ansichtsnamen und klicken Sie dann auf **Duplizieren**.
   * <span class="preview">Klicken Sie in der Vorschau-Umgebung auf das Dropdown-Symbol ![Dropdown-Symbol](assets/drop-down-icon.png) neben dem Namen der aktuellen Ansicht, bewegen Sie den Mauszeiger über den Namen einer Ansicht, klicken Sie auf **Mehr** und dann auf **Duplizieren**.</span>

     ![Menü „Mehr“ in der Ansicht mit Optionen](assets/more-menu-for-views-expanded-with-delete-option.png)

     Die Ansicht wird dupliziert und der Name der neuen Ansicht folgt dem folgenden Muster: `Original view's name (Copy)`. Die neue Ansichtsregisterkarte wird am Ende aller Ansichtsregisterkarten angezeigt.
