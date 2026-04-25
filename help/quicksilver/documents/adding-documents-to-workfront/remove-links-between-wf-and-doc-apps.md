---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Entfernen von Links zwischen Adobe Workfront und externen Anbietern von Dokumentenspeichern
description: When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 14%

---

# Entfernen von Links zwischen Adobe Workfront und externen Anbietern von Dokumentenspeichern

When uploading a document from any service for the first time, Adobe Workfront requests permission from the user to access their document service. When the user provides their document service credentials to log in, the document service links itself to Workfront.

For information about linking external document services to Workfront, see [Linking Documents from External Applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Since the document service is the one allowing permission to link to Workfront, it is not possible for Workfront to remove the permission granted by the document service. You must remove the permission from within the document service application or you must call our Support Team to remove this link from our servers.

>[!NOTE]
>
>Diese Funktion ist im Bereich Neue Dokumente nicht verfügbar.<br>
>Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Remove the link between Workfront and Dropbox

1. Log in to Dropbox.
1. Click your profile picture in the upper right corner, then click **Settings**.
1. Click the **Connected apps** tab, then scroll down to **Linked apps**.

1. Click the **X** next to Workfront.

## Remove the link between Workfront and Box

1. Log in to your Box account.
1. Click your profile picture in the upper right corner.
1. Click **Account Settings**, then the **Security** tab.

1. Find **MyWorkfront** and click the **X** under Forget App.

## Remove the link between Workfront and Google Drive

1. Log in to your Google Drive.
1. Click the gear icon in the upper right corner, then click **Settings**.
1. Click **Manage Apps** on the left side and find **Workfront** in the list.

1. Under the Options drop-down menu, click **Disconnect from Drive**.

## Remove the links between Workfront and Other Document Storage Providers

You must call our Support Team to disconnect Microsoft One Drive or WebDAM from Workfront.

For information about contacting our Support Team, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
