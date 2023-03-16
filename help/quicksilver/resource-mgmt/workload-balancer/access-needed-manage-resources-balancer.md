---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer
description: Ohne korrekten Zugriff oder ohne entsprechende Berechtigungen können Sie Ihre Arbeitsaufgaben möglicherweise nicht im Arbeitslastausgleich anzeigen oder verwalten.
author: Alina
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '535'
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
   <td role="rowheader"><p>Workfront-Plan</p></td> 
   <td> <p>Bereiche, in denen Sie auf den Lastenausgleich zugreifen können</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Team oder höher </td> 
   <td>Lastenausgleich für ein Team oder ein Projekt</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro oder höher</td> 
   <td>Lastenausgleich für mehrere Projekte auf Systemebene</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Workfront-Plänen finden Sie unter [Unsere Pläne](https://www.workfront.com/plans).

Informationen darüber, wo Sie den Lastenausgleich in Workfront finden können, finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Zugriff erforderlich, um den Lastenausgleich anzuzeigen

Sie müssen über folgenden Zugriff verfügen, um den Lastenausgleich anzuzeigen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Planen Sie die Anzeige des Lastenausgleichs im Bereich Ressourcen .</p>
   <p>Arbeiten zum Anzeigen des Workload-Balancers eines Teams oder Projekts</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung anzeigen oder höher</p> <p>Weitere Informationen zur Zugriffsebene auf Resource Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf Resource Management gewähren</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie verfügen über Anzeigeberechtigungen für das Projekt, dessen Zuweisungen Sie anzeigen möchten. </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zugriff erforderlich für die Verwaltung von Zuweisungen im Workload Balancer

Sie müssen über folgenden Zugriff verfügen, um den Lastenausgleich zu verwalten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Planen Sie die Verwaltung von Zuweisungen im Arbeitslastausgleich im Bereich "Ressourcen".</p>
   <p>Arbeiten zum Verwalten von Zuweisungen im Arbeitslastausgleich eines Teams oder Projekts</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Ressourcenverwaltung bearbeiten</p> 
     <p>Weitere Informationen zur Zugriffsebene auf Resource Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf Resource Management gewähren</a>.</p>
     <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Fügen Sie Berechtigungen für das Projekt hinzu, dessen Zuweisungen Sie verwalten möchten. Dazu gehören Berechtigungen zum Zuweisen. </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->