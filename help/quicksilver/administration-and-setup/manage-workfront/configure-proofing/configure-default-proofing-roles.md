---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Standard-Proofing-Rollen konfigurieren
description: Als Adobe Workfront-Administrator können Sie die standardmäßigen Proofing-Rollen für Benutzende und Gastbenutzer konfigurieren, die auf in Workfront erstellte Korrekturabzüge zugreifen. Jede Person, die Benutzende zu einem Korrekturabzug hinzufügt, kann diese Rollen für sie anpassen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

---

# Standard-Proofing-Rollen konfigurieren

Als Adobe Workfront-Administrator können Sie die standardmäßigen Proofing-Rollen für Benutzende und Gastbenutzer konfigurieren, die auf in Workfront erstellte Korrekturabzüge zugreifen. Jede Person, die Benutzende zu einem Korrekturabzug hinzufügt, kann diese Rollen für sie anpassen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Standard-Proofing-Rollen konfigurieren

{{step-1-to-setup}}

<!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klicken Sie **unten** der Liste auf der linken Seite auf „Überprüfen und bestätigen“.
1. Wählen Sie **Abschnitt Rollen für bestimmte Empfängerinnen und Empfänger eines** die Standardrolle für Benutzerinnen und Benutzer sowie Gastbenutzer aus, die zum Workflow eines Korrekturabzugs hinzugefügt werden.

   Unten [Rechte, die Proofing-Rollen ](#rights-associated-with-proofing-roles) sind) finden Sie eine Liste der einzelnen Proofing-Rollen und der damit verbundenen Rechte.

   >[!NOTE]
   >
   >* Diese Einstellung gilt nur für Benutzende, die im Workfront-System erstellt werden, nachdem die Rolle festgelegt wurde, nicht für bestehende Benutzende.
   >* Die Person, die Benutzende zum Korrekturabzug hinzufügt, kann diese Rolle anpassen, wie unter [Hinzufügen von Benutzenden zu einem Korrekturabzug](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) beschrieben.

1. Wählen Sie im Abschnitt **Rollen für Nicht-Empfänger, die einen Korrekturabzug für Dokumente öffnen** die Standardrolle für Benutzer und Gastbenutzer aus, die auf einen Korrekturabzug zugreifen können, aber nicht zum Workflow des Korrekturabzugs hinzugefügt werden.

   Diese Situation tritt auf, wenn Benutzende und Gäste Zugriff auf ein Dokument haben, für das ein Korrekturabzug erstellt wurde: Selbst wenn sie nicht zum Workflow des Korrekturabzugs hinzugefügt wurden, können sie den Korrekturabzug öffnen.

   **Beispiele:** Im Folgenden finden Sie Beispiele, wie Sie diese Einstellung verwenden können:

   * Wählen Sie **Schreibgeschützt** aus, um alle Korrekturabzugsaktivitäten einzuschränken, z. B. Kommentare hinzuzufügen und Entscheidungen gegenüber denjenigen zu treffen, die dazu aufgefordert wurden.
   * Sie wählen **Prüfer** aus, da jedes Teammitglied in der Lage sein soll, Markierungen und Kommentare zu einem Korrekturabzug hinzuzufügen.

1. Klicken Sie auf **Speichern**.

## Mit Proofing-Rollen verknüpfte Rechte {#rights-associated-with-proofing-roles}

In der folgenden Tabelle sind die einzelnen Rollen und die damit verbundenen Rechte aufgeführt:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Korrekturabzug anzeigen</strong> </p> </th> 
   <th> <p><strong>Hinzufügen von Markierungen</strong> </p> </th> 
   <th> <p><strong>Kommentare hinzufügen</strong> </p> </th> 
   <th> <p><strong>Eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind</strong> </p> </th> 
   <th> <p><strong>Entscheidung treffen</strong> </p> </th> 
   <th> <p><strong>Löschen von Kommentaren anderer</strong> </p> </th> 
   <th>Kommentare auflösen</th> 
   <th>Aktionen auf Kommentare anwenden</th> 
   <th> <p><strong>Bearbeiten des Korrekturabzugs</strong> </p> </th> 
   <th>Korrekturabzug für andere freigeben</th> 
   <th>Neue Version erstellen</th> 
   <th> <p><strong>Anzeigen von Genehmigungsanfragen im Bereich „Startseite“</strong> </p> </th> 
   <th>Neue Reviewer hinzufügen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Schreibgeschützt</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Prüfer</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Genehmigende Person</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Prüfer und genehmigende Person</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>author</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Moderator</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ <strong></strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Benutzende mit neuen Workfront-Plänen können allen Benutzenden im System Autoren- oder Moderatorrollen gewähren. Benutzer mit älteren Plänen können Autoren- oder Moderatorrollen an jeden Benutzer mit einer Proof-Lizenz im System vergeben.
