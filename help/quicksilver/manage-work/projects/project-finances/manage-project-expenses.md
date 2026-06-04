---
product-area: projects
navigation-topic: financials
title: Projektausgaben verwalten
description: Der Prozess zum Erstellen und Verwalten von Ausgaben ist für Projekt- und aufgabenbezogene Ausgaben identisch. Alle Ausgaben, die dem Projekt im Business Case hinzugefügt werden, werden der Registerkarte Ausgaben als geplante Ausgaben hinzugefügt.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
TQID: https://experienceleague.adobe.com/b6lcN97EhJ4bD8w12SRE9TGLycM9Y8Si8ZSm8VBlHlA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 499
ht-degree: 10%

---

# Verwalten der Projektausgaben

<!-- Audited: 6/2025 -->

Der Prozess zum Erstellen und Verwalten von Ausgaben ist für Projekt- und aufgabenbezogene Ausgaben identisch. Alle Ausgaben, die dem Projekt im Business Case hinzugefügt werden, werden der Registerkarte Ausgaben als geplante Ausgaben hinzugefügt. Weitere Informationen finden Sie unter [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Der Gesamtbetrag Ihrer Ausgaben aus allen Aufgaben und Projekten trägt zu den Gesamtkosten des Projekts bei. Der geplante Betrag der Ausgaben trägt zu den geplanten Kosten des Projekts bei und der tatsächliche Betrag der Ausgaben trägt zu den Ist-Kosten des Projekts.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Work oder höher</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Projekt bei, mit Berechtigungen zum Anzeigen oder Bearbeiten der allgemeinen Finanzen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Ausgaben hinzufügen

1. Wechseln Sie zu dem Projekt oder der Aufgabe, für das bzw. die Sie Ausgaben eingeben möchten.
1. Klicken Sie **linken** auf „Ausgaben“.
1. Klicken Sie **Kosten hinzufügen**. Das **Kosten hinzufügen** wird angezeigt.
1. Folgende Angaben sind erforderlich:

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
