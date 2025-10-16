---
product-area: projects
navigation-topic: financials
title: Projektausgaben verwalten
description: Der Prozess zum Erstellen und Verwalten von Ausgaben ist für Projekt- und aufgabenbezogene Ausgaben identisch. Alle Ausgaben, die dem Projekt im Business Case hinzugefügt werden, werden der Registerkarte Ausgaben als geplante Ausgaben hinzugefügt.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Projektkosten verwalten

<!-- Audited: 6/2025 -->

Der Prozess zum Erstellen und Verwalten von Ausgaben ist für Projekt- und aufgabenbezogene Ausgaben identisch. Alle Ausgaben, die dem Projekt im Business Case hinzugefügt werden, werden der Registerkarte Ausgaben als geplante Ausgaben hinzugefügt. Weitere Informationen finden Sie unter [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Der Gesamtbetrag Ihrer Ausgaben aus allen Aufgaben und Projekten trägt zu den Gesamtkosten des Projekts bei. Der geplante Betrag der Ausgaben trägt zu den geplanten Kosten des Projekts bei und der tatsächliche Betrag der Ausgaben trägt zu den Ist-Kosten des Projekts.

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
   <p>Arbeit oder höher</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Projekt bei, mit Berechtigungen zum Anzeigen oder Verwalten von Finanzdaten</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ausgaben hinzufügen

1. Wechseln Sie zu dem Projekt oder der Aufgabe, für das bzw. die Sie Ausgaben eingeben möchten.
1. Klicken Sie **linken** auf „Ausgaben“.
1. Klicken Sie **Kosten hinzufügen**. Das **Kosten hinzufügen** wird angezeigt.
1. Geben Sie die folgenden Informationen ein:

   * **Beschreibung:** Geben Sie eine Beschreibung der Ausgabe ein.
   * **Ausgabentyp:** (Erforderlich) Wählen Sie die Kategorie aus, die die Ausgabe am besten beschreibt.
   * **Aufgabe:** Sie den Namen der Aufgabe ein, mit der diese Ausgabe verbunden ist, und klicken Sie dann auf die Aufgabe, wenn sie in der Dropdown-Liste angezeigt wird.
   * **Geplanter Betrag:** Geben Sie den geplanten budgetierten Betrag für die Ausgabe ein. Dies wirkt sich auf die budgetierten Kosten des Projekts aus.

   * **Tatsächlicher Betrag** Geben Sie den Betrag ein, mit dem die tatsächlichen Kosten der Ausgabe berechnet werden. Dies wirkt sich auf die Ist-Kosten des Projekts aus.

   * **Geplantes Datum:** Geben Sie das erwartete Datum ein, an dem die Ausgabe anfallen soll. Sie können das Datum in das Feld im Format *mm/tt/jj* eingeben oder auf das **Kalender**-Symbol ![Kalendersymbol](assets/calendar-icon.png) klicken und das Datum dynamisch auswählen.

   * **Zahlungsdatum:** Sie das Datum ein, an dem die Ausgabe bezahlt wurde, oder wählen Sie es aus.
   * **Fakturierbar:** Wählen Sie diese Option, wenn Sie diese Ausgabe in Rechnung stellen möchten. Die Kategorisierung einer Ausgabe als fakturierbar ist beim Erstellen von Rechnungsnachweisen wichtig.
   * **Erstattungsfähig:** Wählen Sie diese Option, wenn die Ausgabe erstattet werden muss. Sie können die Kosten dann als erstattet markieren, nachdem die Kosten erstattet wurden.

1. Wählen Sie ein **benutzerdefiniertes Formular** und geben Sie alle erforderlichen zusätzlichen Informationen an.

   >[!NOTE]
   >
   >Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einer Ausgabe verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie auf **Speichern**.

## Kosten löschen

1. Gehen Sie zu dem Projekt, für das Sie eine Ausgabe löschen möchten.
1. Klicken Sie **linken** auf „Ausgaben“.
1. Wählen Sie die zu löschenden Ausgaben aus und klicken Sie auf das Symbol **Löschen** &quot;![Löschen](assets/delete.png).
1. Klicken Sie im **Kosten löschen** auf **Ja,**.
