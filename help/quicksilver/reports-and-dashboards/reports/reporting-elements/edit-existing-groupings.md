---
title: Bestehende Gruppierungen bearbeiten
description: Bestehende Gruppierungen bearbeiten
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Bestehende Gruppierungen bearbeiten

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

Sie können eine bestehende Gruppierung anpassen, die Sie ursprünglich erstellt oder für Sie freigegeben haben. Anschließend können Sie sie als neue Gruppierung speichern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkende oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anforderung oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Gruppierung in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten einer Gruppierung in einem Bericht verwalten</p> <p>Berechtigungen für eine Gruppierung verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Vor der Bearbeitung müssen Sie zunächst eine Gruppierung erstellen.

Informationen zum Erstellen einer Gruppierung finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Schritte

1. Gehen Sie zu einer Liste von Objekten, die die anzupassende Gruppierung enthalten.
1. Klicken Sie auf das Symbol **Gruppierung** .
1. Wählen Sie die anzupassende Gruppierung aus und klicken Sie dann auf das Symbol **Bearbeiten** ![Bearbeiten-Symbol](assets/edit-icon.png).

   ![Wählen Sie das Bearbeitungssymbol aus.](assets/customizegrouping-nwe-standard-350x291.png)

   Der Interface Builder zum Anpassen der Gruppierung wird geöffnet.

1. Klicken Sie im Abschnitt **Gruppierungsvorschau** auf **Gruppierung hinzufügen** , um festzulegen, wie die Informationen im Bericht organisiert werden sollen. Unten finden Sie eine Vorschau der Gruppierung im Bericht.

1. Beginnen Sie mit der Eingabe des Namens des Felds, das die Art und Weise darstellt, wie Sie Informationen im Bericht organisieren möchten, und klicken Sie dann darauf, wenn es in der Dropdown-Liste angezeigt wird.
1. (Optional und bedingt) Wenn Sie eine aktualisierte Liste anzeigen, wählen Sie **Diese Gruppierung standardmäßig ausblenden** aus, wenn die Ergebnisse in der Gruppierung reduziert anstatt erweitert angezeigt werden sollen. Diese Einstellung ist standardmäßig deaktiviert und die Ergebnisse der Gruppierung werden immer in der erweiterten Liste angezeigt.

   Informationen zu aktualisierten und alten Listen finden Sie im Abschnitt &quot;Unterschied zwischen aktualisierten und alten Listen&quot;im Artikel [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Wenn Sie Gruppierungen bei der Anzeige einer Liste manuell anpassen, behält sich Workfront Ihre manuellen Voreinstellungen vor, bis Sie sich abmelden. Wenn Sie sich wieder anmelden, wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert, nachdem sie über ein Diagrammelement oder eine veraltete Liste aufgerufen wurden. In diesen Fällen wird diese Einstellung ignoriert.

1. Wiederholen Sie die Schritte 4, 5 und 6, um weitere Gruppierungen zu definieren.\
   Sie können bis zu drei Gruppierungen definieren, um Informationen zu organisieren. Sie können Ihre Informationen mithilfe von bis zu vier Gruppierungen weiter organisieren, indem Sie einen Matrix-Bericht erstellen. Weitere Informationen zu Matrix-Berichten finden Sie unter [Erstellen eines Matrix-Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicken Sie auf **Gruppierung speichern** , um die aktuelle Gruppierung durch Ihre Änderungen zu ersetzen.
