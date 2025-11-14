---
title: Zugriffsanforderungen in der Dokumentation zu Workfront
content-type: reference
product-area: system-administration
keywords: Zugriff,Ebene,System,Administrator,Planer,Worker,Prüfer,Anforderer,extern,Benutzer
navigation-topic: access-levels
description: Artikel mit Anleitungen in der Workfront-Dokumentation enthalten eine Tabelle, in der die für dieses Verfahren erforderlichen Zugriffsberechtigungen erläutert werden. In diesem Artikel wird die Tabelle mit den Zugriffsanforderungen detaillierter erläutert, und es finden sich Links zu weiteren Informationen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 1%

---

# Zugriffsanforderungen in der Dokumentation zu Workfront

Artikel mit Anleitungen zur Workfront-Dokumentation enthalten eine Tabelle, in der die für dieses Verfahren erforderlichen Zugriffs- und Berechtigungsanforderungen erläutert werden. In dieser Tabelle mit den Zugriffsanforderungen erfahren Sie, ob Sie eine bestimmte Aktion in Workfront durchführen können oder warum dies nicht möglich ist. In diesem Artikel werden die einzelnen Elemente der Tabelle mit den Zugriffsanforderungen erläutert und Tipps zur Fehlerbehebung sowie Links zu detaillierteren Informationen bereitgestellt.

Wenn in der Tabelle mit den Zugriffsanforderungen in einem bestimmten Artikel eine Zeile fehlt, gibt es für diese Aktion keine Anforderungen dieses Typs.

>[!NOTE]
>
>Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie Fragen dazu haben, wie eines der Felder in dieser Tabelle auf Sie zutrifft.

## Die Tabelle mit den Zugriffsanforderungen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> Adobe Workfront-Pakete beziehen sich auf die von Ihrem Unternehmen erworbenen Funktionen. Die meisten Workfront-Funktionen sind in allen Packages verfügbar, mit wenigen Ausnahmen, die sich hauptsächlich auf die strategische Planung und Unternehmenssteuerung beziehen. <p>Pakete, die vor 2022 existierten, werden nicht aufgelistet.</p>
   <p>Workfront-Pakete sind in drei Bereiche unterteilt. Einige Bereiche bieten verschiedene Pakete an, z. B. Select, Prime und Ultimate.<p>
   <ul>
   <li><b>Workfront-Workflow</b>: Enthält Funktionen im Zusammenhang mit Vorgängen wie Aufgabenverwaltung, Genehmigungen und Arbeitszeittabellen. Dieses Paket ist weiter unterteilt in die Workflow-Select-, Workflow-Prime- und Workflow-Ultimate-Pakete.</li>
   <li><b>Workfront Planning</b>: Enthält Funktionen für die strategische Planung. Dieses Paket ist in die Pakete Planning Select, Planning Prime und Planning Ultimate unterteilt.</li>
   <li><b>Automatisierung und Integration von Workfront</b>: Umfasst Funktionen zur Automatisierung von Prozessen und zur Integration mit anderen Anwendungen.</li>
   </ul>
  <p>Ihr Unternehmen hat möglicherweise ein Workfront-Paket in einem oder mehreren dieser Bereiche erworben.</p>
  <p>Zuvor bot Workfront Workfront Select-, Workfront Prime- und Workfront Ultimate-Pakete an, ohne zwischen Workflow, Planung sowie Automatisierung und Integration zu unterscheiden. Ihr Unternehmen verwendet möglicherweise eines dieser Legacy-Pakete. 
   <ul><li>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, welches Adobe Workfront-Paket Ihr Unternehmen verwendet, einschließlich der Frage, ob Ihr Unternehmen das aktuelle oder das veraltete Paketmodell verwendet.</li>
   <li>Anweisungen, wie ein Workfront-Administrator das Workfront-Paket Ihres Unternehmens finden kann, finden Sie unter <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Cluster und Workfront-Paket Ihres Unternehmens anzeigen</a>.</li><li>Weitere Informationen zu den Workfront-Packages finden Sie unter <a href="https://business.adobe.com/de/products/workfront/pricing.html">Preise und Verpackung für Adobe Workfront</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> Adobe Workfront-Lizenzen beziehen sich auf die Funktionen von Workfront, die in der Ihnen zugewiesenen Lizenz enthalten sind. Beispielsweise könnte ein Benutzer über eine Lizenz verfügen, die das Kennzeichnen von Arbeitselementen und die Protokollierungszeit umfasst, während ein anderer Benutzer über eine Lizenz verfügt, die es ihm nur ermöglicht, Assets zu genehmigen oder Anfragen zu senden. <p> 
   <ul>
   <li>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, welche Lizenz Ihnen zugewiesen wurde.</li>
   <li>Informationen zu Lizenzen finden Sie unter:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Übersicht über neue Lizenzen</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Lizenzen - Überblick</a></li></ul></li>
   <li>Wenn Sie die richtige Zugriffsebene haben und immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td><p>Da Workfront eng mit anderen Adobe-Produkten zusammenarbeitet, interagieren einige Verfahren in Workfront direkt mit diesen Produkten. Um diese Verfahren zu befolgen, muss Ihr Unternehmen das Produkt gekauft haben. Um beispielsweise eine Funktion verwenden zu können, die es Workfront ermöglicht, mit Adobe Experience Manager Assets zu interagieren, muss Ihr Unternehmen Adobe Experience Manager Assets erworben haben.</p>
   <p>Artikel, in denen die mit zusätzlichen Produkten durchgeführten Verfahren beschrieben werden, führen das gewünschte Produkt in der Produktlinie dieser Tabelle auf.</p>
   <p>Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, ob Ihr Unternehmen eines dieser zusätzlichen Produkte erworben hat.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> Zugriffsebenen sind Berechtigungssätze für Aktionen, die Sie in Workfront ausführen können und die von Ihrem Workfront-Administrator festgelegt werden. <p>Workfront verfügt über integrierte Zugriffsebenen, die den Workfront-Lizenzen entsprechen. Ihr Workfront-Administrator kann jedoch weitere Zugriffsebenen erstellen, um die in Ihrem Unternehmen erforderlichen Berechtigungssätze genauer widerzuspiegeln.</p>
   <ul>
    <li>Informationen zu Zugriffsebenen finden Sie unter:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Übersicht über neue Zugriffsebenen</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Übersicht über Zugriffsebenen</a></li></ul></li>
    <li>Wenden Sie sich an Ihren Workfront-Administrator, um die Details Ihrer Zugriffsebene zu erfahren</li>
    <li>Wenn Sie Workfront-Administrator sind, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurieren des Zugriffs auf Adobe Workfront</a> weitere Informationen darüber, wie Sie Zugriff auf bestimmte Objekte auf der Zugriffsebene gewähren.</li>  
   <li>Wenn Sie die richtige Zugriffsebene haben und immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Objektberechtigungen beziehen sich auf den Zugriff auf einzelne Workfront-Objekte, die Sie erstellen oder die für Sie freigegeben werden. Sie müssen beispielsweise Ansichtszugriff auf ein bestimmtes Projekt haben, um das Projekt anzuzeigen, auch wenn Sie mit Ihrer Zugriffsebene Projekte anzeigen können. In diesem Abschnitt der Tabelle Zugriffsanforderungen werden alle spezifischen Objektberechtigungen beschrieben, die Sie zum Ausführen der Aktion im Artikel benötigen.</p>
   <p>Informationen zum Anfordern zusätzlichen Zugriffs auf ein Objekt finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte</a>.</p><p>Informationen zum Freigeben eines Objekts finden Sie unter <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Freigeben eines Objekts</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Layout-Vorlage</td> 
   <td><p>Layout-Vorlagen steuern, was Sie im Hauptmenü sehen können, und werden von Ihrem Workfront-Administrator konfiguriert. In dieser Zeile sind alle spezifischen Bereiche von Workfront aufgeführt, die zum Ausführen der Aktion in Ihr Hauptmenü aufgenommen werden müssen.</p><p>Wenn Sie in einem Artikel aufgefordert werden, auf einen Bereich im Hauptmenü zu klicken, der in Ihrem Hauptmenü nicht angezeigt wird, wenden Sie sich im Allgemeinen an Ihren Workfront-Administrator, um zu ermitteln, ob dieser Bereich Ihnen zur Verfügung gestellt werden kann.</p><p>
   Informationen dazu, wie Workfront-Admins das Hauptmenü konfigurieren können, finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-Lizenz</td> 
   <td>Adobe Workfront Fusion verfügt über ein anderes Lizenzierungsmodell als Workfront. 
   <ul><li>Das aktuelle Lizenzmodell basiert auf der Anzahl der durchgeführten Vorgänge und hat keine Einschränkungen bezüglich der möglichen Aktionen einer Organisation. </li>
   <li>Legacy-Lizenzen basieren darauf, ob Szenarien mit Anwendungen von Drittanbietern verbunden werden können oder ob die Szenarien nur für die Automatisierung von Workfront verwendet werden. </li>
   </ul>
   Informationen zur Fusion-Lizenzierung finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion-Lizenzen</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
