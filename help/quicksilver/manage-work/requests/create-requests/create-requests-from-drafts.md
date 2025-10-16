---
product-area: requests
navigation-topic: create-requests
title: Anforderungen aus Entwürfen erstellen
description: Zusätzlich zur Verwendung der verfügbaren Entwürfe, die Workfront Ihnen bei der Eingabe einer neuen Anfrage vorschlägt, können Sie auch über den Abschnitt „Entwürfe“ auf eine Entwurfsanfrage zugreifen und die Übermittlung dort abschließen.
author: Becky
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---

# Anforderungen aus Entwürfen erstellen

Zusätzlich zur Verwendung der verfügbaren Entwürfe, die Workfront Ihnen bei der Eingabe einer neuen Anfrage vorschlägt, können Sie auch über den Abschnitt „Entwürfe“ auf eine Entwurfsanfrage zugreifen und die Übermittlung dort abschließen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Sie müssen über Adobe Workfront Planning verfügen, um Planungsanfragen oder Anfrageformulare anzuzeigen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für das Erstellen von Anfragen aus Entwürfen

Sie müssen Folgendes tun, bevor Sie eine Anfrage aus einem Entwurf erstellen können: 

* Erstellen Sie eine Anfrage. Dadurch wird die Anfrage automatisch im Abschnitt Entwürfe als Entwurf gespeichert.

  Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Anforderungen aus Entwürfen erstellen

{{step1-to-requests}}

1. Wählen **Entwürfe** im linken Bedienfeld aus.

   In dieser Liste wird ein Entwurf für jedes Warteschlangenthema jeder Anfragewarteschlange angezeigt.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Optional) Klicken Sie auf eine Spaltenüberschrift, um die Liste nach dieser Spalte zu sortieren.

1. Überprüfen Sie die Informationen zu den einzelnen Entwürfen in den folgenden Spalten der Liste „Entwürfe“:

   | Betreff | Dies ist der Name, den Sie Ihrer Anfrage gegeben haben, als Sie mit der Erstellung begonnen haben. |
   |---|---|
   | Path | Der Name der Anfrage-Warteschlange, der Themengruppen und der Warteschlangenthemen, an die Sie die Anfrage ursprünglich senden wollten. |
   | Eingabedatum | Das Datum, an dem Sie mit der Erstellung der Anfrage begonnen haben. |
   | Datum der letzten Aktualisierung | Das letzte Ihrer letzten Aktualisierung. Wenn Sie sie seit dem ersten Start der Anfrage nicht aktualisiert haben, sollten das Eingabedatum und das Datum der letzten Aktualisierung gleich sein. |

   {style="table-layout:auto"}

1. (Optional) Tippen Sie mithilfe des Schnellfilters oben rechts in der Liste „Entwürfe“ den Namen einer entworfenen Anfrage, einer Anforderungswarteschlange, eines Warteschlangen-Themas oder einer Themengruppe ein und klicken Sie dann auf den Namen eines Entwurfs, um ihn zu öffnen.

   >[!TIP]
   >
   >Permanente Filter können nicht im Bereich Entwürfe des Bereichs Anfragen angewendet werden. Darüber hinaus gibt es keine Optionen, um die Ansicht der Entwurfsliste zu ändern oder zu ändern.

1. Aktualisieren Sie die Informationen für die Anfrage, wie in [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md) beschrieben.
1. (Optional und bedingt) Klicken Sie während der Eingabe der Anfrage jederzeit auf **Verwerfen** Entwurf, wenn Sie den Entwurf löschen möchten. Dadurch wird der Entwurf gelöscht, der nicht wiederhergestellt werden kann. Weitere Informationen zum Löschen von Entwürfen finden Sie unter [Löschen eines Anfrageentwurfs](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Optional) Klicken Sie **Abbrechen** in der linken unteren Ecke der Seite, um Ihre Aktion rückgängig zu machen und den Entwurf beizubehalten.

1. Führen Sie nach dem Ausfüllen der Informationen für die Anfrage einen der folgenden Schritte aus:

   * Klicken Sie **Senden**, wenn Sie bereit sind, die Anfrage zu senden. Die Anfrage wird im Abschnitt Gesendet gespeichert. Abhängig von der Routing-Regel der Anfrage-Warteschlange kann diese Anfrage an ein anderes Projekt als das als Anfrage-Warteschlange bezeichnete weitergeleitet werden. Weitere Informationen zu Routingregeln finden Sie unter [Routingregeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Oder

     Klicken Sie auf **Schließen**, wenn Sie noch nicht bereit sind, ihn zu übermitteln, und Sie möglicherweise später zurückkehren und ihn abschließen. Ihre Anfrage wird im Abschnitt „Entwürfe“ gespeichert und steht Ihnen beim nächsten Senden einer Anfrage für diese Anfrage-Warteschlange zur Verfügung.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Wenn Sie die Anfrage senden, wird der Entwurf gelöscht und kann nicht wiederhergestellt werden.

   >[!NOTE]
   >
   >In der neuen anfordernden -Version befinden sich Entwürfe in derselben Liste wie gesendete Anfragen.
   >Weitere Informationen zum Erstellen von Anfragen in der neuen -Version finden Sie unter [Erstellen von Anfragen und Generieren von Entwürfen in der Workfront-Web](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md#create-requests-and-generate-drafts-in-the-workfront-web-app)App im Artikel Erstellen und Senden von Anfragen .

