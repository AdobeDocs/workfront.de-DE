---
title: Übersicht über die Freigabe von Berechtigungen in Adobe Maestro
description: Sie können Berechtigungen für einen von Ihnen erstellten Adobe Maestro-Arbeitsbereich freigeben oder daraus entfernen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: fda35538234593b66b01f9e0cc0dafd6a63a84dc
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 1%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!-- *********add to TOC****************-->

# Übersicht über die Freigabe von Berechtigungen in Adobe Maestro

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Zugriff auf Maestro zu erhalten.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Berechtigungen für einen von Ihnen erstellten Adobe Maestro-Arbeitsbereich freigeben oder daraus entfernen.

## Objekte, die Sie in Adobe Maestro freigeben können

Sie können die folgenden Objekte in Maestro freigeben:

* Arbeitsbereiche

  Wenn Sie einen Arbeitsbereich freigeben, werden auch alle Datensatztypen, Datensätze und Felder freigegeben, die mit den Arbeitsbereichen verknüpft sind. Ansichten werden nicht freigegeben.

* Ansichten

## Überlegungen zum Freigeben von Objekten in Maestro

* Sie müssen über die folgende Lizenz verfügen, um Arbeitsbereiche in Maestro zu erstellen:

   * Neues Preismodell: Standardlizenz
   * Aktuelles Preismodell: Arbeite oder höhere Lizenz
* Systemadministratoren können von anderen Benutzern erstellte Arbeitsbereiche verwalten und freigeben.
* Wenn Sie kein Systemadministrator sind, können Sie zu Arbeitsbereichen beitragen, die von anderen erstellt wurden, wenn diese für Sie freigegeben sind.
* Arbeitsbereiche können nicht gemeinsam genutzt werden.
* Sie können einen Arbeitsbereich für die folgenden Entitäten freigeben:
   * Benutzende
   * Gruppen
* Andere Benutzer, einschließlich Systemadministratoren, können nur auf Ansichten zugreifen, die sie erstellt haben oder die für sie freigegeben wurden.

## Berechtigungen für Maestro-Objekte freigeben

Die folgende Tabelle zeigt die Höhe der Berechtigungen, die Sie beim Freigeben eines Maestro-Arbeitsbereichs oder einer Ansicht auswählen können:

<table>
  <tr>


</td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td><p><b>Neu: Standardlizenz</b></p> <p><b>Aktuell: Worker-Lizenz oder höhere Lizenz</b></p></strong>
   </td>
   <td><strong>Berechtigungen verwalten</strong>
   </td>
   <td><strong>Berechtigungen beitragen</strong>
   </td>
   <td><strong>Berechtigungen anzeigen</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Erstellen</strong>
   </td>
   <td rowspan="5" ><strong>Arbeitsbereich</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Löschen</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Freigeben</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Bearbeiten</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Erstellen/Löschen</strong>
   </td>
   <td rowspan="3" ><strong>Record Type*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Bearbeiten</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <td><strong>Erstellen/Löschen</strong>
   </td>
   <td rowspan="3" ><strong>Datensatz*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Bearbeiten</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Erstellen</strong>
   </td>
   <td rowspan="5" ><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Löschen</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Freigeben</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Bearbeiten</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>✓
   </td>
  </tr>

<tr>
   <td><strong>Erstellen/Löschen</strong>
   </td>
   <td rowspan="3" ><strong>Felder*</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Bearbeiten</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td><strong>Ansicht</strong>
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
   <td>✓
   </td>
  </tr>



</table>

*Record Types, records and fields erben Berechtigungen aus dem Workspace.

Allgemeine Informationen zum Zugriff auf Maestro finden Sie unter [Übersicht über die Freigabe von Berechtigungen in Adobe Maestro](../access/sharing-permissions-overview.md).

Informationen zum Freigeben von Arbeitsbereichen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/maestro/access/share-workspaces.md).

Informationen zum Freigeben von Ansichten finden Sie unter [Anzeigen freigeben](/help/quicksilver/maestro/access/share-views.md)

