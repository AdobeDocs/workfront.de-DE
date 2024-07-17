---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Verhindern des Spoofens und Hinzufügen von [!DNL Adobe Workfront] SPF-Datensätzen
description: Wenn Benutzer keine [!DNL Adobe Workfront] E-Mail-Benachrichtigungen erhalten, müssen Sie Ihrer Firewall  [!DNL Workfront] SPF-Einträge hinzufügen. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Einträge hinzuzufügen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Verhindern Sie das Spoofing und fügen Sie [!DNL Adobe Workfront] SPF-Datensätze hinzu

## Problem

Wenn Benutzer keine [!DNL Adobe Workfront] E-Mail-Benachrichtigungen erhalten, müssen Sie Ihrer Firewall [!DNL Workfront] SPF-Einträge hinzufügen. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Einträge hinzuzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Wenn Sie die IP-Adressen bereits zu Ihrer Zulassungsliste für Ihre Produktionsumgebung hinzugefügt haben, wie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) beschrieben, und Benutzer weiterhin keine E-Mails erhalten:

1. Fügen Sie Ihrer Firewall den folgenden SPF-Eintrag hinzu:

   *spf.workfront.com*

   Dadurch werden automatisch alle [!DNL Workfront] IP-Adressen zu Ihrer Zulassungsliste in Ihrer Firewall hinzugefügt und alle Spamfilter (die SPF-Einträge verwenden) können [!DNL Workfront]-Server als gültige Absender für Ihre Domäne validieren.

   >[!NOTE]
   >
   > Ein SPF-Eintrag ist ein TXT-Eintrag, der Teil einer DNS-Zone-Datei ist. Das Ändern der DNS-Zonendatei wird nicht unterstützt.

1. Sie müssen angeben, welcher Typ von SPF-Datensatz konfiguriert werden muss. Dies sind die gültigen Typen von SPF-Datensätzen:

   * all (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * exists (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Beispiel: &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Wenn Sie aufgrund von Unternehmensrichtlinien keine SPF-Einträge zu Ihrer Firewall hinzufügen können, wenden Sie sich an Ihren Support-Mitarbeiter für [!DNL Workfront] .
