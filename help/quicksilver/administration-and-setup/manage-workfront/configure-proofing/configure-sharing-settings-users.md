---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurieren Sie Freigabeeinstellungen für Ihre Benutzer
description: Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie die Benutzerkonten konfigurieren, für die Korrekturabzüge freigegeben werden können, ob Benutzende alle Versionen eines Korrekturabzugs sehen können, und den Zeitpunkt festlegen, zu dem Benutzende Zugriff auf freigegebene Elemente erhalten.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
TQID: https://experienceleague.adobe.com/fPxvbgeLZYUO6SU1WUOdU4BJYuGO4pSYWK-4QHSnueU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 2%

---

# Konfigurieren der Freigabeeinstellungen für Ihre Benutzer

Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie die Benutzerkonten konfigurieren, für die Korrekturabzüge freigegeben werden können, ob Benutzende alle Versionen eines Korrekturabzugs sehen können, und den Zeitpunkt festlegen, zu dem Benutzende Zugriff auf freigegebene Elemente erhalten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium oder Select</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>In Ihrem Profil für Korrekturabzugsberechtigungen muss „Administrator“ ausgewählt sein. Weitere Informationen finden Sie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurieren des Proofing-Zugriffs von Benutzenden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Freigabe für andere Konten konfigurieren

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Klicken **im Abschnitt** Freigabe“ rechts neben **Freigabe zulassen für** auf **Setup**.

1. Wählen Sie in der angezeigten Dropdown-Liste eine Option aus, um anzugeben, ob Sie die Testsendungen für alle Personen verfügbar machen möchten, die Freigabe Ihrer Testsendungen auf Ihr eigenes Konto beschränken oder sie auf Ihr eigenes Konto und alle Partnerkonten beschränken möchten, mit denen Sie zusammenarbeiten.
1. Klicken Sie auf **Speichern.**

## Konfigurieren der Sichtbarkeit für alle Versionen eines freigegebenen Korrekturabzugs

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Wählen Sie im Abschnitt **Freigabe** rechts neben **Empfänger können alle Versionen anzeigen** die Option **Aktivieren** oder **Deaktivieren** aus, um anzugeben, ob Sie Empfängern ermöglichen möchten, alle Versionen eines Korrekturabzugs in der Korrekturabzugsansicht anzuzeigen, wenn die Korrekturabzugs-URL aktiviert ist.

## Konfigurieren der Sichtbarkeit von Korrekturabzügen basierend auf der Workflow-Schrittaktivität

Sie können angeben, wann Korrekturabzüge mit einem automatisierten Workflow für Benutzende sichtbar sein sollen, die mit einem bestimmten Schritt verknüpft sind.

>[!NOTE]
>
>* Diese Option ist nur bei Verwendung der eigenständigen Workfront Proof-Anwendung verfügbar. Sie ist nicht verfügbar, wenn eine Workfront Proof-Instanz verwendet wird, die in Workfront integriert ist, oder beim Proofing in Workfront.
>* Benutzer erhalten eine E-Mail-Benachrichtigung über den Korrekturabzug erst, nachdem er in das Stadium eingetreten ist, mit dem der Benutzer verknüpft ist, unabhängig von dieser Einstellung.
>

So konfigurieren Sie, wann Testsendungen mit einem automatisierten Workflow für Benutzende sichtbar sind:

{{step1-to-proofing}}

1. Klicken Sie auf **Einstellungen** > **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Aktivieren oder deaktivieren **im Abschnitt** Freigabe **die Option „Sichtbarkeit von Korrekturabzügen auf Grundlage der Staging-Aktivierung**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deaktiviert</strong> (Standard)</td> 
      <td>Korrekturabzüge sind für Benutzende zum Zeitpunkt der Erstellung des Korrekturabzugs sichtbar.<br><p>Jeder Benutzer, der mit einem Schritt im Workflow für den Korrekturabzug verknüpft ist, kann den Korrekturabzug sofort nach der Erstellung des Korrekturabzugs in den Suchergebnissen sehen.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktiviert</strong> </td> 
      <td> <p>Korrekturabzüge werden Benutzenden erst dann angezeigt, wenn das Stadium, mit dem sie verknüpft sind, <strong>aktiv.</strong></p> <p><b>HINWEIS</b>:   
        <ul> 
         <li><em style="font-style: normal;">Wenn Sie diese Option aktivieren, sind vorhandene Korrekturabzüge weiterhin für Benutzende sichtbar, die sie bei der Erstellung sehen konnten.</em> </li> 
         <li>Nachdem ein(e) Benutzende(r) Zugriff auf eine Version eines Korrekturabzugs erhalten hat (da die Phase, mit der der/die Benutzende verknüpft ist, aktiv wird), kann der/die Benutzende nur die Version sehen, in der die Phase aktiviert ist. Wenn eine frühere Version nie das Stadium erreicht hat, mit dem der/die Benutzende verknüpft ist, kann der/die Benutzende diese Version des Korrekturabzugs nicht sehen.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
