---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das tatsächliche Startdatum des Projekts
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Übersicht über das tatsächliche Startdatum des Projekts

Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.

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
   <td><p>Licht oder höher</p> 
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zu tatsächlichen Startdaten in Workfront

* Das tatsächliche Startdatum befindet sich im Abschnitt Details von Projekten, Aufgaben und Problemen. 
* Das tatsächliche Startdatum eines Projekts, einer Aufgabe oder eines Problems wird beim Erstellen dieser Elemente nicht angegeben.
* Das tatsächliche Startdatum wird zu Beginn der eigentlichen Arbeit an dem Projekt, der Aufgabe oder dem Problem angegeben.
* Das tatsächliche Startdatum wird nicht auf der Registerkarte Projektdetails angezeigt, wenn die Arbeit am Projekt noch nicht begonnen hat.

  Das tatsächliche Startdatum wird auf den Registerkarten „Aufgabe“ und „Problemdetails“ leer angezeigt, wenn die Arbeit daran noch nicht begonnen hat.

* Sie können das tatsächliche Startdatum einer Aufgabe oder eines Problems manuell ändern, aber nicht das tatsächliche Startdatum eines Projekts.

## Überlegungen zu tatsächlichen Startdaten für Projekte

* Workfront legt automatisch das tatsächliche Datum eines Projekts fest, wenn eine der folgenden Situationen eintritt:

   * Ein Aufgabenbevollmächtigter ändert den Status einer Aufgabe von *Neu* in einen anderen Status, der nicht *Neu* entspricht.

   * Ein Aufgabenbevollmächtigter ändert den Bereich „Prozent abgeschlossen“ einer Aufgabe.

     >[!IMPORTANT]
     >
     >Das tatsächliche Startdatum des Projekts wird nicht angezeigt, wenn das Projekt als aktuell markiert ist. Die tatsächliche Arbeit an den Aufgaben des Projekts muss beginnen, bevor das tatsächliche Startdatum des Projekts angegeben wird.

     In diesen Fällen wird das tatsächliche Startdatum des Projekts auf das Datum und die Uhrzeit festgelegt, zu der diese Aktionen für die früheste Aufgabe im Projekt stattgefunden haben. Dies zeigt an, dass das Projekt tatsächlich an diesem Datum und zu dieser Uhrzeit gestartet wurde.

## Suchen des tatsächlichen Startdatums eines Projekts

Sie können das tatsächliche Startdatum eines Projekts in den folgenden Bereichen ermitteln:

* Im Abschnitt Details eines Projekts.
* Fügen Sie in einem Projektbericht oder einer Projektansicht das tatsächliche Startdatum für das Projektobjekt in den Bericht ein.

  Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So suchen Sie das tatsächliche Startdatum im Abschnitt Details des Projekts:

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Workfront und dann auf **Projekte**.
1. Klicken Sie auf das Projekt, für das Sie das tatsächliche Startdatum anzeigen möchten.
1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Abschnitt **Übersicht**.

   Das tatsächliche Startdatum wird zusammen mit anderen Projektdaten angezeigt.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)


