---
title: Zugriff auf Finanzdaten gewähren
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Finanzdaten in Workfront über dessen Zugriffsstufe definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Zugriff auf Finanzdaten gewähren

{{highlighted-preview}}

Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Folgendes über die Zugriffsebene des Benutzers definieren, wie unter [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Finanzinformationen zu Projekten in Workfront
* Ressourcenbudgeting-Informationen in den Tools für die Ressourcenplanung

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Überlegungen zur Gewährung des Zugangs zu Finanzdaten

Beachten Sie Folgendes, wenn Sie Benutzern Zugriff auf Finanzdaten in Workfront gewähren:

* Ein Benutzer, dessen Zugriffsstufe keinen Zugriff auf Finanzdaten zulässt, kann kein Risiko für ein Projekt darstellen. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* Sie können auch eine Zugriffsebene verwenden, um zu bestimmen, welche Ressourcen-Management-Aktivitäten ein Benutzer zum Budget oder zur Anzeige der Ressourcenzuordnung verwenden kann. Weitere Informationen finden Sie unter [Zugriff auf Resource Management gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Benutzerzugriff auf Finanzdaten mithilfe einer benutzerdefinierten Zugriffsebene konfigurieren

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie hier beschrieben: [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) auf **Ansicht** oder **Bearbeiten** rechts neben Finanzdaten, und wählen Sie dann die Fähigkeiten aus, die Sie unter **Einstellungen anpassen**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Optional) Im **Administratorzugriff zulassen für** -Bereich die folgenden Optionen auswählen:

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

1. (Optional) Um die Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene zu konfigurieren, an der Sie arbeiten, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) wie [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugang zu gemeinsamen Finanzinformationen

Sie können finanzielle Informationen zu einem Projekt, einer Aufgabe oder einem Problem mit anderen Benutzern teilen, indem Sie ihnen Berechtigungen erteilen, wie hier beschrieben: [Freigeben von Finanzberechtigungen für ein Objekt](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

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

Informationen darüber, was Benutzer in den einzelnen Zugriffsebenen mit Finanzinformationen tun können, finden Sie im Abschnitt [Finanzdaten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Zugang zu Finanzinformationen durch

Die folgenden Informationen helfen Ihnen dabei zu verstehen, wie Sie mithilfe der Einstellungen auf Zugriffsebene den Zugriff der Benutzer auf Finanzdaten steuern können.

### Kein Zugriff

Ein Benutzer ohne Zugriff auf Finanzdaten hat keinen Zugriff auf Folgendes:

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* <span class="preview">Ratenkarten</span>
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Anzeigen in Schritt 4 oben.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Anzeigen in Schritt 4 oben.

### Zugriff anzeigen

Benutzer mit Zugriff auf Finanzdaten anzeigen können Folgendes anzeigen (nicht bearbeiten):

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Anzeigen in Schritt 4 oben.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Anzeigen in Schritt 4 oben.

### Zugriff bearbeiten

Ein Benutzer mit Zugriff auf Finanzdaten bearbeiten kann Folgendes anzeigen und bearbeiten:

* Finanzabschnitt unter Projekt- und Aufgabenobjekte
* Geschäftsfall
* Abrechnungssätze und Rechnungsbelege
* <span class="preview">Ratenkarten</span>
* Kosten pro Stunde und Abrechnung pro Stunde für Benutzereinstellungen

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Bearbeiten in Schritt 4.

* Kosten pro Stunde und Abrechnung pro Stunde für Job Roles

  Sie können dies über das Zahnradsymbol konfigurieren ![](assets/gear-icon-settings.png) auf die Schaltfläche Bearbeiten in Schritt 4.
