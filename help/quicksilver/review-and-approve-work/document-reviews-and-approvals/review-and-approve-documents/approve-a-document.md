---
product-area: projects
navigation-topic: approvals
title: Dokument genehmigen
description: Wenn Sie als Genehmiger für ein Dokument zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.
author: Nolan
feature: Work Management
source-git-commit: 369a8564f44524d1abed57553435ce69c7c5e170
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# Dokument genehmigen

Wenn Sie als Genehmiger für ein Dokument zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.

Informationen zum Erstellen einer neuen Dokumentgenehmigung finden Sie unter [Dokumentgenehmigung erstellen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf die aktualisierte Funktion zur Dokumentgenehmigung, die nur für bestimmte Konten verfügbar ist. Informationen zu Standardgenehmigungsverfahren finden Sie in den Artikeln unter [Arbeitsgenehmigungen](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
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
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verknüpft sind</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Dokument von der Startseite aus genehmigen

1. Klicken Sie auf **Startseite** icon ![](../assets/home-icon-30x29.png) in der linken oberen Ecke von Adobe Workfront.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann die folgenden Änderungen am Startseiten-Symbol in Ihrer Umgebung vornehmen:
   >
   >* Ersetzen Sie sie durch ein Bild, das zur Veranschaulichung Ihrer Organisation angepasst wurde. In diesem Fall sieht das Symbol anders aus als in diesem Artikel.
   >
   >* Ersetzen Sie die verknüpfte Seite durch eine andere Seite. Klicken Sie in diesem Fall auf die **Hauptmenü** ![](../assets/main-menu-icon.png) in der rechten oberen Ecke der Seite klicken Sie auf **Startseite**.


1. Klicken **Filter** oben links auf der Seite und stellen Sie sicher, dass **Genehmigungen** aktiviert ist.

   Alle Arbeitselemente, für die eine Genehmigung erforderlich ist, werden in der Liste angezeigt.

   >[!NOTE]
   >
   >Genehmigungen, die Auftrags-Rollen oder Gruppen zugewiesen sind, werden nicht auf der Startseite angezeigt. Für Teams zugewiesene Validierungen werden in der Gruppe Teamanfrage in der Arbeitsliste angezeigt.

1. Klicken Sie in der Liste, für die Sie eine Validierungsentscheidung treffen möchten, auf die Validierung des Dokuments. Informationen zur Validierung werden rechts auf der Seite angezeigt.

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Die **Genehmigen** Das Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Dokumentversion keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** weist darauf hin, dass noch einige kleine Änderungen am Dokument erforderlich sind, jedoch unter der Bedingung genehmigt werden, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** wo Sie angeben können, welche Änderungen für die Genehmigung des Dokuments erforderlich sind. Sie können diese Informationen eingeben und auf **Nachricht hinzufügen** oder klicken Sie auf **Überspringen** die Validierungsentscheidung ohne zusätzliche Informationen zu übermitteln.
   * **Arbeiten erforderlich** gibt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.

   Beachten Sie Folgendes bei der Anzeige von Dokumentgenehmigungen auf der Startseite:

   * Der Name des Benutzers, der die Genehmigung angefordert hat, wird über dem Dokumentnamen in Startseite mit dem Text &quot;*Benutzer A* Ihre Zustimmung möchten Sie bitte an...&quot; sowie unter **Gesendet von** in den Validierungsinformationen, die nach Auswahl einer Validierung rechts angezeigt werden.

   * Nachdem eine Entscheidung über eine Genehmigung getroffen wurde, bleibt die Genehmigung im Tab Meine Genehmigungen mit dem Text &quot;Entscheidung getroffen&quot;, bis Sie auf die Schaltfläche **Aktualisieren** oder bis Sie die Browserseite aktualisieren.



## Dokument auf der Dokumentseite genehmigen

1. Klicken Sie auf den Namen des Dokuments, um zur Dokumentseite zu gelangen.

1. Wählen Sie im Dropdown-Menü Version neben dem Dokumentnamen die Version des Dokuments aus, für das die Genehmigung aussteht. Standardmäßig wird die neueste Version ausgewählt.

   Wenn die aktuell ausgewählte Version des Dokuments eine ausstehende Genehmigung für Sie hat, werden die Schaltflächen für die Validierungsentscheidung oben rechts auf der Seite angezeigt. Wenn andere Versionen des Dokuments noch ausstehende Genehmigungen für Sie haben, wird im Dropdown-Menü &quot;Version&quot;ein roter Punkt angezeigt.
   <!--
   ![](../assets/version-dropdown-red-dot.png)   
   -->

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Die **Genehmigen** Das Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Dokumentversion keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** weist darauf hin, dass noch einige kleine Änderungen am Dokument erforderlich sind, jedoch unter der Bedingung genehmigt werden, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** wo Sie angeben können, welche Änderungen für die Genehmigung des Dokuments erforderlich sind. Sie können diese Informationen eingeben und auf **Nachricht hinzufügen** oder klicken Sie auf **Überspringen** die Validierungsentscheidung ohne zusätzliche Informationen zu übermitteln.
   * **Arbeiten erforderlich** gibt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.


## Genehmigen eines Dokuments im Bereich &quot;Dokumentzusammenfassung&quot;

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das Dokument, das Ihre Genehmigung benötigt, und der Bereich Dokumentzusammenfassung wird geöffnet.

1. Wählen Sie die Version des Dokuments aus, das Sie im Dropdown-Menü Version überprüfen möchten. Standardmäßig wird die neueste Version ausgewählt.

   Wenn die aktuell ausgewählte Version des Dokuments eine ausstehende Genehmigung für Sie hat, werden die Schaltflächen für die Validierungsentscheidung in der oberen rechten Ecke des Bereichs Dokumentzusammenfassung angezeigt. Wenn andere Versionen des Dokuments noch ausstehende Genehmigungen für Sie haben, wird im Dropdown-Menü &quot;Version&quot;ein roter Punkt angezeigt.
   <!--
   ![](../assets/version-dropdown-red-dot.png)   
   -->

1. Klicken Sie in der oberen rechten Ecke des Bereichs Dokumentzusammenfassung auf eine der folgenden beiden Genehmigungsoptionen:

   * Die **Genehmigen** Das Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Dokumentversion keine Änderungen erforderlich sind und dass die Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** weist darauf hin, dass noch einige kleine Änderungen am Dokument erforderlich sind, jedoch unter der Bedingung genehmigt werden, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option auswählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** wo Sie angeben können, welche Änderungen für die Genehmigung des Dokuments erforderlich sind. Sie können diese Informationen eingeben und auf **Nachricht hinzufügen** oder klicken Sie auf **Überspringen** die Validierungsentscheidung ohne zusätzliche Informationen zu übermitteln.
   * **Arbeiten erforderlich** gibt an, dass die Dokumentversion nicht genehmigt ist und erhebliche Änderungen erforderlich sind.