---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: IP-Adressen für den Zugriff auf Adobe Workfront Fusion
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 55a4fda46f6d314c71d9ef98864b21b84f946b09
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# IP-Adressen für den Zugriff [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert [!DNL Adobe Workfront Fusion] zusätzlich zu einer [!DNL Adobe Workfront license].

Wenn Ihre Firewall- oder Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen, um eine offene Kommunikation zwischen Ihrer Umgebung und [!DNL Adobe Workfront Fusion].

Fügen Sie die folgenden IP-Adressen zu Ihrer Zulassungsliste hinzu, um [!DNL Workfront Fusion] auf Ihr System zugreifen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] EU-Rechenzentrum</td> 
   <td> 
    <ul> 
     <li>52 30 133 50</li> 
     <li>54 220 93 204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US-Rechenzentrum</p> </td> 
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
>Ausgehende Netzwerkfilter sind selten. Wenden Sie sich an Ihren Netzwerkadministrator, um zu sehen, ob Sie Ihre Zulassungsliste aktualisieren müssen, damit sie berücksichtigt werden kann.

Weitere Informationen zum Einrichten der Zulassungsliste für Ihr Unternehmen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
