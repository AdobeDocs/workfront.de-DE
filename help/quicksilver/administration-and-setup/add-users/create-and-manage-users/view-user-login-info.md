---
title: Anzeigen von Benutzeranmeldedaten
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können sehen, wie oft sich Benutzer bei Workfront anmelden und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass Sie diese Informationen in die Ansicht einer Benutzerliste oder in einen Benutzerbericht aufnehmen möchten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Anzeigen von Benutzeranmeldedaten

Sie können sehen, wie oft sich Benutzer bei Adobe Workfront anmelden und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass Sie diese Informationen in die Ansicht einer Benutzerliste oder in einen Benutzerbericht aufnehmen möchten.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzer-Admin</b> Optionen aktiviert unter <b>Einstellungen anpassen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## So erfasst Workfront Anmeldeinformationen

Workfront zeichnet die folgenden Informationen über Benutzer auf, die sich beim System anmelden:

* **Anzahl der Anmeldungen**: Workfront zählt einen Benutzer, der sich alle 24 Stunden bei der Anwendung anmeldet. Wenn sich ein Benutzer mehrmals mit verschiedenen Browsern, Computern oder Mobilgeräten anmeldet, zählt Workfront alle Anmeldungen, die an einem Tag stattgefunden haben, als eine Anmeldung. Die Anzahl der Anmeldungen umfasst Informationen, die mit dem Zeitpunkt der Erstellung des Benutzers beginnen.
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
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So zeigen Sie Nutzungsinformationen in der Ansicht einer Benutzerliste an:

1. Navigieren Sie zu einer Benutzerliste in Workfront.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Klicken **Spalte hinzufügen** in der rechten unteren Ecke des Bildschirms.
1. Im **In dieser Spalte anzeigen** Feld, Eingabe beginnen **Anzahl der Anmeldungen** und wählen Sie sie dann aus, wenn sie in der Liste unter **Benutzer**.

1. Klicken **Spalte hinzufügen** erneut.
1. Im **In Spalte anzeigen** Feld, Eingabe beginnen **Letztes Anmeldedatum** und wählen Sie sie dann aus, wenn sie in der Liste unter **Benutzer**.

1. (Optional) Klicken Sie auf **Erweiterte Optionen** und wählen Sie dann eine **Feldformat** aus dem Dropdown-Menü, um die Zeit oder den Wochentag der letzten Anmeldung in Ihre Spalte aufzunehmen.

1. Klicken **Ansicht speichern**.\
   Die Ansicht enthält Informationen dazu, wie oft sich die Benutzer angemeldet haben und wann sie sich zuletzt angemeldet haben.
