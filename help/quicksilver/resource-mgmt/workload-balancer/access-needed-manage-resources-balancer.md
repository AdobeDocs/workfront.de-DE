---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zugriff erforderlich, um Ressourcen im Workload Balancer zu verwalten
description: Ohne entsprechende Zugriffsrechte können Sie Ihre Arbeitszuweisungen im Workload-Balancer möglicherweise nicht anzeigen oder verwalten.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 78d73d0d7bd0ffc00ae1afed0adb324501e0c310
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Zugriff zum Verwalten von Ressourcen im Workload Balancer erforderlich

{{preview-fast-release-general}}

Ohne entsprechende Zugriffsrechte können Sie Ihre Arbeitszuweisungen im Workload-Balancer möglicherweise nicht anzeigen oder verwalten.

Sie müssen Zugriff haben, um die Benutzer anzuzeigen, deren Arbeitslast Sie im Workload-Balancer anzeigen oder verwalten möchten. Darüber hinaus müssen Sie über die richtige Zugriffsebene und die richtigen Berechtigungen für die Projekte verfügen, mit denen die Arbeit verknüpft ist.

## Adobe Workfront-Plan musste den Workload Balancer für verschiedene Bereiche verwenden

Die folgende Tabelle zeigt die Verbindung zwischen dem Workfront-Plan Ihres Unternehmens und dem Verwendungsbereich des Workload-Balancer im System:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-Plan (aktuell)</b></p></td> 
   <td> <p><b>Bereiche, in denen Sie auf den Workload Balancer zugreifen können</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team oder höher </td> 
   <td>Workload Balancer für ein Team oder Projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro oder höher</td> 
   <td>Workload Balancer für mehrere Projekte auf Systemebene</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-Plan (neu)</b></p></td> 
   <td> <p><b>Bereiche, in denen Sie auf den Workload Balancer zugreifen können</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Beliebig </td> 
   <td>Zugriff auf den Workload Balancer an einer beliebigen Stelle in Workfront</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Workfront-Plänen finden Sie unter [Unsere Pläne](https://business.adobe.com/products/workfront/pricing.html).

Informationen dazu, wo Sie den Workload-Balancer in Workfront finden können, finden Sie unter [Suchen des Workload-Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Zum Anzeigen des Workload Balancer benötigter Zugriff

Sie müssen über die folgenden Zugriffsrechte verfügen, um den Workload-Balancer anzuzeigen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan, um den Workload Balancer im Bereich Ressourcen anzuzeigen</br>
       Arbeit, um den Workload Balancer eines Teams oder Projekts anzuzeigen</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcen-Management anzeigen oder erhöhen</p> <p>Informationen zur Zugriffsebene für das Ressourcen-Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf das Ressourcen-Management gewähren</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie müssen für das Projekt, dessen Zuweisungen Sie anzeigen möchten, über Anzeigeberechtigungen verfügen. </p> <p>Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<span class="preview">Alle Benutzer haben Zugriff darauf, den Workload-Balancer in ihren eigenen Profilen anzuzeigen. Dies ist weder durch die Lizenz noch durch die Zugriffsebene eingeschränkt. Beachten Sie, dass der Workload Balancer für ein Benutzerprofil schreibgeschützt ist und Zuweisungen und Zuweisungen nicht geändert werden können.</span>

## Zugriff erforderlich, um Zuweisungen im Workload Balancer zu verwalten

Sie müssen über die folgenden Zugriffsrechte verfügen, um den Workload-Balancer zu verwalten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Plan, um Zuweisungen im Workload Balancer im Bereich Ressourcen zu verwalten;</br>
       Arbeit, um Zuweisungen im Workload Balancer eines Teams oder Projekts zu verwalten</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcen-Management bearbeiten</p> 
     <p>Informationen zur Zugriffsebene für das Ressourcen-Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf das Ressourcen-Management gewähren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Tragen Sie Berechtigungen oder höhere Berechtigungen für das Projekt bei, dessen Zuweisungen Sie verwalten möchten, einschließlich Berechtigungen zum Ausführen von Zuweisungen. </p> <p>Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
