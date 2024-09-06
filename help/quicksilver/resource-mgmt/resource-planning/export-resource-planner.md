---
product-area: resource-management
navigation-topic: resource-planning
title: Exportieren von Informationen aus dem Ressourcenplaner
description: Sie können Informationen aus einer beliebigen Ansicht des Resource Planers in eine Excel-Datei (.xlsx) exportieren, die auf Ihrem Computer gespeichert ist.
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 4%

---

# Exportieren von Informationen aus dem Ressourcenplaner

Sie können Informationen aus einer beliebigen Ansicht des Resource Planers in eine Excel-Datei (.xlsx) exportieren, die auf Ihrem Computer gespeichert ist.

>[!IMPORTANT]
>
>Es gibt Einschränkungen hinsichtlich der angezeigten Informationen und der Informationen, die Sie aus dem Ressourcen-Planer exportieren können. Weitere Informationen zu diesen Einschränkungen finden Sie unter [Anzeigebeschränkungen für Ressourcenplaner](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Licht oder höher</p>
       <p>oder</p>
       <p>Aktuell: Überprüfen oder höher</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Anzeigen des Zugriffs oder höher auf Projekte, Benutzer und Ressourcenverwaltung</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Projekte anzeigen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportieren von Informationen aus dem Ressourcenplaner

{{step1-to-resourcing}}

Der **Planer** wird standardmäßig angezeigt.

1. Wählen Sie die Ansicht für den Planer aus. Sie können eine der folgenden Optionen auswählen:

   * Nach Benutzer/Benutzerin anzeigen
   * Nach Projekt anzeigen
   * Nach Funktion anzeigen

1. Klicken Sie auf **Exportieren**.

   Das Dialogfeld &quot;Exportoptionen&quot;wird angezeigt.

   ![](assets/rp-export-options-box-350x421.png)

1. Geben Sie die folgenden Informationen an:\
   **Startdatum**: Das Startdatum Ihres Exports. Die exportierte Datei enthält Zuordnungs- und Verfügbarkeitsinformationen, die mit dem ersten Wochentag beginnen, der den hier angegebenen Tag enthält.\
   **Anzahl der Punkte**: Die Anzahl der Zeiträume, die Sie in Ihre Datei aufnehmen möchten. Der Standardwert ist 4 Punkte.\
   **Typ**: Der Typ der Zeiträume, in denen die Informationen in der exportierten Datei angezeigt werden sollen (Wochen, Monate oder Quartale).\
   Im Folgenden finden Sie die maximalen Zeiträume, die Sie exportieren können:

   * 52 Wochen
   * 36 Monaten
   * 12 Quartale

   **Zu exportieren auswählen**: Je nachdem, welche Ansicht Sie ausgewählt haben, können Sie die Verfügbarkeits- und Budgetierungsinformationen für alle auf dem Bildschirm aufgelisteten Objekte oder für bestimmte Objekte exportieren.
Sie können die folgenden Informationen exportieren:

   * Wählen Sie in der Projektansicht den Export aus:

      * Projekte
      * Projekte und Aufgabengebiete
      * Alles (dies ist die Standardoption)

   * Wählen Sie in der Benutzeransicht den Export aus:

      * Benutzende
      * Benutzende und Projekte
      * Alles (dies ist die Standardoption)

   * Wählen Sie in der Rollenansicht den Export aus:

      * Funktionen
      * Aufgabengebiete und Projekte
      * Alles (dies ist die Standardoption)

   **Datenformatierung**: Wählen Sie je nach der gewünschten Anzeige Ihrer Excel-Datei die folgenden Optionen aus:

   * **Raw**: Wählen Sie diese Option aus, um die Verfügbarkeit und Zuordnungsinformationen anzuzeigen, deren Gruppierung von den Objekten aufgehoben wird, zu denen sie gehört, in der Excel-Datei. (Dies ist die Standardoption)
   * **Gruppiert**: Wählen Sie diese Option aus, um die Verfügbarkeits- und Zuordnungsinformationen anzuzeigen, die nach den Objekten gruppiert sind, zu denen sie gehört. Dadurch werden die exportierten Informationen so angezeigt, wie sie auf dem Bildschirm angezeigt werden.

   Ein Beispiel dafür, wie die Informationen in der exportierten Datei aussehen, finden Sie im Dialogfeld &quot;Exportoptionen&quot;.

1. Klicken Sie auf **Exportieren** , um die Informationen aus dem Ressourcenplaner zu exportieren.\
   Es werden nur die Informationen exportiert, die Sie gespeichert haben.

1. (Bedingt) Wenn Sie nicht gespeicherte Budgetstunden in der Rolle oder Projektansicht haben, klicken Sie auf **Speichern und fortfahren.**
Eine Excel-Datei (.xlsx) wird auf Ihren Computer heruntergeladen.\
   Der Export aus dem Ressourcen-Planer ist nicht verfügbar, während die Datei zum Herunterladen vorbereitet ist.\
   (Bedingt) Wenn Sie eine große Datenmenge exportieren, erhalten Sie eine E-Mail mit einem Link, über den Sie die Datei herunterladen können.\
   ![RP_eamil_with_exporting_planner_attach.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Bedingt) Wenn Sie die E-Mail mit der exportierten Datei erhalten, klicken Sie auf **Download** , um die Datei herunterzuladen.\
   Dadurch gelangen Sie zurück zu Workfront, wo Sie die Datei herunterladen können.\
   Sie müssen bei Workfront angemeldet sein, damit der Download abgeschlossen ist.\
   Wenn Sie die Datei nicht herunterladen, wenn sie bereitgestellt wird, bleibt der Download-Link 7 Tage lang aktiv, nachdem Sie den Export initiiert haben.
