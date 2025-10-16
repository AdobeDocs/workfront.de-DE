---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zugriff erforderlich, um Ressourcen im Workload Balancer zu verwalten
description: Ohne entsprechende Zugriffsrechte können Sie Ihre Arbeitszuweisungen im Workload-Balancer möglicherweise nicht anzeigen oder verwalten.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Zugriff zum Verwalten von Ressourcen im Workload Balancer erforderlich

{{preview-fast-release-general}}

Ohne entsprechende Zugriffsrechte können Sie Ihre Arbeitszuweisungen im Workload-Balancer möglicherweise nicht anzeigen oder verwalten.

Sie müssen Zugriff haben, um die Benutzer anzuzeigen, deren Arbeitslast Sie im Workload-Balancer anzeigen oder verwalten möchten. Darüber hinaus müssen Sie über die richtige Zugriffsebene und die richtigen Berechtigungen für die Projekte verfügen, mit denen die Arbeit verknüpft ist.

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## Zum Anzeigen des Workload Balancer benötigter Zugriff

Sie müssen über die folgenden Zugriffsrechte verfügen, um den Workload-Balancer anzuzeigen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr>
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan, um den Workload-Balancer im Bereich Ressourcen; Arbeit anzuzeigen, um den Workload-Balancer eines Teams oder Projekts anzuzeigen</p></td>
  </tr>  
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcen-Management anzeigen oder erhöhen</p> <p>Informationen zur Zugriffsebene für das Ressourcen-Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">Zugriff auf das Ressourcen-Management gewähren</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Sie müssen für das Projekt, dessen Zuweisungen Sie anzeigen möchten, über Anzeigeberechtigungen verfügen. </p> <p>Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Freigeben eines Projekts in Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Alle Benutzer haben Zugriff darauf, den Workload-Balancer in ihren eigenen Profilen anzuzeigen. Dies ist weder durch die Lizenz noch durch die Zugriffsebene eingeschränkt. Beachten Sie, dass der Workload Balancer für ein Benutzerprofil schreibgeschützt ist und Zuweisungen und Zuweisungen nicht geändert werden können.</span>

## Zugriff erforderlich, um Zuweisungen im Workload Balancer zu verwalten

Sie müssen über die folgenden Zugriffsrechte verfügen, um den Workload-Balancer zu verwalten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Planen Sie, um Zuweisungen im Workload Balancer im Bereich Ressourcen zu verwalten. Arbeiten, um Zuweisungen im Workload Balancer eines Teams oder Projekts zu verwalten.</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td>
   <td> <p>Zugriff auf das Ressourcen-Management bearbeiten</p>
     <p>Informationen zur Zugriffsebene für das Ressourcen-Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >Zugriff auf das Ressourcen-Management gewähren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p> Tragen Sie Berechtigungen oder höhere Berechtigungen für das Projekt bei, dessen Zuweisungen Sie verwalten möchten, einschließlich Berechtigungen zum Ausführen von Zuweisungen. </p> <p>Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Freigeben eines Projekts in Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
