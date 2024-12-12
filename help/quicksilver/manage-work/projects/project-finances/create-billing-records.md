---
navigation-topic: financials
title: Rechnungsdatensätze erstellen
description: Zusätzlich zur Einrichtung von Umsatz- und Tracking-Ausgaben können Sie in einem Projekt Abrechnungsdatensätze für Informationen erstellen, die in Rechnung gestellt werden müssen.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '1896'
ht-degree: 0%

---

# Erstellen von Rechnungsdatensätzen

Zusätzlich zur Einrichtung von Umsatz- und Tracking-Ausgaben können Sie in einem Projekt Abrechnungsdatensätze für Informationen erstellen, die in Rechnung gestellt werden müssen.

Rechnungsdatensätze für Aufgaben können nicht erstellt werden. Sie können nur Rechnungsdatensätze für Projekte erstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten der Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über Rechnungsdatensätze

Rechnungsdatensätze werden als Anhänge zu einem Projekt erstellt und enthalten Finanzdaten aus dem Projekt sowie einige Finanzinformationen zu den Aufgaben in einem Projekt.

Beachten Sie bei der Planung der Verwendung von Rechnungsdatensätzen Folgendes:

* Sie erstellen einen Rechnungsdatensatz, wenn Sie einen mit dem Projekt verbundenen Geldbetrag einem externen Anbieter oder Partner in Rechnung stellen möchten. Neben der Abrechnung eines festen Betrags an eine externe Quelle gibt es auch Fälle, in denen Sie die Arbeitszeit für das Projekt (von angemeldeten Stunden) einem externen Auftragnehmer sowie die angefallenen Ausgaben oder die Höhe der festen Einnahmen abrechnen müssen. Sie können alle diese Informationen in denselben Rechnungsdatensatz aufnehmen.
* Sobald ein Rechnungsdatensatz auf &quot;Abgerechnet&quot;gesetzt ist, kann er nicht mehr bearbeitet werden.

  >[!IMPORTANT]
  >
  >Dies ist wichtig, wenn Ihre Tarife variieren und Sie die Umsatz- und Ausgabedaten in Ihrem Projekt speichern möchten. Wenn Sie ihn zu einem Rechnungsdatensatz hinzufügen und ihn als &quot;Abgerechnet&quot;markieren, wird verhindert, dass er aktualisiert wird, wenn die Preise in Ihrem System aktualisiert werden.

* Ein Projekt mit Rechnungsdatensätzen, die als &quot;Abgerechnet&quot;gekennzeichnet wurden, kann nicht gelöscht werden.

## Erstellen eines Rechnungsdatensatzes

1. Navigieren Sie zu einem Projekt.
1. Klicken Sie im linken Bereich auf **Rechnungsdatensätze** .

   Dieser Abschnitt befindet sich möglicherweise unter &quot;**Mehr anzeigen**&quot;.

1. Klicken Sie bei ausgewähltem **Rechnungsdatensatz-Details** im linken Bereich auf **Neuer Rechnungsdatensatz**.
1. Geben Sie im angezeigten Feld **Neuer Rechnungsdatensatz** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Dies ist ein erforderliches Feld. Geben Sie eine Beschreibung für den Rechnungsdatensatz an, um den Zweck oder die Absicht für diesen Datensatz widerzuspiegeln.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fakturastatus</td> 
      <td> <p>Wählen Sie <strong>Nicht abgerechnet</strong> aus, wenn dieser Datensatz noch nicht abgerechnet wurde.</p> <p>Wählen Sie <strong>Abgerechnet</strong> aus, wenn der Abrechnungsdatensatz in Rechnung gestellt wird.</p> </td> 
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

1. (Optional) Wählen Sie unter **Benutzerdefinierter Forms** ein benutzerdefiniertes Formular für die Rechnungsstellung für Datensätze aus, das Sie zum Rechnungsdatensatz hinzufügen möchten.

   Sie (oder ein anderer Benutzer mit Zugriff auf benutzerdefinierte Formulare) müssen ein benutzerdefiniertes Formular für die Rechnungsstellung erstellen, bevor Sie es hier auswählen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Sie können diesen Schritt wiederholen, um andere benutzerdefinierte Formulare hinzuzufügen, die Sie für den Rechnungsdatensatz benötigen.

1. Klicken Sie auf **Speichern.**

   Der Rechnungsdatensatz wird erstellt. Um abrechenbare Stunden, Ausgaben und feste Umsätze in den Rechnungsdatensatz aufzunehmen, führen Sie die im folgenden Unterabschnitt beschriebenen Schritte aus.

## Rechnungszeit, Ausgaben und Festeinnahmen in einen Rechnungsdatensatz einbeziehen

* [Rechnungsstunden in einen Rechnungsdatensatz einbeziehen](#include-billable-hours-in-a-billing-record)
* [Rechnungskosten in einen Rechnungsdatensatz einbeziehen](#include-billable-expenses-in-a-billing-record)
* [Feste Umsätze in einen Rechnungsdatensatz einbeziehen](#include-fixed-revenues-in-a-billing-record)

### Rechnungszeiten in einen Rechnungsdatensatz einbeziehen {#include-billable-hours-in-a-billing-record}

Sie können Stunden, die bei Aufgaben, Problemen oder dem Projekt protokolliert wurden, in Ihre Rechnungsdatensätze aufnehmen.\
Wenn der Benutzer, der die Stunden oder seine Primäre Auftragsrolle protokolliert, mit einer Abrechnungsrate pro Stunde verknüpft ist, wird der Umsatz aus diesen Stunden zum Rechnungsdatensatz hinzugefügt.

* [Welche Stunden können einem Rechnungsdatensatz hinzugefügt werden](#what-hours-can-be-added-to-a-billing-record)
* [Hinzufügen von Stunden zu einem Rechnungsdatensatz](#add-hours-to-a-billing-record)

#### Welche Stunden können einem Abrechnungsdatensatz hinzugefügt werden? {#what-hours-can-be-added-to-a-billing-record}

Sie können einem Rechnungsdatensatz Stunden hinzufügen, wenn die folgenden Bedingungen erfüllt sind:

* Aufgaben, Probleme oder das Projekt sind Stunden protokolliert.
* Der Stunden-Typ der protokollierten Stunden wird als &quot;Umsatz zählen&quot;markiert.

  Weitere Informationen zu den Stundentypen finden Sie im Artikel [Verwalten von Stundentypen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alle Stunden, die für Probleme oder das Projekt protokolliert werden, können zu einem Rechnungsdatensatz hinzugefügt werden, wenn dem Benutzer, der die Zeit protokolliert, eine Abrechnungsrate pro Stunde oder ihre Primäre Auftragsrolle zugeordnet ist.
* Wenn die Stunden bei einer Aufgabe protokolliert werden, muss die Aufgabe den folgenden Umsatztyp aufweisen:

   * Der Umsatztyp kann nicht auf Nicht abrechenbar gesetzt werden.
   * Wenn der Umsatztyp auf &quot;Benutzer stündlich&quot;festgelegt ist, muss der Benutzer, der die Zeit protokolliert, über eine Abrechnungsrate pro Stunde in seinem Profil verfügen.
   * Wenn der Umsatztyp auf Stündliche Rolle festgelegt ist, muss die Primäre Rolle des Benutzers, der die Zeit protokolliert, über eine Abrechnungsrate pro Stunde verfügen.

     >[!NOTE]
     >
     >Sie können die Abrechnungsraten für Stellenrollen auf Projektebene überschreiben.\
     >Weitere Informationen zum Außerkraftsetzen der Abrechnungsraten für Stellenrollen finden Sie im Abschnitt &quot;Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene&quot;im Artikel [Überblick über die Überschreiben der Abrechnungsraten für Auftragsrollen und Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Wenn unter &quot;Projekteinstellungen&quot;die Option &quot;**Genehmigung der Zeit für dieses Projekt erforderlich**&quot;aktiviert ist, muss der Projektinhaber die protokollierten Stunden genehmigen.\
  Weitere Informationen zum Anfordern einer Genehmigung für Projektzeiten finden Sie im Artikel [Anfordern der Zeit für die Genehmigung eines Projekts](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Hinzufügen von Stunden zu einem Rechnungsdatensatz {#add-hours-to-a-billing-record}

So fügen Sie einem Rechnungsdatensatz abrechnungsfähige Stunden hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken Sie im linken Bereich auf **Rechnungsdatensätze** .

   Dieser Abschnitt befindet sich möglicherweise unter &quot;**Mehr anzeigen**&quot;.

1. Klicken Sie auf die Registerkarte **Beschreibung** eines Abrechnungsdatensatzes, um die Registerkarte **Rechnungsstellungsdetails für Datensatz** zu öffnen.

1. Klicken Sie im linken Bereich auf **Abrechenbare Stunden** .
1. Wenn Stunden in einem Rechnungsdatensatz enthalten sein können, klicken Sie auf **Stunden hinzufügen**.\
   Das Feld **Abrechenbare Stunden hinzufügen** wird geöffnet.

   >[!NOTE]
   >
   >Wenn keine Stunden protokolliert werden oder die protokollierten Stunden nicht die Bedingungen erfüllen, die zum Rechnungsdatensatz hinzugefügt werden müssen, wird die Schaltfläche **Stunden hinzufügen** nicht angezeigt. Weitere Informationen dazu, welche Stunden für einen Rechnungsdatensatz protokolliert werden können, finden Sie im Abschnitt [Welche Stunden können einem Rechnungsdatensatz hinzugefügt werden](#what-hours-can-be-added-to-a-billing-record) in diesem Artikel.

1. Wählen Sie die Stundeneinträge aus, die Sie in den Rechnungsdatensatz aufnehmen möchten, und klicken Sie auf **Stunden hinzufügen**.\
   Die tatsächlichen Kosten der Stunden werden als Betrag von **Rechnungsstunden** dem Betrag von **Rechnungsdatensatz insgesamt** hinzugefügt.

1. (Optional) Klicken Sie auf **Rechnungseinstellungsdetails** , um die Beträge für die **Rechnungsstunden** und für die **Rechnungseinstellungssumme** zu überprüfen. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

### Abrechenbare Ausgaben in einen Abrechnungsdatensatz einbeziehen {#include-billable-expenses-in-a-billing-record}

Wenn Sie dem Rechnungsdatensatz abrechenbare Ausgaben hinzufügen, stellen Sie sicher, dass die Ausgaben für die Aufgaben und das Projekt als abrechnungsfähig markiert sind. Ausgaben, die nicht als &quot;Abrechenbar&quot;gekennzeichnet sind, können in einem Rechnungsdatensatz nicht hinzugefügt werden. Weitere Informationen zum Hinzufügen von Ausgaben finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

So fügen Sie einem Rechnungsdatensatz abrechnungsfähige Ausgaben hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken Sie im linken Bereich auf **Rechnungsdatensätze** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Rechnungseinträge** klicken.

1. Klicken Sie auf die Registerkarte **Beschreibung** eines Abrechnungsdatensatzes, um die Registerkarte **Rechnungsstellungsdetails für Datensatz** zu öffnen.

1. Klicken Sie im linken Bereich auf **Abrechenbare Ausgaben** .
1. (Bedingt) Wenn Sie Ihren Aufgaben oder dem Projekt Ausgaben hinzugefügt und diese als &quot;Abrechenbar&quot;gekennzeichnet haben, klicken Sie auf **Ausgaben hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Ausgaben haben, diese jedoch nicht als &quot;Abrechenbar&quot;gekennzeichnet sind, wird die Schaltfläche **Ausgaben hinzufügen** nicht angezeigt. Nur abrechenbare Ausgaben mit einem tatsächlichen Betrag von mehr als null sind berechtigt, in einen Abrechnungsbericht aufgenommen zu werden.

1. Wählen Sie die Rechnungskosten aus, die dem Rechnungsdatensatz hinzugefügt werden können, und klicken Sie dann auf **Ausgaben hinzufügen**.\
   Der tatsächliche Betrag der Ausgaben wird als Betrag **Abrechenbare Ausgaben** in den Betrag **Rechnungsdatensatz insgesamt** eingefügt.

1. (Optional) Klicken Sie auf **Rechnungseinstellungsdetails** , um die Beträge für die **Rechnungskosten** und die **Rechnungseintragssumme** zu überprüfen. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

### Feste Umsätze in einen Rechnungsdatensatz einbeziehen {#include-fixed-revenues-in-a-billing-record}

Sie können Ihren Rechnungsdatensätzen feste Umsätze hinzufügen, wenn Sie über Aufgaben verfügen, für die feste Umsätze verfügbar sind. Es sind keine anderen Arten von Aufgaben oder Projektumsätzen verfügbar, die in einem Rechnungsdatensatz hinzugefügt werden können. Weitere Informationen zu Umsatztypen finden Sie im Abschnitt [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) in der [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

So fügen Sie einem Rechnungsdatensatz feste Einnahmen hinzu:

1. Wechseln Sie zum Projekt mit den Rechnungsdatensätzen.
1. Klicken Sie im linken Bereich auf **Rechnungsdatensätze** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Rechnungseinträge** klicken.

1. Klicken Sie auf die Registerkarte **Beschreibung** eines Abrechnungsdatensatzes, um die Registerkarte **Rechnungsstellungsdetails für Datensatz** zu öffnen.

1. Wählen Sie die Registerkarte **Feste Umsätze** aus.
1. Wenn Sie feste Umsätze zu Ihren Aufgaben hinzugefügt haben, klicken Sie auf **Feste Umsätze hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Umsatzsummen für Aufgaben haben, diese jedoch nicht als &quot;Fest&quot;markiert sind, wird die Schaltfläche **Fest Umsatz hinzufügen** nicht angezeigt.

1. Wählen Sie die Aufgaben aus, deren feste Einnahmen Sie in den Rechnungsdatensatz aufnehmen möchten, und klicken Sie dann auf **Aufgaben hinzufügen**.\
   Der Betrag **Fester Umsatz** der Aufgaben wird hinzugefügt, da der Betrag **Abrechenbare Einnahmen** dem Betrag **Abrechnungsdatensatz insgesamt** entspricht.

1. (Optional) Klicken Sie auf **Rechnungsdatensatzdetails** , um die Beträge **Abrechenbare Umsätze** und **Abrechnungsdatensätze insgesamt** zu überprüfen. Sie können auch die Gesamtsumme des Rechnungsdatensatzes in der Kopfzeile des Rechnungsdatensatzes sehen.

## Rechnungsdatensatz bearbeiten

Nachdem Sie einen Abrechnungsdatensatz erstellt haben und Stunden, Ausgaben und Umsätze in den Abrechnungsdatensatz eingeschlossen haben, können Sie einige Informationen zum vorhandenen Datensatz bearbeiten, bevor er als Abgerechnet markiert wird.

1. Wechseln Sie zum Rechnungsdatensatz.
1. Wenn im linken Bereich **Rechnungsdatensatzdetails** ausgewählt ist, bearbeiten Sie Informationen in allen verfügbaren Feldern

   Oder

   Klicken Sie oben rechts auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) und bearbeiten Sie dann Informationen in allen verfügbaren Feldern.

   Aktualisieren Sie Folgendes:

   * **Beschreibung**
   * **Rechnungsstatus**

     >[!TIP]
     >
     >Wenn Sie für den Abrechnungsstatus **Abgerechnet** auswählen, kann der Abrechnungsdatensatz nach dem Speichern Ihrer Änderungen nicht bearbeitet werden.

   * **Abrechnungsdatum**
   * **Bestellnummer**
   * **Rechnungskennung**
   * **Zusätzlicher Betrag**

   Die folgenden Felder stehen nicht zur Bearbeitung zur Verfügung:

   * **Abrechenbare Stunden:** Die Gesamtsumme des tatsächlichen Umsatzes der Stunden, die im Abrechnungsdatensatz enthalten sind. Weitere Informationen zum Einbeziehen von Stunden in einen Abrechnungsdatensatz finden Sie im Abschnitt [Abrechenbare Stunden in einen Abrechnungsdatensatz einschließen](#include-billable-hours-in-a-billing-record) in diesem Artikel.

   * **Abrechenbare Ausgaben**: Der Gesamtbetrag der tatsächlichen Summe der im Rechnungsdatensatz enthaltenen abrechnungsfähigen Ausgaben. Weitere Informationen zum Einbeziehen von abrechnungsfähigen Ausgaben in einen Abrechnungsdatensatz finden Sie im Abschnitt [Abrechenbare Ausgaben in einen Abrechnungsdatensatz einschließen](#include-billable-expenses-in-a-billing-record) in diesem Artikel.

   * **Abrechenbare Umsätze**: Die Gesamtsumme des Festumsatzes der im Abrechnungsdatensatz enthaltenen Aufgaben. Weitere Informationen zum Einbeziehen von festen Umsätzen in einen Rechnungsdatensatz finden Sie im Abschnitt [Feste Umsätze in einen Rechnungsdatensatz einbeziehen](#include-fixed-revenues-in-a-billing-record) in diesem Artikel.

   * **Rechnungssumme der Datensätze insgesamt**: Die Summe aller abrechnungsfähigen Beträge. Dies wird anhand der folgenden Formel berechnet:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klicken Sie auf **Speichern***Änderungen**.
