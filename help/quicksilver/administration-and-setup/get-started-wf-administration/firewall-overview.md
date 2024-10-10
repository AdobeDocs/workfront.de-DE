---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Firewall-Übersicht
description: Da Adobe Workfront mit dem Netzwerk Ihres Unternehmens kommuniziert, muss die Firewall Ihres Unternehmens so konfiguriert sein, dass sie diese Kommunikation zulässt. Firewalls sind hochwirksame Sicherheitsmaßnahmen, die durch die Trennung des Netzwerks eines Unternehmens vom Internet funktionieren. Sie stellen sicher, dass nur ausgewählte Daten und Netzwerk-Traffic in das oder aus dem Netzwerk des Unternehmens übertragen werden können. Die Firewall lässt Daten basierend auf der Site zu, die die Daten sendet oder empfängt. Als Adobe Workfront-Administrator müssen Sie sicherstellen, dass an oder von Workfront gesendete Daten über die Firewall Ihres Unternehmens übermittelt werden können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: 5cd1cbd1976d5574668098be53daee780a9cc1fb
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Firewall-Übersicht

Da Adobe Workfront mit dem Netzwerk Ihres Unternehmens kommuniziert, muss die Firewall Ihres Unternehmens so konfiguriert sein, dass sie diese Kommunikation zulässt. Firewalls sind hochwirksame Sicherheitsmaßnahmen, die durch die Trennung des Netzwerks eines Unternehmens vom Internet funktionieren. Sie stellen sicher, dass nur ausgewählte Daten und Netzwerk-Traffic in das oder aus dem Netzwerk des Unternehmens übertragen werden können. Die Firewall lässt Daten basierend auf der Site zu, die die Daten sendet oder empfängt. Als Adobe Workfront-Administrator müssen Sie sicherstellen, dass an oder von Workfront gesendete Daten über die Firewall Ihres Unternehmens übermittelt werden können.

Dies wird durch eine Zulassungsliste erreicht, bei der es sich im Wesentlichen um eine &quot;Liste&quot;von Sites handelt, die Daten über die Firewall senden oder empfangen dürfen. Sites können auf zwei Arten identifiziert werden:

* **IP-Adresse**: eine Reihe von Zahlen wie 52.31.132.175
* **Domäne**: Teil einer URL, z. B. `thisdomain` in `www.thisdomain.com`.

Workfront verwendet bestimmte IP-Adressen und Domänen für die Web-Kommunikation. Diese müssen der Zulassungsliste Ihres Unternehmens hinzugefügt werden, bevor Sie Workfront in Ihrem Unternehmen verwenden können.

Im Allgemeinen wird eine Zulassungsliste von einem Netzwerkadministrator konfiguriert. Wenden Sie sich an den Netzwerkadministrator Ihres Unternehmens, um sicherzustellen, dass Ihre Firewall diese IP-Adressen zulässt. Wenn Sie nicht wissen, wer Ihr Netzwerkadministrator ist, kann die IT-Abteilung Ihres Unternehmens Sie in die richtige Richtung weisen.

>[!IMPORTANT]
>
>Als Workfront-Administrator müssen Sie sicherstellen, dass diese IP-Adressen und Domänen zur Zulassungsliste Ihrer Organisation hinzugefügt werden. Dies trifft auch dann zu, wenn Sie sie nicht selbst hinzufügen. Workfront kann die Zulassungsliste Ihrer Organisation nicht konfigurieren.

## Informationen zur Konfiguration Ihrer Firewall sammeln

Um Ihre Firewall für Workfront zu konfigurieren, muss Ihr Netzwerkadministrator wissen, welche IP-Adressen und Domänen hinzugefügt werden sollen. Einige dieser Informationen stehen nur einem Workfront-Administrator zur Verfügung. Als Workfront-Administrator müssen Sie diese Informationen suchen und sie Ihrem Netzwerkadministrator bereitstellen.

>[!NOTE]
>
>Die Best Practice für die Sicherheit besteht darin, nur die IP-Adressen und Domänen hinzuzufügen, die eine Verbindung zu der Funktion herstellen, die Ihr Unternehmen aktiv verwendet. Durch Angabe dieser Informationen können Sie sicherstellen, dass diese Best Practice eingehalten wird.

Geben Sie Ihrem Netzwerkadministrator die folgenden Informationen an:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Spezifische IP-Adressen und Domänen, die</td> 
   <td> <p>Der Artikel <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Konfigurieren der Zulassungsliste Ihrer Firewall</a> enthält die Liste der IP-Adressen und Domänen, die Ihr Unternehmen zu seiner Zulassungsliste hinzufügen muss. </p> <p>Möglicherweise hat Ihr Netzwerkadministrator keinen Zugriff auf den Artikel "Zulassungsliste der Firewall konfigurieren". In diesem Fall müssen Sie sie ihnen bereitstellen. Es wird nicht empfohlen, eine Papierkopie zu drucken. Mit einer digitalen Kopie kann Ihr Netzwerkadministrator die Adressen kopieren und einfügen. Dies ist schneller und genauer als die Eingabe aus einer Kopie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Cluster</td> 
   <td>Informationen zum Auffinden des Clusters Ihres Unternehmens finden Sie unter <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Cluster- und Workfront-Plan für Ihr Unternehmen anzeigen</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Workfront-Abo</td> 
   <td> <p>Informationen zum Finden des Unternehmensplans finden Sie unter <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Cluster- und Workfront-Plan Ihres Unternehmens anzeigen.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihre Domäne</td> 
   <td> <p>Um Ihre Domäne zu finden, sehen Sie sich die Webadresse an, mit der Sie eine Verbindung zu Workfront herstellen.</p> <p>Beispiel: In der Webadresse <code>greatcompany.my.workfront.com</code> lautet die Domäne "Großunternehmen".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sonstige Adobe Workfront-Produkte</td> 
   <td> <p>Informieren Sie Ihren Netzwerkadministrator, wenn Sie Lizenzen für eine der folgenden Optionen haben:</p> 
    <ul> 
     <li> <p>Adobe Workfront-Testversand</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Integrationen</td> 
   <td>Informieren Sie Ihren Netzwerkadministrator, wenn Sie Folgendes verwenden:
    <ul>
     <li><p>Workfront für Jira</p></li>
     <li><p>Workfront für Google Workspace</p></li>
     <li><p>Workfront für Microsoft Teams</p></li>
     <li><p>Workfront für Outlook</p></li>
     <li><p>Workfront für Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Funktionen</td> 
   <td> <p>Informieren Sie Ihren Netzwerkadministrator, wenn Sie Folgendes verwenden:</p> 
    <ul> 
     <li> <p>Ein Workfront-Testlaufwerk</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Wenn Sie zu einem späteren Zeitpunkt eines dieser Produkte, Integrationen oder Funktionen hinzufügen, müssen Sie sich an Ihren Netzwerkadministrator wenden, damit dieser die Zulassungsliste anpassen kann.

### Cluster- und Workfront-Plan Ihres Unternehmens anzeigen {#view-your-organization-s-cluster-and-workfront-plan}

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **System** .
1. Um den Cluster anzuzeigen, wählen Sie **Kundeninformationen** aus.

   Ihr Cluster wird oben rechts im Abschnitt **Grundlegende Informationen** angezeigt.

   ![](assets/locate-cluster.png)

1. Um Ihren Workfront-Plan anzuzeigen, wählen Sie **Lizenzen** aus.

   Ihr Plan wird in der Nähe der oberen rechten Ecke der Seite angezeigt.

   ![](assets/locate-plan.png)
