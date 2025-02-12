---
product-area: resource-management
navigation-topic: resource-planning
title: Freigeben der Ressourcenplaner-Benutzeransicht für einen Link
description: Adobe Workfront kann eine eindeutige URL für die Benutzeransicht des Ressourcenplaners generieren, die Sie als externe Seite in ein Dashboard einbetten oder separat in einer neuen Browser-Registerkarte öffnen können. Dies ist hilfreich, wenn Sie Informationen zum Ressourcenplaner für Benutzende freigeben, die möglicherweise nicht direkten Zugriff auf den Bereich Ressourcen haben.
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Freigeben der Ressourcenplaner-Benutzeransicht mit einem Link

Adobe Workfront kann eine eindeutige URL für die Benutzeransicht des Ressourcenplaners generieren, die Sie als externe Seite in ein Dashboard einbetten oder separat in einer neuen Browser-Registerkarte öffnen können. Dies ist hilfreich, wenn Sie Informationen zum Ressourcenplaner für Benutzende freigeben, die möglicherweise nicht direkten Zugriff auf den Bereich Ressourcen haben.

![Benutzeransicht mit Link](assets/rp-user-view-with-link-highlight-350x49.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
    <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Ressourcenmanagement, Projekte und Benutzer</p> <p>Anzeigen des Zugriffs auf Finanzdaten zum Anzeigen von Kosteninformationen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zeigen Sie Berechtigungen oder höhere Berechtigungen für die Projekte an, die Sie im Ressourcenplaner anzeigen möchten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Beachten Sie beim Generieren der eindeutigen URL für die Benutzeransicht des Ressourcenplaners Folgendes:

* Sie können eine eindeutige URL nur für die Benutzeransicht erhalten. Die Option zum Generieren der URL ist in den Projekt- oder Rollenansichten nicht vorhanden.
* Sie können die URL für andere Benutzer freigeben, einschließlich „Arbeiten“ und „Lizenzierte Benutzer überprüfen“.\
  Sie müssen Zugriff haben, um andere Benutzer anzeigen zu können, damit sie die Informationen im Ressourcenplaner über die URL anzeigen können, die Sie für sie freigegeben haben.
* Die folgenden Informationen werden gespeichert, wenn Sie die URL für andere Benutzer freigeben:

   * Der Typ der Zeiträume (Woche, Monat, Quartal).
   * Die Filter, die Sie anwenden.
   * Der Anzeigetyp (Stunden oder FTE).

So rufen Sie eine eindeutige URL in der Benutzeransicht des Ressourcenplaners ab und geben sie für andere Benutzer frei:

{{step1-to-resourcing}}

1. Wählen Sie **Nach Benutzer anzeigen** aus.
1. (Optional) Wählen Sie den Zeitrahmen aus, nach dem Sie die Informationen im Ressourcenplaner anzeigen möchten. Wählen Sie aus den folgenden Optionen aus:

   * Woche
   * Monat
   * Quartal

1. (Optional) Wählen Sie aus, ob die Informationen nach **(FTE** oder **Stunden** angezeigt werden sollen.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (Optional) Wenden Sie Filter auf den Ressourcenplaner an.\
   Informationen zum Anwenden von Filtern finden Sie [Filterinformationen im Ressourcenplaner](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Klicken Sie auf das **Hyperlink**-Symbol.\
   ![RP_Storm_generate_URL_with_copy_URL_link.pn](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Klicken Sie auf **URL kopieren**.\
   Damit wird die eindeutige URL des Ressourcenplaners in der Benutzeransicht in die Zwischenablage kopiert.

1. (Optional) Führen Sie einen der folgenden Schritte aus:  

   * Fügen Sie die URL in eine andere Anwendung ein, um sie an einen anderen Benutzer zu senden.\
     Der Benutzer muss bei Workfront angemeldet sein, damit der Ressourcenplaner in der Benutzeransicht angezeigt werden kann.
   * Öffnen Sie eine neue Browser-Registerkarte oder ein neues Fenster und fügen Sie den kopierten Link ein. Klicken Sie dann auf der Tastatur auf die Eingabetaste , um den Ressourcenplaner in einer neuen Registerkarte oder einem neuen Fenster zu öffnen.
   * Gehen Sie folgendermaßen vor:

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Navigieren Sie **Reporting**>**Dashboards**>**Neues Dashboard**>**Externe Seite hinzufügen.**

      1. Fügen Sie den kopierten Link in die Zwischenablage in das Feld **URL** ein.
      1. Klicken Sie **Speichern** und dann **Speichern + Schließen**.\
         Dadurch wird die URL in das Dashboard eingebettet und die Benutzeransicht des Ressourcenplaners wird in einem separaten Dashboard angezeigt.

1. (Optional) Wenn Sie die URL in ein Dashboard eingebettet haben, sollten Sie sie zu einer Layout-Vorlage hinzufügen oder für andere Benutzer freigeben, die möglicherweise keinen Zugriff auf den Bereich „Ressourcenverwaltung“ haben.\
   Informationen zum Hinzufügen von Dashboards zu einer Layout-Vorlage finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   Weitere Informationen zum Freigeben von Dashboards finden Sie unter [Freigeben eines Dashboards](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   Beim Anzeigen der freigegebenen URL können Benutzerinnen und Benutzer die Informationen mit den Einstellungen sehen, die Sie ursprünglich auf den Ressourcenplaner angewendet haben. Sie müssen bei Workfront angemeldet sein, um die freigegebene URL sehen zu können.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
