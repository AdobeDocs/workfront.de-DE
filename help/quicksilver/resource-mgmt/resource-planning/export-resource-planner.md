---
product-area: resource-management
navigation-topic: resource-planning
title: Exportieren von Informationen aus dem Ressourcenplaner
description: Sie können Informationen aus einer beliebigen Ansicht des Resource Planers in eine Excel-Datei (.xlsx) exportieren, die auf Ihrem Computer gespeichert ist.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Exportieren von Informationen aus dem Ressourcenplaner

Sie können Informationen aus einer beliebigen Ansicht des Resource Planers in eine Excel-Datei (.xlsx) exportieren, die auf Ihrem Computer gespeichert ist.

>[!IMPORTANT]
>
>Es gibt Einschränkungen hinsichtlich der angezeigten Informationen und der Informationen, die Sie aus dem Ressourcen-Planer exportieren können. Informationen zu diesen Einschränkungen finden Sie unter [Anzeigebeschränkungen für den Ressourcenplaner](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Benutzer und Ressourcenverwaltung anzeigen oder höher</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Projekte anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Exportieren von Informationen aus dem Ressourcenplaner

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Ressourcen**. Die **Planen** wird standardmäßig angezeigt.

1. Wählen Sie die Ansicht für den Planer aus. Sie können eine der folgenden Optionen auswählen:

   * Nach Benutzer anzeigen
   * Nach Projekt anzeigen
   * Nach Funktion anzeigen

1. Klicken **Export**.

   Das Dialogfeld &quot;Exportoptionen&quot;wird angezeigt.

   ![](assets/rp-export-options-box-350x421.png)

1. Geben Sie die folgenden Informationen an:\
   **Startdatum**: Das Startdatum Ihres Exports. Die exportierte Datei enthält Zuordnungs- und Verfügbarkeitsinformationen, die mit dem ersten Wochentag beginnen, der den hier angegebenen Tag enthält.\
   **Anzahl der Zeiträume**: Die Anzahl der Zeiträume, die Sie in Ihre Datei aufnehmen möchten. Der Standardwert ist 4 Punkte.\
   **Typ**: Der Typ der Zeiträume, in denen die Informationen in der exportierten Datei angezeigt werden sollen (Wochen, Monate oder Quartale).\
   Im Folgenden finden Sie die maximalen Zeiträume, die Sie exportieren können:

   * 52 Wochen
   * 36 Monaten
   * 12 Quartale

   **Zu exportieren auswählen**: Je nach ausgewählter Ansicht können Sie Verfügbarkeits- und Budgetierungsinformationen für alle auf dem Bildschirm aufgelisteten Objekte oder für bestimmte Objekte exportieren.
Sie können die folgenden Informationen exportieren:

   * Wählen Sie in der Projektansicht den Export aus:

      * Projekte
      * Projekte und Aufgabengebiete
      * Alles (dies ist die Standardoption)
   * Wählen Sie in der Benutzeransicht den Export aus:

      * Benutzer
      * Benutzer und Projekte
      * Alles (dies ist die Standardoption)
   * Wählen Sie in der Rollenansicht den Export aus:

      * Funktionen
      * Aufgabengebiete und Projekte
      * Alles (dies ist die Standardoption)

   **Datenformatierung**: Je nachdem, wie Ihre Excel-Datei angezeigt werden soll, wählen Sie die folgenden Optionen aus:

   * **Roh**: Wählen Sie diese Option, um die Verfügbarkeit und Zuordnungsinformationen anzuzeigen, die von den Objekten, zu denen sie gehört, in der Excel-Datei nicht gruppiert wurden. (Dies ist die Standardoption)
   * **gruppiert**: Wählen Sie diese Option aus, um die Verfügbarkeits- und Zuordnungsinformationen anzuzeigen, die nach den Objekten gruppiert sind, zu denen sie gehört. Dadurch werden die exportierten Informationen so angezeigt, wie sie auf dem Bildschirm angezeigt werden.

   Ein Beispiel dafür, wie die Informationen in der exportierten Datei aussehen, finden Sie im Dialogfeld &quot;Exportoptionen&quot;.

1. Klicken **Export** um die Informationen aus dem Ressourcenplaner zu exportieren.\
   Nur die von Ihnen gespeicherten Informationen werden exportiert.

1. (Bedingt) Wenn Sie nicht gespeicherte budgetierte Stunden in der Rolle- oder Projektansicht haben, klicken Sie auf **Speichern und fortfahren.**
Eine Excel-Datei (.xlsx) wird auf Ihren Computer heruntergeladen.
\
   Der Export aus dem Ressourcen-Planer ist nicht verfügbar, während die Datei zum Herunterladen vorbereitet ist.\
   (Bedingt) Wenn Sie eine große Datenmenge exportieren, erhalten Sie eine E-Mail mit einem Link, über den Sie die Datei herunterladen können.\
   ![RP_eamil_with_exporting_planner_attach.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Bedingt) Wenn Sie die E-Mail mit der exportierten Datei erhalten, klicken Sie auf **Download** , um die Datei herunterzuladen.\
   Dadurch gelangen Sie zurück zu Workfront, wo Sie die Datei herunterladen können.\
   Sie müssen bei Workfront angemeldet sein, damit der Download abgeschlossen ist.\
   Wenn Sie die Datei nicht herunterladen, wenn sie bereitgestellt wird, bleibt der Download-Link 7 Tage lang aktiv, nachdem Sie den Export initiiert haben.
