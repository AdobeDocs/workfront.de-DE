---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Testen eines verknüpften Assets mit dem erweiterten Connector
description: Nachdem Sie ein Asset aus Experience Manager Assets verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 3%

---

# Testen eines verknüpften Assets mit dem erweiterten Connector

Nachdem Sie ein Asset aus Experience Manager Assets verknüpft haben, können Sie einen Korrekturabzug erstellen und Benutzende zuweisen, damit sie das Asset überprüfen und Kommentare dazu hinzufügen können. Korrekturabzüge, die aus verknüpften Assets erstellt wurden, werden auf Ihr Korrekturabzugskontingent angerechnet.

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
   <p>Standard</p>
   <p>Arbeit oder höher</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf ein Dokument anzeigen oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>


Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Installieren des erweiterten Connectors für Workfront for Experience Manager

## Erstellen eines Korrekturabzugs

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
      <td role="rowheader">Einfacher Korrekturabzug</td> 
      <td>Mit dieser Option wird ein Korrekturabzug ohne angehängten Workflow erstellt und die Standardeinstellungen für den Korrekturabzug angewendet. Sie können die Standardeinstellungen für den Korrekturabzug aktualisieren oder einen Workflow hinzufügen, nachdem Sie den Korrekturabzug erstellt haben. Weitere Informationen zu Korrekturabzugseinstellungen finden Sie unter <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Bearbeiten von Korrekturabzugseinstellungen</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erweiterter Korrekturabzug</td> 
      <td> <p>Mit dieser Option können Sie einen einfachen oder erweiterten Workflow konfigurieren und die Korrekturabzugseinstellungen für den von Ihnen erstellten Korrekturabzug ändern. Weitere Informationen finden Sie unter  </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Verwalten eines vorhandenen Korrekturabzugs

Nachdem Sie einen Korrekturabzug erstellt haben, können Sie beispielsweise folgende Aufgaben ausführen

* Aktuelle Stadienaktivität anzeigen
* Aktualisieren von Reviewern und Fristen
* Workflow bearbeiten

Weitere Informationen zum Verwalten eines vorhandenen Korrekturabzugs finden Sie unter [Verwalten von Korrekturabzügen in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Überprüfen eines Korrekturabzugs

Zugewiesene Reviewer können beispielsweise folgende Aufgaben ausführen

* Asset anzeigen und Kommentare abgeben
* Aktionen zu Kommentaren hinzufügen
* Versionen vergleichen
* Testversand genehmigen oder ablehnen

Weitere Informationen dazu, was Sie mit dem Proofing-Tool tun können, finden Sie unter [Testsendungen in Adobe Workfront ](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
