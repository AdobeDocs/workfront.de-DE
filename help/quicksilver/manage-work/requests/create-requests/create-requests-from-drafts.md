---
product-area: requests
navigation-topic: create-requests
title: Anforderungen aus Entwürfen erstellen
description: Zusätzlich zur Verwendung der verfügbaren Entwürfe, die Ihnen Workfront bei Eingabe einer neuen Anforderung vorschlägt, können Sie auch über den Bereich Entwürfe auf eine Entwurfsanfrage zugreifen und sie von dort abschicken.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 0f30ff23ef828d32c406cc2d9733c23b095014c9
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Anforderungen aus Entwürfen erstellen

Zusätzlich zur Verwendung der verfügbaren Entwürfe, die Ihnen Workfront bei Eingabe einer neuen Anforderung vorschlägt, können Sie auch über den Bereich Entwürfe auf eine Entwurfsanfrage zugreifen und sie von dort abschicken.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen für das Erstellen von Anforderungen aus Entwürfen

Sie müssen Folgendes tun, bevor Sie eine Anforderung aus einem Entwurf erstellen können: 

* Erstellen Sie eine Anforderung. Dadurch wird die Anforderung im Abschnitt Entwürfe automatisch als Entwurf gespeichert.

   Informationen zum Erstellen von Anforderungen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Anforderungen aus Entwürfen erstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Workfront.
1. Klicken **Anforderungen** > **Entwürfe**.

   In dieser Liste wird für jedes Warteschlangenthema jeder Anforderungswarteschlange ein Entwurf angezeigt.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Optional) Klicken Sie auf eine Spaltenüberschrift, um die Liste nach dieser Spalte zu sortieren.

1. Überprüfen Sie die Informationen zu den einzelnen Entwürfen in den folgenden Spalten der Liste &quot;Entwürfe&quot;:

   | Betreff | Dies ist der Name, den Sie Ihrer Anforderung als Sie mit der Erstellung begonnen haben. |
   |---|---|
   | Pfad | Der Name der Anforderungswarteschlange, Themengruppen und Warteschlangenthemen, an die Sie die Anforderung ursprünglich senden wollten. |
   | Eingabedatum | Das Datum, an dem Sie mit der Erstellung der Anforderung begonnen haben. |
   | Datum der letzten Aktualisierung | Das letzte Ihrer letzten Aktualisierungen. Wenn Sie es seit dem ersten Start der Anfrage nicht aktualisiert haben, sollten das Entrypdatum und das letzte Aktualisierungsdatum identisch sein. |

   {style="table-layout:auto"}

1. (Optional) Geben Sie über den Schnellfilter in der oberen rechten Ecke der Liste &quot;Entwürfe&quot;den Namen einer entworfenen Anforderung, Anforderungswarteschlange, Warteschlangenthema oder Themengruppe ein und klicken Sie dann auf den Namen eines Entwurfs, um ihn zu öffnen.

   >[!TIP]
   >
   >Im Bereich &quot;Entwürfe&quot;des Bereichs &quot;Anforderungen&quot;können Sie keine permanenten Filter anwenden. Darüber hinaus gibt es keine Optionen, um die Ansicht der Entwürfe-Liste zu ändern oder zu ändern.

1. Aktualisieren Sie die Informationen für die Anforderung, wie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Optional und bedingt) Klicken Sie während der Eingabe der Anforderung auf **Verwerfen** Entwurf, wenn Sie den Entwurf löschen möchten. Dadurch wird der Entwurf gelöscht, der nicht wiederhergestellt werden kann. Weitere Informationen zum Löschen von Entwürfen finden Sie unter [Anforderungsentwurf löschen](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Optional) Klicken Sie auf **Abbrechen** in der linken unteren Ecke der Seite, wenn Sie Ihre Aktion wiederherstellen und den Entwurf beibehalten möchten.

1. Führen Sie nach Abschluss der Informationen für die Anfrage einen der folgenden Schritte aus:

   * Klicken **Einsenden** , wenn Sie bereit sind, die Anfrage zu senden. Die Anforderung wird im Abschnitt Gesendet gespeichert. Abhängig von der Routing-Regel der Anforderungswarteschlange kann diese Anforderung an ein anderes Projekt als an das als Anforderungswarteschlange bestimmte weitergeleitet werden. Informationen zu Routing-Regeln finden Sie unter [Erstellen von Routing-Regeln](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      Oder

      Klicken **Schließen** wenn Sie nicht ganz bereit sind, sie einzureichen, und Sie können sie später erneut abschließen. Ihre Anforderung wird im Abschnitt Entwürfe gespeichert und steht Ihnen beim nächsten Senden einer Anforderung für diese Anforderungswarteschlange zur Verfügung.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

      Wenn Sie die Anforderung senden, wird der Entwurf gelöscht und kann nicht wiederhergestellt werden.
