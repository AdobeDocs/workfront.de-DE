---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Festlegen von Stundentypen und Verfügbarkeit für Timesheets
description: Ein Stündentyp ist eine Bezeichnung, mit der Sie die Zeiteingabe kategorisieren können. Je nach den Reporting-Anforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# Festlegen von Stundentypen und Verfügbarkeit für Timesheets

Ein Stündentyp ist eine Bezeichnung, mit der Sie die Zeiteingabe kategorisieren können. Je nach den Reporting-Anforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.

In Adobe Workfront gibt es zwei Stundentypen:

* **Allgemeine Stunden:** Stunden, die nicht mit einem Projekt verbunden sind, wie z. B. Krankheitszeit oder Administration. Sie können allgemeine Stunden nur auf dem Timesheet protokollieren.
* **Projektspezifische Stunden:** Stunden bei Projekten, Aufgaben und Problemen protokolliert. Sie können projektspezifische Stunden von jedem Ort aus protokollieren, an dem Sie die Zeit protokollieren können.

Bei der Protokollierung der Zeit in Workfront hängen die projektspezifischen Stundentypen, die verfügbar sind, von den Konfigurationsoptionen ab, die auf System-, Projekt- und Benutzerebene festgelegt werden. (Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar: Projektzeit, Aufgabenzeit und Problemzeit.)

Die Stundentypen, die bei der Protokollierung (bei Projekten, Aufgaben und Problemen) ausgewählt werden können, werden zuerst durch die vom Systemadministrator systemweit verfügbaren Stundentypen und anschließend durch die auf Projekt- und Benutzerebene ausgewählten Stundentypen bestimmt.

Nachdem die entsprechenden Stundentypen konfiguriert wurden, können Sie die Zeit an mehreren Stellen in Workfront protokollieren, wie hier beschrieben: [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Systemadministratorzugriff zur Definition systemweiter Stundentypen und zur Bearbeitung aller Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten des Zugriffs auf das Projekt zur Definition von Stundentypen für ein Projekt</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Verfügbarkeit auf Systemebene definieren

Der Systemadministrator bestimmt, welche projektspezifischen Stundentypen systemweit zur Verfügung gestellt werden, wie im Abschnitt [Verwalten von Stundentypen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definieren der Verfügbarkeit auf Projektebene {#define-availability-at-the-project-level}

Der Projektinhaber bestimmt, ob alle auf Systemebene definierten Stundentypen für das Projekt verfügbar sind (sowie Aufgaben und Probleme innerhalb des Projekts) oder ob nur eine Untergruppe dieser Stundentypen verfügbar ist. 

1. Wechseln Sie zu dem Projekt, in dem Sie die Verfügbarkeit von Stundentypen ermitteln möchten.
1. Klicken Sie auf **Mehr** Menü neben dem Aufgabennamen und klicken Sie dann auf **Bearbeiten**.

1. Klicks **Projekt bearbeiten**.
1. Im **Einstellungen** -Abschnitt, suchen Sie die **Filtern von Stündentypen** -Option.

1. Auswählen **Nein** , um alle projektspezifischen Stundentypen für das Projekt verfügbar zu machen.

   Oder

   Auswählen **Ja** , um nur eine Untergruppe der projektspezifischen Stundentypen für das Projekt verfügbar zu machen, wählen Sie dann die Stundentypen aus, die verfügbar gemacht werden sollen. (Halten Sie die Umschalttaste gedrückt, um mehrere Stundentypen auszuwählen.)

   Wenn Sie diese Option auswählen, stehen nur die ausgewählten Stundentypen zur Verfügung, die bei der Protokollierung von Stunden im Projekt (oder bei Aufgaben und Problemen im Projekt) ausgewählt werden. Wenn Sie diese Option auswählen und keine Stundentypen auswählen, zeigt das Projekt nur allgemeine Stundentypen an.

   Dieselbe Auswahl muss für jeden Benutzer getroffen werden, damit der Benutzer diese Stundenoptionen im Projekt sehen kann.

1. Klicks **Änderungen speichern**.

## Definieren der Verfügbarkeit auf Benutzerebene

Sie können Stunden für einen bestimmten Stundentyp nur dann für Projekte, Aufgaben und Probleme protokollieren, wenn dieser Stundentyp auf Systemebene, Projektebene und Benutzerebene verfügbar gemacht wurde.

Wenn Sie auf Benutzerebene einen Stundentyp wie in diesem Abschnitt beschrieben verfügbar machen, diesen Stundentyp jedoch bei der Protokollierung der Zeit für ein Projekt, eine Aufgabe oder ein Problem nicht sehen, wurde dieser Stundentyp für das Projekt nicht zur Verfügung gestellt (wie beschrieben in [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level)).

So definieren Sie die für einen Benutzer verfügbaren Stundentypen:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront.

1. Klicken Sie in der linken oberen Ecke auf Ihren Benutzeravatar.
1. Klicken Sie auf **Mehr** Menü neben dem Benutzernamen und klicken Sie dann auf **Bearbeiten**.

1. Nur ein Systemadministrator kann andere Benutzer bearbeiten. Wenn Sie über eine Planungslizenz verfügen, können Sie die Stundentypen in Ihrem eigenen Profil bearbeiten.
1. Im **Ressourcenplanung** im Abschnitt **Verfügbare Stundentypen** im Dropdown-Menü eine der folgenden Aktionen ausführen, je nachdem, welche Stundentypen Sie verfügbar machen möchten, wenn Sie die Zeit für die Protokollierung in einem Projekt, einer Aufgabe oder einem Problem einsetzen:

   * **So stellen Sie alle Stundentypen für den Benutzer zur Verfügung:** Wählen Sie alle Stundentypen aus.\
     Wenn Sie alle Stundentypen deaktiviert lassen, ist dies technisch genauso wie die Auswahl aller Stundentypen. In diesem Fall sind jedoch alle Stundentypen nur für Projekte, Aufgaben und Probleme verfügbar, bei denen **Nein** wird im Feld **Filtern von Stündentypen** Option beim Bearbeiten des Projekts, wie unter [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level).
   * **So stellen Sie dem Benutzer nur eine Teilmenge der Stundentypen zur Verfügung:** Wählen Sie nur die Stundentypen aus, die verfügbar gemacht werden sollen.

     Damit die von Ihnen auf Benutzerebene ausgewählten Stundentypen für Projekte, Aufgaben und Probleme verfügbar sind, müssen diese Stundentypen auch im **Filtern von Stündentypen** Option beim Bearbeiten des Projekts, wie unter [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level).

1. Klicks **Änderungen speichern**.

   Wenn Sie jetzt Stunden für ein Projekt, eine Aufgabe oder ein Problem protokollieren, sind die von Ihnen ausgewählten Stundentypen verfügbar, wenn dieselben Stundentypen auf Projektebene verfügbar sind.


## Wie Stundentypen auf Benutzerebene und auf Projektebene zusammenarbeiten

In der folgenden Liste wird beschrieben, welche Stundentypen für ein Objekt angezeigt werden, nachdem Sie sowohl die Stundentypen auf Benutzerebene als auch auf Projektebene angepasst und gefiltert haben:

* Wenn Sie ein Objekt zum Protokollieren der Zeit öffnen, zeigt das Dropdown-Menü &quot;Stündentyp&quot;standardmäßig die Ihrem Benutzer zugeordneten Standardstundentypen an. Dies geschieht, wenn Sie Ihre Stundentypen nicht angepasst haben.

* Nachdem Sie die Stunden-Typen angepasst und Verfügbare Stunden-Typen für Ihren Benutzer definiert oder die Stunden-Typen für ein Projekt gefiltert haben, gibt es die folgenden Szenarien:

   * Wenn Sie im Profil Ihres Benutzers alle Stundentypen für das Feld Verfügbarer Stunden-Typ ausgewählt haben und die Stundentypen des Projekts nicht gefiltert sind, werden bei der Protokollierung der Zeit alle verfügbaren Stundentypen angezeigt.
   * Wenn Sie im Profil Ihres Benutzers nur eine Untergruppe von Stundentypen für das Feld Verfügbarer Stündentyp ausgewählt haben und die Stündentypen des Projekts nicht gefiltert sind, sehen Sie nur die Stundentypen des Benutzers, wenn Sie die Zeit protokollieren.
   * Wenn Sie im Profil Ihres Benutzers alle Stundentypen für das Feld Verfügbarer Stündentyp ausgewählt und die Stündentypen des Projekts gefiltert haben, werden je nach Objekt nur die Stundentypen des Projekts und die Standardstundentypen wie Projektzeit, Aufgabenzeit und Problemzeit angezeigt.
   * Wenn Sie im Profil Ihres Benutzers nur eine Untergruppe von Stundentypen für das Feld Verfügbarer Stündentyp ausgewählt haben und die Stündentypen des Projekts gefiltert sind, sehen Sie nur die für den Benutzer und das Projekt gemeinsamen Stundentypen. Wenn für den Benutzer und das Projekt keine gemeinsamen Stundentypen gelten, werden nur die Standardstundentypen angezeigt (Projektzeit, Aufgabenzeit, Problemzeit).

>[!TIP]
>
>   Wenn Sie für ein Objekt einen anderen Stunden-Typ und nicht den Standardstundentyp auswählen, wird der Stundentyp fixierbar. Wenn Sie die Zeit das nächste Mal für dasselbe Objekt anmelden, wird für den Typ Stunde automatisch der Typ ausgewählt, den Sie zuletzt ausgewählt haben.

