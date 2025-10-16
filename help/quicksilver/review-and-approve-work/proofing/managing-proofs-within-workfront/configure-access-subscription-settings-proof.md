---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: Konfigurieren der Zugriffs- und Abonnementeinstellungen für einen Testversand
description: Sie können bestimmte Zugriffs- und Abonnementeinstellungen für einzelne Korrekturabzüge konfigurieren, z. B. ob Benutzende sich anmelden müssen und ob Benutzende den Korrekturabzug abonnieren dürfen. Sie können Zugriffs- und Abonnementeinstellungen für einen Korrekturabzug einrichten, während Sie ihn erstellen, oder Sie können sie für einen Korrekturabzug einrichten, der bereits in Workfront vorhanden ist.
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Konfigurieren der Zugriffs- und Abonnementeinstellungen für einen Testversand

Sie können bestimmte Zugriffs- und Abonnementeinstellungen für einzelne Korrekturabzüge konfigurieren, z. B. ob Benutzende sich anmelden müssen und ob Benutzende den Korrekturabzug abonnieren dürfen. Sie können Zugriffs- und Abonnementeinstellungen für einen Korrekturabzug einrichten, während Sie ihn erstellen, oder Sie können sie für einen Korrekturabzug einrichten, der bereits in Workfront vorhanden ist.

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
   <p>Arbeit oder Plan</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriffs- und Abonnementeinstellungen beim Erstellen eines Korrekturabzugs konfigurieren

So richten Sie Zugriffs- und Abonnementeinstellungen für einen Korrekturabzug ein, während Sie ihn erstellen:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem/der Sie den Korrekturabzug anzeigen möchten, und klicken Sie dann auf den Abschnitt **Dokumente**.
1. Klicken **oben rechts auf** Neu hinzufügen“.
1. Scrollen Sie zum Abschnitt **Korrekturabzugseinstellungen** in der rechten unteren Ecke der Seite **Neuer Korrekturabzug**.

1. Konfigurieren Sie die folgenden Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Freigabe des Korrekturabzugs über öffentliche URL oder Einbettungs-Code zulassen</strong> </td> 
      <td>Wenn diese Option ausgewählt ist, kann der Korrekturabzug über eine öffentliche URL oder einen Einbettungs-Code freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonnieren des Korrekturabzugs über eine öffentliche URL oder einen Einbettungs-Code zulassen</strong> </td> 
      <td>Wenn diese Option ausgewählt ist, können Personen, die dem Korrekturabzug nicht explizit hinzugefügt wurden, den Korrekturabzug abonnieren. Der Person, die den Korrekturabzug abonniert, wird die Rolle und die E-Mail-Adresse zugewiesen, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><p><strong>Abonnentenrolle</strong> Die Standardrolle für den Korrekturabzug, die allen Reviewern zugewiesen ist, die den Korrekturabzug abonnieren. </p><p>Wichtig: Wenn <strong>Freigabe zulassen für</strong> in den Workfront Proof-Einstellungen auf einen anderen Wert als <strong>Alle</strong> festgelegt ist, funktioniert das Abonnement nur für Personen innerhalb des Unternehmens. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</p></li>
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten:</strong> Der E-Mail-Warnhinweis, der standardmäßig allen Reviewern zugewiesen wird, die den Testversand abonniert haben.</li>
       </ul><p>
        <ul>
         <li><strong>Zugriff auf Korrekturabzug über einen E-Mail-Link erforderlich für</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Korrekturabzug erhält. Sie können zwischen <strong>Keine E-Mail</strong> (für den Zugriff auf den Korrekturabzug ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung über den Korrekturabzug</strong> (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail ohne Bestätigung) oder <strong>E-Mails zur Validierung und </strong> des Korrekturabzugs (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail und muss auf den Link klicken, um auf den Korrekturabzug zuzugreifen. Diese Option dient dazu, sicherzustellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die er Zugriff hat).</li>
        </ul><p>Hinweis:  Wenn an die Korrekturabzüge ein automatisierter Workflow angehängt ist, generieren alle Abonnements Bestätigungs-E-Mails an die Verantwortlichen des Korrekturabzugs, damit sie entscheiden können, zu welchem Schritt die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Erstellen Sie den Korrekturabzug weiter.

## Zugriffs- und Abonnementeinstellungen für einen vorhandenen Korrekturabzug konfigurieren

So richten Sie Zugriffs- und Abonnementeinstellungen für einen Korrekturabzug ein, der bereits in Workfront vorhanden ist:

1. Wählen Sie im Bereich Dokumente das Dokument aus, das den Korrekturabzug enthält, für den Sie Einstellungen konfigurieren möchten, und klicken Sie dann auf **Dokumentdetails**.
1. Klicken Sie im linken Bedienfeld auf **Proofing Viewer-Einstellungen**.
1. Konfigurieren Sie die folgenden Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Freigabe des Korrekturabzugs über öffentliche URL oder Einbettungs-Code zulassen</strong><strong>e</strong> </td> 
      <td>Wenn diese Option ausgewählt ist, kann der Korrekturabzug über eine öffentliche URL oder einen Einbettungs-Code freigegeben werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Abonnieren des Korrekturabzugs über eine öffentliche URL oder einen Einbettungs-Code zulassen</strong> </td> 
      <td>Wenn diese Option ausgewählt ist, können Personen, die dem Korrekturabzug nicht explizit hinzugefügt wurden, den Korrekturabzug abonnieren. Der Person, die den Korrekturabzug abonniert, wird die Rolle und die E-Mail-Adresse zugewiesen, die Sie in den folgenden Einstellungen definieren:
       <ul>
        <li><p><strong>Abonnentenrolle</strong> Die Standardrolle für den Korrekturabzug, die allen Reviewern zugewiesen ist, die den Korrekturabzug abonnieren. </p><p>Wichtig: Wenn <strong>Freigabe zulassen für</strong> in den Workfront Proof-Einstellungen auf einen anderen Wert als <strong>Alle</strong> festgelegt ist, funktioniert das Abonnement nur für Personen innerhalb des Unternehmens. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</p></li>
        <li><strong>E-Mail-Warnhinweiseinstellungen für Abonnenten:</strong> Der E-Mail-Warnhinweis, der standardmäßig allen Reviewern zugewiesen wird, die den Testversand abonniert haben.</li>
       </ul><p>
        <ul>
         <li><strong>Zugriff auf Korrekturabzug über einen E-Mail-Link erforderlich für</strong> Konfigurieren Sie, ob der Abonnent eine E-Mail mit einem Link zum Korrekturabzug erhält. Sie können zwischen <strong>Keine E-Mail</strong> (für den Zugriff auf den Korrekturabzug ist kein E-Mail-Link erforderlich), <strong>Nur E-Mail-Benachrichtigung über den Korrekturabzug</strong> (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail ohne Bestätigung) oder <strong>E-Mails zur Validierung und </strong> des Korrekturabzugs (der Abonnent erhält einen Link zum Korrekturabzug per E-Mail und muss auf den Link klicken, um auf den Korrekturabzug zuzugreifen. Diese Option dient dazu, sicherzustellen, dass die Person eine korrekte E-Mail-Adresse eingegeben hat, auf die er Zugriff hat).</li>
        </ul><p>Hinweis:  Wenn an die Korrekturabzüge ein automatisierter Workflow angehängt ist, generieren alle Abonnements Bestätigungs-E-Mails an die Verantwortlichen des Korrekturabzugs, damit sie entscheiden können, zu welchem Schritt die Person hinzugefügt werden soll.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
