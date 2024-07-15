---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definieren von Stundentypen und Verfügbarkeit
description: Ein Stündentyp ist eine Bezeichnung, mit der Sie die Zeiteingabe kategorisieren können. Je nach den Reporting-Anforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Definieren von Stundentypen und Verfügbarkeit

Ein Stündentyp ist eine Bezeichnung, mit der Sie die Zeiteingabe kategorisieren können. Je nach den Reporting-Anforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.

In Adobe Workfront gibt es zwei Stundentypen:

* **Allgemeine Stunden:** Stunden, die nicht mit einem Projekt verbunden sind, wie z. B. Krankheitszeit oder Administration. Sie können allgemeine Stunden nur auf dem Timesheet protokollieren.
* **Projektspezifische Stunden:** Stunden, die bei Projekten, Aufgaben und Problemen protokolliert werden. Sie können projektspezifische Stunden von jedem Ort aus protokollieren, an dem Sie die Zeit protokollieren können.

Bei der Protokollierung der Zeit in Workfront hängen die projektspezifischen Stundentypen, die verfügbar sind, von den Konfigurationsoptionen ab, die auf System-, Projekt- und Benutzerebene festgelegt werden. (Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar: Projektzeit, Aufgabenzeit und Problemzeit.)

Die Stundentypen, die bei der Protokollierung (bei Projekten, Aufgaben und Problemen) ausgewählt werden können, werden zuerst durch die vom Systemadministrator systemweit verfügbaren Stundentypen und anschließend durch die auf Projekt- und Benutzerebene ausgewählten Stundentypen bestimmt.

Nachdem die entsprechenden Stundentypen konfiguriert wurden, können Sie die Zeit von mehreren Positionen in Workfront protokollieren, wie unter [Protokollzeit](../../timesheets/create-and-manage-timesheets/log-time.md) beschrieben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
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

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Verfügbarkeit auf Systemebene definieren

Der Systemadministrator bestimmt, welche projektspezifischen Stundentypen systemweit zur Verfügung gestellt werden, wie unter [Verwalten von Stundentypen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) beschrieben.

## Definieren der Verfügbarkeit auf Projektebene {#define-availability-at-the-project-level}

Der Projektinhaber bestimmt, ob alle auf Systemebene definierten Stundentypen für das Projekt verfügbar sind (sowie Aufgaben und Probleme innerhalb des Projekts) oder ob nur eine Untergruppe dieser Stundentypen verfügbar ist.

1. Wechseln Sie zu dem Projekt, in dem Sie die Verfügbarkeit von Stundentypen ermitteln möchten.
1. Klicken Sie auf das Menü **Mehr** neben dem Aufgabennamen und dann auf **Bearbeiten**.

1. Klicken Sie auf **Projekt bearbeiten**.
1. Suchen Sie im Abschnitt **Einstellungen** die Option **Filter Hour Types** .

1. Wählen Sie **Nein** aus, um alle projektspezifischen Stundentypen für das Projekt verfügbar zu machen.

   Oder

   Wählen Sie &quot;**Ja**&quot;, um nur eine Untergruppe der projektspezifischen Stundentypen für das Projekt verfügbar zu machen, und wählen Sie dann die Stundentypen aus, die Sie verfügbar machen möchten. (Halten Sie die Umschalttaste gedrückt, um mehrere Stundentypen auszuwählen.)

   Wenn Sie diese Option auswählen, stehen nur die ausgewählten Stundentypen zur Verfügung, die bei der Protokollierung von Stunden im Projekt (oder bei Aufgaben und Problemen im Projekt) ausgewählt werden. Wenn Sie diese Option auswählen und keine Stundentypen auswählen, zeigt das Projekt nur allgemeine Stundentypen an.

   Dieselbe Auswahl muss für jeden Benutzer getroffen werden, damit der Benutzer diese Stundenoptionen im Projekt sehen kann.

   Wenn der Standardstundentyp des Benutzers und ein Typ &quot;Gefilterte Stunde&quot;des Projekts übereinstimmen, wird dieser Stundentyp bei der Protokollierung standardmäßig ausgewählt.

1. Klicken Sie auf **Änderungen speichern**.

## Definieren der Verfügbarkeit auf Benutzerebene

Sie können Stunden für einen bestimmten Stundentyp nur dann für Projekte, Aufgaben und Probleme protokollieren, wenn dieser Stundentyp auf Systemebene, Projektebene und Benutzerebene verfügbar gemacht wurde.

Wenn Sie einen Stundentyp auf Benutzerebene verfügbar machen, wie in diesem Abschnitt beschrieben, Sie diesen Stundentyp jedoch bei der Protokollierung der Zeit für ein Projekt, eine Aufgabe oder ein Problem nicht sehen, wurde dieser Stundentyp für das Projekt nicht zur Verfügung gestellt (wie unter [Verfügbarkeit auf Projektebene definieren](#define-availability-at-the-project-level) beschrieben).

So definieren Sie die für einen Benutzer verfügbaren Stundentypen:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie in der linken oberen Ecke auf Ihren Benutzeravatar.
1. Klicken Sie auf das Menü **Mehr** neben dem Benutzernamen und dann auf **Bearbeiten**.

1. Nur ein Systemadministrator kann andere Benutzer bearbeiten. Wenn Sie über eine Planungslizenz verfügen, können Sie die Stundentypen in Ihrem eigenen Profil bearbeiten.
1. Führen Sie im Abschnitt **Ressourcenplanung** im Dropdown-Menü **Verfügbare Stündentypen** einen der folgenden Schritte aus, je nachdem, welche Stundentypen Sie verfügbar machen möchten, wenn Sie die Zeit für ein Projekt, eine Aufgabe oder ein Problem protokollieren:

   * **So stellen Sie alle Stundentypen für den Benutzer zur Verfügung:** Wählen Sie alle Stundentypen aus.\
     Wenn Sie alle Stundentypen deaktiviert lassen, ist dies technisch genauso wie die Auswahl aller Stundentypen. In diesem Fall sind jedoch alle Stundentypen für den Benutzer nur für Projekte, Aufgaben und Probleme verfügbar, bei denen **Nr.** bei der Bearbeitung des Projekts in der Option **Filterstündentypen** ausgewählt ist, wie in [Festlegen der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level) beschrieben.
   * **Um nur eine Teilmenge der Stundentypen für den Benutzer verfügbar zu machen:** Wählen Sie nur die Stundentypen aus, die verfügbar gemacht werden sollen.

     Damit die von Ihnen auf Benutzerebene ausgewählten Stundentypen für Projekte, Aufgaben und Probleme verfügbar sind, müssen diese Stundentypen auch bei der Bearbeitung des Projekts in der Option **Filterstündentypen** ausgewählt werden, wie in [Festlegen der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level) beschrieben.

1. (Optional) Wählen Sie im Dropdown-Menü **Standardstündentyp** den Typ &quot;Stunde&quot;aus.

   Wenn der Standardstundentyp des Benutzers und ein Typ &quot;Gefilterte Stunde&quot;des Projekts übereinstimmen, wird dieser Stundentyp bei der Protokollierung standardmäßig ausgewählt.

1. Klicken Sie auf **Änderungen speichern**.

   Wenn Sie jetzt Stunden für ein Projekt, eine Aufgabe oder ein Problem protokollieren, sind die von Ihnen ausgewählten Stundentypen verfügbar, wenn dieselben Stundentypen auf Projektebene verfügbar sind.


## Wie Stundentypen auf Benutzerebene und auf Projektebene zusammenarbeiten

In der folgenden Liste wird beschrieben, welche Stundentypen für ein Objekt angezeigt werden, nachdem Sie sowohl die Stundentypen auf Benutzerebene als auch die Stundentypen auf Projektebene angepasst und gefiltert haben, wenn Sie die Zeit für das Objekt protokollieren:

* Nachdem Sie den Standardstundentyp für den Benutzer und die gefilterten Typen der Projektstunde angepasst haben, zeigt das Dropdown-Menü &quot;Stündentyp&quot;einen der folgenden Stundentypen an:

   * Wenn der Benutzer in seinem Profil über einen Standardstundentyp verfügt und das Projekt denselben gefilterten Stündentyp aufweist, wird dieser Stündentyp bei der Protokollierung der Zeit als Standardeinstellung angezeigt. Für Projekt-, Aufgaben- oder Problemzeit werden zusätzliche Optionen angezeigt.

   * Wenn der Benutzer keinen Standardstundentyp hat und das Projekt gefilterte Stündentypen hat, lautet der Standardstündentyp bei der Protokollierung der Zeit Projekt-, Aufgaben- oder Problemzeit. Die gefilterten Stündentypen aus dem Projekt werden jedoch auch als zusätzliche Optionen angezeigt.

   * Wenn der Benutzer keinen Standardstundentyp hat und das Projekt keine gefilterten Stündentypen hat, werden je nach dem Objekt, für das Sie die Protokollierungszeit verwenden, nur die Stundentypen Projekt, Aufgabe oder Problemzeit als Standardwerte angezeigt.

   * Wenn der Benutzer über einen Standardstundentyp verfügt und das Projekt keine gefilterten Stündentypen hat, werden Projekt-, Aufgaben- oder Problem-APIme bei der Protokollierung der Zeit für die Objekte standardmäßig angezeigt. Es sind keine weiteren Stündentypen als Optionen verfügbar, einschließlich des Standardstundentyps des Benutzers.

* Nachdem Sie die Stunden-Typen angepasst und Verfügbare Stunden-Typen für Ihren Benutzer definiert oder die Stunden-Typen für ein Projekt gefiltert haben, gibt es die folgenden Szenarien:

   * Wenn Sie im Profil Ihres Benutzers alle Stundentypen für das Feld Verfügbarer Stunden-Typ ausgewählt haben und die Stundentypen des Projekts nicht gefiltert sind, werden bei der Protokollierung der Zeit alle verfügbaren Stundentypen angezeigt.
   * Wenn Sie im Profil Ihres Benutzers nur eine Untergruppe von Stundentypen für das Feld Verfügbarer Stündentyp ausgewählt haben und die Stündentypen des Projekts nicht gefiltert sind, sehen Sie nur die Stundentypen des Benutzers, wenn Sie die Zeit protokollieren.
   * Wenn Sie alle Stundentypen für das Feld &quot;Verfügbarer Stündentyp&quot;im Profil Ihres Benutzers ausgewählt haben und die Stündentypen des Projekts gefiltert sind, sehen Sie je nach Objekt nur die Stundentypen des Projekts und die Standardstundentypen wie Projektzeit, Aufgabenzeit und Problemzeit.
   * Wenn Sie im Profil Ihres Benutzers nur eine Untergruppe von Stundentypen für das Feld Verfügbarer Stündentyp ausgewählt haben und die Stündentypen des Projekts gefiltert sind, sehen Sie nur die für den Benutzer und das Projekt gemeinsamen Stundentypen. Wenn für den Benutzer und das Projekt keine gemeinsamen Stundentypen gelten, werden nur die Standardstundentypen angezeigt (Projektzeit, Aufgabenzeit, Problemzeit).

>[!TIP]
>
>   Wenn Sie für ein Objekt einen anderen Stunden-Typ und nicht den Standardstundentyp auswählen, wird der Stundentyp fixierbar. Wenn Sie die Zeit das nächste Mal für dasselbe Objekt anmelden, wird für den Typ Stunde automatisch der Typ ausgewählt, den Sie zuletzt ausgewählt haben.

