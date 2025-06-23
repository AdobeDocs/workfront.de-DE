---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Stundentypen und Verfügbarkeit definieren
description: Ein Stundentyp ist eine Bezeichnung, mit der Sie Zeiteinträge kategorisieren können. Je nach den Berichtsanforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 0%

---

# Stundentypen und Verfügbarkeit definieren

<!--Audited: 6/2025-->

Ein Stundentyp ist eine Bezeichnung, mit der Sie Zeiteinträge kategorisieren können. Je nach den Berichtsanforderungen Ihres Unternehmens für Stunden kann dies ein wesentlicher Teil der Protokollierungszeit sein.

In Adobe Workfront gibt es zwei Gruppen von Stundentypen:

* **Allgemeine Stunden**: Stunden, die keinem Projekt zugeordnet sind, z. B. Krankenstand oder Administration. Sie können nur allgemeine Stunden auf der Arbeitszeittabelle protokollieren.
* **Projektspezifische Stunden**: Stunden, die für Projekte, Aufgaben und Probleme protokolliert wurden. Sie können projektspezifische Stunden von jedem Ort aus protokollieren, an dem Sie die Zeit erfassen können.

Beim Protokollieren der Zeit in Workfront hängen die verfügbaren projektspezifischen Stundentypen von den Konfigurationsoptionen ab, die auf System-, Projekt- und Benutzerebene festgelegt werden. (Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar: Projektzeit, Aufgabenzeit und Anfragezeit.)

Die Stundentypen, die bei der Protokollierung der Zeit (für Projekte, Aufgaben und Probleme) ausgewählt werden können, werden zunächst durch die Stundentypen bestimmt, die vom Systemadministrator systemweit zur Verfügung gestellt werden, und dann durch die Stundentypen, die auf Projekt- und Benutzerebene ausgewählt werden.

Nachdem die entsprechenden Stundentypen konfiguriert wurden, können Sie die Zeit an mehreren Stellen in Workfront protokollieren. Weitere Informationen finden Sie unter [Zeit erfassen](../../timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p> 
   <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministratorzugriff zur Definition systemweiter Stundentypen und zur Bearbeitung aller Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten des Zugriffs auf das Projekt, um Stundentypen für ein Projekt zu definieren</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definieren der Verfügbarkeit auf Systemebene

Der Systemadministrator bestimmt, welche projektspezifischen Stundentypen systemweit zur Verfügung gestellt werden. Weitere Informationen finden Sie unter [Verwalten von Stundentypen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definieren der Verfügbarkeit auf Projektebene {#define-availability-at-the-project-level}

Der Projektbesitzer bestimmt, ob alle auf Systemebene definierten Stundentypen für das Projekt (und die Aufgaben und Probleme innerhalb des Projekts) verfügbar sind oder ob nur eine Teilmenge dieser Stundentypen verfügbar ist.

{{step1-to-projects}}

1. Wählen **auf** Seite „Projekte“ das Projekt aus, für das Sie die Verfügbarkeit von Stundentypen bestimmen möchten.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) neben dem Projektnamen in der Kopfzeile und dann auf **Bearbeiten**. Das Bedienfeld **Projekt bearbeiten** wird geöffnet.

1. Suchen Sie im **Projekteinstellungen** die Einstellung **Stundentypen filtern**.

1. Wählen **Nein**, um alle projektspezifischen Stundentypen für das Projekt verfügbar zu machen.

   Oder

   Wählen Sie **Ja**, um nur eine Teilmenge der projektspezifischen Stundentypen für das Projekt verfügbar zu machen, und wählen Sie dann die **Stundentypen**, die Sie verfügbar machen möchten. Sie können mehrere Stundentypen auswählen.

   >[!NOTE]
   >
   >   Beachten Sie Folgendes:
   >   
   >   * Wenn Sie **Ja** auswählen, stehen nur die ausgewählten Stundentypen zur Auswahl, wenn Stunden für das Projekt (oder für Aufgaben und Probleme innerhalb des Projekts) protokolliert werden.
   >   
   >   * Wenn Sie **Ja** und keine Stundentypen auswählen, zeigt das Projekt nur allgemeine Stundentypen an.
   >
   >   * Dieselben Auswahlen müssen auf der Ebene der einzelnen Benutzer vorgenommen werden, damit diese Stundentypoptionen im Projekt angezeigt werden.
   >
   >   * Wenn der Standardstundentyp des Benutzers und ein projektgefilterter Stundentyp übereinstimmen, wird dieser Stundentyp beim Protokollieren der Zeit standardmäßig ausgewählt.

1. Klicken Sie auf **Speichern**.

## Definieren der Verfügbarkeit auf Benutzerebene

Sie können Stunden für einen bestimmten Stundentyp nur dann für Projekte, Aufgaben und Probleme protokollieren, wenn dieser Stundentyp auf System-, Projekt- und Benutzerebene verfügbar gemacht wurde.

Wenn Sie einen Stundentyp wie in diesem Abschnitt beschrieben auf Benutzerebene verfügbar machen, diesen Stundentyp jedoch beim Protokollieren der Zeit für ein Projekt, eine Aufgabe oder ein Problem nicht sehen, wurde dieser Stundentyp nicht für das Projekt verfügbar gemacht. Weitere Informationen finden Sie im folgenden Abschnitt in diesem Artikel: [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level).

So definieren Sie die Stundentypen, die einem Benutzer zur Verfügung stehen:

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront und dann auf Ihren Benutzeravatar in der linken oberen Ecke.

   Oder

   Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/adobe-main-menu.png) in der oberen rechten Ecke (falls verfügbar) und dann auf **Workfront-Profil**.

1. Klicken Sie auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) neben dem Benutzernamen und dann auf **Bearbeiten**. Das **Person bearbeiten** wird geöffnet.

   >[!IMPORTANT]
   >
   >Andere Benutzer können nur von Systemadmins bearbeitet werden. Wenn Sie über eine Planlizenz verfügen, können Sie die Stundentypen in Ihrem eigenen Profil bearbeiten.


1. Führen Sie im **Ressourcenplanung** im Dropdown-Menü **Verfügbare Stundentypen** einen der folgenden Schritte aus, je nachdem, welche Stundentypen bei der Zeitprotokollierung für ein Projekt, eine Aufgabe oder ein Problem verfügbar gemacht werden sollen:

   * **Um alle Stundentypen für den Benutzer verfügbar zu machen** wählen Sie alle Stundentypen aus.\
     Wenn Sie alle Stundentypen deaktiviert lassen, ist dies technisch dasselbe wie die Auswahl aller Stundentypen. In diesem Fall sind jedoch alle Stundentypen für den Benutzer nur bei Projekten, Aufgaben und Problemen verfügbar, bei denen **Nein** in der Option **Stundentypen filtern** ausgewählt ist, wenn das Projekt bearbeitet wird, wie unter [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level).
   * **Um nur eine Teilmenge der Stundentypen für den Benutzer verfügbar zu machen** wählen Sie nur die Stundentypen aus, die Sie verfügbar machen möchten.

     Damit die von Ihnen auf Benutzerebene ausgewählten Stundentypen für Projekte, Aufgaben und Probleme verfügbar sind, müssen dieselben Stundentypen auch bei der Bearbeitung des Projekts in der Option **Stundentypen filtern** ausgewählt werden, wie in [Definieren der Verfügbarkeit auf Projektebene](#define-availability-at-the-project-level) beschrieben.

1. (Optional) Wählen Sie **Dropdown-Menü** Standardstundentyp) einen Stundentyp aus. Wenn der Benutzer-Standardstundentyp und ein projektgefilterter Stundentyp übereinstimmen, wird dieser Stundentyp beim Protokollieren der Zeit standardmäßig ausgewählt.

1. Klicken Sie **Änderungen speichern**. Wenn Sie jetzt Stunden für ein Projekt, eine Aufgabe oder ein Problem protokollieren, sind die ausgewählten Stundentypen verfügbar, wenn dieselben Stundentypen auf Projektebene verfügbar gemacht wurden.

## So arbeiten Stundentypen auf Benutzerebene und auf Projektebene zusammen

In der folgenden Liste wird beschrieben, welche Stundentypen für ein Objekt angezeigt werden, nachdem Sie beim Protokollieren der Zeit für das Objekt sowohl die Stundentypen auf Benutzerebene als auch die Stundentypen auf Projektebene angepasst und gefiltert haben:

* Nachdem Sie den Standardstundentyp für den Benutzer und die gefilterten Projektstundentypen angepasst haben, zeigt das Dropdown-Menü Stundentyp einen der folgenden Stundentypen an:

   * Wenn der/die Benutzende einen Standardstundentyp in seinem/ihrem Profil hat und das Projekt denselben gefilterten Stundentyp hat, wird dieser Stundentyp als ausgewählter Standard angezeigt, wenn die Zeit protokolliert wird. Projekt, Aufgabe oder Problemzeit werden als zusätzliche Optionen angezeigt.

   * Wenn der/die Benutzende keinen standardmäßigen Stundentyp hat und das Projekt gefilterte Stundentypen hat, sind der standardmäßige Stundentyp bei der Zeitprotokollierung Projekt, Aufgabe oder Problemzeit, aber die gefilterten Stundentypen aus dem Projekt werden auch als zusätzliche Optionen angezeigt.

   * Wenn der/die Benutzende keinen Standardstundentyp hat und das Projekt keine gefilterten Stundentypen hat, werden nur die Stundentypen „Projekt“, „Aufgabe“ oder „Problemzeit“ als Standardstundentypen angezeigt, je nachdem, zu welchem Objekt Sie Zeit protokollieren.

   * Wenn der/die Benutzende einen Standardstundentyp hat und das Projekt keine gefilterten Stundentypen hat, werden das Projekt, die Aufgabe oder die Problemzeit beim Protokollieren der Zeit auf den Objekten als Standardstundentypen angezeigt, und es sind keine anderen Stundentypen als Optionen verfügbar, einschließlich des Standardstundentyps des/r Benutzenden.

* Nachdem Sie die Stundentypen angepasst und die verfügbaren Stundentypen für Ihren Benutzer definiert oder die Stundentypen für ein Projekt gefiltert haben, sind die folgenden Szenarien vorhanden:

   * Wenn Sie alle Stundentypen für das Feld Verfügbarer Stundentyp im Benutzerprofil ausgewählt haben und die Stundentypen des Projekts nicht gefiltert werden, werden beim Protokollieren der Zeit alle verfügbaren Stundentypen angezeigt.
   * Wenn Sie nur eine Teilmenge von Stundentypen für das Feld Verfügbarer Stundentyp im Profil Ihres Benutzers ausgewählt haben und die Stundentypen des Projekts nicht gefiltert werden, sehen Sie beim Protokollieren der Zeit nur die Stundentypen des Benutzers.
   * Wenn Sie alle Stundentypen für das Feld Verfügbarer Stundentyp im Benutzerprofil ausgewählt haben und die Stundentypen des Projekts gefiltert werden, sehen Sie je nach Objekt nur die Stundentypen des Projekts und die standardmäßigen Stundentypen wie Projektzeit, Aufgabenzeit, Problemzeit.
   * Wenn Sie im Profil Ihres Benutzers nur eine Untergruppe von Stundentypen für das Feld Verfügbarer Stundentyp ausgewählt haben und die Stundentypen des Projekts gefiltert werden, sehen Sie nur die Stundentypen, die für den Benutzer und das Projekt gelten. Wenn Benutzende und Projekt keine Stundentypen gemeinsam haben, werden nur die standardmäßigen Stundentypen angezeigt (Projektzeit, Aufgabenzeit, Problemzeit).

>[!TIP]
>
>   Wenn Sie für ein Objekt einen anderen Stundentyp als den Standardstundentyp auswählen, bleibt der Stundentyp erhalten. Wenn Sie sich das nächste Mal für dasselbe Objekt anmelden, wird für den Stundentyp automatisch der zuletzt ausgewählte verwendet.

