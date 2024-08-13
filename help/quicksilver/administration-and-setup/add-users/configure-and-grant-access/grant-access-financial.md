---
title: Zugriff auf Finanzdaten gewähren
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Finanzdaten in Workfront über dessen Zugriffsstufe definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Zugriff auf Finanzdaten gewähren

{{highlighted-preview}}

Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Folgendes über die Zugriffsebene des Benutzers definieren, wie in der Übersicht über die Zugriffsstufen [](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben:

* Finanzinformationen zu Projekten in Workfront
* Ressourcenbudgeting-Informationen in den Tools für die Ressourcenplanung

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Überlegungen zur Gewährung des Zugangs zu Finanzdaten

Beachten Sie Folgendes, wenn Sie Benutzern Zugriff auf Finanzdaten in Workfront gewähren:

* Ein Benutzer, dessen Zugriffsstufe keinen Zugriff auf Finanzdaten zulässt, kann kein Risiko für ein Projekt darstellen. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* Sie können auch eine Zugriffsebene verwenden, um zu bestimmen, welche Ressourcen-Management-Aktivitäten ein Benutzer zum Budget oder zur Anzeige der Ressourcenzuordnung verwenden kann. Weitere Informationen finden Sie unter [Zugriff auf die Ressourcenverwaltung gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Benutzerzugriff auf Finanzdaten mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Beginnen Sie mit der Erstellung oder Bearbeitung der Zugriffsebene, wie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) beschrieben.
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche **Ansicht** oder **Bearbeiten** rechts neben Finanzdaten und wählen Sie dann die Fähigkeiten aus, die Sie unter **Feinabstimmung Ihrer Einstellungen** gewähren möchten.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Optional) Wählen Sie im Bereich **Administratorzugriff für** zulassen die folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Wechselkurse</td> 
      <td> <p>Neue Währung in Workfront hinzufügen.</p> <p>Ohne diesen Zugriff kann der Benutzer einem von ihm erstellten Projekt nur eine vorhandene Währung hinzufügen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td> <p>Zeigen Sie alle Ausgaben für Objekte in Workfront an.</p> <p>Dadurch kann der Benutzer keine neuen Ausgabentypen erstellen.</p> <p>Ohne diesen Zugriff kann der Benutzer nur Folgendes anzeigen:</p> 
       <ul> 
        <li>Ausgaben für von ihnen verwaltete Projekte, Aufgaben oder Probleme</li> 
        <li>Ihre eigenen Ausgaben</li> 
        <li>Die Kosten für ihre Untergebenen</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugang zu gemeinsamen Finanzinformationen

Sie können finanzielle Informationen zu einem Projekt, einer Aufgabe oder einem Problem für andere Benutzer freigeben, indem Sie ihnen Berechtigungen erteilen, wie unter [Finanzberechtigungen für ein Objekt freigeben](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md) beschrieben.

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Wenn Sie ein Objekt für einen anderen Benutzer freigeben, werden die Rechte des Empfängers für dieses Objekt durch eine Kombination aus zwei Faktoren bestimmt:

* Die Berechtigungen, die Sie Ihrem Empfänger für das Objekt gewähren
* Einstellungen der Zugriffsebene des Empfängers für den Objekttyp

## Zugang zu Finanzinformationen nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Finanzinformationen tun können, finden Sie im Abschnitt [Finanzdaten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugang zu Finanzinformationen durch

Die folgenden Informationen helfen Ihnen dabei zu verstehen, wie Sie mithilfe der Einstellungen auf Zugriffsebene den Zugriff der Benutzer auf Finanzdaten steuern können.

### Kein Zugriff

Ein Benutzer ohne Zugriff auf Finanzdaten hat keinen Zugriff auf Folgendes:

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* <span class="preview">Karten bewerten</span>
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Anzeigen in Schritt 4 konfigurieren.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Anzeigen in Schritt 4 konfigurieren.

### Zugriff anzeigen

Benutzer mit Zugriff auf Finanzdaten anzeigen können Folgendes anzeigen (nicht bearbeiten):

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Anzeigen in Schritt 4 konfigurieren.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Anzeigen in Schritt 4 konfigurieren.

### Zugriff bearbeiten

Ein Benutzer mit Zugriff auf Finanzdaten bearbeiten kann Folgendes anzeigen und bearbeiten:

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* <span class="preview">Karten bewerten</span>
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Bearbeiten in Schritt 4 konfigurieren.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies mit dem Zahnradsymbol ![](assets/gear-icon-settings.png) auf der Schaltfläche Bearbeiten in Schritt 4 konfigurieren.
