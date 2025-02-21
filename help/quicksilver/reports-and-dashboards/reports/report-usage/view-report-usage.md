---
product-area: reporting
navigation-topic: report-usage
title: Berichtsnutzung anzeigen
description: Berichtsnutzung anzeigen
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 1%

---

# Berichtsnutzung anzeigen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Um zu verstehen, wie häufig Berichte in Ihrem System verwendet werden, können Sie die folgenden Informationen in einer Liste von Berichten anzeigen:

* Letzte 10 Benutzer, die den Bericht angesehen haben
* Anzeigen der Anzahl innerhalb eines bestimmten Zeitraums

  >[!NOTE]
  >
  >Adobe Workfront zählt eine Ansicht pro Benutzerin bzw. Benutzer pro Tag. Wenn Sie mehrmals am Tag auf denselben Bericht zugreifen, zählt Workfront dies als eine Ansicht für diesen Bericht. Wenn derselbe Bericht von einem anderen Benutzer am selben Tag aufgerufen wird, zählt Workfront dies als neue Ansicht für den zweiten Benutzer.

* Zuletzt angezeigt am
* Zuletzt angezeigt von Benutzer
* Eine Liste der Dashboards, die den Bericht enthalten\
  Weitere Informationen zum Anzeigen des Namens der Dashboards, denen Berichte in einer Liste von Berichten hinzugefügt werden können, finden Sie im Artikel [So organisieren Sie Berichte in einem Dashboard](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Sie können eine Ansicht für eine Liste von Berichten erstellen, in der Sie diese Informationen anzeigen können.\
Sie können eine Liste von Berichten nach einigen dieser Felder filtern.\
Weitere Informationen dazu, nach welchen Feldern Sie einen Bericht filtern können, finden Sie im Artikel [Filtern einer Berichtsliste nach Nutzungsinformationen](#filter-a-report-list-by-usage-information).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Anzeigen von Berichtverwendungsinformationen in der Ansicht einer Berichtsliste

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Workfront und dann auf **Berichte**.

1. Klicken Sie in der Berichtsliste auf das **Anzeigen** Dropdown-Menü.
1. (Optional) Wählen Sie die Ansicht **Berichtsnutzung**, um die häufigsten Berichtverwendungsinformationen anzuzeigen.\
   Oder

1. Klicken Sie **Neue Ansicht**, um eine benutzerdefinierte Ansicht zu erstellen.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Beginnen Sie mit der Eingabe eines der folgenden Felder und wählen Sie sie aus, wenn sie in der Liste unter dem **Berichtobjekt** angezeigt werden, um sie zu einer neuen Spalte hinzuzufügen:

   * **Letzte 10 Benutzer**: Zeigt die Namen der letzten 10 Benutzer an, die den Bericht angesehen haben.
   * **Ansichten**: Zeigt die Anzahl der Ansichten innerhalb eines der folgenden Zeitrahmen an:

      * **Diesen Monat, Quartal, Jahr**
      * **Letzter Monat, Quartal, Jahr**
      * **Alle Ansichten**: Zeigt eine Gesamtanzahl für alle Ansichten im Bericht an

   * **Zuletzt angezeigt von**: Zeigt Informationen zum Benutzer an, der den Bericht zuletzt angezeigt hat
   * **Zuletzt angezeigt am**: Zeigt das Datum an, an dem der Bericht zuletzt angezeigt wurde

1. Klicken Sie auf **Ansicht speichern**.\
   Die Nutzungsinformationen des Berichts werden in den Spalten angezeigt, die Sie der Ansicht hinzugefügt haben.\
   Sie können auch einen Bericht für das Berichtsobjekt erstellen und diese Ansicht im Bericht verwenden.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Sie müssen Bearbeitungszugriff auf Berichte in Ihrer Zugriffsebene haben, um einen Bericht zu erstellen.\
   Weitere Informationen zum Zugriff auf Berichte finden Sie im Artikel [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Filtern einer Berichtsliste nach Nutzungsinformationen {#filter-a-report-list-by-usage-information}

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Workfront und dann auf **Berichte**.
1. Klicken Sie in der Berichtsliste auf das **Filter** Dropdown-Menü.
1. Klicken Sie **Neuer Filter** und dann auf **Filterregel hinzufügen**.
1. Beginnen Sie mit der Eingabe eines der folgenden Felder und wählen Sie sie aus, wenn sie in der Liste unter dem **Berichtsobjekt** angezeigt werden, um sie als neue Filterregel hinzuzufügen:

   * **Ansichten**: Zeigt die Anzahl der Ansichten innerhalb eines der folgenden Zeitrahmen an:

      * **Diesen Monat, Quartal, Jahr**
      * **Letzter Monat, Quartal, Jahr**
      * **Alle Ansichten**

   * **Zuletzt angezeigt von**: Zeigt Informationen zum Benutzer an, der den Bericht zuletzt angezeigt hat
   * **Zuletzt angezeigt am**: Zeigt das Datum an, an dem der Bericht zuletzt angezeigt wurde

1. Wählen Sie einen Modifikator für Ihr Feld aus und geben Sie bei Aufforderung einen Wert an.\
   ![Filterstatistiken zur Berichtsnutzung](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klicken Sie auf **Filter speichern**.\
   Dadurch wird eine Liste von Berichten angezeigt, die den von Ihnen definierten Nutzungsinformationen entsprechen.\
   Sie können auch einen Bericht für das Berichtsobjekt erstellen und diesen Filter im Bericht verwenden.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Sie müssen Bearbeitungszugriff auf Berichte in Ihrer Zugriffsebene haben, um einen Bericht zu erstellen.\
   Weitere Informationen zum Zugriff auf Berichte finden Sie im Artikel [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Ausnahmen beim Anzeigen von Berichtverwendungsinformationen

>[!IMPORTANT]
>
>Die Berichtverwendungsinformationen werden seit März 2018 erfasst. Informationen, die vor diesem Datum liegen, sind nicht verfügbar.

Im Folgenden finden Sie einige Ausnahmen, die bei der Arbeit mit Informationen zur Berichtsnutzung zu beachten sind:

* Jedes Mal, wenn ein Bericht auf einem Dashboard oder einer benutzerdefinierten Registerkarte angezeigt wird, wird er als eine Ansicht gezählt. Der Benutzer, der diesen Bericht auf seinem Dashboard anzeigt, wird als „Zuletzt angezeigt von: Benutzername“ angezeigt und das Datum, an dem das Dashboard angezeigt wurde, wird als „Zuletzt angezeigt am“ angezeigt.
* Workfront erfasst keine Nutzungsinformationen für integrierte Berichte.\
  Weitere Informationen zu integrierten Berichten in Workfront finden Sie im Artikel [Verwenden von integrierten Berichten in Adobe Workfront](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront erfasst keine Nutzungsinformationen zu bereitgestellten Berichten. Ein zugestellter Bericht zählt nicht als eine Ansicht.\
  Weitere Informationen über bereitgestellte Berichte finden Sie im Artikel [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Wenn sich ein System- oder Gruppenadministrator als ein anderer Benutzer anmeldet, werden die Ansichten für den System- oder Gruppenadministrator gezählt und mit ihm verknüpft.
* Workfront erfasst keine Nutzungsinformationen für Berichte nach benutzerdefinierten Quartalen. In den Feldern zur Berichtsnutzung wird nur auf die standardmäßigen integrierten Quartale verwiesen.
* Workfront erfasst keine Nutzungsinformationen für Berichte, die freigegeben und öffentlich angezeigt werden. Wenn ein öffentlicher Bericht von jemandem angezeigt wird, ohne sich bei Workfront anzumelden, werden die Berichtsansichten nicht gezählt.\
  Weitere Informationen zum Freigeben von Berichten finden Sie im Artikel [Freigeben eines Berichts in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
