---
product-area: projects
navigation-topic: approvals
title: Dokument in Workfront genehmigen
description: Wenn Sie als Genehmiger für ein Dokument zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 3755eb0d384e7274b88fbeafc2affa85f735efbc
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# Dokument in Workfront genehmigen

Wenn Sie als Genehmiger für ein Dokument zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.

Weitere Informationen zum Erstellen einer neuen Dokumentgenehmigung finden Sie unter [Erstellen einer Dokumentüberprüfung oder einer Genehmigungsanforderung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf die aktualisierte Funktion zur Dokumentgenehmigung, die nur für bestimmte Konten verfügbar ist. Informationen zu Standardgenehmigungsverfahren finden Sie in den Artikeln unter [Arbeitsgenehmigungen](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Objekte, die Genehmigungen zugeordnet sind, anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verknüpft sind</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Dokument von der Startseite aus genehmigen

1. Klicken Sie oben links in Adobe Workfront auf das Symbol **Startseite** ![](../assets/home-icon-30x29.png) .

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann die folgenden Änderungen am Startseiten-Symbol in Ihrer Umgebung vornehmen:
   >
   >* Ersetzen Sie sie durch ein Bild, das zur Veranschaulichung Ihrer Organisation angepasst wurde. In diesem Fall sieht das Symbol anders aus als in diesem Artikel.
   >
   >* Ersetzen Sie die verknüpfte Seite durch eine andere Seite. Klicken Sie in diesem Fall auf das **Hauptmenü** ![](../assets/main-menu-icon.png) in der oberen rechten Ecke der Seite und klicken Sie dann auf **Startseite**.

1. Klicken Sie oben links auf der Seite auf **Filter** und stellen Sie sicher, dass **Genehmigungen** aktiviert ist.

   Alle Arbeitselemente, für die eine Genehmigung erforderlich ist, werden in der Liste angezeigt.

   >[!NOTE]
   >
   >Genehmigungen, die Auftrags-Rollen oder Gruppen zugewiesen sind, werden nicht auf der Startseite angezeigt. Für Teams zugewiesene Validierungen werden in der Gruppe Teamanfrage in der Arbeitsliste angezeigt.

1. Klicken Sie in der Liste, für die Sie eine Validierungsentscheidung treffen möchten, auf die Validierung des Dokuments. Informationen zur Validierung werden rechts auf der Seite angezeigt.

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Das Dropdown-Menü **Genehmigen** enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** bedeutet, dass einige kleine Änderungen am Dokument noch erforderlich sind, die Genehmigung jedoch unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit dem Textfeld **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen erforderlich sind, damit das Dokument genehmigt werden kann. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Erforderlich funktioniert** zeigt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.

   Beachten Sie Folgendes bei der Anzeige von Dokumentgenehmigungen auf der Startseite:

   * Der Name des Benutzers, der die Genehmigung angefordert hat, wird über dem Dokumentnamen in der Startseite mit dem Text &quot;*Benutzer A* möchte Ihre Genehmigung für ...&quot;sowie unter &quot;**Gesendet von**&quot;in den Genehmigungsinformationen angezeigt, die rechts angezeigt werden, sobald eine Genehmigung ausgewählt wurde.

   * Nachdem eine Entscheidung über eine Genehmigung getroffen wurde, bleibt die Genehmigung auf der Registerkarte Meine Genehmigungen mit dem Text &quot;Entscheidungsfindung&quot;erhalten, bis Sie auf die Schaltfläche **Aktualisieren** klicken oder bis Sie die Browser-Seite aktualisieren.

## Dokument auf der Dokumentseite genehmigen

1. Klicken Sie auf den Namen des Dokuments, um zur Dokumentseite zu gelangen.

1. Wählen Sie im Dropdown-Menü Version neben dem Dokumentnamen die Version des Dokuments aus, für das die Genehmigung aussteht. Standardmäßig wird die neueste Version ausgewählt.

   Wenn für die aktuell ausgewählte Version des Dokuments eine Genehmigung aussteht, werden die Schaltflächen für die Validierungsentscheidung oben rechts auf der Seite angezeigt. Wenn für andere Versionen des Dokuments ausstehende Genehmigungen vorliegen, wird im Dropdown-Menü für die Version ein roter Punkt angezeigt.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Das Dropdown-Menü **Genehmigen** enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** bedeutet, dass einige kleine Änderungen am Dokument noch erforderlich sind, die Genehmigung jedoch unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit dem Textfeld **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen erforderlich sind, damit das Dokument genehmigt werden kann. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Erforderlich funktioniert** zeigt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.

## Genehmigen eines Dokuments im Bereich Dokumentzusammenfassung

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.

1. Klicken Sie auf das Dokument, das Ihre Genehmigung benötigt, und der Bereich Dokumentzusammenfassung wird geöffnet.

1. Wählen Sie die Version des Dokuments aus, das Sie im Dropdown-Menü Version überprüfen möchten. Standardmäßig wird die neueste Version ausgewählt.

   Wenn die aktuell ausgewählte Version des Dokuments eine ausstehende Genehmigung für Sie hat, werden die Schaltflächen für die Validierungsentscheidung oben rechts im Bereich &quot;Dokumentzusammenfassung&quot;angezeigt. Wenn für andere Versionen des Dokuments ausstehende Genehmigungen vorliegen, wird im Dropdown-Menü für die Version ein roter Punkt angezeigt.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Klicken Sie in der oberen rechten Ecke des Bereichs Dokumentzusammenfassung auf eine der folgenden beiden Genehmigungsoptionen:

   * Das Dropdown-Menü **Genehmigen** enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** bedeutet, dass einige kleine Änderungen am Dokument noch erforderlich sind, die Genehmigung jedoch unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit dem Textfeld **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen erforderlich sind, damit das Dokument genehmigt werden kann. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Erforderlich funktioniert** zeigt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.