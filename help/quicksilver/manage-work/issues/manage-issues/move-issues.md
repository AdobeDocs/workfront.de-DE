---
product-area: projects
navigation-topic: manage-issues
title: Probleme verschieben
description: Sie können Probleme zwischen Projekten und Aufgaben verschieben.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# Probleme verschieben

Sie können Probleme zwischen den folgenden Objekten verschieben:

* Von einem Projekt zu einem anderen Projekt
* Von einer Aufgabe zu einer anderen Aufgabe im selben Projekt oder in einem anderen Projekt
* Von einer Aufgabe zum Projekt oder zu einem anderen Projekt
* Von einem Projekt zu einer Aufgabe im selben Projekt oder einer Aufgabe in einem anderen Projekt

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Überprüfen Sie oder eine höhere Lizenz, um Probleme im Abschnitt Probleme eines Projekts zu verschieben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> <p>Contribute-Berechtigungen für das Element, in das Sie das Problem verschieben und Probleme hinzufügen können.</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Verschieben von Problemen

Beachten Sie Folgendes beim Verschieben von Problemen, die Dokumente enthalten oder mit einer Anforderungswarteschlange verknüpft sind:

* **Wenn ein Problem mit einer Anforderungswarteschlange verknüpft ist:** Wenn Sie ein Problem in ein anderes Objekt verschieben und das Problem mit einer Anforderungswarteschlange verknüpft ist, wird das verschobene Problem nicht mehr mit der ursprünglichen Warteschlange verknüpft, aus der das erste Problem stammt.
* **Wenn ein Dokument an das Problem angehängt ist:** Wenn Sie ein Problem in ein anderes Objekt verschieben und das Problem ein Dokument angehängt hat, werden das Dokument, seine Versionen und Testsendungen ebenfalls an das neue Problem weitergeleitet. Alle mit dem Dokument verknüpften Genehmigungen werden nicht verschoben.
* **Wenn ein Problem mit einem Dokument oder Ordner verknüpft ist:** Wenn Sie ein Problem verschieben, bei dem Dokumente oder Ordner mit einem Drittanbieterdienst wie Google Drive verknüpft sind, werden die Links zu den Dokumenten mit dem Problem verschoben.

## Verschieben von Problemen in eine Liste

Sie können ein oder mehrere Probleme aus einer Liste von Problemen oder aus einem Problembericht verschieben.

1. Wechseln Sie zu dem Projekt, das das Problem oder die Probleme enthält, die Sie verschieben möchten.

   Oder

   Gehen Sie zu einem Problembericht.

1. Wenn Sie ausgewählt haben, dass ein Projekt aufgerufen werden soll, klicken Sie im linken Bereich auf **Probleme** .
1. Wählen Sie das Problem oder die Probleme aus, die Sie verschieben möchten, und klicken Sie oben in der Liste auf das Menü **Mehr** und dann auf **Verschieben nach**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Fahren Sie mit dem Verschieben des Problems fort, wie im Abschnitt [Verschieben eines einzelnen Problems](#move-a-single-issue) beschrieben, beginnend mit Schritt 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Ein einzelnes Problem verschieben {#move-a-single-issue}

Sie können ein Problem bei der Anzeige verschieben.

### Verschieben eines einzelnen Problems in der Vorschau-Umgebung

1. Wechseln Sie zu einem Problem, das Sie kopieren möchten, klicken Sie auf das Menü **Mehr** ![](assets/more-icon.png) rechts neben dem Namen des Problems und wählen Sie dann **Verschieben** nach.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   Das Feld **Problem beim Verschieben** wird angezeigt.

   ![](assets/move-issue-box-nwe-350x280.png)

1. Geben Sie im Abschnitt **Zielprojekt auswählen** den Namen des Projekts an, in das Sie die Probleme verschieben möchten. Der Name des aktuellen Projekts wird standardmäßig angezeigt.

   >[!TIP]
   >
   >In der Liste werden nur 100 Projekte angezeigt.

1. (Bedingt) Klicken Sie auf **Zugriffsanfrage anfordern** , wenn Sie keinen Zugriff zum Verschieben von Problemen in das Projekt haben.
1. (Bedingt) Verschieben Sie das Problem weiterhin auf das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Probleme zu einer der Aufgaben im Zielprojekt hinzuzufügen.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt noch nicht genehmigt, abgeschlossen oder deaktiviert ist, wenn der Workfront-Administrator verhindert, dass Probleme zu diesen Projekten hinzugefügt werden. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) Heben Sie im Abschnitt **Optionen** die Auswahl eines der in der folgenden Tabelle aufgeführten Elemente auf, um sie aus dem verschobenen Problem zu entfernen. Alle Optionen sind standardmäßig ausgewählt.

   >[!IMPORTANT]
   >
   >Wenn Sie Elemente in der Optionsliste deaktivieren, gehen Daten verloren. Informationen aus dem bestehenden Problem werden entfernt und können nicht wiederhergestellt werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus dem Problem zu entfernen, wenn sie an die neue Position verschoben werden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td>Entfernt Benutzer, Auftrags-Rollen oder Teams, die dem Problem zugewiesen sind.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Entfernt ggf. den prozentualen Abschluss des Problems. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Dokumente</p></td> 
      <td> <p>Entfernt alle Elemente auf der Registerkarte "Dokumente", einschließlich Dokumentversionen, verknüpften Dokumenten und Ordnern.

   <b>NOTE</b>

   Wenn Sie sich dafür entscheiden, die Dokumente nicht mit dem Problem zu verschieben, werden die Dokumente gelöscht und 30 Tage lang im Papierkorb abgelegt. Ein Administrator kann sie wiederherstellen und wird beim verschobenen Problem wiederhergestellt.

   Wenn das Problem nach dem Verschieben gelöscht wird, werden die wiederhergestellten Dokumente im Bereich &quot;Dokumente&quot;der Benutzerseite des Administrators platziert, der sie wiederherstellt.
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td>Entfernt die Entitäten, für die das Problem freigegeben ist. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Entfernt Kommentare aus dem Abschnitt Aktualisierungen des Problems.</td> 
     </tr> 
    </tbody> 
   </table>


1. (Optional) Wählen Sie im Abschnitt **Aufgabe auswählen** die Aufgabe aus, in die Sie das Problem verschieben möchten.
1. Klicken Sie auf **Problem verschieben** oder **Probleme beim Verschieben**, wenn Sie mehrere Probleme in einer Liste ausgewählt haben.

   Die verschobenen Probleme werden dem angegebenen Projekt hinzugefügt.




