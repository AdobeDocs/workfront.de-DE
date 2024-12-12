---
product-area: projects
navigation-topic: financials
title: Verwalten von Informationen im Bereich "Projekt-Finanzen"
description: Sie können die Finanzinformationen eines Projekts anzeigen oder bearbeiten, indem Sie auf den Bereich "Finanzen"im Abschnitt "Projektdetails"zugreifen.
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 2%

---

# Verwalten von Informationen im Bereich &quot;Projekt-Finanzen&quot;

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Sie können die Finanzinformationen eines Projekts anzeigen oder bearbeiten, indem Sie auf den Bereich &quot;Finanzen&quot;im Abschnitt &quot;Projektdetails&quot;zugreifen. Es gibt eine begrenzte Anzahl von Feldern, die Sie in diesem Bereich anzeigen oder bearbeiten können. Informationen zum Bearbeiten aller Informationen für ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Neu: Licht oder höher</p>
   <p>oder</p>
   <p>Aktuell: Überprüfen oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Anzeigen oder Verbessern des Zugriffs auf Projekte und Finanzdaten</p> <p>Zugriff auf Projekte und Finanzdaten bearbeiten, um Finanzinformationen zu dem Projekt zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für ein Projekt oder höher, die View Finance-Berechtigungen enthalten</p> <p>Verwalten von Berechtigungen für das Projekt, die "Verwalten von Finanzinformationen"zum Bearbeiten von Finanzinformationen für das Projekt enthalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über den Finanzbereich

Beachten Sie Folgendes beim Anzeigen oder Bearbeiten von Informationen im Bereich &quot;Finanzen&quot;:

* Die Finanzinformationen, die Sie im Bereich &quot;Finanzen&quot;unter &quot;Projektdetails&quot;finden, stellen Werte dar, die aus Aufgaben bis zur Projektebene aggregiert werden, sowie direkt im Projekt eingegebene Informationen. Manche Finanzinformationen können sowohl auf Projekt- als auch Aufgabenebene verwaltet werden.
* Sie müssen über Anzeigeberechtigungen für das Projekt sowie Zugriff auf Finanzdaten von Ihrer Zugriffsebene verfügen, um den Finanzbereich für ein Projekt anzeigen zu können.
* Sie müssen über Verwaltungsberechtigungen für das Projekt sowie Zugriff auf Finanzdaten von Ihrer Zugriffsebene verfügen, um die Informationen im Finanzbereich bearbeiten zu können. Es wird jedoch empfohlen, dass nur der Projekteigentümer die Informationen zu diesem Bereich bearbeiten sollte.

## Anzeigen von Finanzinformationen für ein Projekt

1. Wechseln Sie zu einem Projekt.
1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke des Detailbereichs und dann auf **Finanzen**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator Ihre Layout-Vorlage konfiguriert hat, wird der Abschnitt Übersicht möglicherweise nicht zuerst aufgeführt. In diesem Fall wird er reduziert. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Zeigen Sie die folgenden Felder im Bereich &quot;Finanzen&quot;des Projekts an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance-Index-Methode</td> 
      <td> Steuert die Methode, die Workfront zur Berechnung der Earned Value-Metriken verwendet. Es kann stundenbasiert oder kostenbasiert sein. <br>Weitere Informationen zum PIM finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Festlegen der Leistungsindex-Methode (PIM)</a> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Dies sind Metriken zur Projektleistung, die die Leistung Ihres Projekts zu einem bestimmten Zeitpunkt anzeigen. Ihre Werte werden auf der Grundlage der Leistungsindex-Methode berechnet.<br>Weitere Informationen finden Sie in den folgenden Artikeln: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calculate Cost Performance Index (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Planen Sie den Leistungs-Index (SPI) berechnen </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Berechnen des Performance-Index des Kostenplans (CSI)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung bei Fertigstellung</td> 
      <td> Die prognostizierten Gesamtkosten Ihres Projekts werden in Stunden dargestellt, wenn die Performance Index Method (PIM) stundenbasiert ist und in einem Währungswert dargestellt wird, wenn die Performance Index Method (PIM) kostenbasiert ist.<br>Weitere Informationen zur Berechnung der Schätzung nach Abschluss finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Schätzung nach Abschluss berechnen (EAC) berechnen</a> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Dies ist der Budgetsatz für das Projekt. Dies wird vom Projekteigentümer manuell angegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixkosten</td> 
      <td>Dies sind die Fixkosten des Projekts, unabhängig von anderen Aktivitäten des Projekts. Sie werden vom Projekteigentümer manuell eingegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Kosten</td> 
      <td>Die geschätzten Kosten des Projekts basierend auf den geplanten Stunden und den mit der Aufgabe verbundenen Raten (Stellenrollen oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist-Kosten</td> 
      <td>Alle Kosten des Projekts. Die tatsächlichen Kosten sind die Summe aller tatsächlichen Kosten: Arbeitskosten (basierend auf tatsächlichen Stunden und den mit den Arbeitsplatzrollen oder den Nutzern, die sie protokollieren, verbundenen Tarifen), Ausgaben und Festkosten, die mit einem Projekt oder einer Aufgabe verknüpft werden können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Festeinnahmen</td> 
      <td>Legen Sie die erwarteten Einnahmen basierend auf dem Projektplan fest. Der feste Umsatz wird vom Projekteigentümer manuell angegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Einnahmen</td> 
      <td>Erwartete Einnahmen basierend auf den geplanten Stunden und den mit der Aufgabe verbundenen Raten (Stellenrollen oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Einnahmen</td> 
      <td>Tatsächliches Ergebnis des Projekts basierend auf den tatsächlichen Stunden und den mit der Aufgabe verbundenen Raten (Stellenrollen oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">In Rechnung gestellte Einnahmen</td> 
      <td> <p>Umsatz, der Kunden oder anderen Parteien in Rechnung gestellt und in Rechnungsaufzeichnungen erfasst wird. Weitere Informationen zu Rechnungsdatensätzen finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Erstellen von Rechnungsdatensätzen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Bearbeiten von Finanzinformationen zu einem Projekt

Als Projekteigentümer können Sie die Informationen auf der Unterregisterkarte &quot;Finanzen&quot;eines Projekts bearbeiten.

So bearbeiten Sie Informationen auf der Unterregisterkarte Projekt-Finanzen :

1. Gehen Sie zu einem Projekt, dessen Eigentümer Sie sind.

   >[!NOTE]
   >
   >Für die folgenden Schritte benötigen Sie die Berechtigung zum Verwalten des Projekts. Es wird außerdem empfohlen, dass nur der Projekteigentümer Änderungen an der Unterregisterkarte &quot;Finanzen&quot;des Projekts vornimmt.

1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) in der oberen rechten Ecke des Bereichs Details und klicken Sie dann auf **Finanzen** . Dadurch wird der Finanzbereich zur Bearbeitung geöffnet.
1. Bearbeiten Sie alle Felder, die bearbeitet werden können, indem Sie mit einem einzigen Klick auf das Feld klicken oder auf **+Hinzufügen** klicken, um Informationen zu einem leeren Feld hinzuzufügen.

   >[!TIP]
   >
   >Felder können nicht bearbeitet werden, wenn sie automatisch von Workfront berechnet werden oder wenn Sie nicht über Bearbeitungsberechtigungen verfügen.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Aktualisieren Sie eines der folgenden Felder.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator unsere Layoutvorlage eingerichtet hat, unterscheiden sich die Felder im Abschnitt Projektdetails möglicherweise in Ihrer Umgebung. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance-Index-Methode</td> 
      <td> <p>Steuert die Methode, die Workfront zur Berechnung der Projektleistungsmetriken verwendet. Diese wird von Ihrem Administrator auf Systemebene eingerichtet, Sie können sie aber auch auf Projektebene bearbeiten. Wählen Sie eine der folgenden Optionen aus:</p> 
       <ul> 
        <li><strong>Stündlich:</strong>Workfront verwendet die geplanten Stunden zur Berechnung des CPI und des EAC des Projekts, und die EAC des Projekts wird als Zahl in Stunden angezeigt. </li> 
        <li><strong>Kostenbasiert:</strong>Workfront verwendet die geplanten Arbeitskosten zur Berechnung des CPI und des EAC des Projekts, und der EAC wird als Währungswert angezeigt. Wenn Sie diese Option auswählen, stellen Sie sicher, dass Ihre Aufgabenverantwortlichen (Auftragsrollen oder Benutzer) den Kostenstellen zugeordnet sind.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung bei Fertigstellung</td> 
      <td> <p>Stellt die voraussichtlichen Gesamtkosten Ihres Projekts oder Ihrer Aufgabe nach Abschluss dar. Diese wird von Ihrem Administrator auf Systemebene eingerichtet, Sie können sie aber auch auf Projektebene bearbeiten. Wählen Sie eine der folgenden Optionen aus:</p> 
       <ul> 
        <li><strong>Auf Projektebene berechnen</strong>: Die EAC für die übergeordnete Aufgabe und das Projekt wird durch Eingabe der tatsächlichen Stunden/ tatsächlichen Arbeitskosten in die EAC-Formeln bestimmt. Diese Berechnung umfasst die tatsächlichen Stunden/ Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</li> 
        <li><strong>Aufrollen aus Aufgaben/Unteraufgaben</strong>: Die EAC für die übergeordnete Aufgabe und das Projekt wird durch Addieren der EAC für jede untergeordnete Aufgabe bestimmt. Diese Berechnung schließt tatsächliche Stunden/-kosten und -aufwendungen aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Geben Sie das Budget für dieses Projekt an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixkosten</td> 
      <td>Geben Sie die Festkosten für dieses Projekt an. Dies sollte keine Arbeits- oder Ausgabenkosten beinhalten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Festeinnahmen</td> 
      <td> <p>Geben Sie den festen Umsatz für dieses Projekt an. Dies sollte keine Einnahmen aus Abrechnungseinträgen umfassen, die an Partner oder Dritte in Rechnung gestellt werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektwährung</td> 
      <td> <p>Geben Sie eine Währung für dieses Projekt an, wenn diese von der Standardwährung in Ihrem System abweicht. Die Standardwährung in Ihrem System wird von Ihrem Workfront-Administrator definiert. Weitere Informationen zur Einrichtung von Wechselkursen in Workfront finden Sie im Artikel <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf **Änderungen speichern**.
