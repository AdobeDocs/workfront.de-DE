---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials
description: Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Testversand erstellen und Benutzer zum Überprüfen und Hinzufügen von Kommentaren zum Asset zuweisen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials

Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Testversand erstellen und Benutzer zum Überprüfen und Hinzufügen von Kommentaren zum Asset zuweisen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Arbeit oder höher</p>
   <p>Sie müssen die Testversandfunktion für Ihren Benutzer aktiviert haben.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff anzeigen oder höher</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der as a Cloud Service Integration von Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Integration von Experience Manager Assets Essentials konfigurieren](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Korrekturabzug erstellen

Sie können statische, Video- oder interaktive Testsendungen erstellen.

So erstellen Sie einen Testversand:

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf die Schaltfläche **Dokumente** Abschnitt.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie auf **Testversand erstellen** -Link, der unter dem Dokumentnamen angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie **Automatische Erstellung von Testsendungen beim Hochladen von Dokumenten** in Ihrem Benutzerprofil aktiviert ist, erstellt das System automatisch einen einfachen Testversand.

1. Wählen Sie eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Einfacher Testversand</strong></td> 
      <td>Diese Option erstellt einen Testversand ohne angehängten Workflow und wendet die standardmäßigen Testversandeinstellungen an. Sie können die standardmäßigen Testversandeinstellungen aktualisieren oder einen Workflow hinzufügen, nachdem Sie den Testversand erstellt haben. Weitere Informationen zu den Testversandeinstellungen finden Sie unter <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Testversandeinstellungen bearbeiten</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Erweiterter Testversand</strong></td> 
      <td> <p>Mit dieser Option können Sie einen einfachen oder erweiterten Workflow konfigurieren und die Testversandeinstellungen für den von Ihnen erstellten Testversand ändern. Weitere Informationen finden Sie unter </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Testversands mit einem einfachen Workflow</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Testversands mit einem automatisierten Workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Vorhandenen Testversand verwalten

Nachdem Sie einen Testversand erstellt haben, können Sie Dinge wie

* Aktuelle Staging-Aktivität anzeigen
* Aktualisieren von Validierungsverantwortlichen und Terminen
* Workflow bearbeiten

Weitere Informationen zur Verwaltung eines vorhandenen Testversands finden Sie unter [Verwalten von Testsendungen in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Testversand überprüfen

Zugewiesene Überprüfer können beispielsweise Folgendes tun:

* Asset anzeigen und Kommentare erstellen
* Hinzufügen von Aktionen zu Kommentaren
* Versionen vergleichen
* Testversand genehmigen oder ablehnen

Weitere Informationen dazu, was Sie mit dem Testool tun können, finden Sie unter [Überprüfen von Testsendungen in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
