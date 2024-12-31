---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials
description: Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials

Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Für den Benutzer muss Proofing aktiviert sein.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über Experience Manager-as a Cloud Service oder Assets Essentialss verfügen und dem Produkt als Benutzerin bzw. Benutzer in der Admin Console hinzugefügt werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Korrekturabzug erstellen

Sie können statische, Video- oder interaktive Korrekturabzüge erstellen.

So erstellen Sie einen Korrekturabzug:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem/der Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf den Abschnitt **Dokumente**.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf den **Korrekturabzug erstellen** Link, der unter dem Dokumentnamen angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie in **Benutzerprofil „Korrekturabzüge beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Korrekturabzug.

1. Wählen Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Einfacher Korrekturabzug</strong></td> 
      <td>Mit dieser Option wird ein Korrekturabzug ohne angehängten Workflow erstellt und die Standardeinstellungen für den Korrekturabzug angewendet. Sie können die Standardeinstellungen für den Korrekturabzug aktualisieren oder einen Workflow hinzufügen, nachdem Sie den Korrekturabzug erstellt haben. Weitere Informationen zu Korrekturabzugseinstellungen finden Sie unter <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Bearbeiten von Korrekturabzugseinstellungen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Erweiterter Korrekturabzug</strong></td> 
      <td> <p>Mit dieser Option können Sie einen einfachen oder erweiterten Workflow konfigurieren und die Korrekturabzugseinstellungen für den von Ihnen erstellten Korrekturabzug ändern. Weitere Informationen finden Sie unter </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Verwalten eines vorhandenen Korrekturabzugs

Nachdem Sie einen Korrekturabzug erstellt haben, können Sie beispielsweise folgende Aufgaben ausführen

* Aktuelle Stadienaktivität anzeigen
* Aktualisieren von Reviewern und Fristen
* Workflow bearbeiten

Weitere Informationen zum Verwalten eines vorhandenen Korrekturabzugs finden Sie unter [Verwalten von Korrekturabzügen in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Überprüfen eines Korrekturabzugs

Zugewiesene Reviewer können beispielsweise folgende Aufgaben ausführen

* Asset anzeigen und Kommentare abgeben
* Aktionen zu Kommentaren hinzufügen
* Versionen vergleichen
* Testversand genehmigen oder ablehnen

Weitere Informationen dazu, was Sie mit dem Proofing-Tool tun können, finden Sie unter [Testsendungen in Adobe Workfront ](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
