---
title: Anzeigen von Benutzeranmeldeinformationen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Sie können sehen, wie oft sich Benutzende bei Workfront angemeldet haben und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass diese Informationen in der Ansicht einer Benutzerliste oder in einem Bericht für Benutzende enthalten sein sollen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f8d04790caefd12c9811ea3ed94e1f892311d031
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# Benutzeranmeldeinformationen anzeigen

Sie können sehen, wie oft sich Benutzende bei Adobe Workfront angemeldet haben und wann sie sich zuletzt angemeldet haben, indem Sie angeben, dass diese Informationen in der Ansicht einer Benutzerliste oder in einem Bericht für Benutzende enthalten sein sollen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wie Workfront Anmeldeinformationen aufzeichnet

Workfront zeichnet die folgenden Informationen über Benutzer auf, die sich beim System anmelden:

* **Anzahl der Anmeldungen**: Workfront zählt eine Benutzerin oder einen Benutzer, die bzw. der sich alle 24 Stunden bei der Anwendung anmeldet. Wenn sich ein(e) Benutzende(r) mehrmals mit verschiedenen Browsern, Computern oder Mobilgeräten anmeldet, zählt Workfront alle an einem Tag erfolgten Anmeldungen als eine Anmeldung. Die Anzahl der Anmeldungen enthält Informationen, die mit dem Zeitpunkt beginnen, zu dem der Benutzer erstellt wurde.
* **Letztes Anmeldedatum**: Das letzte Datum, an dem sich ein Benutzer angemeldet hat. Das Datum jeder Anmeldung über einen Browser, ein Mobilgerät oder eine andere Anwendung wird in diesem Feld aufgezeichnet.

Die Anmeldung bei Workfront auf eine der folgenden Arten zählt als Anmeldung bei Workfront:

* Die Workfront-Webanwendung
* Die Workfront Mobile Apps (iOS- oder Android-Geräte)
* Jede unterstützte Workfront-Integration mit einer anderen Drittanbieteranwendung (z. B. Slack)
* Jede benutzerdefinierte Integration zwischen Workfront und einer anderen Drittanbieteranwendung.
* Die Workfront-API

  >[!NOTE]
  >
  >Die Anmeldung bei Workfront über die Workfront-API ist nur für Organisationen verfügbar, die noch nicht in die Adobe Business-Plattform integriert wurden.

## Anzeigen von Nutzungsinformationen in einer Benutzerliste oder einem Bericht

Sie können die Felder Anmeldeanzahl und Letztes Anmeldedatum in der Ansicht einer Benutzerliste oder in einem Bericht für Benutzer anzeigen.\
Weitere Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So zeigen Sie Nutzungsinformationen in der Ansicht einer Benutzerliste an:

1. Navigieren Sie zu einer Benutzerliste in Workfront.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Klicken **unten rechts** Bildschirm auf „Spalte hinzufügen“.
1. Beginnen Sie im Feld **In dieser Spalte anzeigen** mit der Eingabe **Anmeldeanzahl** und wählen Sie es aus, wenn es in der Liste unter &quot;**&quot;**.

1. Klicken Sie erneut auf **Spalte hinzufügen**.
1. Beginnen Sie im Feld **In der Spalte anzeigen** mit der Eingabe **Letztes Anmeldedatum** und wählen Sie es aus, wenn es in der Liste unter **Benutzer** angezeigt wird.

1. (Optional) Klicken Sie **Erweiterte Optionen** und wählen Sie dann aus dem **-Menü ein** Feldformat“ aus, um die Uhrzeit oder den Wochentag der letzten Anmeldung in Ihre Spalte aufzunehmen.

1. Klicken Sie auf **Ansicht speichern**.\
   Die Ansicht enthält Informationen darüber, wie oft sich die Benutzer angemeldet haben und wann sie sich zuletzt angemeldet haben.
