---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials
description: Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 2%

---

# Testen eines verknüpften Assets für Experience Manager Assets oder Assets Essentials

Nachdem Sie ein Asset aus Experience Manager Assets Essentials verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können.

## Zugriffsanforderungen

<!-- Audited: 4/2025 -->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Standard</p>
   <p>Arbeit oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Weitere Produkte</td> 
   <td>Sie müssen über Experience Manager as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Ansichtszugriff oder höher</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen:

* Ihr Workfront-Administrator muss eine Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Korrekturabzug erstellen

Sie können statische, Video- oder interaktive Korrekturabzüge erstellen.

So erstellen Sie einen Korrekturabzug:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem/der Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf den Abschnitt **Dokumente**.
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf den **Korrekturabzug erstellen** Link, der unter dem Dokumentnamen angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie in **Benutzerprofil „Korrekturabzüge beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Korrekturabzug.

1. Wählen Sie eine der folgenden Optionen aus der Dropdown-Liste aus:

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
      <td> <p>Mit dieser Option können Sie einen einfachen oder erweiterten Workflow konfigurieren und die Korrekturabzugseinstellungen für den von Ihnen erstellten Korrekturabzug ändern. Weitere Informationen finden Sie unter: </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Verwalten eines vorhandenen Korrekturabzugs

Nachdem Sie einen Korrekturabzug erstellt haben, können Sie Folgendes tun:

* Aktuelle Stadienaktivität anzeigen
* Aktualisieren von Reviewern und Fristen
* Workflow bearbeiten

Weitere Informationen zum Verwalten eines vorhandenen Korrekturabzugs finden Sie unter [Verwalten von Korrekturabzügen in Adobe Workfront: Artikelindex](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Überprüfen eines Korrekturabzugs

Zugewiesene Reviewer können Folgendes tun:

* Asset anzeigen und Kommentare abgeben
* Aktionen zu Kommentaren hinzufügen
* Versionen vergleichen
* Testversand genehmigen oder ablehnen

Weitere Informationen dazu, was Sie mit dem Proofing-Tool tun können, finden Sie unter [Testsendungen in Adobe Workfront überprüfen: Artikelindex](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
