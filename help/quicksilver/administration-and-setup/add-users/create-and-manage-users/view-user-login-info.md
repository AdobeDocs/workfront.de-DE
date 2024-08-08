---
title: Anzeigen von Informationen zur Benutzeranmeldung
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können sehen, wie oft sich Benutzer bei Workfront anmelden und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass Sie diese Informationen in die Ansicht einer Benutzerliste oder in einen Bericht für Benutzer aufnehmen möchten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# Anzeigen von Benutzeranmeldedaten

Sie können sehen, wie oft sich Benutzer bei Adobe Workfront anmelden und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass Sie diese Informationen in die Ansicht einer Benutzerliste oder in einen Bericht für Benutzer aufnehmen möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs eines Benutzers</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsebene, die für den Zugriff auf <b>Bearbeiten</b> konfiguriert ist, wobei <b>Erstellen</b> und mindestens eine der beiden Optionen <b>Benutzeradministrator</b> unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png"> aktiviert sind. </p> <p>Wenn von diesen beiden Optionen Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zur Einstellung <b>Benutzer</b> in einer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

## So erfasst Workfront Anmeldeinformationen

Workfront zeichnet die folgenden Informationen über Benutzer auf, die sich beim System anmelden:

* **Anmeldenummer**: Workfront zählt einen Benutzer, der sich alle 24 Stunden bei der Anwendung anmeldet. Wenn sich ein Benutzer mehrmals mit verschiedenen Browsern, Computern oder Mobilgeräten anmeldet, zählt Workfront alle Anmeldungen, die an einem Tag stattgefunden haben, als eine Anmeldung. Die Anzahl der Anmeldungen umfasst Informationen, die mit dem Zeitpunkt der Erstellung des Benutzers beginnen.
* **Letztes Anmeldedatum**: Das letzte Datum, an dem sich ein Benutzer angemeldet hat. In diesem Feld wird das Datum jeder Anmeldung über einen Browser, ein Mobilgerät oder andere Anwendungen aufgezeichnet.

Die Anmeldung bei Workfront zählt auf eine der folgenden Arten als Anmeldung bei Workfront:

* Die Workfront-Webanwendung
* Die Workfront Mobile Apps (iOS- oder Android-Geräte)
* Jede unterstützte Workfront-Integration mit einer anderen Drittanbieteranwendung (Slack, Jira)
* Jede benutzerdefinierte Integration zwischen Workfront und einer anderen Drittanbieteranwendung.
* Die Workfront-API

  >[!NOTE]
  >
  >Die Anmeldung bei Workfront über die Workfront-API ist nur für Unternehmen verfügbar, die noch nicht in der Adobe Business Platform integriert sind.

## Anzeigen von Nutzungsinformationen in einer Benutzerliste oder einem Bericht

Sie können die Felder &quot;Anzahl der Anmeldungen&quot;und &quot;Datum der letzten Anmeldung&quot;in der Ansicht einer Benutzerliste oder in einem Bericht für Benutzer anzeigen.\
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So zeigen Sie Nutzungsinformationen in der Ansicht einer Benutzerliste an:

1. Navigieren Sie zu einer Benutzerliste in Workfront.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Klicken Sie unten rechts im Bildschirm auf **Spalte hinzufügen** .
1. Geben Sie im Feld **In dieser Spalte anzeigen** den Wert **Anmeldenummer** ein und wählen Sie ihn aus, wenn er in der Liste unter **Benutzer** angezeigt wird.

1. Klicken Sie erneut auf **Spalte hinzufügen**.
1. Geben Sie im Feld **In der Spalte anzeigen** den Wert **Letztes Anmeldedatum** ein und wählen Sie ihn aus, wenn er in der Liste unter **Benutzer** angezeigt wird.

1. (Optional) Klicken Sie auf **Erweiterte Optionen** und wählen Sie dann im Dropdownmenü ein **Feldformat** aus, um die Uhrzeit oder den Wochentag der letzten Anmeldung in Ihrer Spalte einzuschließen.

1. Klicken Sie auf **Ansicht speichern**.\
   Die Ansicht enthält Informationen dazu, wie oft sich die Benutzer angemeldet haben und wann sie sich zuletzt angemeldet haben.
