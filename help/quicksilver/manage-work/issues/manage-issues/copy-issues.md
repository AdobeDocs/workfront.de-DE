---
product-area: projects
navigation-topic: manage-issues
title: Probleme kopieren
description: Sie können ein Problem oder eine Anfrage kopieren und im selben oder einem anderen Projekt speichern. Sie können ein Problem auch von einer Aufgabe in ein anderes Projekt kopieren.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Probleme kopieren

<!--Audited: 08/2025-->

Sie können ein Problem oder eine Anfrage kopieren und im selben oder einem anderen Projekt speichern. Sie können ein Problem auch von einer Aufgabe in ein anderes Projekt kopieren.

Sie können Probleme aus den folgenden Objekten kopieren:

* Aus einem Projekt in dasselbe Projekt (duplizieren Sie es im selben Projekt)
* Von einer Aufgabe an dieselbe Aufgabe (doppelt vorhanden bei derselben Aufgabe)
* Von einem Projekt zu einem anderen Projekt
* Von einer Aufgabe zu einem Projekt

>[!TIP]
>
>„Probleme“ und „Anfragen“ werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um unvorhergesehene Arbeiten anzuzeigen, die bearbeitet werden müssen. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anfrage-Warteschlange bezeichnet wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <ul><li><p>Mitwirkender oder höher</p> </li>
   <li><p>Leichte oder höhere Lizenz zum Kopieren eines Problems im Abschnitt „Probleme“ eines Projekts</p></li></ul>
   Oder
   <ul><li><p>Antragsteller oder höher</p> </li>
   <li><p>Reviewer oder höhere Lizenz zum Kopieren eines Problems im Abschnitt „Probleme“ eines Projekts</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Anzeigen oder Hochladen des Zugriffs auf Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> <p>Tragen Sie Berechtigungen für das Element bei, in das Sie das Problem kopieren, mit der Möglichkeit, Probleme hinzuzufügen.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to copy an issue in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are copying the issue to with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen beim Kopieren von Problemen

### Allgemeine Überlegungen beim Kopieren von Problemen

Sie haben die Möglichkeit, während des Kopiervorgangs einige mit dem Problem verknüpfte Elemente in das kopierte Problem zu kopieren. Einige Elemente werden jedoch standardmäßig auf das neue Problem übertragen, andere nicht, wie in den folgenden Listen beschrieben.

Die folgenden Elemente werden standardmäßig in die neue Anfrage kopiert:

* Hauptansprechpartner
* Benutzerdefinierte Formulare. Die Informationen in den benutzerdefinierten Feldern werden nur dann in das neue Problem kopiert, wenn Sie beim Kopieren „Benutzerdefinierte Daten“ auswählen.
* Genehmigungen
* Geplanter Start und geplante Abschlussdaten

Die folgenden Objekte werden standardmäßig nicht in das neue Problem kopiert:

* Protokollierte Stunden

### Überlegungen zu Problemen im Zusammenhang mit Dokumenten oder Anfrage-Warteschlangen

Beachten Sie beim Kopieren von Problemen, die Dokumente enthalten oder mit einer Anfrage-Warteschlange verbunden sind, Folgendes:

* **Wenn ein Problem mit einer Anfrage-Warteschlange verknüpft ist:** Wenn Sie ein Problem in ein anderes Objekt kopieren und das Problem mit einer Anfrage-Warteschlange verknüpft ist, ist das kopierte Problem nicht mehr mit der ursprünglichen Warteschlange verknüpft, von der das erste Problem stammt.
* **Wenn ein Dokument an das Problem angehängt wird:** Wenn Sie ein Problem in ein anderes Objekt kopieren und dem Problem ein Dokument angehängt ist, werden das Dokument und seine Versionen ebenfalls an das neue Problem angehängt. Korrekturabzüge oder Genehmigungen, die mit dem Dokument verknüpft sind, werden nicht verschoben.
* **Wenn ein Problem mit einem Dokument oder Ordner verknüpft ist:** Wenn Sie ein Problem kopieren, das Dokumente oder Ordner mit einem Drittanbieterdienst wie Google Drive verknüpft hat, werden die Links zu den Dokumenten auf das kopierte Problem übertragen.

## Probleme in eine Liste kopieren

Sie können ein oder mehrere Probleme aus einer Problemliste oder aus einem Problembericht kopieren.

1. Wechseln Sie zu dem Projekt, das das Problem oder die Probleme enthält, die Sie kopieren möchten.

   Oder

   Zu einem Problembericht gehen.

1. Wenn Sie sich für ein Projekt entschieden haben, klicken Sie im **Bereich auf** Probleme“.
1. Wählen Sie das oder die zu kopierenden Probleme aus und klicken Sie oben in der Problemliste auf **Mehr** und dann auf **Kopieren nach**.

   ![Problem in Liste kopieren](assets/copy-issue-in-list-nwe-350x169.png)

1. Fahren Sie mit dem Kopieren des Problems fort, wie im Abschnitt [Kopieren eines einzelnen Problems](#copy-a-single-issue) beschrieben, beginnend mit Schritt 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Einzelnes Problem kopieren {#copy-a-single-issue}

Sie können ein Problem kopieren, wenn Sie es anzeigen.

1. Gehen Sie zu einem Problem, das Sie kopieren möchten, und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-icon.png) rechts neben dem Problemnamen und dann **Kopieren nach**.

   ![Kopie auf Anfrageebene](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   Das **Problem kopieren** wird angezeigt.

   ![Problemfeld kopieren](assets/copy-issue-box-nwe-350x285.png)

1. Geben **im Abschnitt „Zielprojekt auswählen** den Namen des Projekts an, in das Sie die Probleme kopieren möchten. Der Name des aktuellen Projekts wird standardmäßig angezeigt.

   >[!TIP]
   >
   >In der Liste werden nur 100 Projekte angezeigt.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** wenn Sie keinen Zugriff haben, um Probleme in das Projekt zu kopieren.
1. (Bedingt) Kopieren Sie das Problem weiterhin in das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff zum Hinzufügen von Problemen zu einer der Aufgaben im Zielprojekt haben.

   ![Problem kopieren und Zugriff anfordern](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt ausstehend, genehmigt, abgeschlossen oder eingestellt ist und der Workfront-Administrator das Hinzufügen von Problemen zu diesen Projekten verhindert. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) Heben Sie im **Optionen** die Auswahl eines der in der folgenden Tabelle aufgelisteten Elemente auf, um sie aus dem neuen Problem zu entfernen. Alle Optionen sind standardmäßig ausgewählt.

   >[!NOTE]
   >
   >Dies betrifft nur die kopierten Probleme, nicht aber die ursprünglichen Probleme.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td>Entfernt Benutzende, Aufgabengebiete oder Teams, die dem Problem zugewiesen sind.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Entfernt den Prozentwert der Fertigstellung (falls vorhanden) des Problems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td><span style="line-height: 1.5;">Entfernt alle Elemente auf der Registerkarte „Dokumente“, einschließlich Dokumentversionen, verknüpfter Dokumente und Ordner.</span> <br>Standardmäßig können Korrekturabzüge und Genehmigungen nicht in ein anderes Problem kopiert werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td>Entfernt die Entitäten, für die das Problem freigegeben ist. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Entfernt Kommentare aus dem Abschnitt „Aktualisierungen“ des Problems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td>Entfernt die Informationen zum Problem aus dem benutzerdefinierten Formular sowie die Informationen zu den benutzerdefinierten Formularen, die mit den an das Problem angehängten Dokumenten verknüpft sind, wenn diese ebenfalls mit dem Problem kopiert werden. Die benutzerdefinierten Formulare bleiben an die Probleme und Dokumente angehängt, die Informationen auf den Formularen werden jedoch nicht auf das neue Problem übertragen. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen Sie im **Aufgabe auswählen** die Aufgabe aus, in die Sie das Problem verschieben möchten.
1. Klicken Sie auf **Problem kopieren** oder **Probleme kopieren**, wenn Sie mehrere Probleme in einer Liste ausgewählt haben.

   Die kopierten Probleme werden dem angegebenen Projekt hinzugefügt.


