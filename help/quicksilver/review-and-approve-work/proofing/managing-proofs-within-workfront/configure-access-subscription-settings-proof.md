---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Zugriffs- und Abonnementeinstellungen für einen Testversand konfigurieren
description: Sie können bestimmte Zugriffs- und Abonnementeinstellungen für einzelne Testsendungen konfigurieren, z. B. ob Benutzer sich anmelden müssen und ob Benutzer den Testversand abonnieren dürfen. Sie können Zugriffs- und Abonnementeinstellungen für einen Testversand während der Erstellung einrichten oder einen Testversand einrichten, der bereits in Workfront existiert.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 3%

---

# Zugriffs- und Abonnementeinstellungen für einen Testversand konfigurieren

Sie können bestimmte Zugriffs- und Abonnementeinstellungen für einzelne Testsendungen konfigurieren, z. B. ob Benutzer sich anmelden müssen und ob Benutzer den Testversand abonnieren dürfen. Sie können Zugriffs- und Abonnementeinstellungen für einen Testversand während der Erstellung einrichten oder einen Testversand einrichten, der bereits in Workfront existiert.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Zugriffs- und Abonnementeinstellungen beim Erstellen eines Testversands konfigurieren

So richten Sie Zugriffs- und Abonnementeinstellungen für einen Testversand während der Erstellung ein:

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf die Schaltfläche **Dokumente** Abschnitt.
1. Klicken **Neu hinzufügen** oben rechts.
1. Scrollen Sie zum **Testversandeinstellungen** in der rechten unteren Ecke des **Neuer Testversand** Seite.

1. Konfigurieren Sie die folgenden Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Freigabe des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</strong> </td> 
      <td>Wenn diese Option aktiviert ist, kann der Testversand über eine öffentliche URL oder einen Einbettungscode freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonnement des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</strong> </td> 
      <td>Wenn diese Option aktiviert ist, können Personen, die dem Testversand nicht explizit hinzugefügt wurden, den Testversand abonnieren. Die Person, die den Testversand abonniert, erhält die Rolle und E-Mail, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><p><strong>Abonnentenrolle:</strong> Die standardmäßige Testversand-Rolle, die allen Prüfern zugewiesen wird, die den Testversand abonnieren. </p><p>Wichtig: Wenn <strong>Freigabe zulassen mit</strong> auf alles andere als <strong>Alle</strong> in den Testversandeinstellungen von Workfront funktioniert das Abonnement nur für Personen innerhalb des Unternehmens. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren von Testeinstellungen in Workfront Testversand</a>.</p></li>
        <li><strong>Einstellungen für E-Mail-Warnhinweise für Abonnenten:</strong> Der Standard-E-Mail-Warnhinweis, der allen Prüfern zugewiesen wird, die den Testversand abonnieren.</li>
       </ul><p>
        <ul>
         <li><strong>Der Zugriff per E-Mail-Link ist nachweislich für folgende Zwecke erforderlich:</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Testversand erhält. Sie können <strong>Keine E-Mail</strong> (Für den Zugriff auf den Testversand ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung zum Testversand</strong> (Der Abonnent erhält einen Link zum Testversand per E-Mail ohne Überprüfung) oder <strong>Validierungs- und Testversand-Benachrichtigungs-E-Mails</strong> (Der Abonnent erhält per E-Mail einen Link zum Testversand und muss auf den Link klicken, um auf einen Testversand zugreifen zu können. Mit dieser Option soll sichergestellt werden, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die sie Zugriff hat.)</li>
        </ul><p>Hinweis:  Wenn die Testsendungen den automatisierten Workflow angehängt haben, generieren alle Abonnements Bestätigungs-E-Mails an die Testversand-Inhaber, sodass diese entscheiden können, zu welcher Stufe die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit der Erstellung Ihres Testversands fort.

## Zugriffs- und Abonnementeinstellungen für einen vorhandenen Testversand konfigurieren

So richten Sie Zugriffs- und Abonnementeinstellungen für einen bereits in Workfront vorhandenen Testversand ein:

1. Wählen Sie im Bereich Dokumente das Dokument aus, das den Testversand enthält, für den Sie die Einstellungen konfigurieren möchten, und klicken Sie dann auf **Dokumentdetails**.
1. Klicken Sie im linken Bereich auf **Testen der Viewer-Einstellungen**.
1. Konfigurieren Sie die folgenden Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Freigabe über öffentliche URL oder Einbettungscode zulassen</strong><strong>e</strong> </td> 
      <td>Wenn diese Option aktiviert ist, kann der Testversand über eine öffentliche URL oder einen Einbettungscode freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonnement des Korrekturabzugs über öffentliche URL oder eingebetteten Code erlauben</strong> </td> 
      <td>Wenn diese Option aktiviert ist, können Personen, die dem Testversand nicht explizit hinzugefügt wurden, den Testversand abonnieren. Die Person, die den Testversand abonniert, erhält die Rolle und E-Mail, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><p><strong>Abonnentenrolle:</strong> Die standardmäßige Testversand-Rolle, die allen Prüfern zugewiesen wird, die den Testversand abonnieren. </p><p>Wichtig: Wenn <strong>Freigabe zulassen mit</strong> auf alles andere als <strong>Alle</strong> in den Testversandeinstellungen von Workfront funktioniert das Abonnement nur für Personen innerhalb des Unternehmens. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren von Testeinstellungen in Workfront Testversand</a>.</p></li>
        <li><strong>Einstellungen für E-Mail-Warnhinweise für Abonnenten:</strong> Der Standard-E-Mail-Warnhinweis, der allen Prüfern zugewiesen wird, die den Testversand abonnieren.</li>
       </ul><p>
        <ul>
         <li><strong>Der Zugriff per E-Mail-Link ist nachweislich für folgende Zwecke erforderlich:</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Testversand erhält. Sie können <strong>Keine E-Mail</strong> (Für den Zugriff auf den Testversand ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung zum Testversand</strong> (Der Abonnent erhält einen Link zum Testversand per E-Mail ohne Überprüfung) oder <strong>Validierungs- und Testversand-Benachrichtigungs-E-Mails</strong> (Der Abonnent erhält per E-Mail einen Link zum Testversand und muss auf den Link klicken, um auf einen Testversand zugreifen zu können. Mit dieser Option soll sichergestellt werden, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die sie Zugriff hat.)</li>
        </ul><p>Hinweis:  Wenn die Testsendungen den automatisierten Workflow angehängt haben, generieren alle Abonnements Bestätigungs-E-Mails an die Testversand-Inhaber, sodass diese entscheiden können, zu welcher Stufe die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
