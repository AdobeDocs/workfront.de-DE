---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurieren der Zulassungsliste Ihrer Firewall
description: Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet und Ihre Benutzer können Nachrichten von Workfront senden und SSO mit Active Directory oder LDAP verwenden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 32d3cd97fc21b9679e0a615c3c07c3d69cd81225
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# Konfigurieren der Zulassungsliste Ihrer Firewall

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>Informationen zum Konfigurieren Ihrer Zulassungsliste, wenn Ihr Unternehmen in die Adobe Admin Console integriert wurde, finden Sie unter [Domänen, die für Adobe-Apps und -Dienste zulässig sein sollen](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Die Art und Weise, wie ein Unternehmen seine Zulassungsliste konfiguriert, ist für jede Organisation eindeutig. Arbeiten Sie mit Ihrem IT-Team zusammen, um das Verfahren Ihres Unternehmens zu ermitteln und diese Ergänzungen zu implementieren.

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet und die folgenden Prozesse sind möglich:

* Nachrichten von der Workfront-Anwendung senden

  >[!NOTE]
  >
  >Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

* Verwenden von Dokument-Webhooks beim Konfigurieren von benutzerdefinierten Dokumentintegrationen
* Verwenden von Workfront-Ereignisabonnements

  Weitere Informationen finden Sie unter [Ereignisabonnement-API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Sie müssen auch bestimmte Ports öffnen, damit E-Mail-Nachrichten beim Versand verschlüsselt werden können.

## Workfront-auf die Zulassungsliste setzte

Wenn Ihr Unternehmen über den Enterprise-Plan verfügt, können Sie auch zwei Workfront-auf die Zulassungsliste setzte konfigurieren:

* **E-Mail-Zulassungsliste**: Hiermit können Sie steuern, wo Benutzer in Workfront gespeicherte E-Mail-Daten versenden können. Weitere Informationen finden Sie unter [Konfigurieren der E-Mail-Zulassungsliste](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP-Zulassungsliste**: Beschränkt den Zugriff auf Workfront auf 45 IP-Adressen oder IP-Adressbereiche, die Sie angeben, und bietet eine zusätzliche Sicherheitsschicht für die Workfront-Anwendung. Weitere Informationen finden Sie unter [Zugriff auf Adobe Workfront nach IP-Adresse einschränken](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Workfront-Cluster suchen

Die IP-Adressen, die Sie Ihrer Zulassungsliste in Ihrer Firewall hinzufügen müssen, hängen vom Cluster ab, in dem Ihre Produktionsumgebung ausgeführt wird.

So suchen Sie den Cluster Ihres Unternehmens:

1. Als Workfront-Administrator klicken Sie auf das **Hauptmenü** icon ![Hauptmenü](assets/main-menu-icon.png)Klicken Sie auf **Einrichtung**.
1. Klicken Sie im linken Navigationsbereich auf **System**, wählen Sie **Kundeninformationen**.
1. Suchen Sie die **Cluster-Einrichtung** -Feld in der rechten oberen Ecke der Seite. Der Cluster Ihres Unternehmens ist hier aufgeführt.

   CL01 bezieht sich auf Cluster 1, CL02 ist Cluster 2 usw.

Weitere Informationen finden Sie im Abschnitt . [Cluster- und Workfront-Plan Ihres Unternehmens anzeigen](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) im Artikel [Firewall-Übersicht](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## IP-Adressen, die der Zulassungsliste hinzugefügt werden sollen

>[!IMPORTANT]
>
>Einige Workfront-Integrationen funktionieren nicht, wenn die Zulassungsliste aktiviert ist, da sie nicht mit einer statischen IP-Adresse konfiguriert werden können. Um die folgenden Integrationen zu verwenden, müssen Sie die Zulassungsliste deaktivieren.
>
>* Workfront für G Suite
>* Workfront für Outlook
>* Workfront für Salesforce

* [IP-Adressen, die die Cluster 1, 2, 3, 5, 7, 8 und 9 zulassen](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [IP-Adressen für Cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [IP-Adressen für Cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [IP-Adressen, um ein Testlaufwerk zu ermöglichen](#IP%20Addre2)
* [IP-Adressen, die bei der Implementierung von Ereignisabonnements zulässig sind](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [IP-Adressen, um eine erweiterte Authentifizierung zu ermöglichen](#ip-addresses-to-allow-for-enhanced-authentication)
* [IP-Adressen für den Zugriff auf Workfront Fusion hinzufügen](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [IP-Adressen, die zur Verwendung von Workfront für Jira hinzugefügt werden sollen](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URLs, die für alle Cluster Workfront hinzugefügt werden sollen](#urls-to-add-for-all-clusters-workfront)

### IP-Adressen, die die Cluster 1, 2, 3, 5, 7, 8 und 9 zulassen {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Wenn sich Ihre Produktionsumgebung auf Cluster 1, 2, 3, 5 oder 7 befindet, müssen Sie die folgenden IP-Adressen zulassen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Für SSO, Dokument-Webhooks oder andere Funktionen</td> 
   <td> 
    <ul> 
     <li>35 160 0 242</li> 
     <li>34 213 36 118</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 36 154 34</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">So erhalten Sie E-Mails von der Workfront-Anwendung</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13 58 86 183</li> 
     <li>34 209 181 84</li> 
     <li>35 161 82 137</li> 
     <li>52 14 70 114</li> 
     <li>52 15 230 220</li> 
     <li>54 71 252 65</li> 
    </ul> <p>Weitere Informationen zu den folgenden IP-Adressen finden Sie unter <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Neue IP-Adressen für Adobe Workfront-E-Mails mit Version 21.1</a></p> 
    <ul> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>23 251 237 109</li> 
     <li>23 251 237 106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen für Cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Wenn sich Ihre Produktionsumgebung auf Cluster 4 befindet, fügen Sie die folgenden IP-Adressen für SSO, Dokument-Webhook-Integrationen hinzu und erhalten Sie E-Mails von der Workfront-Anwendung:

* 52 31 132 175
* 52 19 188 226
* 52 28 49 94
* 52 29 41 175
* 52 29 197 69
* 52 48 124 108
* 69 169 230 231
* 69 169. 230,232
* 3 121 91 129
* 3 122 11 35
* 34 246 27 40
* 52 208 123 166
* 52 208 159 124
* 52 17 130 201
* 34 252 250 191
* 52 30 133 50
* 54 220 93 204
* 34 254 76 122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

Weitere Informationen zu den folgenden IP-Adressen finden Sie unter [Neue IP-Adressen für Adobe Workfront-E-Mails mit Version 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23 251 239 98
* 23 251 239 99

### IP-Adressen für Cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Wenn sich Ihre Produktionsumgebung auf Cluster 6 befindet, fügen Sie die folgenden IP-Adressen hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">So erhalten Sie E-Mails von der Workfront-Anwendung</td> 
   <td> 
    <ul> 
     <li>34 94 227 64</li> 
     <li>34 94 227 65</li> 
     <li>34 94 227 66</li> 
     <li>34 94 227 67</li> 
     <li>34 66 82 64</li> 
     <li>34 66 82 65</li> 
     <li>34 66 82 66</li> 
     <li>34 66 82 67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">So verwenden Sie den E-Mail-Dienst</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13 58 86 183</li> 
     <li>34 209 181 84</li> 
     <li>35 161 82 137</li> 
     <li>52 14 70 114</li> 
     <li>52 15 230 220</li> 
     <li>54 71 252 65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">So verwenden Sie den E-Mail-Dienst Mailpiste</td> 
   <td> 
    <ul> 
     <li>143 55 228 56 </li> 
     <li>209 61 151 229</li> 
     <li>69,72,43,7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen, um ein Testlaufwerk zu ermöglichen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">So erhalten Sie E-Mails von der Workfront-Anwendung bei Verwendung eines Testlaufwerks</td> 
   <td> 
    <ul> 
     <li>69 42 126 188 </li> 
     <li>66 119 37 185</li> 
     <li>66 119 37 186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für SSO- und Dokument-Webhook-Integrationen bei Verwendung eines Testlaufwerks</td> 
   <td> 
    <ul> 
     <li> <p>69 42 126 188:</p> <p>Diese Adresse muss auch zu Ihrer Zulassungsliste hinzugefügt werden, damit Ihre Benutzer E-Mails von Workfront erhalten können.</p> </li> 
     <li>66 119 37 186</li> 
     <li>66 119 37 167</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen, die bei der Implementierung von Ereignisabonnements zulässig sind  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Fügen Sie für alle Umgebungen die folgenden IP-Adressen hinzu, um Nutzlasten von Workfront-Ereignisabonnenten zu empfangen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Für Kunden in Europa</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>52 17 130 201</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für Kunden an anderen Standorten als Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52 36 154 34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 39 217 230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen, um eine erweiterte Authentifizierung zu ermöglichen {#ip-addresses-to-allow-for-enhanced-authentication}

Fügen Sie die folgenden IP-Adressen hinzu, um die erweiterte Authentifizierung für die Vorschau oder Produktion zu verwenden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wenn Ihre Umgebung auf Cluster 1, 2, 3, 5, 7, 8 oder 9 basiert</td> 
   <td> 
    <ul> 
     <li>35 167 74 121</li> 
     <li>35 166 202 113</li> 
     <li>35 160 3 103</li> 
     <li>54 183 64 135</li> 
     <li>54 67 77 38</li> 
     <li>54 67 15 170</li> 
     <li>54 183 204 205</li> 
     <li>35 171 156 124</li> 
     <li>18 233 90 226</li> 
     <li>3 21 189 167</li> 
     <li>18 232 225 224</li> 
     <li>34 233 19 82</li> 
     <li>52 204 128 250</li> 
     <li>3 132 201 78</li> 
     <li>3 19 44 88</li> 
     <li>3 20 244 231</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn Ihre Umgebung auf Cluster 4 basiert</td> 
   <td> 
    <ul> 
     <li>52 28 56 226</li> 
     <li>52 28 45 240</li> 
     <li>52 16 224 164</li> 
     <li>52 16 193 66</li> 
     <li>34 253 4 94</li> 
     <li>52 50 106 250</li> 
     <li>52 211 56 181</li> 
     <li>52 213 38 246</li> 
     <li>52 213 74 69</li> 
     <li>52 213 216 142</li> 
     <li>35 156 51 163</li> 
     <li>35 157 221 52</li> 
     <li>52 28 184 187</li> 
     <li>52 28 212 16</li> 
     <li>52 29 176 99</li> 
     <li>52 57 230 214</li> 
     <li>54 76 184 103</li> 
     <li>52 210 122 50</li> 
     <li>52 208 95 174</li> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### IP-Adressen für den Zugriff auf Workfront Fusion hinzufügen  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Fügen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzu, um Workfront Fusion den Zugriff auf Ihr System zu ermöglichen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Rechenzentrum</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US-Rechenzentrum</p> </td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>44 241 82 96</li> 
     <li>100 20 126 137</li>
     <li>34 223 32 44</li>
     <li>52 39 176 220</li>
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

Wenn Ihr Unternehmen die Filterung ausgehender Netzwerke verwendet, fügen Sie Ihrer Zulassungsliste die folgende Domäne hinzu, damit Ihr System auf Workfront Fusion zugreifen kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Rechenzentrum</td> 
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
>Ausgehende Netzwerkfilter sind selten. Wenden Sie sich an Ihren Netzwerkadministrator, um zu sehen, ob Sie Ihre Zulassungsliste aktualisieren müssen, damit sie berücksichtigt werden kann.

### IP-Adressen, die zur Verwendung von Workfront für Jira hinzugefügt werden sollen {#ip-addresses-to-add-for-using-workfront-for-jira}

Fügen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzu, um die Workfront für die Jira-Integration zu verwenden.

Die Domäne jira.workfront.com muss auch von Ihren Unternehmensservern aus zugänglich sein. Diese Domäne ist erforderlich, da sie als Middleware zwischen Workfront und Jira dient.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Für Kunden in Europa</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>52 208 159 124</li> 
     <li>54 220 93 204</li> 
     <li>52 17 130 201</li> 
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
     <li>35 162 128 73</li> 
     <li>52 42 25 64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li> <p>3 209 27 146</p> </li> 
     <li> <p>18 205 251,4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Für Kunden an anderen Standorten als Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52 36 154 34</li> 
     <li>34 211 224,9</li> 
     <li>54 218 48 56</li> 
     <li>52 39 217 230</li> 
     <li>35 162 128 73</li> 
     <li>52 42 25 64</li> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242 </li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domänen, die für den Zugriff auf Workfront hinzugefügt werden sollen

Wenn Ihr Unternehmen ausgehende Netzwerkfilter verwendet, fügen Sie Ihrer Zulassungsliste die folgenden Domänen hinzu, damit Ihr System auf Workfront zugreifen kann.

>[!NOTE]
>
>Ausgehende Netzwerkfilter sind selten. Wenden Sie sich an Ihren Netzwerkadministrator, um zu sehen, ob Sie Ihre Zulassungsliste aktualisieren müssen, damit sie berücksichtigt werden kann.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/
* *.static.workfront.com

  Hierbei handelt es sich um eine statische Domäne, die alle folgenden Domänen umfasst. Sie können die einzelnen Domänen hinzufügen, wenn Sie Folgendes bevorzugen:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com


## URLs, die für alle Cluster Workfront hinzugefügt werden sollen {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">So ermöglichen Sie die Anzeige von Hilfeinhalten in Ihrer Workfront-Umgebung</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Um Workfront Proof den Zugriff auf Workfront in einem beliebigen Cluster zu ermöglichen, fügen Sie diese zu allen Umgebungen hinzu</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Erforderlich für die Anzeige von Testsendungen in Workfront</li> 
     <li>*.proofhq.com - Erforderlich für die Anzeige von Testsendungen in Workfront Proof</li> 
     <li>*.proofhq.eu - Erforderlich, um Testsendungen in Workfront Proof anzuzeigen</li> 
    </ul> <p><b>NOTE</b>:  <p>Das Hinzufügen von IP-Adressen zu Ihrer Zulassungsliste für Workfront Proof wird nicht unterstützt. Sie waren dynamisch, nachdem Workfront nach AWS verschoben wurde. Stattdessen empfehlen wir, nur Workfront Proof-Domänen zuzulassen.</p> <p>Wenn es ein Problem beim Hinzufügen dieser Domänen zu Ihrer Zulassungsliste gibt und Sie stattdessen eine IP-Adresse benötigen, wenden Sie sich an den Workfront-Kundensupport.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## IP-Adressen und URLs, die für den Zugriff auf Workfront Proof hinzugefügt werden sollen

Sie müssen die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzufügen, um verschiedene Funktionen nutzen zu können.

* [Für Rückrufe und Weberfassungs-Testsendungen](#for-callbacks-and-webcapture-proofs)
* [Ausgehende E-Mail](#for-outgoing-email)

### Für Rückrufe und Weberfassungs-Testsendungen {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (Clusters 1, 2, 3, 5 und 7)</td> 
   <td> 
    <ul> 
     <li>34 213 36 118</li> 
     <li>35 160 0 242</li> 
     <li>3 209 27 146</li> 
     <li>18 205 251,4</li> 
     <li>35 165 152 202</li> 
     <li>54 184 151 122</li> 
     <li>35 84 40 190</li> 
     <li>54 218 48 56</li> 
     <li>34 211 224,9</li> 
     <li>52 36 154 34</li> 
     <li>34 232 138 38</li> 
     <li>54 237 6 156</li> 
     <li>54 237 12 32</li> 
     <li>44 241 82 96</li> 
     <li>54 244 142 219</li> 
     <li>52 39 217 230</li> 
     <li>52 207 47 153</li> 
     <li>50 16 118 214</li> 
     <li>52 54 180 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>34 246 27 40</li> 
     <li>52 208 123 166</li> 
     <li>3 121 91 129</li> 
     <li>3 122 11 35</li> 
     <li>34 241 103 51</li> 
     <li>46 51 203 201</li> 
     <li>54 247 174 227</li> 
     <li>52 208 159 124</li> 
     <li>52 17 130 201</li> 
     <li>34 252 250 191</li> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> <p><b>NOTE</b>: DNS-Serveroptionen werden nicht mehr unterstützt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Ausgehende E-Mail {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (Clusters 1, 2, 3, 5 und 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23 251 237 106</li> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23 251 239 98</li> 
     <li>69 169 230 231</li> 
     <li>69 169 230 232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ports für optimale Workfront Proof-Leistung öffnen

Öffnen Sie die folgenden Ports, wenn Probleme beim Laden von Testsendungen auftreten oder in Workfront Proof nicht funktionieren:

* 5671
* 5672
* 15671

## Für verschlüsselte E-Mails zu öffnende Ports

E-Mails aus der Workfront-Anwendung werden mit den Ports 465 und 587 verschlüsselt gesendet. Wenn Ihr E-Mail-Server verschlüsselte E-Mails nicht unterstützt, werden E-Mails unverschlüsselt über Port 25 zugestellt.

## E-Mail-Benachrichtigungen vom Workfront-Support

Wenn Sie keine E-Mails vom Workfront-Support erhalten, stellen Sie sicher, dass Sie die benötigten Salesforce-IP-Adressen und -Domänen hinzufügen. Weitere Informationen finden Sie im Salesforce-Hilfeartikel zu den zuzulassenden Salesforce-IP-Adressen und -Domänen.
