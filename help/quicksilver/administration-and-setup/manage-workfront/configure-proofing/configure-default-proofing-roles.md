---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurieren von standardmäßigen Testrollen
description: Als Adobe Workfront-Administrator können Sie die standardmäßigen Testversandrollen für Benutzer und Gastbenutzer konfigurieren, die auf in Workfront erstellte Testsendungen zugreifen. Jeder Benutzer, der Benutzer zu einem Testversand hinzufügt, kann diese Rollen anpassen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Konfigurieren von standardmäßigen Testrollen

Als Adobe Workfront-Administrator können Sie die standardmäßigen Testversandrollen für Benutzer und Gastbenutzer konfigurieren, die auf in Workfront erstellte Testsendungen zugreifen. Jeder Benutzer, der Benutzer zu einem Testversand hinzufügt, kann diese Rollen anpassen.

## Zugriffsanforderungen

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen Workfront-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Konfigurieren von standardmäßigen Testrollen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klicken **Überprüfung und Genehmigung** am unteren Rand der Liste, die auf der linken Seite angezeigt wird.
1. Im **Rollen für bestimmte Empfänger eines Dokumentversands** die Standardrolle für Benutzer und Gastbenutzer auswählen, die zum Workflow eines Testversands hinzugefügt werden.

   Siehe [Rechte in Verbindung mit Testing-Rollen](#rights-associated-with-proofing-roles) unten für eine Liste der einzelnen Testing-Rollen und der damit verbundenen Rechte.

   >[!NOTE]
   >
   >* Diese Einstellung gilt nur für Benutzer, die im Workfront-System erstellt werden, nachdem die Rolle festgelegt wurde. nicht für bestehende Benutzer.
   >* Die Person, die Benutzer zum Testversand hinzufügt, kann diese Rolle anpassen, wie unter [Benutzer zu Testversand hinzufügen](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Freigeben eines Testversands in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. Im **Rollen für Nicht-Empfänger, die einen Dokumentversand öffnen** -Bereich die Standardrolle für Benutzer und Gastbenutzer auswählen, die auf einen Testversand zugreifen können, aber nicht zum Testversand-Workflow hinzugefügt werden.

   Diese Situation tritt auf, wenn Benutzer und Gäste Zugriff auf ein Dokument haben, für das ein Testversand erstellt wurde: selbst wenn sie nicht zum Testversand-Workflow hinzugefügt wurden, können sie den Testversand öffnen.

   **Beispiele:** Im Folgenden finden Sie Beispiele für die Verwendung dieser Einstellung:

   * Wählen Sie **Schreibgeschützt** , um alle Testsendungen zu beschränken, z. B. das Hinzufügen von Kommentaren und die Entscheidungsfindung für diejenigen, die dazu aufgefordert wurden.
   * Wählen Sie **Überprüfer** weil Sie möchten, dass jedes Mitglied des Teams Markierungen und Kommentare zu einem Testversand hinzufügen kann.

1. Klicken Sie auf **Speichern**.

## Rechte in Verbindung mit Testing-Rollen {#rights-associated-with-proofing-roles}

In der folgenden Tabelle sind alle Rollen und damit verbundenen Rechte aufgeführt:

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
   <th> <p><strong>Testversand anzeigen</strong> </p> </th> 
   <th> <p><strong>Markierungen hinzufügen</strong> </p> </th> 
   <th> <p><strong>Kommentare hinzufügen</strong> </p> </th> 
   <th> <p><strong>Eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind</strong> </p> </th> 
   <th> <p><strong>Entscheidungsfindung</strong> </p> </th> 
   <th> <p><strong>Löschen von Kommentaren anderer Benutzer</strong> </p> </th> 
   <th>Kommentare auflösen</th> 
   <th>Anwenden von Aktionen auf Kommentare</th> 
   <th> <p><strong>Testversand bearbeiten</strong> </p> </th> 
   <th>Testversand für andere freigeben</th> 
   <th>Neue Version erstellen</th> 
   <th> <p><strong>Genehmigungsanfragen im Startbereich anzeigen</strong> </p> </th> 
   <th>Hinzufügen neuer Validierungsverantwortlicher</th> 
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
   <td> <p><strong>Autor</strong> </p> </td> 
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
   <td> <p><strong>✓</strong> </p> </td> 
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
>Benutzer mit neuen Workfront-Plänen können allen Benutzern im System Autoren- oder Moderatorrollen zuweisen. Benutzer mit älteren Plänen können Autoren- oder Moderatorrollen jedem Benutzer mit einer Testversandlizenz im System zuweisen.
