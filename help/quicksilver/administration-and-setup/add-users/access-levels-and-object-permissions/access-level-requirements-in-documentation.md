---
title: Zugriffsanforderungen
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,planer,worker,reviewer,requestor,external,user
navigation-topic: access-levels
description: Die Anleitungsartikel zur Workfront-Dokumentation enthalten eine Tabelle, in der der Zugriff und die Berechtigungen erläutert werden, die für dieses Verfahren erforderlich sind. In diesem Artikel wird die Tabelle mit den Zugriffsanforderungen ausführlicher erläutert und es werden Links für weitere Informationen aufgeführt.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: d786a5bd86bcc1a4fbacf022cc9fbee9cb321da5
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Anforderungen an die Zugriffsstufen in der Dokumentation zu Workfront

Die Anleitungsartikel zur Workfront-Dokumentation enthalten eine Tabelle, in der die Zugriffs- und Berechtigungsanforderungen für dieses Verfahren erläutert werden. In dieser Tabelle mit den Zugriffsanforderungen erfahren Sie, ob Sie eine bestimmte Aktion in Workfront durchführen können oder warum Sie dies möglicherweise nicht tun können. In diesem Artikel werden die einzelnen Elemente der Tabelle mit den Zugriffsanforderungen erläutert und Tipps zur Fehlerbehebung sowie Links zu ausführlicheren Informationen bereitgestellt.

Wenn in der Tabelle mit den Zugriffsanforderungen in einem bestimmten Artikel keine Zeile vorhanden ist, sind für diese Aktion keine Anforderungen dieses Typs erforderlich.

>[!NOTE]
>
>Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Fragen dazu haben, wie sich die Felder in dieser Tabelle auf Sie beziehen.

## Die Tabelle Zugriffsanforderungen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> Adobe Workfront-Pläne beziehen sich auf die Funktionen, die Ihr Unternehmen erworben hat. Die meisten Workfront-Funktionen stehen in allen Plänen zur Verfügung, mit einigen wenigen Ausnahmen, die sich hauptsächlich auf die strategische Planung und Kontrolle von Unternehmen beziehen. 
   <ul><li>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, welchen Adobe Workfront-Plan Ihr Unternehmen verwendet, einschließlich der Frage, ob sich Ihr Unternehmen unter dem neuen oder aktuellen Verpackungsmodell befindet.</li>
   <li>Anweisungen dazu, wie ein Workfront-Administrator den Workfront-Plan Ihres Unternehmens finden kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Cluster- und Workfront-Plan Ihres Unternehmens anzeigen</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> Adobe Workfront-Lizenzen beziehen sich auf die Workfront-Funktionen, die in der Ihnen zugewiesenen Lizenz enthalten sind. Beispielsweise kann ein Benutzer über eine Lizenz verfügen, die das Markieren der abgeschlossenen Arbeitselemente und die Protokollierungszeit umfasst, während ein anderer Benutzer über eine Lizenz verfügt, mit der er nur Assets genehmigen oder Anforderungen senden kann. <p> 
   <ul>
   <li>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, welche Lizenz Ihnen zugewiesen ist.</li>
   <li>Adobe Workfront ist dabei, ein neues Preismodell und ein neues Verpackungsmodell zu entwickeln. Weitere Informationen zu Lizenzen finden Sie unter:
   <ul>
   <li>Neu: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Übersicht über neue Lizenzen</a></li>
   <li>Aktuell: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Überblick über Lizenzen</a></li></ul></li>
   <li>Wenn Sie über die richtige Zugriffsstufe verfügen und dennoch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> Zugriffsebenen sind Berechtigungssätze für Aktionen, die Sie in Workfront ausführen können. Diese werden von Ihrem Workfront-Administrator festgelegt. <p>Workfront verfügt über integrierte Zugriffsebenen, die den Workfront-Lizenzen entsprechen. Ihr Workfront-Administrator kann jedoch mehr Zugriffsebenen erstellen, um die in Ihrem Unternehmen benötigten Berechtigungssätze genauer widerzuspiegeln.</p>
   <ul>
    <li>Adobe Workfront ist dabei, ein neues Preismodell und ein neues Verpackungsmodell zu entwickeln. Informationen zu den Zugriffsebenen für die einzelnen Modelle finden Sie unter:
   <ul>
   <li>Neu: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Übersicht über die neuen Zugriffsebenen</a></li>
   <li>Aktuell: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Übersicht über Zugriffsebenen</a></li></ul></li>
    <li>Wenden Sie sich an Ihren Workfront-Administrator, um die Details Ihrer Zugriffsstufe zu erfahren.</li>
    <li>Wenn Sie Workfront-Administrator sind, lesen Sie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a> , um mehr über die Gewährung des Zugriffs auf bestimmte Objekte auf der Zugriffsebene zu erfahren.</li>  
   <li>Wenn Sie über die richtige Zugriffsstufe verfügen und dennoch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Objektberechtigungen beziehen sich auf den Zugriff auf einzelne Workfront-Objekte, wenn Sie sie erstellen oder für Sie freigegeben haben. Sie müssen beispielsweise Zugriff auf Ansicht für ein bestimmtes Projekt haben, um das Projekt anzuzeigen, auch wenn Ihre Zugriffsebene es Ihnen ermöglicht, Projekte anzuzeigen. In diesem Abschnitt der Tabelle mit den Zugriffsanforderungen werden die spezifischen Objektberechtigungen beschrieben, die Sie für die in diesem Artikel beschriebenen Aktionen benötigen.</p>
   <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff auf ein Objekt finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Workfront bietet einige Produkte, die zusätzlich zu Workfront erworben werden können.
   <p>In Artikeln, in denen Verfahren beschrieben werden, die innerhalb dieser zusätzlichen Produkte durchgeführt werden, wird das erforderliche Produkt hier aufgelistet.</p>
   <ul>
   <li>Adobe Experience Manager Assets oder Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront-Ziele</li>
   <li>Workfront-Szenario-Planer</li>
   </ul>
   <p>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, ob Ihr Unternehmen eines dieser zusätzlichen Produkte erworben hat.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-Lizenz</td> 
   <td>Adobe Workfront Fusion verfügt über ein eigenes Lizenzmodell als Workfront. 
   <ul><li>Aktuell: Das aktuelle Lizenzmodell basiert auf der Anzahl der durchgeführten Vorgänge und hat keine Einschränkungen hinsichtlich der Aktionen, die ein Unternehmen ausführen kann. </li>
   <li>Veraltet: Legacy-Lizenzen basieren darauf, ob Szenarien eine Verbindung zu Drittanbieteranwendungen herstellen können oder ob die Szenarien nur für die Automatisierung durch Workfront verwendet werden. </li>
   </ul>
   Informationen zur Fusionslizenzierung finden Sie unter <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion-Lizenzen</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


