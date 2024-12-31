---
title: Bearbeiten vorhandener Gruppierungen
description: Bearbeiten vorhandener Gruppierungen
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Bearbeiten vorhandener Gruppierungen

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

Sie können eine bestehende Gruppierung, die Sie ursprünglich erstellt haben oder die für Sie freigegeben wurde, anpassen. Anschließend können Sie sie als neue Gruppierung speichern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkender oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anfrage oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Gruppierung in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht zum Bearbeiten einer Gruppierung in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Gruppierung</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen eine Gruppierung erstellen, bevor Sie sie bearbeiten können.

Informationen zum Erstellen einer Gruppierung finden Sie unter [Gruppierungen in Adobe Workfront erstellen](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Anleitungsschritte

1. Navigieren Sie zu einer Liste mit Objekten, die die Gruppierung enthalten, die Sie anpassen möchten.
1. Klicken Sie auf **Gruppierung**.
1. Wählen Sie die anzupassende Gruppierung aus und klicken Sie auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).

   ![Wählen Sie das Bearbeitungssymbol aus.](assets/customizegrouping-nwe-standard-350x291.png)

   Der Interface Builder zum Anpassen der Gruppierung wird geöffnet.

1. Klicken Sie im **Gruppierungsvorschau** auf **Gruppierung hinzufügen**, um festzulegen, wie die Informationen im Bericht organisiert werden sollen. Nachfolgend finden Sie eine Vorschau der Gruppierung im Bericht.

1. Geben Sie den Namen des Felds ein, das die Art und Weise darstellt, wie Sie Informationen im Bericht organisieren möchten, und klicken Sie dann auf den Bericht, wenn er in der Dropdown-Liste angezeigt wird.
1. (Optional und bedingt) Wählen Sie beim Anzeigen einer aktualisierten Liste die Option **Diese Gruppierung standardmäßig reduzieren**, wenn die Ergebnisse in der Gruppierung reduziert anstatt erweitert angezeigt werden sollen. Diese Einstellung ist standardmäßig deaktiviert und die Ergebnisse der Gruppierung werden immer in der erweiterten Liste angezeigt.

   Informationen zu aktualisierten und veralteten Listen finden Sie im Abschnitt „Der Unterschied zwischen aktualisierten und veralteten Listen“ im Artikel [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Wenn Sie beim Anzeigen einer Liste Gruppierungen manuell anpassen, speichert Workfront Ihre manuellen Einstellungen, bis Sie sich abmelden. Beim erneuten Anmelden wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert angezeigt, nachdem über ein Diagrammelement oder in einer Legacy-Liste darauf zugegriffen wurde. In diesen Fällen wird diese Einstellung ignoriert.

1. Wiederholen Sie die Schritte 4, 5 und 6, um zusätzliche Gruppierungen zu definieren.\
   Sie können bis zu drei Gruppierungen zum Organisieren von Informationen definieren. Sie können Ihre Informationen mit bis zu vier Gruppierungen weiter organisieren, indem Sie einen Matrixbericht erstellen. Weitere Informationen zu Matrixberichten finden Sie unter [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicken Sie **Gruppierung speichern**, um die aktuelle Gruppierung durch Ihre Änderungen zu ersetzen.
