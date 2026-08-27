---
title: Konfigurieren von Geschäftsregeln für Datensatztypen
description: Sie können Geschäftsregeln für Datensatztypen konfigurieren, die festlegen, wie Datensätze dieses Typs in Adobe Workfront Planning verwaltet werden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 914f1f8a25aa5b9e1045d2f940ed15061301c21b
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 5%

---


# Konfigurieren von Geschäftsregeln für Datensatztypen

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Sie können Geschäftsregeln für Datensatztypen konfigurieren, die festlegen, wie Datensätze dieses Typs in Adobe Workfront Planning verwaltet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen, um die Schritte in diesem Artikel auszuführen:  

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
<li><p>Beliebige Workfront oder Workflows mit einem Planungspaket</p></li>
ODER
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Workflow-Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Planungsstandard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Sie müssen der Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen, wenn Sie sowohl einen Workflow als auch ein Planning-Paket haben</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und einen Datensatztyp</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen beim Konfigurieren von Geschäftsregeln

* Sie können Regeln konfigurieren, nach denen Datensätze je nach definierten Bedingungen bearbeitet oder gelöscht werden können.

  Sie können beispielsweise Bedingungen erstellen, die verlangen, dass bestimmte Felder einen Wert enthalten. Wenn der Wert in diesen Feldern fehlt, können Benutzende diesen Datensatz nicht bearbeiten oder löschen.
* Sie können keine Geschäftsregeln zu globalen Datensatztypen in ihren primären oder sekundären Arbeitsbereichen hinzufügen.
* Regeln für den Zeitpunkt der Datensatzerstellung können nicht konfiguriert werden. Jeder, der über Verwaltungsberechtigungen für den Datensatztyp verfügt, kann Datensätze erstellen.
* Sie können eine Bedingung für Ihre Geschäftsregel erstellen, die auf alle Feldtypen mit Ausnahme der folgenden verweist:
  * Formelfelder
  * Suchfelder
  * Referenzfelder

## Geschäftsregeln konfigurieren

1. Zu einem Datensatztyp gehen.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf Geschäftsregeln.



