---
product-area: projects
navigation-topic: approvals
title: Genehmigen eines Dokuments in Workfront
description: Wenn Sie einem Dokument als genehmigende Person zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 7572dd64a7f23d6f8dcae374a327d67f2d6738c5
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Genehmigen eines Dokuments in Workfront

Wenn Sie einem Dokument als genehmigende Person zugewiesen sind, gibt es mehrere Möglichkeiten, Ihre Genehmigungsentscheidung zu treffen.

Weitere Informationen zum Erstellen einer neuen Dokumentgenehmigung finden Sie unter [Erstellen einer Dokumentüberprüfung oder Genehmigungsanfrage](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Der Inhalt dieses Artikels bezieht sich auf aktualisierte Dokumentgenehmigungsfunktionen, die nur für bestimmte Konten verfügbar sind. Informationen zu standardmäßigen Genehmigungsprozessen finden Sie in den Artikeln, die unter [Arbeitsgenehmigungen“ aufgeführt ](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <p>Mitwirkender oder höher</p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Objekte, die mit Genehmigungen verknüpft sind, anzeigen oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verbunden sind</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Genehmigen eines Dokuments von der Startseite aus

1. Klicken Sie auf **Startseite**-Symbol ![Startseite](../assets/home-icon-30x29.png) in der linken oberen Ecke von Adobe Workfront.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann die folgenden Änderungen am Startseiten-Symbol in Ihrer Umgebung vornehmen:
   >
   >* Ersetzen Sie sie durch ein Bild, das Ihre Organisation illustriert. In diesem Fall sieht das Symbol anders aus als in diesem Artikel gezeigt.
   >
   >* Ersetzen Sie die damit verknüpfte Seite durch eine andere Seite. Klicken Sie in diesem Fall auf **Hauptmenü** ![Hauptmenüsymbol](../assets/main-menu-icon.png) in der oberen rechten Ecke der Seite und dann auf **Startseite**.

1. Klicken **oben links auf** Filter“ und stellen Sie sicher, dass **Genehmigungen** aktiviert ist.

   In der Liste werden alle Arbeitselemente angezeigt, die Ihrer Genehmigung bedürfen.

   >[!NOTE]
   >
   >* Genehmigungen, die Aufgabengebieten oder Gruppen zugewiesen wurden, werden nicht auf der Startseite aufgelistet.
   >* Genehmigungen, die Teams zugewiesen wurden, werden auf der Startseite im Widget Meine Genehmigungen jedes einzelnen Teammitglieds angezeigt.

1. Klicken Sie in der Liste, für die Sie eine Genehmigungsentscheidung treffen möchten, auf die Dokumentgenehmigung. Informationen zur Genehmigung werden rechts auf der Seite angezeigt.

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Das **Genehmigen** Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass eine Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** gibt an, dass einige kleine Änderungen am Dokument weiterhin erforderlich sind, aber die Genehmigung unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option wählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen für das zu genehmigende Dokument erforderlich sind. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Muss überarbeitet werden** gibt an, dass die Dokumentversion nicht genehmigt ist und umfangreiche Änderungen erfordert.

   Beachten Sie beim Anzeigen von Dokumentgenehmigungen auf der Startseite Folgendes:

   * Der Name des Benutzers, der die Genehmigung angefordert hat, wird in der Startseite über dem Dokumentnamen mit dem Text &quot;*Benutzer A* möchte Ihre Genehmigung für…“ sowie unter **Gesendet von** in den Genehmigungsinformationen angezeigt, die rechts angezeigt werden, wenn eine Genehmigung ausgewählt wird.

   * Nachdem eine Entscheidung über eine Genehmigung getroffen wurde, bleibt die Genehmigung auf der Registerkarte Meine Genehmigungen mit dem Text „Entscheidung getroffen“, bis Sie auf die Schaltfläche **Aktualisieren** klicken oder bis Sie die Browser-Seite aktualisieren.

## Genehmigen eines Dokuments auf der Dokumentseite

1. Navigieren Sie zur Dokumentseite, indem Sie auf den Namen des Dokuments klicken.

1. Wählen Sie die Version des Dokuments, das noch nicht genehmigt wurde, in der Dropdown-Liste Version neben dem Namen des Dokuments aus. Standardmäßig wird die neueste Version ausgewählt.

   Wenn für die aktuell ausgewählte Version des Dokuments eine ausstehende Genehmigung aussteht, werden die Schaltflächen für die Genehmigungsentscheidung oben rechts auf der Seite angezeigt. Wenn andere Versionen des Dokuments ausstehende Genehmigungen für Sie haben, wird im Dropdown-Menü Version ein roter Punkt angezeigt.

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Klicken Sie oben rechts auf der Seite auf eine der beiden folgenden Genehmigungsoptionen:

   * Das **Genehmigen** Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass eine Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** gibt an, dass einige kleine Änderungen am Dokument weiterhin erforderlich sind, aber die Genehmigung unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option wählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen für das zu genehmigende Dokument erforderlich sind. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Muss überarbeitet werden** gibt an, dass die Dokumentversion nicht genehmigt ist und umfangreiche Änderungen erfordert.

## Genehmigen eines Dokuments im Bedienfeld Dokumentzusammenfassung

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.

1. Klicken Sie auf das Dokument, das Ihrer Genehmigung bedarf, und das Bedienfeld Dokumentzusammenfassung wird geöffnet.

1. Wählen Sie in der Dropdown-Liste Version die Version des Dokuments aus, das Sie überprüfen möchten. Standardmäßig wird die neueste Version ausgewählt.

   Wenn für die aktuell ausgewählte Version des Dokuments eine ausstehende Genehmigung aussteht, werden die Schaltflächen für Genehmigungsentscheidungen in der oberen rechten Ecke des Bedienfelds Dokumentzusammenfassung angezeigt. Wenn andere Versionen des Dokuments ausstehende Genehmigungen für Sie haben, zeigt das Dropdown-Menü Version einen roten Punkt an.
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. Klicken Sie oben rechts im Bedienfeld Dokumentzusammenfassung auf eine der beiden folgenden Genehmigungsoptionen:

   * Das **Genehmigen** Dropdown-Menü enthält zwei Optionen:

      * **Genehmigen** gibt an, dass für diese Version des Dokuments keine Änderungen erforderlich sind und dass eine Genehmigung erteilt wird.

      * **Mit Änderungen genehmigen** gibt an, dass einige kleine Änderungen am Dokument weiterhin erforderlich sind, aber die Genehmigung unter der Bedingung erteilt wird, dass diese Änderungen vorgenommen werden. Wenn Sie diese Option wählen, wird ein Fenster mit einem Textfeld mit dem Namen **Nächste Schritte** angezeigt, in dem Sie angeben können, welche Änderungen für das zu genehmigende Dokument erforderlich sind. Sie können entweder diese Informationen eingeben und auf **Nachricht hinzufügen** klicken oder auf **Überspringen** klicken, um die Genehmigungsentscheidung ohne zusätzliche Informationen zu senden.

   * **Muss überarbeitet werden** gibt an, dass die Dokumentversion nicht genehmigt ist und umfangreiche Änderungen erfordert.


## Genehmigen eines Dokuments über die Korrekturabzugsansicht

So überprüfen und genehmigen Sie ein Dokument:

1. Gehen Sie zu Ihrer E-Mail-Benachrichtigung und klicken Sie auf **Zum Überprüfen gehen**.

1. Wenn Sie sich in Workfront befinden, klicken Sie auf **Zum Korrekturabzug gehen**.

1. Überprüfen Sie den Inhalt und fügen Sie Kommentare oder Markup hinzu. Weitere Informationen zur Verwendung der Proofing-Anzeige finden Sie unter [Testsendungen in Adobe Workfront überprüfen: Artikelindex](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Wählen Sie eine der folgenden Entscheidungen:

   * **Genehmigen**: Das Dokument muss nicht geändert werden und ist einsatzbereit.
   * **Mit Änderungen genehmigen**: Das Dokument benötigt Änderungen und ist nach deren Vornahme zur Verwendung bereit. Eine zusätzliche Genehmigung ist nicht erforderlich.
   * **Muss überarbeitet werden**: Das Dokument muss geändert werden und ist nicht einsatzbereit. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Dokument als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. Weitere Informationen zum Hochladen einer neuen Version finden Sie unter [Erstellen einer neuen Version nach Bedarf](#create-a-new-version-as-needed) in diesem Artikel.

Sobald Sie eine Entscheidung treffen, wird der Dokumentverantwortliche per E-Mail benachrichtigt.


