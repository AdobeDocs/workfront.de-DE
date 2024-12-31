---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen
description: Wenn in Adobe Workfront mehrere Wechselkurse konfiguriert wurden, können Sie Finanzwerte in Berichten und Listen so einstellen, dass sie in einer anderen Währung als der Standardwährung angezeigt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 2322415c173919a1fecffabb4b561645d33eea8d
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 0%

---

# Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen

<!-- Audited: 11/2024 -->

Wenn in Adobe Workfront mehrere Wechselkurse konfiguriert wurden, können Sie Finanzwerte in Berichten und Listen so einstellen, dass sie in einer anderen Währung als der Standardwährung angezeigt werden.

>[!IMPORTANT]
>
>Wenn Sie in einer Ansicht eine andere Währung als die Standardwährung auswählen, werden die Links **Weitere Aufgaben hinzufügen** und **Weitere Probleme hinzufügen** unten in einer Projektliste nicht mehr angezeigt.

Informationen zum Ändern der Standardwährung für ein bestimmtes Projekt finden Sie unter [Ändern der ](../../../manage-work/projects/project-finances/change-project-currency.md).

Wenn der Bericht Projekte mit einer einzigen Währung enthält, werden die Summen in Gruppierungen auch in der Standardwährung des Systems angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen*</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie alternative Währungen wie in diesem Abschnitt beschrieben anzeigen können, muss der Workfront-Administrator zunächst mehrere Währungen im Bereich „Einrichten“ von Workfront aktivieren und konfigurieren. Weitere Informationen finden Sie [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Finanzwerte auf einen Bericht anwenden {#apply-financial-values-to-a-report}

So konvertieren Sie Finanzwerte bei der Arbeit mit Berichten zwischen Währungen:

1. Wechseln Sie zu dem Bericht, in dem Sie Finanzwerte in eine andere Währung umrechnen möchten.
1. Klicken Sie auf **Ansicht** Dropdown-Liste, klicken Sie auf **Währung ändern** und wählen Sie dann eine der folgenden Währungen aus, in der Sie Finanzwerte anzeigen möchten:

   * Originalwährung des Projekts
   * Eine der anderen Währungen

     >[!TIP]
     >
     >Sie können nur Währungen auswählen, die zuvor in „Setup“ ausgewählt wurden.

   Mit dieser Option können Sie Finanzwerte in einem Bericht schnell zwischen Kurswerten konvertieren.

   ![Währung ändern](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## Standardwährung für mehrere Projekte mit unterschiedlichen Währungen anzeigen

Wenn Sie die Währung auf Projektebene anpassen und Informationen aus allen Projekten im selben Bericht anzeigen möchten, gibt es die folgenden Szenarien:

* Wenn Sie einen Bericht erstellen, der Finanzinformationen aus zwei oder mehr Projekten mit unterschiedlichen Währungen enthält, spiegelt die Gruppierungsübersicht standardmäßig die Standardwährung des Systems wider, die vom Workfront-Administrator ausgewählt wurde.
* Wenn Sie einen Bericht für zwei oder mehr Projekte erstellen, die dieselbe Währung haben, sich aber von der Standardwährung des Systems unterscheiden, werden die Summen in den Gruppierungen in der Standardwährung des Systems angezeigt.
* Wenn Sie einen Bericht für zwei oder mehr Projekte erstellen, denen Aufgabengebietszuweisungen mit einer Währungsüberschreibungen verknüpft sind, konvertiert Workfront die Finanzinformationen aus den überschriebenen Währungskursen des Aufgabengebiets entweder in die Projektwährung (wenn Sie die Originalwährung des Projekts in der Ansicht auswählen) oder in eine andere Währung, die Sie beim Anzeigen des Berichts auswählen. Informationen zum Außerkraftsetzen der Währung eines Aufgabengebiets finden Sie unter [Erstellen und Verwalten von ](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)&quot;.

So zeigen Sie zwei Projekte mit benutzerdefinierten Währungen in einem Bericht an:

1. Erstellen Sie zwei Projekte mit unterschiedlichen Währungen.

   ![](assets/qs-currency-350x217.png)

1. Stunden für beide Projekte protokollieren.

   Weitere Informationen zur Zeitprotokollierung finden Sie unter [Zeit protokollieren](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Klicken Sie auf das **Hauptmenü**-Symbol ![](assets/main-menu-icon.png) und dann auf **Reporting**.
1. Klicken Sie **Neuer Bericht**, dann **Projektbericht**.
1. Fügen Sie auf der Registerkarte **Spalten (Ansicht)** die Spalte **Istkosten** hinzu und fassen Sie sie nach **Summe** zusammen.

   Informationen zum Erstellen einer Spalte finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Wenden Sie auf **Registerkarte** eine Gruppierung **Geplantes Abschlussdatum** an.

   Informationen zum Erstellen einer Gruppierung finden Sie unter ([ Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Fügen Sie auf **Registerkarte** einen Filter für **Projektname** hinzu und wählen Sie die beiden Projekte mit den verschiedenen Währungen aus.

   Informationen zum Erstellen eines Filters finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Klicken Sie auf **Speichern + schließen**.

   Die Summe der **Ist-Kosten** wird in der Gruppierung unter Verwendung der Systemstandardwährung angezeigt, unabhängig von der Währung der Projekte im Bericht.

   Wenn die beiden Projekte unterschiedliche Währungen haben, wird die Standardwährung des Systems auch in der Gruppierung des Berichts angezeigt.

## Zeigen Sie die Projektwährung in einem Bericht auf Projektebene an

Wenn innerhalb eines Projekts eine Gruppierung auf eine Aufgaben- oder Stundenliste angewendet wird, werden die Summen in der Gruppierung in der Projektwährung angezeigt.

1. Erstellen Sie ein Projekt mit einer benutzerdefinierten Währung, die sich von der Standardwährung des Systems unterscheidet.
1. Wechseln Sie zum Projekt und stellen Sie sicher, dass es Stunden enthält, die für Aufgaben protokolliert wurden.

   Weitere Informationen zur Zeitprotokollierung finden Sie unter [Zeit protokollieren](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >Die Aufgaben sollten Benutzern oder Aufgabengebieten mit Kostensätzen pro Stunde zugewiesen werden.

1. Klicken Sie auf **Aufgaben**.
1. Erweitern Sie das **Ansicht** Dropdown-Menü und wählen Sie **Neue Ansicht**.
1. Fügen Sie **Istkosten** in der neuen Ansicht als neue Spalte hinzu und fassen Sie sie nach &quot;**&quot;**.
1. Klicken Sie **Fertig** und dann auf **Ansicht speichern**.
1. Erweitern Sie das **Gruppierung** Dropdown-Menü und wählen Sie **Neue Gruppierung**.
1. Fügen Sie **neue Gruppierung das** Tatsächliches Abschlussdatum“ als neues Feld hinzu und klicken Sie dann auf **Gruppierung speichern**.

   Die Spalte **Istkosten** wird in der neuen Gruppierung zusammengefasst und zeigt den Gesamtbetrag in der Währung des Projekts an.

## Berichte mit eindeutigen Währungen bearbeiten

Die Finanzfelder in einem Bericht können erst bearbeitet werden, wenn die Berichtseinstellung so geändert wurde, dass die Originalwährung für Projekte angezeigt wird.

So bearbeiten Sie ein Finanzfeld in einem Bericht inline:

1. Navigieren Sie zu einem Bericht.

   >[!NOTE]
   >
   >Wenn die Standardwährung für eine Liste in keinem anderen Bereich angezeigt wird, können Sie die Ansicht so bearbeiten, dass die Standardwährung angezeigt wird.\
   >Informationen zum Ändern der Währung in einer Ansicht finden Sie im Abschnitt in diesem Artikel [Anwenden von Finanzwerten auf einen Bericht](#apply-financial-values-to-a-report).

1. Klicken Sie **Berichtsaktionen** und wählen Sie dann **Bearbeiten**.
1. Klicken Sie **Berichteinstellungen**.
1. Klicken Sie auf **Dropdown-** „Standardwährung“ und wählen Sie dann **Originalwährung des Projekts**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Klicken Sie **Fertig**.
