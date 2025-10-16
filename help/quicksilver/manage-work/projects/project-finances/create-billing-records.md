---
navigation-topic: financials
title: Rechnungsnachweise erstellen
description: Zusätzlich zur Einrichtung von Einnahmen und zur Verfolgung von Ausgaben können Sie Rechnungsnachweise für ein Projekt erstellen, um Informationen zu erhalten, die in Rechnung gestellt werden müssen.
author: Lisa
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 1%

---

# Rechnungsnachweise erstellen

<!-- Audited: 6/2025 -->

Zusätzlich zur Einrichtung von Einnahmen und zur Verfolgung von Ausgaben können Sie Rechnungsnachweise für ein Projekt erstellen, um Informationen zu erhalten, die in Rechnung gestellt werden müssen.

Sie können keine Rechnungsnachweise für Aufgaben erstellen; Sie können nur Rechnungsnachweise für Projekte erstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt mit Berechtigungen zum Verwalten von Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rechnungsnachweise - Übersicht

Rechnungsnachweise werden als Anlagen zu einem Projekt erstellt und enthalten Finanzdaten aus dem Projekt sowie die Finanzinformationen der Projektaufgaben.

Beachten Sie bei der Planung der Verwendung von Rechnungsnachweisen Folgendes:

* Sie erstellen einen Rechnungsnachweis, wenn Sie einen Geldbetrag im Zusammenhang mit dem Projekt einem externen Anbieter oder Partner in Rechnung stellen möchten. Neben der Fakturierung eines festen Betrags an eine externe Quelle gibt es Fälle, in denen Sie den Arbeitsaufwand für das Projekt (ab protokollierten Stunden) einem externen Auftragnehmer in Rechnung stellen müssen, sowie die angefallenen Ausgaben oder den Betrag der festen Einnahmen. Sie können alle diese Informationen in denselben Rechnungsnachweis aufnehmen.
* Sobald ein Rechnungsnachweis auf „In Rechnung gestellt“ gesetzt wurde, kann er nicht mehr bearbeitet werden.

  >[!IMPORTANT]
  >
  >Dies ist wichtig, wenn Ihre Sätze variieren und Sie die Umsatz- und Ausgabeninformationen für Ihr Projekt sperren möchten. Wenn Sie ihn zu einem Rechnungsnachweis hinzufügen und als „In Rechnung gestellt“ markieren, wird er nicht aktualisiert, wenn die Tarife in Ihrem System aktualisiert werden.

* Ein Projekt mit Rechnungsnachweisen, die als In Rechnung gestellt gekennzeichnet wurden, kann nicht gelöscht werden.

## Rechnungsnachweis erstellen

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie **linken** auf Rechnungsnachweise .
1. Klicken Sie **Neuer Rechnungsnachweis**.
1. Geben Sie **Feld „Neuer**&quot; die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>(Erforderlich) Geben Sie eine Beschreibung für den Rechnungsnachweis ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abrechnungsstatus</td> 
      <td> <p>Wählen <strong>Nicht in Rechnung gestellt</strong> wenn dieser Datensatz noch nicht in Rechnung gestellt wurde.</p> <p>Wählen Sie <strong>In Rechnung gestellt</strong> aus, wenn der Rechnungsnachweis in Rechnung gestellt wurde.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abrechnungsdatum</td> 
      <td>Wählen Sie das Datum aus, an dem dieser Rechnungsnachweis in Rechnung gestellt wurde, indem Sie auf das Kalendersymbol klicken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bestellnummer</td> 
      <td>Geben Sie die Bestellnummer ein, die diesem Rechnungsnachweis zugeordnet ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rechnungsnummer</td> 
      <td>Geben Sie die diesem Rechnungsnachweis zugeordnete Rechnung ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zusätzlicher Betrag</td> 
      <td>Geben Sie den Festbetrag Ihres Rechnungsnachweises ein. Dies ist der Betrag, den Sie einem externen Kunden, Auftragnehmer oder Partner für dieses Projekt in Rechnung stellen möchten. Dieser Betrag kann nicht mehr geändert werden, nachdem der Status des Abrechnungs-Datensatzes in „In Rechnung gestellt“ geändert wurde.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen **unter „Benutzerdefinierte Forms** ein benutzerdefiniertes Formular für Rechnungsnachweise aus, das Sie dem Datensatz hinzufügen möchten.

   Ein benutzerdefiniertes Formular für Rechnungsnachweise muss erstellt werden, bevor Sie es hier auswählen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie auf **Speichern.** Der Rechnungsnachweis wird erstellt.

## Fakturierbare Stunden, Ausgaben und Festeinnahmen in einen Rechnungsnachweis einschließen

### Fakturierbare Stunden in einen Rechnungsnachweis einbeziehen {#include-billable-hours-in-a-billing-record}

Sie können Stunden, die für Aufgaben, Probleme oder das Projekt protokolliert wurden, in Ihre Rechnungsnachweise aufnehmen.

Wenn der Benutzer, der die Stunden oder sein primäres Aufgabengebiet protokolliert, mit einem Abrechnungssatz pro Stunde verknüpft ist, wird der Umsatz aus diesen Stunden zum Abrechnungs-Datensatz hinzugefügt.

* [Welche Stunden können einem Rechnungsnachweis hinzugefügt werden](#what-hours-can-be-added-to-a-billing-record)
* [Hinzufügen von Stunden zu einem Rechnungsnachweis](#add-hours-to-a-billing-record)

#### Welche Stunden können einem Rechnungsnachweis hinzugefügt werden? {#what-hours-can-be-added-to-a-billing-record}

Sie können einem Rechnungsnachweis Stunden hinzufügen, wenn die folgenden Bedingungen erfüllt sind:

* Für die Aufgaben, Probleme oder das Projekt wurden Stunden protokolliert.
* Der Stundentyp der protokollierten Stunden wird als „Umsatz zählen“ gekennzeichnet.

  Weitere Informationen finden Sie im Artikel [Verwalten von Stundentypen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* Alle für Probleme oder das Projekt protokollierten Stunden können einem Rechnungsnachweis hinzugefügt werden, wenn dem Benutzer, der die Zeit protokolliert, ein Abrechnungssatz pro Stunde oder sein primäres Aufgabengebiet zugeordnet ist.
* Wenn Stunden für eine Aufgabe protokolliert werden, muss die Aufgabe den folgenden Umsatztyp aufweisen:

   * Der Umsatztyp kann nicht auf „Nicht fakturierbar“ festgelegt werden.
   * Wenn der Umsatztyp auf „Benutzer pro Stunde“ festgelegt ist, muss für den Benutzer, der die Zeit protokolliert, der Satz „Abrechnung pro Stunde“ in seinem Profil festgelegt sein.
   * Wenn der Umsatztyp auf „Funktion pro Stunde“ festgelegt ist, muss die primäre Rolle des Benutzers, der die Zeit protokolliert, über einen Abrechnungssatz pro Stunde verfügen.

     >[!NOTE]
     >
     >Sie können Abrechnungssätze für Aufgabengebiete auf Projektebene überschreiben.\
     >Weitere Informationen finden Sie im Abschnitt „Überschreiben der Abrechnungssätze für Aufgabengebiete auf Projektebene“ im Artikel [Übersicht über das Überschreiben der Abrechnungssätze für Aufgabengebiete und die Berechnung des Umsatzes für ein Projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* Wenn die Option Für dieses Projekt zu genehmigende Zeit erforderlich in den Projekteinstellungen ausgewählt ist, muss der Projektbesitzer die protokollierten Stunden genehmigen.\
  Weitere Informationen finden Sie unter [Für die Genehmigung eines Projekts ist Zeit erforderlich](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### Hinzufügen von Stunden zu einem Rechnungsnachweis {#add-hours-to-a-billing-record}

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie **linken** auf Rechnungsnachweise .
1. Klicken Sie auf den Rechnungsnachweis **Beschreibung**, um die Registerkarte **Details zum Rechnungsnachweis** zu öffnen.
1. Klicken Sie **linken Bedienfeld auf** Abrechnungsfähige Stunden“.
1. Wenn ein Rechnungsnachweis Stunden enthalten kann, klicken Sie auf **Stunden hinzufügen**. Das **Abrechnungsfähige Stunden hinzufügen** wird geöffnet.

   >[!NOTE]
   >
   >Wenn keine Stunden protokolliert werden oder die protokollierten Stunden die Bedingungen für das Hinzufügen zu einem Rechnungsnachweis nicht erfüllen, wird die Schaltfläche **Stunden hinzufügen** nicht angezeigt. Weitere Informationen finden Sie im folgenden Abschnitt dieses Artikels: [Welche Stunden können einem Rechnungsnachweis hinzugefügt werden](#what-hours-can-be-added-to-a-billing-record).

1. Wählen Sie die Stundeneinträge aus, die Sie in den Rechnungsnachweis aufnehmen möchten, und klicken Sie dann auf **Stunden hinzufügen**. Die Ist-Kosten der Stunden werden als „Abrechnungsfähige **&quot;** „Rechnungsnachweissumme **hinzugefügt**.

1. (Optional) Klicken Sie auf **Rechnungsnachweisdetails**, um die Beträge **Abrechnungsfähige Stunden** und **Rechnungsnachweissumme** sowie die Summe des Rechnungsnachweises in der Kopfzeile des Rechnungsnachweises zu überprüfen.

### Verrechenbare Ausgaben in einen Rechnungsnachweis einschließen {#include-billable-expenses-in-a-billing-record}

Wenn Sie verrechenbare Ausgaben zum Rechnungsnachweis hinzufügen, stellen Sie sicher, dass die Ausgaben für die Aufgaben und das Projekt als verrechenbar markiert sind. Ausgaben, die nicht als „verrechenbar“ gekennzeichnet sind, können nicht in einem Rechnungsnachweis hinzugefügt werden. Weitere Informationen zum Hinzufügen von Ausgaben finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).

So fügen Sie verrechenbare Ausgaben zu einem Rechnungsnachweis hinzu:

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie **linken** auf Rechnungsnachweise .
1. Klicken Sie auf den Rechnungsnachweis **Beschreibung**, um die Registerkarte **Details zum Rechnungsnachweis** zu öffnen.
1. Klicken Sie **linken** auf „Abrechnungsfähige Ausgaben“.
1. (Bedingt) Wenn Sie Ihren Aufgaben oder dem Projekt Kosten hinzugefügt und diese als fakturierbar markiert haben, klicken Sie auf **Kosten hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Ausgaben haben, diese jedoch nicht als „Verrechenbar“ gekennzeichnet sind, wird die Schaltfläche **Ausgaben hinzufügen** nicht angezeigt. Nur fakturierbare Ausgaben mit einem tatsächlichen Betrag größer als null können in einen Rechnungsnachweis aufgenommen werden.

1. Wählen Sie die fakturierbaren Ausgaben aus, die dem Rechnungsnachweis hinzugefügt werden können, und klicken Sie dann auf **Ausgaben hinzufügen**.  Der tatsächliche Betrag der Kosten wird als &quot;**Kosten“** „Rechnungsnachweissumme **hinzugefügt**.

1. (Optional) Klicken Sie auf **Rechnungsnachweisdetails**, um die Beträge **Abrechnungsfähige Ausgaben** und **Rechnungsnachweissumme** sowie die Summe des Rechnungsnachweises in der Kopfzeile des Rechnungsnachweises zu überprüfen.

### Festeinnahmen in einen Rechnungsnachweis einbeziehen {#include-fixed-revenues-in-a-billing-record}

Sie können Festeinnahmen zu Ihren Rechnungsnachweisen hinzufügen, wenn Sie Aufgaben mit Festeinnahmen haben. Es steht kein anderer Typ von Aufgaben- oder Projektumsatz zur Verfügung, der einem Rechnungsnachweis hinzugefügt werden kann. Weitere Informationen zu Umsatztypen finden Sie im Abschnitt „Übersicht über Abrechnung und Umsatz“ im Artikel [Übersicht über Abrechnung und Umsatz](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

{{step1-to-projects}}

1. Wählen Sie auf **Seite** ein Projekt aus.
1. Klicken Sie **linken** auf Rechnungsnachweise .
1. Klicken Sie auf die **Beschreibung) des Rechnungsnachweises** um die Registerkarte **Details des Rechnungsnachweises** zu öffnen.
1. Wählen Sie die **Festeinnahmen** aus.
1. Wenn Sie Festeinnahmen zu Ihren Aufgaben hinzugefügt haben, klicken Sie auf **Festeinnahmen hinzufügen**.

   >[!NOTE]
   >
   >Wenn Sie Umsatzbeträge für Aufgaben haben, diese jedoch nicht als „Feste Einnahmen“ gekennzeichnet sind **wird die Schaltfläche „Feste** hinzufügen“ nicht angezeigt.

1. Wählen Sie die Aufgaben aus, deren Festeinnahmen Sie in den Rechnungsnachweis aufnehmen möchten, und klicken Sie dann auf **Aufgaben hinzufügen**.  Der **Festeinnahmen** der Aufgaben wird als &quot;**Einnahmen“** „Rechnungsnachweissumme **hinzugefügt**.

1. (Optional) Klicken Sie auf **Rechnungsnachweisdetails**, um die Beträge **Abrechnungsfähige Einnahmen** und **Rechnungsnachweissumme** sowie die Summe des Rechnungsnachweises in der Kopfzeile des Rechnungsnachweises zu überprüfen.

## Rechnungsnachweis bearbeiten

Nachdem Sie einen Rechnungsnachweis erstellt und ihm Stunden, Ausgaben und Einnahmen hinzugefügt haben, können Sie einige Informationen zum vorhandenen Datensatz bearbeiten, bevor er als „In Rechnung gestellt“ markiert wird.

1. Navigieren Sie zum Rechnungsnachweis.
1. Wählen **Rechnungsnachweisdetails** im linken Bedienfeld aus.
1. Bearbeiten Sie die Informationen in allen verfügbaren Feldern.

   Oder

   Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png) in der oberen rechten Ecke und bearbeiten Sie dann Informationen in allen verfügbaren Feldern.

   Aktualisieren Sie Folgendes:

   * **Beschreibung**
   * **Fakturierungsdatum**
   * **Fakturastatus**

     >[!TIP]
     >
     >Wenn Sie für **Fakturastatus die** „In Rechnung gestellt“ wählen, kann der Rechnungsnachweis nach dem Speichern der Änderungen nicht mehr bearbeitet werden.

   * **Rechnungs-ID**
   * **Bestellnummer**
   * **Zusätzlicher Betrag**

   Die folgenden Felder können nicht bearbeitet werden:

   * **Fakturierbare Stunden:** Der Gesamtbetrag der tatsächlichen Einnahmen aus den im Rechnungsnachweis enthaltenen Stunden. Weitere Informationen finden Sie im folgenden Abschnitt dieses Artikels: [Abrechnungsfähige Stunden in einen Rechnungsnachweis einbeziehen](#include-billable-hours-in-a-billing-record).

   * **Verrechenbare Ausgaben**: Der Gesamtbetrag der tatsächlichen Summe der verrechenbaren Ausgaben, die im Rechnungsnachweis enthalten sind. Weitere Informationen finden Sie im folgenden Abschnitt dieses Artikels: [Abrechnungsfähige Ausgaben in einen Rechnungsnachweis einbeziehen](#include-billable-expenses-in-a-billing-record).

   * **Fakturierbare Einnahmen**: Der Gesamtbetrag der Festeinnahmen der Aufgaben, die im Rechnungsnachweis enthalten sind. Weitere Informationen finden Sie im folgenden Abschnitt dieses Artikels: [Festeinnahmen in einen Rechnungsnachweis ](#include-fixed-revenues-in-a-billing-record).

   * **Rechnungsnachweissumme**: Die Summe aller fakturierbaren Beträge. Dies wird nach folgender Formel berechnet:

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. Klicken Sie auf **Änderungen speichern**.
