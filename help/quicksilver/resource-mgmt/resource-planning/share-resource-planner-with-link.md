---
product-area: resource-management
navigation-topic: resource-planning
title: Freigeben der User-Ansicht "Resource Planer"über einen Link
description: Adobe Workfront kann eine eindeutige URL für die Benutzeransicht des Ressourcen-Planers generieren, die Sie als externe Seite in ein Dashboard einbetten oder separat in einer neuen Browser-Registerkarte öffnen können. Dies ist hilfreich, wenn Sie die Ressourcen-Planer-Informationen für Benutzer freigeben, die möglicherweise keinen direkten Zugriff auf den Ressourcen-Bereich haben.
author: Alina
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Freigeben der User-Ansicht &quot;Resource Planer&quot;über einen Link

Adobe Workfront kann eine eindeutige URL für die Benutzeransicht des Ressourcen-Planers generieren, die Sie als externe Seite in ein Dashboard einbetten oder separat in einer neuen Browser-Registerkarte öffnen können. Dies ist hilfreich, wenn Sie die Ressourcen-Planer-Informationen für Benutzer freigeben, die möglicherweise keinen direkten Zugriff auf den Ressourcen-Bereich haben.

![](assets/rp-user-view-with-link-highlight-350x49.png)

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Ressourcenverwaltung, Projekte und Benutzer</p> <p>Zugriff auf Finanzdaten anzeigen, um Kosteninformationen anzuzeigen </p> <p><b>NOTE</b> Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für die Projekte, die Sie im Ressourcenplaner anzeigen möchten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.


Beachten Sie Folgendes beim Generieren der eindeutigen URL für die Benutzeransicht des Ressourcen-Planers:

* Sie können eine eindeutige URL nur für die Benutzeransicht abrufen. Die Option zum Generieren der URL existiert nicht in den Projekt- oder Rollenansichten.
* Sie können die URL für andere Benutzer freigeben, darunter für Benutzer, die eine Lizenz besitzen, einschließlich &quot;Arbeiten&quot;und &quot;Überprüfen&quot;.\
   Sie müssen Zugriff haben, um andere Benutzer anzuzeigen, damit sie die Informationen im Ressourcenplaner aus der URL anzeigen können, die Sie für sie freigeben.
* Die folgenden Informationen werden gespeichert, wenn Sie die URL für andere Benutzer freigeben:

   * Die Art der Zeiträume (Woche, Monat, Quartal).
   * Die angewendeten Filter.
   * Die Art der Anzeige (Stunden oder FTE).

So rufen Sie eine eindeutige URL in der Benutzeransicht des Ressourcen-Planers ab und geben sie für andere Benutzer frei:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Ressourcen**.
1. Wählen Sie in der **Ansicht nach Benutzer**.
1. (Optional) Wählen Sie den Zeitraum aus, nach dem die Informationen im Ressourcenplaner angezeigt werden sollen. Wählen Sie aus den folgenden Optionen aus:

   * Woche
   * Monat
   * Quartal

1. (Optional) Wählen Sie aus, ob Sie die Informationen anzeigen möchten, indem Sie **FTE** oder **Stunden**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (Optional) Wenden Sie Filter auf den Ressourcenplaner an.\
   Informationen zum Anwenden von Filtern finden Sie unter [Filtern von Informationen im Ressourcenplaner](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Klicken Sie auf **Hyperlink** Symbol.\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Klicken **URL kopieren**.\
   Dadurch wird die eindeutige URL des Ressourcenplaners in der Benutzeransicht in die Zwischenablage kopiert.

1. (Optional) Führen Sie einen der folgenden Schritte aus:  

   * Fügen Sie die URL in eine andere Anwendung ein, um sie an einen anderen Benutzer zu senden.\
      Der Benutzer muss bei Workfront angemeldet sein, um den Ressourcenplaner in der Ansicht &quot;User&quot;anzuzeigen.
   * Öffnen Sie eine neue Browser-Registerkarte oder ein neues Fenster und fügen Sie den kopierten Link ein. Klicken Sie dann auf die Eingabetaste auf der Tastatur, um den Ressourcen-Planer in einer neuen Registerkarte oder in einem neuen Fenster zu öffnen.
   * Gehen Sie wie folgt vor:

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Navigieren Sie zu **Berichterstellung**>**Dashboards**>**Neues Dashboard**>**Externe Seite hinzufügen.**

      1. Fügen Sie den Link, den Sie in die Zwischenablage kopiert haben, im **URL** -Feld.
      1. Klicken **Speichern**, dann **Speichern und schließen**.\
         Dadurch wird die URL in das Dashboard eingebettet und die Benutzeransicht des Ressourcen-Planers wird in einem separaten Dashboard angezeigt.

1. (Optional) Wenn Sie die URL in ein Dashboard eingebettet haben, sollten Sie sie zu einer Layoutvorlage hinzufügen oder sie für andere Benutzer freigeben, die möglicherweise keinen Zugriff auf den Bereich &quot;Ressourcenverwaltung&quot;haben.\
   Informationen zum Hinzufügen von Dashboards zu einer Layoutvorlage finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   Informationen zum Freigeben von Dashboards finden Sie unter [Dashboard freigeben](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   Beim Anzeigen der freigegebenen URL können Benutzer die Informationen mit den Einstellungen sehen, die Sie ursprünglich auf den Ressourcenplaner angewendet haben. Sie müssen bei Workfront angemeldet sein, um die freigegebene URL anzuzeigen.\
   ![user_view_dashoard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
