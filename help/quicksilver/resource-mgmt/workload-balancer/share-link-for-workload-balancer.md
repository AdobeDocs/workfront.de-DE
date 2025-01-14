---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Freigeben des Workload Balancer für einen Link
description: Sie können den Workload-Balancer für andere Benutzende freigeben, denen der Bereich „Ressourcen“ möglicherweise nicht zur Verfügung steht. Weitere Informationen zur Verwendung des Workload-Balancer finden Sie unter Navigieren im Workload-Balancer .
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 233e61c011cc87f49d0d4082a20b7790104c96c8
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 1%

---

# Freigeben des Workload Balancer für einen Link

Sie können den Workload-Balancer für andere Benutzer freigeben, für die der Bereich Ressourcen möglicherweise nicht im Hauptmenü verfügbar ist. Weitere Informationen zur Verwendung des Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan, wenn der Workload Balancer im Bereich „Ressourcen“ verwendet wird</br>
       Arbeit bei Verwendung des Workload Balancer eines Teams oder Projekts</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Folgendes anzeigen oder höher:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen oder Erweitern von Berechtigungen für die Projekte, Aufgaben und Probleme</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Im Workload Balancer enthaltene Informationen, wenn er über einen freigegebenen Link angezeigt wird

Wenn Sie einen Link zum Workload Balancer für andere Benutzer freigeben, enthält der freigegebene Link die folgenden Informationen:

* Der Bereich Zugewiesene Arbeit im Workload Balancer.
* Projekt, Aufgabe, Benutzerinformationen. Dazu gehören die Informationen zur Benutzerzuordnung.
* Die Informationen werden entsprechend dem ausgewählten Filter angezeigt.

  >[!IMPORTANT]
  >
  >Wenn Sie die Filter löschen, nachdem Sie den Link freigegeben haben, erhalten die Benutzenden, die den Workload-Balancer über den Link anzeigen, eine Warnung, dass die Filter gelöscht wurden. Sie zeigen alle Benutzer im Bereich Zugewiesene Arbeit an. Dies ist die Standardansicht für den Workload-Balancer.

* Die Anzahl der zuvor ausgewählten Wochen.

Die folgenden Optionen stehen Benutzenden zur Verfügung, die den Workload-Balancer über einen freigegebenen Link aufrufen, um sich selbst zu aktualisieren:

* Die folgenden Zeitleisten-Auswahlen:

   * Heute
   * Symbole für Vor- und Rückwärts
   * Kalenderauswahl

* Die Symbole Tag, Woche und Monat
* Das Symbol Einstellungen .
* Das Symbol Zuteilungen anzeigen

  Weitere Informationen zur Verwendung dieser Optionen finden Sie unter [Navigieren im Workload-Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Das Symbol „Rollenzuweisungen anzeigen“

  Dies ist nur für den Workload-Balancer eines Projekts verfügbar.

Der Benutzer, der den freigegebenen Link erhält, kann über diesen Link nicht Folgendes im Workload Balancer tun:

* Zuweisen von Arbeitselementen zu Benutzern
* Benutzerzuweisungen verwalten
* Erstellen neuer oder Aktualisieren ursprünglich angewendeter Filter

## Zugriff erforderlich, um Informationen im Workload Balancer über einen freigegebenen Link anzuzeigen

Sie benötigen den folgenden Zugriff, um Informationen im Workload Balancer über einen freigegebenen Link anzuzeigen:

* Eine gültige Adobe Workfront-Lizenz und Sie müssen bei Workfront angemeldet sein.
* Zeigen Sie zumindest den Zugriff auf die Ressourcenverwaltung in Ihrer Zugriffsebene an. Informationen zum Gewähren des Zugriffs auf die Ressourcenverwaltung finden Sie [Gewähren des Zugriffs auf die Ressourcenverwaltung](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Anzeigen von Berechtigungen für die im Workload-Balancer angezeigten Projekte, Aufgaben, Probleme und Benutzenden.

## Workload Balancer über einen Link für andere Benutzer freigeben

1. Zum Workload Balancer wechseln

   Weitere Informationen zum Zugriff auf den Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Optional) Führen Sie einen oder mehrere der folgenden Schritte aus:

   * Aktualisieren Sie die Auswahl des Zeitraums .
   * Klicken Sie auf **Tag,** oder **Monat**, um tägliche, wöchentliche oder monatliche Informationen anzuzeigen.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Wenden Sie Filter auf die Bereiche Nicht zugewiesene und Zugewiesene Arbeit an.

     Informationen zum Filtern von Informationen im Workload Balancer finden Sie unter [Filtern von Informationen im Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Klicken Sie auf **Link-Symbol** ![](assets/wb-shearable-link-icon-small.png).

   Dadurch wird der Link zur Zwischenablage hinzugefügt.

1. Führen Sie einen der folgenden Schritte aus, um den Link für andere freizugeben:

   * Fügen Sie sie in eine E-Mail, Chat-Nachricht oder eine andere Anwendung ein und teilen Sie diese mit anderen Benutzern.
   * Fügen Sie ihn einem benutzerdefinierten Abschnitt als externe Seite hinzu, fügen Sie den benutzerdefinierten Abschnitt dem Profil eines Benutzers oder einer Layout-Vorlage hinzu und geben Sie die Layout-Vorlage dann für Benutzer, Teams, Aufgabengebiete oder Gruppen frei.

     Informationen zum Erstellen einer externen Seite finden Sie unter [Externe Web-Seite in ein Dashboard einbetten](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Informationen zum Hinzufügen benutzerdefinierter Abschnitte zu einer Layout-Vorlage finden Sie unter [Anpassen des linken Bedienfelds mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Wenn Sie den Workload-Balancer zum benutzerdefinierten Abschnitt eines -Objekts hinzufügen, werden die Informationen im Workload-Balancer nicht nach dem -Objekt gefiltert. Der Workload Balancer zeigt die Informationen an, die von den ursprünglich angewendeten Filtern gefiltert wurden.
