---
product-area: projects
navigation-topic: financials
title: Verwalten von Projektausgaben
description: Die Erstellung und Verwaltung von Ausgaben ist für Projekt- und Aufgabenausgaben identisch. Alle Ausgaben, die dem Projekt im Geschäftsfall hinzugefügt werden, werden dem Tab Ausgaben als geplante Ausgaben hinzugefügt. Weitere Informationen zum Geschäftsfall finden Sie im Artikel Erstellen eines Geschäftsfeldes für ein Projekt.
author: Lisa
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 1%

---

# Verwalten von Projektausgaben

Die Erstellung und Verwaltung von Ausgaben ist für Projekt- und Aufgabenausgaben identisch. Alle Ausgaben, die dem Projekt im Geschäftsfall hinzugefügt werden, werden dem Tab Ausgaben als geplante Ausgaben hinzugefügt. Weitere Informationen zum Geschäftsfall finden Sie im Artikel [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Der Gesamtbetrag Ihrer Ausgaben für alle Aufgaben und das Projekt trägt zu den Gesamtkosten des Projekts bei. Der geplante Betrag der Ausgaben trägt zu den geplanten Kosten des Projekts bei, und der tatsächliche Betrag der Ausgaben trägt zu den tatsächlichen Kosten des Projekts bei.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Arbeit oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td>Zugriff auf Projekte und Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Contribute oder höhere Berechtigungen für das Projekt mit Berechtigungen zum Anzeigen oder Verwalten von Finanzmitteln</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ausgaben hinzufügen

1. Gehen Sie zu dem Projekt, in das Sie die Ausgaben eingeben möchten.\
   Wenn Sie einer Aufgabe Ausgaben hinzufügen möchten, navigieren Sie stattdessen zu einer Aufgabe. 
1. Klicken Sie auf **Mehr anzeigen** und dann auf **Ausgaben**.
1. Klicken Sie auf **Hinzufügen von Kosten** .
Das Dialogfeld **Hinzufügen von Ausgaben** wird angezeigt.
1. Aktualisieren Sie Folgendes:

   * **Beschreibung:** Beschreibung der Ausgabe.

   * **Ausgabentyp:** (Erforderlich) Wählen Sie die Kategorie aus, die die Kosten am besten beschreibt.
   * **Aufgabe:** Geben Sie den Namen der Aufgabe ein, mit der diese Kosten verbunden sind, und klicken Sie dann auf sie, wenn sie in der Dropdownliste angezeigt wird.
   * **Geplanter Betrag:** Der geplante veranschlagte Betrag für die Kosten.\
     Dies wirkt sich auf die budgetierten Kosten des Projekts aus.

   * **Tatsächlicher Betrag:** Der Betrag, der die tatsächlichen Kosten verursacht.\
     Dies wirkt sich auf die tatsächlichen Kosten des Projekts aus.

   * **Geplantes Datum:** Das erwartete Datum für die Ausgabe. Sie können das Datum im Feld im Format *mm/tt/jj* eingeben oder auf das Kalendersymbol klicken  2} und wählen Sie das Datum dynamisch aus.![](assets/calendar-icon.png)

   * **Datum der Bezahlung:** Das Datum, an dem die Ausgabe bezahlt wurde.
   * **Abrechenbar:** Wählen Sie diese Option, wenn Sie diese Kosten in Rechnung stellen möchten. Bei der Erstellung von Rechnungsdatensätzen ist es wichtig, eine Ausgabe als abrechnungsfähig zu kategorisieren.
   * **Erstattbar:** Wählen Sie diese Option, wenn die Kosten erstattet werden müssen. Sie können die Kosten dann nach Rückerstattung der Kosten als erstattet kennzeichnen.

1. Wählen Sie ein **benutzerdefiniertes Formular** aus und geben Sie zusätzliche erforderliche Informationen an. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einer Ausgabe verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie auf **Änderungen speichern**.

## Kosten löschen

1. Gehen Sie zum Projekt, in dem Sie Ausgaben löschen möchten.
1. Klicken Sie auf **Mehr anzeigen** und dann auf **Ausgaben**.
1. Wählen Sie die Ausgaben aus, die Sie löschen möchten, und klicken Sie dann auf **Löschen** ![Löschen](assets/delete.png).

1. Klicken Sie auf **Ja, löschen Sie es** , um den Löschvorgang zu bestätigen.
