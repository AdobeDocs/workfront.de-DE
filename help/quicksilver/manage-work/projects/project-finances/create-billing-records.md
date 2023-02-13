---
navigation-topic: financials
title: Rechnungsdatensätze erstellen
description: Zusätzlich zur Einrichtung von Umsatz- und Tracking-Ausgaben können Sie in einem Projekt Abrechnungsdatensätze für Informationen erstellen, die in Rechnung gestellt werden müssen.
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# Rechnungsdatensätze erstellen

Zusätzlich zur Einrichtung von Umsatz- und Tracking-Ausgaben können Sie in einem Projekt Abrechnungsdatensätze für Informationen erstellen, die in Rechnung gestellt werden müssen.

Rechnungsdatensätze für Aufgaben können nicht erstellt werden. Sie können nur Rechnungsdatensätze für Projekte erstellen.

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
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übersicht über Rechnungsdatensätze

Rechnungsdatensätze werden als Anhänge zu einem Projekt erstellt und enthalten Finanzdaten aus dem Projekt sowie einige Finanzinformationen zu den Aufgaben in einem Projekt.

Beachten Sie bei der Planung der Verwendung von Rechnungsdatensätzen Folgendes:

* Sie erstellen einen Rechnungsdatensatz, wenn Sie einen mit dem Projekt verbundenen Geldbetrag einem externen Anbieter oder Partner in Rechnung stellen möchten. Neben der Abrechnung eines festen Betrags an eine externe Quelle gibt es auch Fälle, in denen Sie den Betrag der Arbeit an dem Projekt (von angemeldeten Stunden) an einen externen Auftragnehmer sowie die angefallenen Ausgaben oder den Betrag der festen Einnahmen abrechnen müssen. Sie können alle diese Informationen in denselben Rechnungsdatensatz aufnehmen.
* Sobald ein Rechnungsdatensatz auf &quot;Abgerechnet&quot;gesetzt ist, kann er nicht mehr bearbeitet werden.

   >[!IMPORTANT]
   >
   >Dies ist wichtig, wenn Ihre Tarife variieren und Sie die Umsatz- und Ausgabedaten in Ihrem Projekt speichern möchten. Wenn Sie ihn zu einem Rechnungsdatensatz hinzufügen und ihn als &quot;Abgerechnet&quot;markieren, wird verhindert, dass er aktualisiert wird, wenn die Preise in Ihrem System aktualisiert werden.

* Ein Projekt mit Rechnungsdatensätzen, die als &quot;Abgerechnet&quot;gekennzeichnet wurden, kann nicht gelöscht werden.

## Rechnungsdatensatz erstellen

1. Navigieren Sie zu einem Projekt.
1. Klicken **Rechnungsdatensätze** im linken Bereich.

   Dieser Abschnitt befindet sich möglicherweise unter **Mehr anzeigen**.

1. Mit **Rechnungsdatensatzdetails** im linken Bereich ausgewählt ist, klicken Sie auf **Neuer Rechnungsdatensatz**.
1. Im **Neuer Rechnungsdatensatz** die folgenden Informationen angeben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Dies ist ein Pflichtfeld. Geben Sie eine Beschreibung für den Rechnungsdatensatz an, um den Zweck oder die Absicht für diesen Datensatz widerzuspiegeln.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fakturastatus</td> 
      <td> <p>Auswählen <strong>Nicht in Rechnung gestellt</strong>, wenn dieser Datensatz noch nicht abgerechnet wurde.</p> <p>Auswählen <strong>Rechnungsstellung</strong> wenn der Rechnungsdatensatz in Rechnung gestellt wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fakturierungsdatum</td> 
      <td>Wählen Sie durch Klicken auf das Kalendersymbol das Datum für die Abrechnung dieses Abrechnungsdatensatzes aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bestellnummer</td> 
      <td>Wenn diesem Rechnungsdatensatz eine Bestellnummer zugeordnet ist, geben Sie diese Informationen in dieses Feld ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechnungsnummer</td> 
      <td>Wenn diesem Rechnungsdatensatz eine Rechnung zugeordnet ist, geben Sie diese Informationen in dieses Feld ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zusätzlicher Betrag</td> 
      <td>Geben Sie den festen Betrag Ihres Rechnungsdatensatzes ein. Dies ist der Betrag, den Sie einem externen Kunden, Auftragnehmer oder Partner für dieses Projekt in Rechnung stellen möchten. Dieser Betrag kann nicht geändert werden, nachdem der Status des Rechnungsdatensatzes in "Abgerechnet"geändert wurde.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Unter **Benutzerdefinierte Forms** wählen Sie ein benutzerdefiniertes Formular für die Rechnungsstellung aus, das Sie zum Rechnungsdatensatz hinzufügen möchten.

   Sie (oder ein anderer Benutzer mit Zugriff auf benutzerdefinierte Formulare) müssen ein benutzerdefiniertes Formular für die Rechnungsstellung erstellen, bevor Sie es hier auswählen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   Sie können diesen Schritt wiederholen, um andere benutzerdefinierte Formulare hinzuzufügen, die Sie für den Rechnungsdatensatz benötigen.

1. Klicken Sie auf **Speichern.**

   Der Rechnungsdatensatz wird erstellt. Um abrechenbare Stunden, Ausgaben und feste Umsätze in den Rechnungsdatensatz aufzunehmen, führen Sie die im folgenden Unterabschnitt beschriebenen Schritte aus.

## Rechnungszeit, Ausgaben und Festeinnahmen in einen Rechnungsdatensatz einbeziehen

* [Rechnungszeiten in einen Rechnungsdatensatz einbeziehen](#include-billable-hours-in-a-billing-record)
* [Abrechenbare Ausgaben in einen Abrechnungsdatensatz einbeziehen](#include-billable-expenses-in-a-billing-record)
* [Feste Umsätze in einen Rechnungsdatensatz einbeziehen](#include-fixed-revenues-in-a-billing-record)

### Rechnungszeiten in einen Rechnungsdatensatz einbeziehen {#include-billable-hours-in-a-billing-record}

Sie können Stunden, die bei Aufgaben, Problemen oder dem Projekt protokolliert wurden, in Ihre Rechnungsdatensätze aufnehmen.\
Wenn der Benutzer, der die Stunden oder seine Primäre Auftragsrolle protokolliert, mit einer Abrechnungsrate pro Stunde verknüpft ist, wird der Umsatz aus diesen Stunden zum Rechnungsdatensatz hinzugefügt.

* [Welche Stunden können einem Abrechnungsdatensatz hinzugefügt werden?](#what-hours-can-be-added-to-a-billing-record)
* [Hinzufügen von Stunden zu einem Rechnungsdatensatz](#add-hours-to-a-billing-record)

#### Welche Stunden können einem Abrechnungsdatensatz hinzugefügt werden? {#what-hours-can-be-added-to-a-billing-record}

Sie können einem Rechnungsdatensatz Stunden hinzufügen, wenn die folgenden Bedingungen erfüllt sind:

* Aufgaben, Probleme oder das Projekt sind Stunden protokolliert.
* Der Stunden-Typ der protokollierten Stunden wird als &quot;Umsatz zählen&quot;markiert.

   Weitere Informationen zu den Stundentypen finden Sie im Artikel [Stundentypen verwalten](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alle Stunden, die für Probleme oder das Projekt protokolliert werden, können zu einem Rechnungsdatensatz hinzugefügt werden, wenn dem Benutzer, der die Zeit protokolliert, eine Abrechnungsrate pro Stunde oder ihre Primäre Auftragsrolle zugeordnet ist.
* Wenn die Stunden bei einer Aufgabe protokolliert werden, muss die Aufgabe den folgenden Umsatztyp aufweisen:

   * Der Umsatztyp kann nicht auf Nicht abrechenbar gesetzt werden.
   * Wenn der Umsatztyp auf &quot;Benutzer stündlich&quot;festgelegt ist, muss der Benutzer, der die Zeit protokolliert, über eine Abrechnungsrate pro Stunde in seinem Profil verfügen.
   * Wenn der Umsatztyp auf Stündliche Rolle festgelegt ist, muss die Primäre Rolle des Benutzers, der die Zeit protokolliert, über eine Abrechnungsrate pro Stunde verfügen.

      >[!NOTE]
      >
      >Sie können die Abrechnungsraten für Stellenrollen auf Projektebene überschreiben.\
      >Weitere Informationen zum Außerkraftsetzen von Gebühren für die Abrechnung von Stellenwerten finden Sie im Abschnitt &quot;Außerkraftsetzen von Abrechnungsraten für Auftragsrollen auf Projektebene&quot;im Artikel [Übersicht über die Außerkraftsetzung der Abrechnungsraten von Auftragsrollen und die Berechnung des Umsatzes eines Projekts](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Wenn **Genehmigung für dieses Projekt erforderlich** unter &quot;Projekteinstellungen&quot;aktiviert ist, muss der Projektinhaber die protokollierten Stunden genehmigen.\
   Weitere Informationen zum Anfordern einer Genehmigung für Projektzeiten finden Sie im Artikel [Genehmigung für ein Projekt erforderlich](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Hinzufügen von Stunden zu einem Rechnungsdatensatz {#add-hours-to-a-billing-record}

So fügen Sie einem Rechnungsdatensatz abrechnungsfähige Stunden hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken **Rechnungsdatensätze** im linken Bereich.

   Dieser Abschnitt befindet sich möglicherweise unter **Mehr anzeigen**.

1. Klicken Sie auf **Beschreibung** eines Rechnungsdatensatzes zum Öffnen der **Rechnungsdatensatzdetails** Registerkarte.

1. Klicken **Abrechenbare Stunden** im linken Bereich.
1. Wenn Stunden in einem Rechnungsdatensatz enthalten sein können, klicken Sie auf **Stunden hinzufügen**.\
   Die **Hinzufügen von abrechnungsfähigen Stunden** wird geöffnet.

   >[!NOTE]
   >
   >Wenn keine Stunden protokolliert werden oder die protokollierten Stunden nicht die Bedingungen erfüllen, die zum Rechnungsdatensatz hinzugefügt werden müssen, wird die **Stunden hinzufügen** -Schaltfläche wird nicht angezeigt. Weitere Informationen dazu, welche Stunden für einen Rechnungsdatensatz protokolliert werden können, finden Sie im Abschnitt [Welche Stunden können einem Abrechnungsdatensatz hinzugefügt werden?](#what-hours-can-be-added-to-a-billing-record) in diesem Artikel.

1. Wählen Sie die Stundeneinträge aus, die Sie in den Rechnungsdatensatz aufnehmen möchten, und klicken Sie auf **Stunden hinzufügen**.\
   Die tatsächlichen Kosten der Stunden werden als **Abrechenbare Stunden** dem **Rechnungsdatensatz gesamt**.

1. (Optional) Klicken Sie auf **Details zu Rechnungsdatensätzen** zur Überprüfung der **Abrechenbare Stunden** und **Rechnungsdatensatz gesamt** Beträge. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

### Abrechenbare Ausgaben in einen Abrechnungsdatensatz einbeziehen {#include-billable-expenses-in-a-billing-record}

Wenn Sie dem Rechnungsdatensatz abrechenbare Ausgaben hinzufügen, stellen Sie sicher, dass die Ausgaben für die Aufgaben und das Projekt als abrechnungsfähig markiert sind. Ausgaben, die nicht als &quot;Abrechenbar&quot;gekennzeichnet sind, können in einem Rechnungsdatensatz nicht hinzugefügt werden. Weitere Informationen zur Hinzufügung von Ausgaben finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

So fügen Sie einem Rechnungsdatensatz abrechnungsfähige Ausgaben hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken **Rechnungsdatensätze** im linken Bereich.

   Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Rechnungsdatensätze**.

1. Klicken Sie auf **Beschreibung** eines Rechnungsdatensatzes zum Öffnen der **Rechnungsdatensatzdetails** Registerkarte.

1. Klicken **Abrechenbare Ausgaben** im linken Bereich.
1. (Bedingt) Wenn Sie Ihren Aufgaben oder dem Projekt Ausgaben hinzugefügt und diese als &quot;Abrechenbar&quot;gekennzeichnet haben, klicken Sie auf **Ausgaben hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Kosten haben, diese jedoch nicht als abrechenbar gekennzeichnet sind, wird die **Ausgaben hinzufügen** -Schaltfläche wird nicht angezeigt. Nur abrechenbare Ausgaben mit einem tatsächlichen Betrag von mehr als null sind berechtigt, in einen Abrechnungsbericht aufgenommen zu werden.

1. Wählen Sie die Abrechnungskosten aus, die zum Rechnungsdatensatz hinzugefügt werden können, und klicken Sie dann auf **Ausgaben hinzufügen**.\
   Der tatsächliche Betrag der Ausgaben wird als **Abrechenbare Ausgaben** dem **Rechnungsdatensatz gesamt**.

1. (Optional) Klicken Sie auf **Details zu Rechnungsdatensätzen** zur Überprüfung der **Abrechenbare Ausgaben** und **Rechnungsdatensatz gesamt** Beträge. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

### Feste Umsätze in einen Rechnungsdatensatz einbeziehen {#include-fixed-revenues-in-a-billing-record}

Sie können Ihren Rechnungsdatensätzen feste Umsätze hinzufügen, wenn Sie über Aufgaben verfügen, für die feste Umsätze verfügbar sind. Es sind keine anderen Arten von Aufgaben oder Projektumsätzen verfügbar, die in einem Rechnungsdatensatz hinzugefügt werden können. Weitere Informationen zu Umsatztypen finden Sie unter [Übersicht über Rechnungsstellung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) Abschnitt in [Übersicht über Rechnungsstellung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

So fügen Sie einem Rechnungsdatensatz feste Einnahmen hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken **Rechnungsdatensätze** im linken Bereich.

   Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Rechnungsdatensätze**.

1. Klicken Sie auf **Beschreibung** eines Rechnungsdatensatzes zum Öffnen der **Rechnungsdatensatzdetails** Registerkarte.

1. Wählen Sie die **Festeinnahmen** Registerkarte.
1. Wenn Sie Ihren Aufgaben feste Umsätze hinzugefügt haben, klicken Sie auf **Hinzufügen fester Umsätze**.

   >[!NOTE]
   >
   >Wenn Sie Umsätze für Aufgaben haben, diese jedoch nicht als &quot;Fest&quot;gekennzeichnet sind, wird die Variable **Fixierten Umsatz hinzufügen** -Schaltfläche wird nicht angezeigt.

1. Wählen Sie die Aufgaben aus, deren feste Umsätze Sie in den Rechnungsdatensatz aufnehmen möchten, und klicken Sie dann auf **Aufgaben hinzufügen**.\
   Die **Fester Umsatz** Die Anzahl der Aufgaben wird als **Abrechenbare Einnahmen** dem **Rechnungsdatensatz gesamt**.

1. (Optional) Klicken Sie auf **Details zu Rechnungsdatensätzen** zur Überprüfung der **Abrechenbare Einnahmen** und **Rechnungsdatensatz gesamt** Beträge. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

## Rechnungsdatensatz bearbeiten

Nachdem Sie einen Abrechnungsdatensatz erstellt haben und Stunden, Ausgaben und Umsätze in den Abrechnungsdatensatz eingeschlossen haben, können Sie einige Informationen zum vorhandenen Datensatz bearbeiten, bevor er als Abgerechnet markiert wird.

1. Wechseln Sie zum Rechnungsdatensatz.
1. Mit **Rechnungsdatensatzdetails** im linken Bereich ausgewählt sind, Informationen in allen verfügbaren Feldern bearbeiten

   Oder

   Klicken Sie auf **Symbol Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke und dann Informationen in allen verfügbaren Feldern bearbeiten.

   Aktualisieren Sie Folgendes:

   * **Beschreibung**
   * **Fakturastatus**

      >[!TIP]
      >
      >Wenn Sie **Rechnungsstellung** für den Rechnungsstatus kann der Rechnungsdatensatz nach dem Speichern Ihrer Änderungen nicht mehr bearbeitet werden.

   * **Fakturierungsdatum**
   * **Bestellnummer**
   * **Rechnungsnummer**
   * **Zusätzlicher Betrag**

   Die folgenden Felder stehen nicht zur Bearbeitung zur Verfügung:

   * **Abrechnungszeiten:** Die Gesamtsumme des tatsächlichen Umsatzes der Stunden, die im Rechnungsdatensatz enthalten sind. Weitere Informationen zum Einbeziehen von Stunden in einen Rechnungsdatensatz finden Sie im Abschnitt [Rechnungszeiten in einen Rechnungsdatensatz einbeziehen](#include-billable-hours-in-a-billing-record) in diesem Artikel.

   * **Abrechenbare Ausgaben**: Der Gesamtbetrag des tatsächlichen Betrags der im Rechnungsabschluss enthaltenen abrechnungsfähigen Ausgaben. Weitere Informationen zur Einbeziehung von Abrechnungskosten in einen Abrechnungsdatensatz finden Sie im Abschnitt [Abrechenbare Ausgaben in einen Abrechnungsdatensatz einbeziehen](#include-billable-expenses-in-a-billing-record) in diesem Artikel.

   * **Abrechenbare Einnahmen**: Die Gesamtsumme des festen Umsatzes der im Rechnungsdatensatz enthaltenen Aufgaben. Weitere Informationen zum Einbeziehen von festen Umsätzen in einen Abrechnungsdatensatz finden Sie im Abschnitt [Feste Umsätze in einen Rechnungsdatensatz einbeziehen](#include-fixed-revenues-in-a-billing-record) in diesem Artikel.

   * **Rechnungsdatensatz gesamt**: Die Summe aller abrechnungsfähigen Beträge. Dies wird anhand der folgenden Formel berechnet:

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. Klicken **Speichern***Änderungen**.
