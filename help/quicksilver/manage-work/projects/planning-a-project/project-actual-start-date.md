---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das tatsächliche Projektstartdatum
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront das tatsächliche Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe im Projekt als In Bearbeitung markiert oder abgeschlossen markiert wurde.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Übersicht über das tatsächliche Projektstartdatum

Projekte, Aufgaben und Probleme haben in Adobe Workfront das tatsächliche Startdatum. Bei Aufgaben und Problemen ist dies das Datum, an dem sie als In Bearbeitung markiert wurden. Bei Projekten ist dies das Datum, an dem die erste Aufgabe im Projekt als In Bearbeitung markiert oder abgeschlossen markiert wurde.

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum tatsächlichen Startdatum in Workfront

* Das tatsächliche Startdatum befindet sich im Abschnitt Details von Projekten, Aufgaben und Problemen. 
* Das tatsächliche Startdatum eines Projekts, einer Aufgabe oder eines Problems wird bei der Erstellung dieser Elemente nicht angegeben.
* Das tatsächliche Startdatum wird ausgefüllt, wenn die Arbeit tatsächlich mit dem Projekt, der Aufgabe oder dem Problem beginnt.
* Das tatsächliche Startdatum wird nicht auf der Registerkarte Projektdetails angezeigt, wenn die Arbeit am Projekt noch nicht begonnen hat.

   Das tatsächliche Startdatum wird auf den Registerkarten &quot;Aufgabe&quot;und &quot;Problemdetails&quot;leer angezeigt, wenn die Arbeit noch nicht begonnen hat.

* Sie können das tatsächliche Startdatum einer Aufgabe oder eines Problems manuell ändern, aber das tatsächliche Startdatum eines Projekts kann nicht geändert werden.

## Überlegungen zum tatsächlichen Startdatum für Projekte

* Workfront legt automatisch das tatsächliche Datum eines Projekts fest, an dem eines der folgenden Ereignisse eintritt:

   * Ein Aufgabenverantwortlicher ändert den Status einer Aufgabe von *Neu* zu jedem anderen Status hinzu, der nicht *Neu*.

   * Ein Aufgabenverantwortlicher ändert den &quot;Percent Complete&quot;einer Aufgabe.

      >[!IMPORTANT]
      >
      >Das tatsächliche Projektstartdatum wird nicht angezeigt, wenn das Projekt als &quot;Aktuell&quot;markiert ist. Die tatsächliche Arbeit muss mit den Aufgaben des Projekts beginnen, bevor das tatsächliche Anfangsdatum des Projekts eingetragen wird.

      In diesen Fällen wird das tatsächliche Anfangsdatum des Projekts auf das Datum und die Uhrzeit festgelegt, zu der diese Aktionen für die früheste Aufgabe des Projekts durchgeführt wurden. Dies bedeutet, dass das Projekt an diesem Datum und zu dieser Uhrzeit tatsächlich gestartet wurde.

## Tatsächliches Projektstartdatum ermitteln

Sie können das tatsächliche Startdatum eines Projekts in den folgenden Bereichen ermitteln:

* Im Bereich Details eines Projekts.
* Wenn Sie in einem Projektbericht oder einer Ansicht das tatsächliche Startdatum für das Objektprojekt zum Bericht hinzufügen.

   Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

So suchen Sie das tatsächliche Startdatum im Abschnitt Details des Projekts:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Projekte**.
1. Klicken Sie auf das Projekt, für das Sie das tatsächliche Startdatum anzeigen möchten.
1. Klicken **Projektdetails** Navigieren Sie im linken Bereich zu **Übersicht** Abschnitt.

   Das tatsächliche Startdatum wird zusammen mit anderen Projektdaten angezeigt.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
