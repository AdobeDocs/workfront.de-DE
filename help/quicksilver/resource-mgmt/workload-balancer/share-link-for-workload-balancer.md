---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Den Lastenausgleich mit einem Link freigeben
description: Sie können den Lastenausgleich für andere Benutzer freigeben, für die möglicherweise nicht der Bereich "Ressourcen"verfügbar ist. Weitere Informationen zur Verwendung des Workload-Balancers finden Sie unter Navigieren im Arbeitslastausgleich .
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 1%

---

# Den Lastenausgleich über einen Link freigeben

Sie können den Lastenausgleich für andere Benutzer freigeben, für die möglicherweise nicht der Bereich &quot;Ressourcen&quot;verfügbar ist. Informationen zur Verwendung des Lastenausgleichs finden Sie unter [Navigieren im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie bei Verwendung des Workload-Balancers im Ressourcenbereich;</br>
       Arbeiten bei Verwendung des Workload Balancers für ein Team oder Projekt</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zeigen Sie den Zugriff auf Folgendes an oder höher:</p> 
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
   <td>Anzeigen von oder höheren Berechtigungen für die Projekte, Aufgaben und Probleme</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informationen, die im Lastenausgleich enthalten sind, wenn er von einem freigegebenen Link angezeigt wird

Wenn Sie einen Link zum Lastenausgleich für andere Benutzer freigeben, sind die folgenden Informationen im freigegebenen Link enthalten:

* Der zugewiesene Arbeitsbereich des Arbeitslastausgleichs.
* Projekt, Aufgabe, Benutzerinformationen. Dazu gehören die Informationen zur Benutzerzuordnung.
* Die Informationen werden entsprechend dem ausgewählten Filter angezeigt.

  >[!IMPORTANT]
  >
  >Wenn Sie die Filter löschen, nachdem Sie den Link freigegeben haben, erhalten die Benutzer, die den Lastenausgleich aus dem Link anzeigen, eine Warnung, dass die Filter gelöscht wurden. Sie zeigen alle Benutzer im Bereich Zugewiesene Arbeit an. Dies ist die Standardansicht für den Lastenausgleich.

* Die Anzahl der zuvor ausgewählten Wochen.

Die folgenden Optionen stehen Benutzern zur Verfügung, die den Lastenausgleich über einen freigegebenen Link anzeigen, um sich selbst zu aktualisieren:

* Die folgenden Timeline-Auswahlen:

   * Heute
   * Symbole für Zurück und Vorwärts
   * Kalenderauswahl

* Symbole Tag, Woche und Monat
* Das Symbol Einstellungen
* Symbol Zuordnungen anzeigen

  Weitere Informationen zur Verwendung dieser Optionen finden Sie unter [Navigieren im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Symbol &quot;Rollenzuweisungen anzeigen&quot;

  Dies ist nur für den Lastenausgleich eines Projekts verfügbar.

Der Benutzer, der den freigegebenen Link erhält, kann im Lastenausgleich von diesem Link aus Folgendes nicht tun:

* Zuweisen von Arbeitselementen zu Benutzern
* Verwalten von Benutzerzuordnungen
* Erstellen neuer oder aktualisierter ursprünglich angewendeter Filter

## Zugriff erforderlich, um Informationen in Workload Balancer über einen freigegebenen Link anzuzeigen

Sie benötigen den folgenden Zugriff, um Informationen über einen freigegebenen Link im Arbeitslastausgleich anzuzeigen:

* Eine gültige Adobe Workfront-Lizenz und Sie müssen bei Workfront angemeldet sein.
* Zeigen Sie mindestens den Zugriff auf die Ressourcenverwaltung auf Ihrer Zugriffsebene an. Informationen zur Gewährung des Ressourcenverwaltungszugriffs finden Sie unter [Gewähren des Zugriffs auf die Ressourcenverwaltung](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Zeigen Sie Berechtigungen für die Projekte, Aufgaben, Probleme und Benutzer an, die im Arbeitslastausgleich angezeigt werden.

## Freigeben des Workload Balancers für andere Benutzer über einen Link

1. Wechseln Sie zum Lastenausgleich .

   Informationen zum Zugriff auf den Lastenausgleich finden Sie unter [Navigieren im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Optional) Führen Sie einen oder mehrere der folgenden Schritte aus:

   * Aktualisieren Sie die Zeitraumauswahl.
   * Klicken Sie auf **Tag, Woche** oder **Monat** , um tägliche, wöchentliche oder monatliche Informationen anzuzeigen.

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Wenden Sie Filter auf die Bereiche Nicht zugewiesene und Zugewiesene Arbeit an.

     Informationen zum Filtern von Informationen im Arbeitslastausgleich finden Sie unter [Informationen im Arbeitslastausgleich filtern](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Klicken Sie auf das Symbol **Link** ![](assets/wb-shearable-link-icon-small.png).

   Dadurch wird der Link zur Zwischenablage hinzugefügt.

1. Führen Sie einen der folgenden Schritte aus, um den Link für andere freizugeben:

   * Fügen Sie ihn in eine E-Mail, eine Chat-Nachricht oder eine andere Anwendung ein und geben Sie ihn für andere Benutzer frei.
   * Fügen Sie ihn zu einem benutzerdefinierten Abschnitt als externe Seite hinzu, fügen Sie den benutzerdefinierten Abschnitt zum Profil eines Benutzers oder zu einer Layout-Vorlage hinzu und geben Sie die Layout-Vorlage für Benutzer, Teams, Vorgangsrollen oder Gruppen frei.

     Informationen zum Erstellen einer externen Seite finden Sie unter [Einbetten einer externen Webseite in ein Dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Weitere Informationen zum Hinzufügen benutzerdefinierter Abschnitte zu einer Layout-Vorlage finden Sie unter [Anpassen des linken Bereichs mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

     >[!IMPORTANT]
     >
     >Wenn Sie den Lastenausgleich zum benutzerdefinierten Abschnitt eines Objekts hinzufügen, werden die Informationen im Arbeitslastausgleich nicht durch das -Objekt gefiltert. Der Lastenausgleich zeigt die Informationen an, die nach den ursprünglich angewendeten Filtern gefiltert wurden.
