---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Spoofing und Add-SPF [!DNL Adobe Workfront] Einträge verhindern
description: Wenn Benutzer keine E [!DNL Adobe Workfront] Mail-Benachrichtigungen erhalten, müssen Sie  [!DNL Workfront] -SPF-Einträge zu Ihrer Firewall hinzufügen. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Datensätze hinzuzufügen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# Spoofing verhindern und [!DNL Adobe Workfront] SPF-Datensätze hinzufügen

## Problem

Wenn Benutzer keine [!DNL Adobe Workfront]-E-Mail-Benachrichtigungen erhalten, müssen Sie [!DNL Workfront] SPF-Einträge zu Ihrer Firewall hinzufügen. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Datensätze hinzuzufügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

Wenn Sie bereits die IP-Adressen Ihrer für Ihre Produktionsumgebung hinzugefügt haben, wie unter [Konfigurieren der-Zulassungsliste auf die Zulassungsliste setzte Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md), und Benutzer immer noch keine E-Mails erhalten:

1. Fügen Sie der Firewall den folgenden SPF-Eintrag hinzu:

   *spf.workfront.com*

   Auf die Zulassungsliste setzen Dadurch werden automatisch alle [!DNL Workfront] IP-Adressen zu Ihrer in Ihrer Firewall hinzugefügt und alle Spam-Filter (die SPF-Einträge verwenden) können [!DNL Workfront] Server als gültige Absender für Ihre Domain validieren.

   >[!NOTE]
   >
   > Ein SPF-Eintrag ist ein TXT-Eintrag, der Teil einer DNS-Zonendatei ist. Wir unterstützen nicht die Änderung Ihrer DNS-Zonendatei.

1. Sie müssen angeben, welcher Typ von SPF-Eintrag konfiguriert werden muss. Dies sind die gültigen Typen von SPF-Einträgen:

   * Alle (https://dmarcian.com/spf-syntax-table/#all)
   * IP4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * IP6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * A (https://dmarcian.com/spf-syntax-table/#a)
   * MX (https://dmarcian.com/spf-syntax-table/#mx)
   * PTR (https://dmarcian.com/spf-syntax-table/#ptr)
   * existiert (https://dmarcian.com/spf-syntax-table/#exists)
   * Include (https://dmarcian.com/spf-syntax-table/#include)

   Beispiel: „v=spf1 a mx include: spf.workfront.com -all“

Wenn Sie aufgrund von Unternehmensrichtlinien keine SPF-Datensätze zu Ihrer Firewall hinzufügen können, wenden Sie sich bitte an Ihren [!DNL Workfront] Support-Mitarbeiter.
