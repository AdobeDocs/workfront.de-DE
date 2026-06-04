---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: Zugreifen auf Favoriten und aktuelle Elemente über [!DNL Slack]
description: Nachdem Sie Slack installiert und  [!DNL Adobe Workfront]  haben, können Sie in Slack Ihre Workfront-Favoriten und die letzten Elemente anzeigen und auf Elemente in beiden Listen zugreifen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4bf62192-66fe-42a7-b8c0-23b7bdef45e8
TQID: https://experienceleague.adobe.com/Fqy-Tqgyza2C4STR6qD78-HsyKDiydUM1NTnzLY1-FE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 323
ht-degree: 9%

---

# Zugreifen auf Favoriten und aktuelle Elemente aus [!DNL Slack]

Nachdem Sie [!DNL Adobe Workfront for Slack] installiert und konfiguriert haben, können Sie Ihre [!UICONTROL Workfront]-Favoriten und die letzten Elemente anzeigen und in beiden Listen auf Elemente zugreifen[!DNL Slack].

Weitere Informationen zum Konfigurieren von [!DNL Workfront with Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Beliebig</p>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

Bevor Sie über [!DNL Slack] auf Ihre Favoriten und zuletzt verwendeten Elemente zugreifen können, müssen Sie Folgendes tun

* Konfigurieren von [!DNL Workfront for Slack]\
   Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Zugreifen auf Ihre [!UICONTROL Favoriten]-Liste über [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld [!UICONTROL Nachricht] ein: `/workfront favorites`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Eine Liste Ihrer Favoriten wird angezeigt.

1. (Optional) Klicken Sie auf **[!UICONTROL Mehr anzeigen]**, um weitere Favoriten aufzulisten.
1. Klicken Sie auf den Namen eines Favoriten, um ihn in [!DNL Workfront] in einer neuen Browser-Registerkarte zu öffnen.

## Zugriff auf die Liste der zuletzt verwendeten Elemente über [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] an und melden Sie sich von Slack aus bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld [!UICONTROL Nachricht] ein: `/workfront recent`

   >[!NOTE]
   >
   >Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden. Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Eine Liste Ihrer letzten Elemente wird in der Reihenfolge angezeigt, in der sie zuletzt aufgerufen wurden, wobei die letzten Elemente oben stehen. Die Elemente werden jeweils drei aufgelistet und nach Objekttyp gruppiert.\

1. (Optional) Klicken Sie auf **[!UICONTROL Mehr anzeigen]**, um die neuesten Elemente aufzulisten.
1. (Optional) Klicken Sie auf den Namen eines Elements, auf das Sie kürzlich zugegriffen haben, um es in [!DNL Workfront] in einer neuen Browser-Registerkarte zu öffnen.
