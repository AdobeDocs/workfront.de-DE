---
title: Berichte, Dashboards und Kalender freigeben
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Berichten, Dashboards und Kalendern, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter Zugriff auf Berichte, Dashboards und Kalender gewähren .
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Berichte, Dashboards und Kalender freigeben

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Berichten, Dashboards und Kalendern, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsstufe, die Benutzern gewährt wird, können Sie ihnen auch die Berechtigung zum Anzeigen oder Verwalten bestimmter Berichte, Dashboards oder Kalender erteilen, auf die Sie Zugriff haben. Informationen zum Gewähren von Berechtigungen für Benutzer, die Objekte freigeben, finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Berichte](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Überlegungen zur Freigabe eines Berichts, Dashboards oder Kalenders

Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

* Der Ersteller eines Berichts, Dashboards oder Kalenders verfügt standardmäßig über die Berechtigung Verwalten .
* Die Freigabe von Berichten, Dashboards und Kalendern erfolgt ähnlich wie die Freigabe anderer Objekte in Workfront.

  Weitere Informationen zum Freigeben von Objekten in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

  In den folgenden Artikeln erfahren Sie außerdem, wie Sie Berichte, Dashboards und Kalender freigeben:

   * [Bericht in Adobe Workfront freigeben](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dashboard freigeben](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Kalenderberichte freigeben](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* Sie können Berichte und Dashboards einzeln freigeben oder gemeinsam nutzen.

  Sie können Kalender nur einzeln freigeben. Sie können sie nicht gemeinsam nutzen.

* Sie können keine integrierten Systemberichte freigeben. Sie können nur benutzerdefinierte Berichte freigeben.

  Weitere Informationen zum Speichern eines Systemberichts als neuen benutzerdefinierten Bericht finden Sie unter [Erstellen einer Kopie eines Berichts](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

* Sie können die folgenden Berechtigungen für Berichte, Dashboards und Kalender gewähren:

   * Anzeigen

     ![](assets/screen-shot-2014-01-22-at-10.19.55-am.png)

   * Verwalten

     ![](assets/screen-shot-2014-01-22-at-10.20.13-am.png)

* Wenn Sie ein Dashboard freigeben, haben Benutzer standardmäßig Anzeigeberechtigungen für alle Berichte, Kalender und externen Seiten im Dashboard.
* Benutzer mit einer Anfragelizenz können keinen systemweiten Bericht anzeigen. Ein Bericht muss für die Anforderer einzeln freigegeben werden, wenn sie ihn anzeigen möchten.
* Wenn ein Bericht eine Eingabeaufforderung enthält und Sie ihn öffentlich freigeben, müssen die Benutzer, die auf den Bericht zugreifen, bei Workfront angemeldet sein, damit der Bericht über die Eingabeaufforderung ausgeführt werden kann. Wenn sie sich nicht bei Workfront anmelden können, wird der Bericht angezeigt, ohne dass eine Eingabeaufforderung darauf angewendet wird.\
  Weitere Informationen zu Einschränkungen bei der Freigabe von Berichten für Aufforderungen finden Sie im Abschnitt [Einschränkungen für die Freigabe erforderlicher Berichte](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) im Artikel [Eingabeaufforderung zu einem Bericht hinzufügen](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Sie können geerbte Berechtigungen aus einem Bericht oder Kalender entfernen.

  Weitere Informationen zum Entfernen von geerbten Berechtigungen aus Objekten finden Sie unter [Berechtigungen aus Objekten entfernen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

* Sie können auch einen Bericht oder einen Kalender öffentlich oder systemweit freigeben.

  Sie können ein Dashboard nicht öffentlich freigeben, aber systemweit freigeben.

  >[!CAUTION]
  >
  >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen für externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.
