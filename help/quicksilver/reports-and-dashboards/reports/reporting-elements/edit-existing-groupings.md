---
title: Vorhandene Gruppierungen bearbeiten
description: Vorhandene Gruppierungen bearbeiten
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Vorhandene Gruppierungen bearbeiten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

Sie können eine bestehende Gruppierung anpassen, die Sie ursprünglich erstellt oder für Sie freigegeben haben. Anschließend können Sie sie als neue Gruppierung speichern.

## Zugriffsanforderungen

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Gruppierung in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten einer Gruppierung in einem Bericht verwalten</p> <p>Berechtigungen für eine Gruppierung verwalten </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen eine Gruppierung erstellen, bevor Sie sie bearbeiten können.

Informationen zum Erstellen einer Gruppierung finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## Anleitungsschritte

1. Gehen Sie zu einer Liste von Objekten, die die anzupassende Gruppierung enthalten.
1. Klicken Sie auf **Gruppierung** Symbol.
1. Wählen Sie die anzupassende Gruppierung aus und klicken Sie auf die Schaltfläche **Bearbeiten** Symbol.

   ![Wählen Sie das Bearbeitungssymbol aus.](assets/customizegrouping-nwe-standard-350x291.png)

   Der Interface Builder zum Anpassen der Gruppierung wird geöffnet.

1. Im **Gruppierungsvorschau** Abschnitt, klicken Sie auf **Gruppierung hinzufügen** um festzulegen, wie die Informationen im Bericht organisiert werden sollen. Unten finden Sie eine Vorschau der Gruppierung im Bericht.

1. Beginnen Sie mit der Eingabe des Namens des Felds, das die Art und Weise darstellt, wie Sie Informationen im Bericht organisieren möchten, und klicken Sie dann darauf, wenn es in der Dropdown-Liste angezeigt wird.
1. (Optional und bedingt) Wählen Sie beim Anzeigen einer aktualisierten Liste die Option **Diese Gruppierung standardmäßig reduzieren** wenn die Ergebnisse in der Gruppierung minimiert anstatt erweitert angezeigt werden sollen. Diese Einstellung ist standardmäßig deaktiviert und die Ergebnisse der Gruppierung werden immer in der erweiterten Liste angezeigt.

   Informationen zu aktualisierten und alten Listen finden Sie im Artikel unter &quot;Unterschied zwischen aktualisierten und alten Listen&quot;. [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* Wenn Sie Gruppierungen bei der Anzeige einer Liste manuell anpassen, behält sich Workfront Ihre manuellen Voreinstellungen vor, bis Sie sich abmelden. Wenn Sie sich wieder anmelden, wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert, nachdem sie über ein Diagrammelement oder eine veraltete Liste aufgerufen wurden. In diesen Fällen wird diese Einstellung ignoriert.


1. Wiederholen Sie die Schritte 4, 5 und 6, um weitere Gruppierungen zu definieren.\
   Sie können bis zu drei Gruppierungen definieren, um Informationen zu organisieren. Sie können Ihre Informationen mithilfe von bis zu vier Gruppierungen weiter organisieren, indem Sie einen Matrix-Bericht erstellen. Weitere Informationen zu Matrix-Berichten finden Sie unter [Erstellen eines Matrix-Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicken **Als neue Gruppierung speichern** , um die aktuelle Gruppierung durch Ihre Änderungen zu ersetzen.
