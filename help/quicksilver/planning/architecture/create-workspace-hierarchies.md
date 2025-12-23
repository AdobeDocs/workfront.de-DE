---
title: Erstellen von Workspace-Hierarchien
description: Als Workspace-Manager können Sie in Adobe Workfront Planning mehrere Workspace-Hierarchien zwischen den Datensatztypen erstellen. Nachdem Sie Datensatztypen in einem Arbeitsbereich verbunden und eine Hierarchie erstellt haben, werden Datensatztypen miteinander verbunden, wobei ein Datensatztyp als übergeordneter Datensatz und bis zu drei andere Datensatztypen als untergeordnete Datensätze konfiguriert sind.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 34921b12ad902ba7390e4ea34825331280e7a8d6
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---


# Workspace-Hierarchien erstellen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie in Adobe Workfront Planning mehrere Workspace-Hierarchien zwischen Datensatztypen erstellen.

Nachdem Datensatztypen in einem Arbeitsbereich verbunden sind, können Sie eine Hierarchie erstellen, die diese Verbindungen organisiert. Hierarchien organisieren Datensatz- und Objekttypen in hierarchischen Beziehungen und können bis zu vier Ebenen von Objekttypen enthalten.

Wenn noch keine Verbindung zwischen zwei Datensatztypen besteht, kann sie beim Einrichten der Hierarchie erstellt werden. Nach der Definition richtet die Hierarchie einen strukturierten Pfad über verwandte Datensatztypen hinweg im Arbeitsbereich ein.

Hierarchien generieren Breadcrumbs für die jeweiligen Datensätze, die in ihren Kopfzeilen angezeigt werden. Auf diese Weise wissen die Benutzer in jeder Phase ihres Workflows, wo sie sich in der Hierarchie befinden.

Allgemeine Informationen zu Hierarchien und Breadcrumbs finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

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

Sie können bis zu 5 Hierarchien in einem Arbeitsbereich erstellen.

{#step1-to-planning}

1. Klicken Sie auf eine Workspace-Karte.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Workspace-Namen und klicken Sie dann auf **Einstellungen**.
Der **Hierarchien** Abschnitt wird standardmäßig geöffnet.
1. Klicken Sie **Neue**) in der oberen rechten Ecke der Seite **Hierarchien**.
1. Klicken Sie **Objekt hinzufügen** und wählen Sie im Dropdown-Menü einen Objekttyp aus. Dies wird der erste Objekttyp in Ihrer Hierarchie sein. <!--logged bug to correct to "Add object type"-->

   Der erste Objekttyp kann nur ein Planungs-Datensatztyp sein.

   Workfront-Projekte können nicht als übergeordnete Elemente anderer Objekttypen in einer Hierarchie ausgewählt werden.

1. Klicken Sie **Objekt hinzufügen**, um einen zweiten Objekttyp hinzuzufügen, der das erste untergeordnete Element in Ihrer Hierarchie ist, und wählen Sie dann im Dropdown-Menü einen anderen Objekttyp aus.
Alle zusätzlichen Objekttypen werden zu untergeordneten Objekten der vorherigen Objekttypen.

   ![Neues Hierarchiefeld ohne Feld ausgewählt](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Klicken Sie **Verbundenes Feld auswählen**, um anzugeben, welches Feld die beiden Objekte verbindet.
1. (Bedingt) Wenn mehrere Verbindungsfelder vorhanden sind, wählen Sie eines aus der Liste aus.

   ODER

   Klicken Sie **Neue Verbindung hinzufügen**, um ein neues Verbindungsfeld hinzuzufügen.

   Dadurch wird ein Verbindungsfeld aus dem Datensatztyp erstellt, den Sie als übergeordnetes Element verwenden, und ein entsprechendes Verbindungsfeld zu ihm aus dem Datensatztyp, den Sie als untergeordnetes Element verwenden.

   Wenn Sie eine Verbindung zu Workfront-Projekten herstellen, wird kein Feld im Projekt erstellt.

1. (Bedingt) Wenn keine verbundenen Felder verfügbar sind, klicken Sie auf **Verbindung erstellen** und fügen Sie eine neue Verbindung hinzu. Klicken Sie dann auf **Speichern**.

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
      * **Bild**

      Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Klicken Sie auf **Speichern**.

1. (Bedingt) Wenn das Feld **Entsprechendes Feld für verknüpften Datensatztyp erstellen** beim Erstellen des verbundenen Felds nicht ausgewählt wurde, wird ein Fehler angezeigt und Sie müssen zunächst Folgendes tun: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Klicken Sie **&#x200B;**&#x200B;Feld **Neue Hierarchie** auf „Abbrechen“.
   1. Klicken Sie links neben dem Arbeitsbereichsnamen auf den Rückwärtspfeil und dann auf die Karte des Datensatztyps, den Sie als übergeordneten Datensatz auswählen möchten.
   1. Öffnen Sie die Tabellenansicht des Datensatztyps, den Sie im obigen Schritt ausgewählt haben, wechseln Sie dann zum Verbindungsfeld mit dem Objekttyp, den Sie als untergeordnetes Element verwenden möchten, bewegen Sie den Mauszeiger über die Spaltenüberschrift und klicken Sie dann auf **Bearbeiten** Feld.
   1. Aktivieren Sie die Einstellung **entsprechendes Feld für verknüpften Datensatztyp erstellen** und klicken Sie dann auf **Speichern**.
   1. Kehren Sie zum Bereich **Einstellungen“ des Arbeitsbereichs zurück** klicken Sie erneut auf **Neue**) und führen Sie dann die Schritte zum Erstellen einer Hierarchie aus.

1. (Optional) Fügen Sie Ihren Hierarchien wie oben beschrieben bis zu 4 Objekttypen hinzu. Sie können zuerst alle Objekttypen hinzufügen und dann die Verbindungsfelder zwischen ihnen hinzufügen.
1. (Optional) Klicken Sie auf das **Entfernen**-Symbol ![Entfernen](assets/minus-icon.png), um eine Verbindung zu entfernen.
1. Klicken Sie auf **Speichern**, um Ihre Hierarchie zu speichern.

   >[!TIP]
   >
   >Die **Speichern**-Schaltfläche ist abgeblendet, wenn nicht alle verbundenen Felder vorhanden sind.

   Folgendes geschieht:

   * Die Hierarchie wird zum Abschnitt **Hierarchien** des Arbeitsbereichs hinzugefügt.
   * Die Datensätze, die die Verbindungsfelder ausfüllen, zeigen alle Verbindungen in ihren Breadcrumbs an, wenn Sie zur Seite eines Datensatzes gehen.

   >[!NOTE]
   >
   >Sie können einen Datensatz eines untergeordneten Datensatztyps mit bis zu 10 Datensätzen eines übergeordneten Datensatztyps verbinden.
   >
   >Weitere Informationen finden Sie unter [Hierarchie und Breadcrumb - Übersicht](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Hierarchie und klicken Sie dann auf das Menü **Mehr**.

   ![Hierarchie Mehr Menü erweitert](assets/hierarchy-more-menu-expanded.png)

1. Klicken Sie auf eine der folgenden Optionen:

   * **Bearbeiten**: Dadurch wird das Feld &quot;**bearbeiten** geöffnet, in dem Sie Änderungen vornehmen können.
   * **Löschen**: Dadurch wird die Hierarchie dauerhaft gelöscht. Gelöschte Hierarchien können nicht wiederhergestellt werden. Verbindungsfelder werden nicht gelöscht.





