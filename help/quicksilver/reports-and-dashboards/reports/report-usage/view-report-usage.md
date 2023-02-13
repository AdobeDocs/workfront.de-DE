---
product-area: reporting
navigation-topic: report-usage
title: Berichtverwendung anzeigen
description: Berichtverwendung anzeigen
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Berichtverwendung anzeigen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

Um zu verstehen, wie intensiv Berichte in Ihrem System verwendet werden, können Sie die folgenden Informationen in einer Liste von Berichten anzeigen:

* Letzte 10 Benutzer, die den Bericht angezeigt haben
* Anzahl innerhalb eines bestimmten Zeitraums anzeigen

   >[!NOTE]
   >
   >Adobe Workfront zählt eine Ansicht pro Benutzer und Tag. Wenn Sie mehrmals täglich auf denselben Bericht zugreifen, zählt Workfront dies für Sie als eine Ansicht des Berichts. Wenn derselbe Bericht von einem anderen Benutzer am selben Tag aufgerufen wird, zählt Workfront dies als neue Ansicht für den zweiten Benutzer.

* Zuletzt angezeigt am
* Zuletzt von Benutzern angezeigt
* Eine Liste der Dashboards, die den Bericht enthalten\
   Weitere Informationen zur Anzeige des Namens der Dashboards, zu denen Berichte in einer Liste von Berichten hinzugefügt werden können, finden Sie im Artikel [So organisieren Sie Berichte in einem Dashboard](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

Sie können eine Ansicht für eine Liste von Berichten erstellen, in der Sie diese Informationen anzeigen können.\
Sie können eine Liste von Berichten nach einigen dieser Felder filtern.\
Weitere Informationen darüber, nach welchen Feldern ein Bericht gefiltert werden kann, finden Sie im Artikel [Berichtsliste nach Nutzungsinformationen filtern](#filter-a-report-list-by-usage-information).

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Berichtverwendungsinformationen in der Berichtansicht anzeigen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Klicken Sie in der Liste der Berichte auf die **Ansicht** Dropdown-Menü.
1. (Optional) Wählen Sie die **Nutzung von Berichten** angezeigt, um die häufigsten Berichtverwendungsinformationen anzuzeigen.\
   Oder

1. Klicken **Neue Ansicht** , um eine benutzerdefinierte Ansicht zu erstellen.
1. Klicken **Spalte hinzufügen**.
1. Beginnen Sie mit der Eingabe eines der folgenden Felder und wählen Sie sie aus, wenn sie in der Liste unter der **Bericht** -Objekt, um sie einer neuen Spalte hinzuzufügen:

   * **Letzte 10 Benutzer**: Zeigt die Namen der zehn letzten Benutzer an, die den Bericht angezeigt haben.
   * **Ansichten**: Zeigt die Anzahl der Ansichten in einem der folgenden Zeitrahmen an:

      * **Diesen Monat, Quartal, Jahr**
      * **Letzter Monat, Quartal, Jahr**
      * **Alle Ansichten**: Zeigt eine Gesamtanzahl aller Ansichten im Bericht an
   * **Zuletzt angezeigt von**: Zeigt Informationen über den Benutzer an, der den Bericht zuletzt angesehen hat
   * **Zuletzt angezeigtes Datum**: Zeigt das Datum der letzten Ansicht des Berichts an


1. Klicken **Ansicht speichern**.\
   Die Nutzungsinformationen zum Bericht werden in den Spalten angezeigt, die Sie der Ansicht hinzugefügt haben.\
   Sie können auch einen Bericht für das Berichtsobjekt erstellen und diese Ansicht im Bericht verwenden.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   Sie müssen Zugriff auf Berichte bearbeiten auf Ihrer Zugriffsebene haben, um einen Bericht zu erstellen.\
   Weitere Informationen zum Zugriff auf Berichte finden Sie im Artikel [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Berichtsliste nach Nutzungsinformationen filtern {#filter-a-report-list-by-usage-information}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.
1. Klicken Sie in der Liste der Berichte auf die **Filter** Dropdown-Menü.
1. Klicken **Neuer Filter** Klicken Sie auf **Filterregel hinzufügen**.
1. Beginnen Sie mit der Eingabe eines der folgenden Felder und wählen Sie sie aus, wenn sie in der Liste unter der **Bericht** -Objekt, um sie als neue Filterregel hinzuzufügen:

   * **Ansichten**: Zeigt die Anzahl der Ansichten in einem der folgenden Zeitrahmen an:

      * **Diesen Monat, Quartal, Jahr**
      * **Letzter Monat, Quartal, Jahr**
      * **Alle Ansichten**
   * **Zuletzt angezeigt von**: Zeigt Informationen über den Benutzer an, der den Bericht zuletzt angesehen hat
   * **Zuletzt angezeigtes Datum**: Zeigt das Datum der letzten Ansicht des Berichts an


1. Wählen Sie einen Modifikator für Ihr Feld aus und geben Sie dann einen Wert an, wenn Sie dazu aufgefordert werden.\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. Klicken **Filter speichern**.\
   Dadurch wird eine Liste von Berichten angezeigt, die den von Ihnen definierten Nutzungsinformationen entsprechen.\
   Sie können auch einen Bericht für das Berichtsobjekt erstellen und diesen Filter im Bericht verwenden.\
   Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Sie müssen Zugriff auf Berichte bearbeiten auf Ihrer Zugriffsebene haben, um einen Bericht zu erstellen.\
   Weitere Informationen zum Zugriff auf Berichte finden Sie im Artikel [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## Ausnahmen bei der Anzeige von Informationen zur Berichtsverwendung

>[!IMPORTANT]
>
>Die Nutzungsinformationen des Berichts wurden seit März 2018 erfasst. Informationen, die vor diesem Datum liegen, sind nicht verfügbar.

Im Folgenden finden Sie einige Ausnahmen, die Sie bei der Arbeit mit Berichtverwendungsinformationen beachten sollten:

* Jedes Mal, wenn ein Bericht auf einem Dashboard oder einer benutzerdefinierten Registerkarte angezeigt wird, wird er als eine Ansicht gezählt. Der Benutzer, der diesen Bericht in seinem Dashboard anzeigt, wird als Letzte Ansicht angezeigt von: Name: Benutzer und das Datum, an dem das Dashboard angezeigt wurde, werden als Datum der letzten Ansicht angezeigt.
* Workfront erfasst keine Nutzungsinformationen für integrierte Berichte.\
   Weitere Informationen zu integrierten Berichten in Workfront finden Sie im Artikel [Integrierte Adobe Workfront-Berichte verwenden](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront erfasst keine Nutzungsinformationen zu gelieferten Berichten. Ein bereitgestellter Bericht zählt nicht als eine Ansicht.\
   Weitere Informationen zu gelieferten Berichten finden Sie im Artikel [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* Wenn sich ein System- oder Gruppenadministrator als ein anderer Benutzer anmeldet, werden die Ansichten gezählt und dem System- oder Gruppenadministrator zugeordnet.
* Workfront erfasst keine Nutzungsinformationen für Berichte nach benutzerdefinierten Quartalen. In den Berichtsverwendungsfeldern werden nur die standardmäßigen integrierten Quartale referenziert.
* Workfront erfasst keine Nutzungsinformationen für Berichte, die freigegeben und öffentlich angezeigt werden. Wenn ein öffentlicher Bericht von einer Person angezeigt wird, die sich nicht bei Workfront angemeldet hat, werden die Berichtsansichten nicht gezählt.\
   Weitere Informationen zum Freigeben von Berichten finden Sie im Artikel [Bericht in Adobe Workfront freigeben](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
