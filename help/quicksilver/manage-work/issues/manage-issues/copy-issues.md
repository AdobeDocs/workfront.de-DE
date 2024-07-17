---
product-area: projects
navigation-topic: manage-issues
title: Probleme kopieren
description: Sie können ein Problem oder eine Anfrage kopieren und im selben oder in einem anderen Projekt speichern. Sie können ein Problem auch von einer Aufgabe in ein anderes Projekt kopieren.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 1%

---

# Probleme kopieren

Sie können ein Problem oder eine Anfrage kopieren und im selben oder in einem anderen Projekt speichern. Sie können ein Problem auch von einer Aufgabe in ein anderes Projekt kopieren.

Sie können Probleme aus den folgenden Objekten kopieren:

* Von einem Projekt zum selben Projekt (duplizieren Sie es auf demselben Projekt)
* Von einer Aufgabe zur selben Aufgabe (Duplizieren, wenn für dieselbe Aufgabe)
* Von einem Projekt zu einem anderen Projekt
* Von einer Aufgabe zu einem Projekt

>[!TIP]
>
>&quot;Probleme&quot;und &quot;Anforderungen&quot;werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um auf unvorhergesehene Arbeit hinzuweisen, die behoben werden muss. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anforderungswarteschlange bezeichnet wird.

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
   <td> <p>Anforderung oder höher</p> <p>Überprüfen Sie oder eine höhere Lizenz, um ein Problem im Abschnitt Probleme eines Projekts zu kopieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsstufe*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem verwalten</p> <p>Contribute-Berechtigungen für das Element, in das Sie das Problem kopieren, mit der Möglichkeit, Probleme hinzuzufügen.</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Kopieren von Problemen

### Allgemeine Überlegungen zum Kopieren von Problemen

Sie haben die Möglichkeit, beim Kopieren einige mit dem Problem verknüpfte Elemente in das kopierte Problem zu kopieren. Einige Elemente werden jedoch standardmäßig an das neue Problem übertragen, andere nicht, wie in den folgenden Listen beschrieben.

Die folgenden Elemente werden standardmäßig in das neue Problem kopiert:

* Hauptansprechpartner
* Benutzerdefinierte Formulare. Die Informationen in den benutzerdefinierten Feldern werden nur dann in das neue Problem kopiert, wenn Sie im Kopiervorgang Benutzerdefinierte Daten auswählen.
* Genehmigungen
* Geplante Start- und geplante Abschlussdaten

Die folgenden Objekte werden standardmäßig nicht in das neue Problem kopiert:

* Protokollierte Stunden

### Überlegungen zu Problemen im Zusammenhang mit Dokumenten oder Anforderungswarteschlangen

Beachten Sie beim Kopieren von Problemen, die Dokumente enthalten oder mit einer Anforderungswarteschlange verknüpft sind, Folgendes:

* **Wenn ein Problem mit einer Anforderungswarteschlange verknüpft ist:** Wenn Sie ein Problem in ein anderes Objekt kopieren und das Problem mit einer Anforderungswarteschlange verknüpft ist, wird das kopierte Problem nicht mehr mit der ursprünglichen Warteschlange verknüpft, aus der das erste Problem stammt.
* **Wenn ein Dokument an das Problem angehängt ist:** Wenn Sie ein Problem in ein anderes Objekt kopieren und an das Problem ein Dokument angehängt ist, werden das Dokument und seine Versionen ebenfalls zum neuen Problem verschoben. Testsendungen oder Genehmigungen, die mit dem Dokument verknüpft sind, werden nicht verschoben.
* **Wenn ein Problem mit einem Dokument oder Ordner verknüpft ist:** Wenn Sie ein Problem kopieren, bei dem Dokumente oder Ordner mit einem Drittanbieterdienst wie Google Drive verknüpft sind, werden die Links zu den Dokumenten an das kopierte Problem weitergeleitet.

## Probleme in eine Liste kopieren

Sie können ein oder mehrere Probleme aus einer Liste von Problemen oder aus einem Problembericht kopieren.

1. Wechseln Sie zu dem Projekt, das das Problem oder die Probleme enthält, die Sie kopieren möchten.

   Oder

   Gehen Sie zu einem Problembericht.

1. Wenn Sie ausgewählt haben, dass ein Projekt aufgerufen werden soll, klicken Sie im linken Bereich auf **Probleme** .
1. Wählen Sie das Problem bzw. die Probleme aus, die Sie kopieren möchten, und klicken Sie oben in der Liste auf das Menü **Mehr** und dann auf **Kopieren nach**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. Fahren Sie mit dem Kopieren des Problems fort, wie im Abschnitt [Kopieren eines einzelnen Problems](#copy-a-single-issue) beschrieben, beginnend mit Schritt 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Ein einzelnes Problem kopieren {#copy-a-single-issue}

Sie können ein Problem kopieren, wenn Sie es anzeigen.

1. Gehen Sie zu einem Problem, das Sie kopieren möchten, und klicken Sie dann auf das Menü **Mehr** ![](assets/more-icon.png) rechts neben dem Namen des Problems und dann auf **Kopieren** nach.

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   Das Feld **Problem kopieren** wird angezeigt.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. Geben Sie im Abschnitt **Zielprojekt auswählen** den Namen des Projekts an, in das Sie die Probleme kopieren möchten. Der Name des aktuellen Projekts wird standardmäßig angezeigt.

   >[!TIP]
   >
   >In der Liste werden nur 100 Projekte angezeigt.

1. (Bedingt) Klicken Sie auf **Zugriffsanfrage anfordern** , wenn Sie keinen Zugriff auf das Kopieren von Problemen in das Projekt haben.
1. (Bedingt) Kopieren Sie das Problem weiterhin in das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Probleme zu einer der Aufgaben im Zielprojekt hinzuzufügen.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt noch nicht genehmigt, abgeschlossen oder deaktiviert ist, wenn der Workfront-Administrator verhindert, dass Probleme zu diesen Projekten hinzugefügt werden. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) Heben Sie im Abschnitt **Optionen** die Auswahl eines der in der folgenden Tabelle aufgeführten Elemente auf, um sie aus dem neuen Problem zu entfernen. Alle Optionen sind standardmäßig ausgewählt.

   >[!NOTE]
   >
   >Dies betrifft nur die kopierten Probleme, nicht die ursprünglichen Probleme.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td>Entfernt Benutzer, Auftrags-Rollen oder Teams, die dem Problem zugewiesen sind.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Entfernt ggf. den prozentualen Abschluss des Problems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td><span style="line-height: 1.5;">Entfernt alle Elemente auf der Registerkarte "Dokumente", einschließlich Dokumentversionen, verknüpften Dokumenten und Ordnern.</span> <br> Standardmäßig können Dokumentsendungen und -genehmigungen nicht in ein anderes Problem kopiert werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td>Entfernt die Entitäten, für die das Problem freigegeben ist. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Entfernt Kommentare aus dem Abschnitt Aktualisierungen des Problems.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td>Entfernt die Informationen zum Problem aus dem benutzerdefinierten Formular sowie die Informationen zu den benutzerdefinierten Formularen, die mit Dokumenten verknüpft sind, die mit dem Problem verknüpft sind, sofern diese ebenfalls mit dem Problem kopiert werden. Die benutzerdefinierten Formulare bleiben an die Probleme und Dokumente angehängt, die Informationen auf den Formularen werden jedoch nicht in die neue Ausgabe übernommen. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen Sie im Abschnitt **Aufgabe auswählen** die Aufgabe aus, in die Sie das Problem verschieben möchten.
1. Klicken Sie auf **Problem kopieren** oder auf **Probleme kopieren** , wenn Sie mehrere Probleme in einer Liste ausgewählt haben.

   Die kopierten Probleme werden dem angegebenen Projekt hinzugefügt.


