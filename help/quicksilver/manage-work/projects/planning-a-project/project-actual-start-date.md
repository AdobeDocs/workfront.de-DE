---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das tatsächliche Startdatum des Projekts
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Übersicht über das tatsächliche Startdatum des Projekts

Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe für das Projekt als In Bearbeitung markiert oder abgeschlossen wurde.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

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

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Workfront und dann auf **Projekte**.
1. Klicken Sie auf das Projekt, für das Sie das tatsächliche Startdatum anzeigen möchten.
1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Abschnitt **Übersicht**.

   Das tatsächliche Startdatum wird zusammen mit anderen Projektdaten angezeigt.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
