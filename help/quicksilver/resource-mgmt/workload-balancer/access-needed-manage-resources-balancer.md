---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zugriff erforderlich für die Verwaltung von Ressourcen im Lastenausgleich
description: Ohne korrekten Zugriff oder ohne entsprechende Berechtigungen können Sie Ihre Arbeitsaufgaben möglicherweise nicht im Arbeitslastausgleich anzeigen oder verwalten.
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer

Ohne korrekten Zugriff oder ohne entsprechende Berechtigungen können Sie Ihre Arbeitsaufgaben möglicherweise nicht im Arbeitslastausgleich anzeigen oder verwalten.

Sie müssen Zugriff haben, um die Benutzer anzuzeigen, deren Arbeitslast Sie im Lastenausgleich anzeigen oder verwalten möchten. Darüber hinaus müssen Sie über die richtige Zugriffsstufe und die richtigen Berechtigungen für die Projekte verfügen, mit denen die Arbeit verknüpft ist.

## Adobe Workfront-Plan zur Verwendung des Lastenausgleichs für verschiedene Bereiche erforderlich

Die folgende Tabelle zeigt die Verbindung zwischen dem Workfront-Plan, den Ihr Unternehmen hat, und wo im System Sie den Lastenausgleich verwenden können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-Plan (aktuell)</b></p></td> 
   <td> <p><b>Bereiche, in denen Sie auf den Lastenausgleich zugreifen können</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team oder höher </td> 
   <td>Lastenausgleich für ein Team oder ein Projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro oder höher</td> 
   <td>Lastenausgleich für mehrere Projekte auf Systemebene</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p><b>Workfront-Plan (neu)</b></p></td> 
   <td> <p><b>Bereiche, in denen Sie auf den Lastenausgleich zugreifen können</b></p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Alle </td> 
   <td>Zugriff auf den Lastenausgleich überall in Workfront</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Workfront-Plänen finden Sie unter [Unsere Pläne](https://www.workfront.com/plans).

Informationen darüber, wo Sie den Lastenausgleich in Workfront finden können, finden Sie unter [Suchen des Lastenausgleichs](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Zugriff erforderlich, um den Lastenausgleich anzuzeigen

Sie müssen über folgenden Zugriff verfügen, um den Lastenausgleich anzuzeigen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie, den Arbeitslastausgleich im Ressourcenbereich anzuzeigen;</br>
       Arbeiten, um den Lastenausgleich eines Teams oder Projekts anzuzeigen</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung anzeigen oder höher</p> <p>Weitere Informationen zur Zugriffsebene für die Ressourcenverwaltung finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf die Ressourcenverwaltung gewähren</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie müssen über Anzeigeberechtigungen für das Projekt verfügen, dessen Zuweisungen Sie anzeigen möchten. </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Projekt in Adobe Workfront freigeben</a> .</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Zugriff erforderlich für die Verwaltung von Zuweisungen im Workload Balancer

Sie müssen über folgenden Zugriff verfügen, um den Lastenausgleich zu verwalten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie die Verwaltung von Zuweisungen im Arbeitslastausgleich im Ressourcenbereich;</br>
       Arbeiten, um Zuweisungen im Arbeitslastausgleich eines Teams oder Projekts zu verwalten</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten</p> 
     <p>Weitere Informationen zur Zugriffsebene für die Ressourcenverwaltung finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf die Ressourcenverwaltung gewähren</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Contribute oder höhere Berechtigungen für das Projekt, dessen Zuweisungen Sie verwalten möchten, einschließlich Berechtigungen zum Zuweisen. </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Projekt in Adobe Workfront freigeben</a> .</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->