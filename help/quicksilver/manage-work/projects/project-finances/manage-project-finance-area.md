---
product-area: projects
navigation-topic: financials
title: Verwalten von Informationen im Bereich Projektfinanzierung
description: Sie können die Finanzinformationen eines Projekts anzeigen oder bearbeiten, indem Sie auf den Bereich Finanzen des Abschnitts Projektdetails zugreifen.
author: Lisa
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 2%

---

# Verwalten von Informationen im Projektfinanzierungsbereich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Sie können die Finanzinformationen eines Projekts anzeigen oder bearbeiten, indem Sie auf den Bereich Finanzen des Abschnitts Projektdetails zugreifen. Es gibt eine begrenzte Anzahl von Feldern, die Sie in diesem Bereich anzeigen oder bearbeiten können. Informationen zum Bearbeiten aller Informationen für ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td>
   <p>Neu: Licht oder höher</p>
   <p>oder</p>
   <p>Aktuell: Überprüfung oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte und Finanzdaten</p> <p>Zugriff auf Projekte und Finanzdaten bearbeiten, um Finanzinformationen zum Projekt zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für ein Projekt oder höher, die Berechtigungen zum Anzeigen von Finanzdaten enthalten</p> <p>Verwalten Sie Berechtigungen für das Projekt, einschließlich Verwalten von Finanzinformationen zum Bearbeiten von Finanzinformationen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überblick über den Finanzbereich

Beachten Sie beim Anzeigen oder Bearbeiten von Informationen im Bereich „Finanzen“ Folgendes:

* Die Finanzinformationen, die Sie im Bereich Finanzen der Projektdetails finden, stellen Werte dar, die sich aus den Aufgaben auf Projektebene summieren, sowie Informationen, die direkt in das Projekt eingegeben wurden. Einige Finanzinformationen können sowohl auf Projekt- als auch auf Aufgabenebene verwaltet werden.
* Sie müssen über Anzeigeberechtigungen für das Projekt sowie über Zugriff auf Finanzdaten auf Ihrer Zugriffsebene verfügen, um den Finanzbereich für ein Projekt anzeigen zu können.
* Sie müssen über Verwaltungsberechtigungen für das Projekt sowie über Zugriff auf Finanzdaten von Ihrer Zugriffsebene verfügen, um die Informationen im Finanzbereich bearbeiten zu können. Wir empfehlen jedoch, dass nur der Projektinhaber die Informationen in diesem Bereich bearbeiten sollte.

## Finanzinformationen zu einem Projekt anzeigen

1. Gehe zu einem Projekt.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![](assets/edit-icon.png) in der oberen rechten Ecke des Abschnitts Details und dann auf **Finanzen**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Je nachdem, wie Workfront-Admins Ihre Layout-Vorlage konfiguriert haben, wird der Abschnitt Übersicht möglicherweise nicht zuerst aufgeführt. In diesem Fall wird er reduziert. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Sehen Sie sich die folgenden Felder im Bereich Finanzen des Projekts an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance-Index-Methode</td> 
      <td> Steuert die Methode, die Workfront zur Berechnung von Earned Value-Metriken verwendet. Es kann stundenbasiert oder kostenbasiert sein. <br>Weitere Informationen zum PIM finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Festlegen der Leistungsindexmethode (PIM)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>Dies sind Projektleistungsmetriken, die zeigen, wie Ihr Projekt zu einem bestimmten Zeitpunkt funktioniert. Die Werte werden anhand der Performance-Index-Methode berechnet.<br>Weitere Informationen finden Sie in den folgenden Artikeln: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Kostenentwicklungsindex (Cost Performance Index, CPI) berechnen</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Planleistungsindex (SPI)-</a> berechnen </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Kostenplan-Leistungsindex (CSI) berechnen</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung bei Fertigstellung</td> 
      <td> Projizierte Gesamtkosten Ihres Projekts in Stunden, wenn die Leistungsindexmethode (PIM) stundenbasiert ist, und in einem Währungswert dargestellt, wenn die Leistungsindexmethode (PIM) kostenbasiert ist.<br>Weitere Informationen zur Berechnung der Schätzung bis zum Abschluss finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Berechnung der Schätzung bis zum Abschluss (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Dies ist das Budget für das Projekt. Dies wird vom Projektbesitzer manuell angegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixkosten</td> 
      <td>Dies sind die Fixkosten des Projekts, unabhängig von anderen Aktivitäten im Projekt. Sie werden vom Projektbesitzer manuell eingegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Kosten</td> 
      <td>Die geschätzten Kosten des Projekts, basierend auf den geplanten Stunden und den mit den Aufgabenzugewiesenen verknüpften Sätzen (Aufgabengebiete oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist-Kosten</td> 
      <td>Alle dem Projekt entstehenden Kosten. Ist-Kosten sind die Summe aller Ist-Kosten: Arbeitskosten (auf der Basis der Ist-Stunden und der Sätze, die mit den Aufgabengebieten oder Benutzern verknüpft sind, die sie protokollieren), Ausgaben und Fixkosten, die mit einem Projekt oder einer Aufgabe verknüpft werden können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Festeinnahmen</td> 
      <td>Berechnete Einnahmen basierend auf dem Projektzeitplan festlegen Festeinnahmen werden vom Projektbesitzer manuell angegeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplante Einnahmen</td> 
      <td>Voraussichtliches Einkommen basierend auf den geplanten Stunden und den mit den Aufgabenzugewiesenen verknüpften Sätzen (Aufgabengebiete oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliche Einnahmen</td> 
      <td>Tatsächliches Einkommen aus dem Projekt basierend auf den tatsächlichen Stunden und den mit den Aufgabenzugewiesenen verknüpften Sätzen (Aufgabengebiete oder Benutzer).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">In Rechnung gestellte Einnahmen</td> 
      <td> <p>Einnahmen, die Kunden oder anderen Parteien in Rechnung gestellt werden und in Rechnungsnachweisen erfasst werden. Weitere Informationen zu Rechnungsnachweisen finden Sie im Artikel <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Rechnungsnachweise erstellen</a>. </p> </td> 
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

## Finanzinformationen zu einem Projekt bearbeiten

Als Projektbesitzer können Sie die Informationen auf der Unterregisterkarte „Finanzen“ eines Projekts bearbeiten.

So bearbeiten Sie Informationen zur Unterregisterkarte „Projektfinanzierung“:

1. Wechseln Sie zu einem Projekt, dessen Besitzer Sie sind.

   >[!NOTE]
   >
   >Sie müssen Berechtigungen verwalten für das Projekt, um die folgenden Schritte ausführen zu können. Es wird außerdem empfohlen, dass nur der/die Projektbesitzer(in) Änderungen an der Unterregisterkarte Finanzen des Projekts vornehmen sollte.

1. Klicken Sie **linken** auf „Projektdetails“.
1. Klicken Sie auf **Bearbeiten**-Symbol ![](assets/edit-icon.png) in der oberen rechten Ecke des Abschnitts Details und dann auf **Finanzen** . Dadurch wird der Bereich Finanzen zur Bearbeitung geöffnet.
1. Bearbeiten Sie alle Felder, die bearbeitet werden können, indem Sie einfach auf das Feld klicken oder auf **+Hinzufügen** klicken, um einem leeren Feld Informationen hinzuzufügen.

   >[!TIP]
   >
   >Felder können nicht bearbeitet werden, wenn sie automatisch von Workfront berechnet werden oder wenn keine Bearbeitungsberechtigungen dafür vorliegen.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Aktualisieren Sie eines der folgenden Felder.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator Ihre Layout-Vorlage einrichtet, können die Felder im Abschnitt Projektdetails in Ihrer Umgebung unterschiedlich sein. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Performance-Index-Methode</td> 
      <td> <p>Steuert die Methode, die Workfront zum Berechnen von Projektleistungsmetriken verwendet. Diese wird von Ihrem Administrator auf Systemebene eingerichtet, Sie können sie jedoch auch auf Projektebene bearbeiten. Erwägen Sie die Auswahl einer der folgenden Optionen:</p> 
       <ul> 
        <li><strong>Stundenbasiert:</strong>Workfront verwendet die geplanten Stunden für die Berechnung des CPI und der EAC des Projekts. Die EAC des Projekts wird als eine Zahl in Stunden angezeigt. </li> 
        <li><strong>Kostenbasiert:</strong>Workfront verwendet bei der Berechnung des CPI und der EAC des Projekts die geplanten Lohnkosten. Die EAC wird als Währungswert angezeigt. Wenn Sie diese Option auswählen, stellen Sie sicher, dass Ihre Aufgabenzugewiesenen (Aufgabengebiete oder Benutzer) mit Kostensätzen verknüpft sind.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schätzung bei Fertigstellung</td> 
      <td> <p>Stellt die erwarteten Gesamtkosten Ihres Projekts oder Ihrer Aufgabe dar, wenn es abgeschlossen ist. Diese wird von Ihrem Administrator auf Systemebene eingerichtet, Sie können sie jedoch auch auf Projektebene bearbeiten. Erwägen Sie die Auswahl einer der folgenden Optionen:</p> 
       <ul> 
        <li><strong>Auf Projektebene berechnen</strong>: Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt wird durch Eingabe der tatsächlichen Stunden/tatsächlichen Arbeitskosten in die BK-Formeln bestimmt. Diese Berechnung beinhaltet die tatsächlichen Stunden/Kosten und Ausgaben, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</li> 
        <li><strong>Aus Aufgaben/Teilaufgaben aggregieren</strong>: Die BK für die übergeordnete Aufgabe und das übergeordnete Projekt wird bestimmt, indem die BK für jede untergeordnete Aufgabe zusammengefasst werden. Diese Berechnung schließt die tatsächlichen Stunden/Kosten und Ausgaben aus, die direkt zur übergeordneten Aufgabe oder zum übergeordneten Projekt hinzugefügt werden.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Budget</td> 
      <td>Budget für dieses Projekt angeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fixkosten</td> 
      <td>Geben Sie die Fixkosten für dieses Projekt an. Dies sollte keine Arbeits- oder Ausgabenkosten beinhalten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Festeinnahmen</td> 
      <td> <p>Geben Sie die Festeinnahmen dieses Projekts an. Dies sollte keine Einnahmen aus Rechnungsnachweisen enthalten, die Partnern oder Dritten in Rechnung gestellt werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projektwährung</td> 
      <td> <p>Geben Sie eine Währung für dieses Projekt an, wenn sie sich von der Standardwährung in Ihrem System unterscheidet. Die Standardwährung in Ihrem System wird von Ihrem Workfront-Administrator festgelegt. Weitere Informationen zum Einrichten von Wechselkursen in Workfront finden Sie im Artikel <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> </td> 
     </tr>
    </tbody> 
   </table>

1. Klicken Sie auf **Änderungen speichern**.
