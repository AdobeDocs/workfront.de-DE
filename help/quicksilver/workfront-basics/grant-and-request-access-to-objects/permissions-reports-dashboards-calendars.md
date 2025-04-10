---
title: Berichte, Dashboards und Kalender freigeben
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Berichten, Dashboards und Kalendern, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter Gewähren des Zugriffs auf Berichte, Dashboards und Kalender.
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Berichte, Dashboards und Kalender freigeben

Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Berichten, Dashboards und Kalendern, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Berichte, Dashboards und Kalender finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Berichte, Dashboards oder Kalender gewähren, auf die Sie Zugriff haben. Informationen zum Gewähren von Berechtigungen für Benutzende für Objekte finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann.

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Problemen tun können, finden Sie im Abschnitt [Berichte](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Überlegungen zur Freigabe eines Berichts, Dashboards oder Kalenders

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

* Der Ersteller eines Berichts, Dashboards oder Kalenders hat standardmäßig Verwaltungsberechtigungen für ihn.
* Die Freigabe von Berichten, Dashboards und Kalendern ähnelt der Freigabe anderer Objekte in Workfront.

  Weitere Informationen zum Freigeben von Objekten in Workfront finden Sie unter [Freigeben eines ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

  In den folgenden Artikeln erfahren Sie außerdem, wie Sie Berichte, Dashboards und Kalender freigeben:

   * [Freigeben eines Berichts in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Freigeben eines Dashboards](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Kalenderbericht freigeben](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* Sie können Berichte und Dashboards einzeln oder zusammen freigeben.

  Kalender können nur einzeln freigegeben werden. Sie können sie nicht zusammen freigeben.

* Integrierte Systemberichte können nicht freigegeben werden. Sie können nur benutzerdefinierte Berichte freigeben.

  Weitere Informationen zum Speichern eines Systemberichts als neuen benutzerdefinierten Bericht finden Sie unter [Erstellen einer Berichtskopie](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

* Sie können die folgenden Berechtigungen für Berichte, Dashboards und Kalender gewähren:

   * Anzeigen
   * Verwalten

* Wenn Sie ein Dashboard freigeben, haben Benutzer standardmäßig Anzeigeberechtigungen für alle Berichte, Kalender und externen Seiten im Dashboard.
* Benutzende mit einer Anfragelizenz können keinen systemweiten Bericht anzeigen. Ein Bericht muss für die Antragsteller einzeln freigegeben werden, wenn sie ihn anzeigen müssen.
* Wenn ein Bericht eine Eingabeaufforderung enthält und Sie ihn öffentlich freigeben, müssen die Benutzenden, die auf den Bericht zugreifen, bei Workfront angemeldet sein, damit der Bericht über die Eingabeaufforderung ausgeführt werden kann. Wenn er sich nicht bei Workfront anmelden kann, wird der Bericht ohne die Eingabeaufforderung angezeigt.\
  Weitere Informationen zu den Einschränkungen bei der Freigabe von Berichten mit Eingabeaufforderungen finden Sie im Abschnitt [Einschränkungen bei der Freigabe ](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) Berichten) im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Sie können geerbte Berechtigungen aus einem Bericht oder Kalender entfernen.

  Weitere Informationen zum Entfernen geerbter Berechtigungen aus Objekten finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

* Sie können einen Bericht oder Kalender auch öffentlich oder systemweit freigeben.

  Sie können ein Dashboard nicht öffentlich freigeben, sondern systemweit.

  >[!CAUTION]
  >
  >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen an externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne ein Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.
