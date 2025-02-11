---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Firewall-Übersicht
description: Da Adobe Workfront mit dem Netzwerk Ihres Unternehmens kommuniziert, muss die Firewall Ihres Unternehmens so konfiguriert sein, dass diese Kommunikation möglich ist. Firewalls sind hochwirksame Sicherheitsmaßnahmen, die durch die Trennung des Unternehmensnetzwerks vom Internet funktionieren. Sie stellen sicher, dass nur ausgewählte Daten und der Netzwerk-Traffic in das Netzwerk des Unternehmens bzw. aus diesem heraus verschoben werden können. Die Firewall lässt Daten basierend auf der Website, die die Daten sendet oder empfängt, zu oder blockiert diese. Als Adobe Workfront-Administrator müssen Sie sicherstellen, dass Daten, die an oder von Workfront gesendet werden, die Firewall Ihres Unternehmens durchlaufen können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 1%

---

# Firewall-Übersicht

Da Adobe Workfront mit dem Netzwerk Ihres Unternehmens kommuniziert, muss die Firewall Ihres Unternehmens so konfiguriert sein, dass diese Kommunikation möglich ist. Firewalls sind hochwirksame Sicherheitsmaßnahmen, die durch die Trennung des Unternehmensnetzwerks vom Internet funktionieren. Sie stellen sicher, dass nur ausgewählte Daten und der Netzwerk-Traffic in das Netzwerk des Unternehmens bzw. aus diesem heraus verschoben werden können. Die Firewall lässt Daten basierend auf der Website, die die Daten sendet oder empfängt, zu oder blockiert diese. Als Adobe Workfront-Administrator müssen Sie sicherstellen, dass Daten, die an oder von Workfront gesendet werden, die Firewall Ihres Unternehmens durchlaufen können.

Dies wird durch eine -Zulassungsliste erreicht, die im Wesentlichen eine „Liste“ von Sites ist, die „erlaubt“ sind, Daten über die Firewall zu senden oder zu empfangen. Websites können auf zwei Arten identifiziert werden:

* **IP-Adresse**: eine Reihe von Zahlen wie 52.31.132.175
* **Domain**: Teil einer URL, z. B. `thisdomain` in `www.thisdomain.com`.

Workfront verwendet bestimmte IP-Adressen und Domains für die Web-Kommunikation. Diese müssen zur Zulassungsliste Ihres Unternehmens hinzugefügt werden, bevor Sie Workfront in Ihrem Unternehmen verwenden können.

Im Allgemeinen wird eine Zulassungsliste von einem Netzwerkadministrator konfiguriert. Arbeiten Sie mit dem Netzwerkadministrator Ihres Unternehmens zusammen, um sicherzustellen, dass Ihre Firewall diese IP-Adressen zulässt. Wenn Sie nicht wissen, wer Ihr Netzwerkadministrator ist, kann die IT-Abteilung Ihres Unternehmens Sie in die richtige Richtung weisen.

>[!IMPORTANT]
>
>Als Workfront-Administrator müssen Sie sicherstellen, dass diese IP-Adressen und Domains zur Zulassungsliste Ihres Unternehmens hinzugefügt werden. Dies gilt auch, wenn Sie sie nicht selbst hinzufügen. Workfront kann die Zulassungsliste Ihres Unternehmens nicht konfigurieren.

## Sammeln von Informationen zur Konfiguration der Firewall

Um Ihre Firewall für Workfront zu konfigurieren, muss Ihr Netzwerkadministrator wissen, welche IP-Adressen und Domains hinzugefügt werden sollen. Einige dieser Informationen sind nur für Workfront-Admins verfügbar. Als Workfront-Administrator müssen Sie diese Informationen suchen und sie Ihrem Netzwerkadministrator bereitstellen.

>[!NOTE]
>
>Es empfiehlt sich, nur die IP-Adressen und Domains hinzuzufügen, die mit den Funktionen verbunden sind, die Ihr Unternehmen aktiv verwendet. Mit diesen Informationen können Sie sicherstellen, dass diese Best Practice befolgt wird.

Geben Sie dem Netzwerkadministrator die folgenden Informationen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Spezifische IP-Adressen und Domains, die zugelassen werden sollen</td> 
   <td> <p>Der Artikel <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Zulassungsliste auf die Zulassungsliste setzte der Firewall konfigurieren</a> enthält die Liste der IP-Adressen und Domains, die Ihr Unternehmen zu seiner hinzufügen muss. </p> <p>Ihr Netzwerkadministrator hat möglicherweise keinen Zugriff auf den Artikel „Konfigurieren der Firewall-Zulassungsliste". In diesem Fall müssen Sie sie bereitstellen. Es wird nicht empfohlen, eine gedruckte (Papier-)Kopie zu drucken. Mit einer digitalen Kopie können Netzwerkadministratoren die Adressen kopieren und einfügen, was schneller und genauer ist als die Eingabe von einer Papierkopie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Cluster</td> 
   <td>Informationen zum Auffinden des Clusters Ihres Unternehmens finden Sie unter <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Cluster- und Workfront-Plan Ihres Unternehmens anzeigen</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihr Workfront-Plan</td> 
   <td> <p>Informationen zum Auffinden des Plans Ihres Unternehmens finden Sie unter <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Cluster- und Workfront-Plan Ihres Unternehmens anzeigen.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ihre Domain</td> 
   <td> <p>Um Ihre Domain zu finden, überprüfen Sie die Webadresse, mit der Sie eine Verbindung zu Workfront herstellen.</p> <p>Beispiel: Im <code>greatcompany.my.workfront.com</code> „Webadresse“ lautet die Domain „GreatCompany“</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere Adobe Workfront-Produkte</td> 
   <td> <p>Informieren Sie Ihren Netzwerkadministrator, wenn Sie Lizenzen für einen der folgenden Bereiche besitzen:</p> 
    <ul> 
     <li> <p>Adobe Workfront-Testversand</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Integrationen</td> 
   <td>Informieren Sie Ihren Netzwerkadministrator, wenn Sie einen der folgenden Punkte verwenden:
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
     <li> <p>Eine Workfront-Testfahrt</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Wenn Sie eines dieser Produkte, Integrationen oder Funktionen zu einem späteren Zeitpunkt hinzufügen, müssen Sie sich an Ihren Netzwerkadministrator wenden, damit dieser die Zulassungsliste anpassen kann.

### Cluster- und Workfront-Plan Ihres Unternehmens anzeigen {#view-your-organization-s-cluster-and-workfront-plan}

{{step-1-to-setup}}

1. Klicken Sie **linken** auf „System“
1. Um Ihren Cluster anzuzeigen, wählen Sie **Kundeninformationen**.

   Ihr Cluster wird oben rechts im Abschnitt **Basisinformationen** angezeigt.

   ![Cluster suchen](assets/locate-cluster.png)

1. Um Ihren Workfront-Plan anzuzeigen, wählen Sie **Lizenzen** aus.

   Der Plan wird oben rechts auf der Seite angezeigt.

   ![Plan suchen](assets/locate-plan.png)
