---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Firewall-Zulassungsliste konfigurieren
description: Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern eröffnet und Ihren Benutzern ermöglicht, Nachrichten von Workfront zu senden und SSO mit Active Directory oder LDAP zu verwenden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
TQID: https://experienceleague.adobe.com/voAiMROhu9NJkN-WLjPWcpDu-x8YYgtlZNeNWk8dFjA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: ec8965fc-2f75-47f6-a9bb-730e8c2725f3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1456
ht-degree: 6%

---

# Firewall-Zulassungsliste konfigurieren

<!-- Audited: 12/2023 -->

<!--Follow up October 2026-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in Admin Console erhalten haben. Da nun alle Organisationen in die Adobe Admin Console integriert wurden, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Informationen zum Konfigurieren Ihrer Zulassungsliste nach dem Onboarding Ihres Unternehmens für die Adobe Admin Console finden Sie unter [Domains dürfen für Adobe-Apps und -Services nicht verwendet werden](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Administrationsunterschiede zwischen Adobe Workfront und Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Die Art und Weise, wie ein Unternehmen seine Zulassungsliste konfiguriert, ist für jedes Unternehmen einzigartig. Arbeiten Sie mit Ihrem IT-Team zusammen, um die Vorgehensweise Ihres Unternehmens zu ermitteln und diese Ergänzungen zu implementieren.

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern eröffnet und die folgenden Prozesse ermöglicht:

* Verwenden von Dokument-Webhooks beim Konfigurieren von benutzerdefinierten Dokumentintegrationen
* Verwenden von Workfront-Ereignisabonnements

  Weitere Informationen finden Sie unter [Ereignisabonnement-API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Sie müssen auch bestimmte Ports öffnen, damit E-Mail-Nachrichten beim Versand verschlüsselt werden.

## Workfront-Zulassungslisten, die Sie verwenden können

Wenn Ihr Unternehmen über den Unternehmensplan verfügt, können Sie auch zwei Workfront-Zulassungslisten konfigurieren:

* **E-Mail** Zulassungsliste: Hiermit können Sie steuern, wo Benutzer in Workfront gespeicherte E-Mail-Daten senden können. Weitere Informationen finden Sie unter [Konfigurieren Ihrer E-Mail](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP** Zulassungsliste: Beschränkt den Zugriff auf Workfront auf 75 angegebene IP-Adressen oder IP-Adressbereiche und bietet eine zusätzliche Sicherheitsebene für das Workfront-Programm. Weitere Informationen finden Sie unter [Zugriff auf Adobe Workfront nach IP-Adresse beschränken](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Workfront-Cluster suchen

Die IP-Adressen, die Sie Ihrer Firewall zur Zulassungsliste hinzufügen müssen, hängen vom Cluster ab, auf dem Ihre Produktionsumgebung ausgeführt wird.

So suchen Sie den Cluster Ihrer Organisation:

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **System** und wählen Sie dann **Kundeninformationen** aus.
1. Suchen Sie das **Cluster-Setup** oben rechts auf der Seite. Der Cluster Ihrer Organisation wird hier aufgelistet.

   CL01 bezieht sich auf Cluster 1, CL02 ist Cluster 2 usw.

Weitere Informationen finden Sie im Abschnitt [Anzeigen des Cluster- und Workfront-Plans Ihres ](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) im Artikel [Firewall-Übersicht](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Der Zulassungsliste hinzuzufügende IP-Adressen

* [IP-Adressen für die Cluster 1, 2, 3, 5, 7, 8 und 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [IP-Adressen, um Cluster 4 zuzulassen](#ip-addresses-to-allow-for-cluster-4)
* [IP-Adressen, um Cluster 6 zuzulassen](#ip-addresses-to-allow-for-cluster-6)
* [IP-Adressen, die Cluster 10 zulassen](#ip-addresses-to-allow-for-cluster-10)
* [IP-Adressen, um eine Testfahrt zu ermöglichen](#IP%20Addre2)
* [IP-Adressen, die bei der Implementierung von Ereignisabonnements zulässig sind](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [IP-Adressen, die für den Zugriff auf Workfront Fusion hinzugefügt werden sollen](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [IP-Adressen, die für die Verwendung von Workfront for Jira hinzugefügt werden sollen](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Hinzuzufügende URLs für alle Cluster in Workfront](#urls-to-add-for-all-clusters-workfront)

### So empfangen Sie E-Mails von der Workfront-Anwendung

Wenn Ihre Firewall oder Ihr E-Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzufügen, um E-Mails von der Workfront-Anwendung zu erhalten.

#### US-Regionen: Cluster 1, 2, 3, 5, 6, 7, 8, 9 und 10

* 206.55.149.211
* 206.55.149.212
* 206.55.149.213
* 206.55.149.214
* 206.55.149.215
* 23.251.237.106
* 23.251.237.107
* 23.251.237.108
* 23.251.237.109
* 54.240.119.54
* 54.240.119.55
* 54.240.60.174
* 54.240.60.175
* 54.240.61.222
* 54.240.61.223

#### EU-Regionen: Cluster 4, 11, 12 und 13

* 23.251.239.98
* 23.251.239.99
* 24.110.76.223
* 24.110.76.224
* 69.169.230.231
* 69.169.230.232


### SSO, Document Webhook-Integrationen und andere Funktionen

#### US-Regionen: Cluster 1, 2, 3, 5, 6, 7, 8, 9 und 10

**Cluster 1, 2, 3, 5, 6, 7, 8, 9**


* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4
* 34.211.224.9
* 54.218.48.56
* 52.36.154.34
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 54.203.255.135/32
* 35.155.2.51/32
* 52.34.192.77/32

**Cluster 10**

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

#### EU-Regionen: Cluster 4 und 11


**Cluster 4**

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32


### IP-Adressen, um eine Testfahrt zu ermöglichen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">So empfangen Sie E-Mails von der Workfront-Anwendung bei Verwendung einer Testlaufwerk</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für SSO- und Dokument-Webhook-Integrationen bei Verwendung einer Testfahrt</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Diese Adresse muss auch Ihrer Zulassungsliste hinzugefügt werden, damit Ihre Benutzerinnen und Benutzer E-Mails von Workfront erhalten können.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen, die bei der Implementierung von Ereignisabonnements zulässig sind  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Fügen Sie für alle Umgebungen die folgenden IP-Adressen hinzu, um Payloads von Workfront-Ereignisabonnements zu erhalten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Für Kunden in Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für Kunden an anderen Standorten als Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Für den Zugriff auf Workfront Fusion hinzuzufügende IP-Adressen  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Fügen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzu, damit Workfront Fusion auf Ihr System zugreifen kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU-Rechenzentrum</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US-Rechenzentrum</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] im Microsoft Azure-Cluster</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Wenn Ihr Unternehmen ausgehende Netzwerkfilter verwendet, fügen Sie außerdem die folgende Domain zu Ihrer Zulassungsliste hinzu, damit Ihr System auf Workfront Fusion zugreifen kann. Diese URLs werden für Webhooks in Fusion verwendet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU-Rechenzentrum</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US-Rechenzentrum</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] im Microsoft Azure-Cluster</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Filterung ausgehender Netzwerke ist ungewöhnlich. Erkundigen Sie sich bei Ihrem Netzwerkadministrator, ob Sie Ihre Zulassungsliste aktualisieren müssen, um sie zu berücksichtigen.

### IP-Adressen, die für die Verwendung von Workfront for Jira hinzugefügt werden sollen {#ip-addresses-to-add-for-using-workfront-for-jira}

Fügen Sie Ihrer Zulassungsliste die folgenden IP-Adressen hinzu, um die Integration von Workfront for Jira zu verwenden.

Die Domain jira.workfront.com muss auch von Ihren Unternehmensservern aus zugänglich sein. Diese Domain ist erforderlich, da sie als Middleware zwischen Workfront und Jira dient.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Für Kunden in Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für Kunden an anderen Standorten als Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Für den Zugriff auf Workfront hinzuzufügende Domains

Wenn Ihr Unternehmen ausgehende Netzwerkfilter verwendet, fügen Sie die folgenden Domains zu Ihrer Zulassungsliste hinzu, damit Ihr System auf Workfront zugreifen kann.

>[!NOTE]
>
>Filterung ausgehender Netzwerke ist ungewöhnlich. Erkundigen Sie sich bei Ihrem Netzwerkadministrator, ob Sie Ihre Zulassungsliste aktualisieren müssen, um sie zu berücksichtigen.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* In: snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Dies ist eine statische Domain, die alle folgenden Domains umfasst. Sie können die einzelnen Domains hinzufügen, wenn Sie es vorziehen:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Da sich Ihr Unternehmen auf dem einheitlichen Adobe-Erlebnis befindet, verwendet es die folgenden Domains. Diese Domains werden unter `*.adobe.com` behandelt, können jedoch bei Bedarf hinzugefügt werden.

* &lt;Ihre Domain>.my.workfront.adobe.com
* &lt;Ihre Domain>.preview.workfront.adobe.com
* &lt;Ihre Domain>.sb01.workfront.adobe.com
* &lt;Ihre Domain>.sb02.workfront.adobe.com


Fügen Sie für Workfront Fusion die folgenden Domains hinzu:

<!--Remove me October 2026-->

* Für Unternehmen, die nicht am einheitlichen Adobe-Erlebnis teilnehmen:
   * app.workfrontfusion.com (US AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* Für die Organisation des einheitlichen Adobe-Erlebnisses
(Diese Domains werden unter `*.adobe.com` behandelt, können jedoch bei Bedarf hinzugefügt werden.)

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## Hinzuzufügende URLs für alle Cluster in Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">So können Sie Hilfeinhalte in Ihrer Workfront-Umgebung anzeigen</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um Workfront Proof Zugriff auf Workfront auf einem beliebigen Cluster zu ermöglichen, fügen Sie diese zu allen Umgebungen hinzu</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Erforderlich, um Testsendungen in Workfront anzuzeigen</li> 
     <li>*.proofhq.com - Erforderlich, um Testsendungen in Workfront Proof anzuzeigen</li> 
     <li>*.proofhq.eu - Erforderlich, um Testsendungen in Workfront Proof anzuzeigen</li> 
    </ul> <p><b>HINWEIS</b>:  <p>Das Hinzufügen von IP-Adressen zu Ihrer Zulassungsliste für Workfront Proof wird von uns nicht unterstützt. Sie waren dynamisch, nachdem Workfront zu AWS gewechselt war. Stattdessen empfehlen wir, nur Workfront Proof-Domains zuzulassen.</p> <p>Wenn beim Hinzufügen dieser Domains zu Ihrer Zulassungsliste ein Problem auftritt und Sie stattdessen eine IP-Adresse benötigen, wenden Sie sich an den Kunden-Support von Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Für den Zugriff auf Workfront Proof hinzuzufügende IP-Adressen und URLs

Sie müssen die folgenden IP-Adressen zu Ihrer -Zulassungsliste hinzufügen, um verschiedene Funktionen verwenden zu können.

* [Für Callbacks und WebCapture-Korrekturabzüge](#for-callbacks-and-webcapture-proofs)
* [Für ausgehende E-Mails](#for-outgoing-email)

### Für Callbacks und WebCapture-Korrekturabzüge {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">prod-us (Cluster 1, 2, 3, 5 und 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">PROD-EU (Cluster 4)</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>HINWEIS</b>: DNS-Serveroptionen werden nicht mehr unterstützt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Für ausgehende E-Mails {#for-outgoing-email}

Siehe Abschnitt [So empfangen Sie E-Mails von der Workfront](#to-receive-email-from-the-workfront-application)Anwendung oben.


## Zu öffnende Ports für optimale Workfront Proof-Leistung

Öffnen Sie die folgenden Ports, wenn Sie Probleme beim Laden von Korrekturabzügen haben oder nicht in Workfront Proof arbeiten:

* 5671
* 5672
* 15671

## Für verschlüsselte E-Mails zu öffnende Ports

E-Mails aus der Workfront-Anwendung werden verschlüsselt über die Ports 465 und 587 gesendet. Wenn Ihr Mailserver verschlüsselte E-Mails nicht unterstützt, werden E-Mails unverschlüsselt über Port 25 zugestellt.

## E-Mail-Benachrichtigungen vom Workfront-Support

Wenn Sie keine E-Mails vom Workfront-Support erhalten, stellen Sie sicher, dass Sie die benötigten Salesforce-IP-Adressen und Domains hinzufügen. Weitere Informationen finden Sie im Salesforce-Hilfeartikel zu Salesforce-IP-Adressen und Domains, die zulässig sind.
