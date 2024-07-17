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
source-wordcount: '554'
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
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen Workfront-Administrator sein. Weitere Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Konfigurieren von standardmäßigen Testrollen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klicken Sie unten in der Liste, die links angezeigt wird, auf **Überprüfen und Genehmigen** .
1. Wählen Sie im Abschnitt **Rollen für bestimmte Empfänger eines Testversands** die Standardrolle für Benutzer und Gastbenutzer aus, die dem Workflow eines Testversands hinzugefügt werden.

   Unter [Berechtigungen, die mit Testing-Rollen verknüpft sind](#rights-associated-with-proofing-roles) unten finden Sie eine Liste der einzelnen Testing-Rollen und der damit verbundenen Rechte.

   >[!NOTE]
   >
   >* Diese Einstellung gilt nur für Benutzer, die im Workfront-System erstellt werden, nachdem die Rolle festgelegt wurde, nicht für bestehende Benutzer.
   >* Die Person, die Benutzer zum Testversand hinzufügt, kann diese Rolle anpassen, wie unter [Hinzufügen von Benutzern zu einem Testversand](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Freigeben eines Testversands in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) beschrieben.

1. Wählen Sie im Abschnitt **Rollen für Nicht-Empfänger, die einen Testversand öffnen** die Standardrolle für Benutzer und Gastbenutzer aus, die auf einen Testversand zugreifen können, aber nicht zum Testversand-Workflow hinzugefügt werden.

   Diese Situation tritt auf, wenn Benutzer und Gäste Zugriff auf ein Dokument haben, für das ein Testversand erstellt wurde. Selbst wenn sie nicht zum Testversand-Workflow hinzugefügt wurden, können sie den Testversand öffnen.

   **Beispiele:** Hier sind Beispiele für die Verwendung dieser Einstellung:

   * Sie wählen **Schreibgeschützt** aus, um alle Testversandaktivitäten zu beschränken, z. B. das Hinzufügen von Kommentaren und das Treffen von Entscheidungen zu den Personen, die dazu aufgefordert wurden.
   * Sie wählen **Überprüfer** aus, da Sie möchten, dass jedes Mitglied des Teams Markierungen und Kommentare zu einem Testversand hinzufügen kann.

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
   <th> <p><strong>Anzeigen eines Testversands</strong> </p> </th> 
   <th> <p><strong>Markups hinzufügen</strong> </p> </th> 
   <th> <p><strong>Kommentare hinzufügen</strong> </p> </th> 
   <th> <p><strong>Eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind</strong> </p> </th> 
   <th> <p><strong>Entscheidungsfindung</strong> </p> </th> 
   <th> <p><strong>Kommentare anderer Benutzer löschen</strong> </p> </th> 
   <th>Kommentare auflösen</th> 
   <th>Anwenden von Aktionen auf Kommentare</th> 
   <th> <p><strong>Testversand bearbeiten</strong> </p> </th> 
   <th>Testversand für andere freigeben</th> 
   <th>Neue Version erstellen</th> 
   <th> <p><strong>Genehmigungsanforderungen im Startbereich anzeigen</strong> </p> </th> 
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
   <td> <p><strong>Überprüfer und Genehmiger</strong> </p> </td> 
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
