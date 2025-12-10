---
title: Erstellen von Workspace-Hierarchien
description: Als Workspace-Manager können Sie in Adobe Workfront Planning mehrere Workspace-Hierarchien zwischen den Datensatztypen erstellen. Nachdem Sie Datensatztypen in einem Arbeitsbereich verbunden und eine Hierarchie erstellt haben, werden Datensatztypen miteinander verbunden, wobei ein Datensatztyp als übergeordneter Datensatz und bis zu 6 andere Datensatztypen als untergeordnete Datensätze konfiguriert sind.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Workspace-Hierarchien erstellen

Als Workspace-Manager können Sie in Adobe Workfront Planning mehrere Workspace-Hierarchien zwischen den Datensatztypen erstellen.

Nachdem Sie Datensatztypen in einem Arbeitsbereich verbunden und eine Hierarchie erstellt haben, werden Datensatztypen miteinander verbunden, wobei ein Datensatztyp als übergeordneter Datensatz und bis zu 6 andere Datensatztypen als untergeordnete Datensätze konfiguriert sind. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

Hierarchien generieren Breadcrumbs für die Datensatztypen und Datensätze, <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> in ihren Kopfzeilen angezeigt werden. Auf diese Weise wissen die Benutzer in jeder Phase ihres Workflows, wo sie sich in der Hierarchie befinden.

Allgemeine Informationen zu Hierarchien und Breadcrumbs finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Zugriffsanforderungen

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

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
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
ODER
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
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Workspace-Hierarchie erstellen

{#step1-to-planning}

1. Klicken Sie auf eine Workspace-Karte.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Workspace-Namen und klicken Sie dann auf **Einstellungen**.
Der **Hierarchien** Abschnitt wird standardmäßig geöffnet.
1. Klicken Sie **Neue**) in der oberen rechten Ecke der Seite **Hierarchien**.
1. Klicken Sie **Objekt hinzufügen** und wählen Sie ein Objekt aus dem Dropdown-Menü aus. Dies wird das übergeordnete Objekt in Ihrer Hierarchie sein.
Sie können einen Datensatztyp aus dem aktuellen Arbeitsbereich oder ein Projekt aus Workfront auswählen.
1. Klicken Sie **Objekt hinzufügen**, um ein zweites Objekt hinzuzufügen, das das erste untergeordnete Objekt in Ihrer Hierarchie ist, und wählen Sie dann im Dropdown-Menü ein anderes Objekt aus.
   ![Neues Hierarchiefeld ohne Feld ausgewählt](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Klicken Sie **Verbundenes Feld auswählen**, um anzugeben, welches Feld die beiden Objekte verbindet.
1. (Bedingt) Wenn ein verbundenes Feld zwischen den beiden Objekttypen vorhanden ist, wählen Sie es aus der Liste aus. Klicken Sie andernfalls auf **Neue Verbindung hinzufügen**.

   >[!WARNING]
   >
   >Wenn das **entsprechendes Feld für verknüpften Datensatztyp erstellen** beim Erstellen des verbundenen Felds nicht ausgewählt wurde, müssen Sie das Feld zuerst bearbeiten, bevor Sie fortfahren können.

1. (Bedingt) Wenn Sie eine neue Verbindung hinzufügen, gehen Sie wie folgt vor:

   1. Fügen Sie dem Feld „Name“ einen Namen für **verbundene Feld**.
   1. Wählen Sie aus den folgenden Verbindungstypen aus:

      * **Viele zu viele**
      * **Eins zu viele**
      * **Viele zu eins**
      * **Eins zu eins**
   1. Bitte eine der folgenden Arten von Darstellungen von Datensätzen auswählen:

      * **Name und Bild**
      * **Name**
      * **image**
Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   1. Klicken Sie auf **Speichern**.
1. (Optional) Fügen Sie Ihren Hierarchien wie oben beschrieben bis zu 4 Objekttypen hinzu. Sie können zuerst alle Objekttypen hinzufügen und dann die Verbindungsfelder zwischen ihnen hinzufügen.
1. (Optional) Klicken Sie auf das **Entfernen**-Symbol ![Entfernen](assets/minus-icon.png), um eine Verbindung zu entfernen.
1. Klicken Sie auf **Speichern**, um Ihre Hierarchie zu speichern.

   >[!TIP]
   >
   >Die **Speichern**-Schaltfläche ist abgeblendet, wenn nicht alle verbundenen Felder vorhanden sind.

   Folgendes geschieht:

   * Die Hierarchie wird zum Abschnitt **Hierarchien** des Arbeitsbereichs hinzugefügt.
   * Die Datensätze, die die Verbindungsfelder ausfüllen, zeigen alle Verbindungen in ihren Breadcrumbs an, wenn Sie zur Seite eines Datensatzes gehen.
1. (Optional) Bewegen Sie den Mauszeiger über eine Hierarchie und klicken Sie dann auf das **Mehr**-Menü und dann auf eine der folgenden Aktionen:

   * **Bearbeiten**: Dadurch wird das Feld &quot;**bearbeiten** geöffnet, in dem Sie Änderungen vornehmen können.
   * **Löschen**: Dadurch wird die Hierarchie dauerhaft gelöscht. Gelöschte Hierarchien können nicht wiederhergestellt werden. Verbindungsfelder werden nicht gelöscht.





