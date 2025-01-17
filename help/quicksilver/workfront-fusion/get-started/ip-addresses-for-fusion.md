---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP-Adressen für den Zugriff auf Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# IP-Adressen für den [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* auf die Zulassungsliste setzen [Konfigurieren von IP-Adressen für Fusion in der Ihres Unternehmens](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] benötigt zusätzlich zu einer [!DNL Adobe Workfront license] eine [!DNL Adobe Workfront Fusion].

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu seiner Zulassungsliste hinzufügen, um eine offene Kommunikation zwischen Ihrer Umgebung und [!DNL Adobe Workfront Fusion] zu ermöglichen.

Sie können alle IP-Adressen und Domains von Fusion zu Ihrer Zulassungsliste hinzufügen oder Ihren Fusion-Cluster suchen und nur die IP-Adressen und Domains für diesen Cluster hinzufügen.

## Alle IP-Adressen und Domains von Fusion hinzufügen

Fügen Sie Ihrer Zulassungsliste die folgenden IP-Adressen hinzu:

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

Wenn Ihr Unternehmen ausgehende Netzwerkfilter verwendet, fügen Sie außerdem die folgende Domain zu Ihrer Zulassungsliste hinzu, damit Ihr System auf Workfront Fusion zugreifen kann. Diese werden für Webhooks verwendet.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Fügen Sie Fusion IP-Adressen und Domains nur für Ihren Cluster hinzu

### Identifizieren des Rechenzentrums

Die IP-Adressen variieren je nachdem, wo Ihre Daten gespeichert werden.

Wenn Sie über eine URL auf Fusion zugreifen, können Sie die URL überprüfen, um Ihr Rechenzentrum zu finden.

| URL | Rechenzentrum |
| --- | --- |
| `https://app.workfrontfusion.com/` | US-Rechenzentrum |
| `https://app-eu.workfrontfusion.com/` | EU-Rechenzentrum |
| `https://app-az.workfrontfusion.com/` | Azure-Rechenzentrum |

Wenn Sie über experience.adobe.com auf Fusion zugreifen, können Sie die Registerkarte Netzwerk in Ihrem Browser überprüfen, um das Rechenzentrum zu identifizieren.

| URL | Rechenzentrum |
| --- | --- |
| Aufrufe an `https://fusion.adobe.com` | US-Rechenzentrum |
| Aufrufe an `https://eu.fusion.adobe.com` | EU-Rechenzentrum |
| Aufrufe an `https://az.fusion.adobe.com` | Azure-Rechenzentrum |

### Hinzufügen von IP-Adressen und Domains für Ihr Rechenzentrum

Fügen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzu, um [!DNL Workfront Fusion] den Zugriff auf Ihr System zu ermöglichen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU-Rechenzentrum</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US-Rechenzentrum</p> </td> 
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

Wenn Ihr Unternehmen ausgehende Netzwerkfilter verwendet, fügen Sie außerdem die folgende Domain zu Ihrer Zulassungsliste hinzu, damit Ihr System auf Workfront Fusion zugreifen kann.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU-Rechenzentrum</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US-Rechenzentrum</p> </td> 
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

Weitere Informationen zum Einrichten der Zulassungsliste Ihres Unternehmens finden Sie unter [Konfigurieren der Firewall-Zulassungsliste ](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
