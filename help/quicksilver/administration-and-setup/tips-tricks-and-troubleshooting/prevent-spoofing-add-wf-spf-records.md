---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Verhindern Sie das Spoofing und fügen Sie [!DNL Adobe Workfront] SPF-Datensätze
description: Wenn Benutzer keine [!DNL Adobe Workfront] E-Mail-Benachrichtigungen hinzufügen [!DNL Workfront] SPF registriert Ihre Firewall. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Einträge hinzuzufügen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Verhindern Sie das Spoofing und fügen Sie [!DNL Adobe Workfront] SPF-Datensätze

## Problem

Wenn Benutzer keine [!DNL Adobe Workfront] E-Mail-Benachrichtigungen hinzufügen [!DNL Workfront] SPF registriert Ihre Firewall. Sie müssen mit Ihrem IT-Team zusammenarbeiten, um SPF-Einträge hinzuzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Wenn Sie die IP-Adressen bereits zu Ihrer Zulassungsliste für Ihre Produktionsumgebung hinzugefügt haben, wie hier beschrieben: [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) und die Benutzer immer noch keine E-Mails erhalten:

1. Fügen Sie Ihrer Firewall den folgenden SPF-Eintrag hinzu:

   *spf.workfront.com*

   Dadurch werden automatisch alle [!DNL Workfront] IP-Adressen auf Ihre Zulassungsliste in Ihrer Firewall und ermöglichen es allen Spamfiltern (die SPF-Einträge verwenden), zu validieren [!DNL Workfront] -Server als gültige Absender für Ihre Domäne.

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

   Beispiel: &quot;v=spf1 a mx: [spf.workfront.com](http://spf.workfront.com/) -all&quot;

Wenn Sie aufgrund von Unternehmensrichtlinien keine SPF-Einträge zu Ihrer Firewall hinzufügen können, wenden Sie sich an Ihre [!DNL Workfront] Support-Mitarbeiter.
