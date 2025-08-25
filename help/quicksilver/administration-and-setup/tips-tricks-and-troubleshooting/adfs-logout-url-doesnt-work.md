---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS-Abmelde-URL funktioniert nicht
description: Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Adobe Admin Console integriert haben.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 1%

---

# ADFS-Abmelde-URL funktioniert nicht

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die [!UICONTROL Adobe Admin Console integriert &#x200B;].
>
>Wenn Ihre Organisation das Onboarding für die [!UICONTROL Adobe Admin Console] durchgeführt hat, lesen Sie den Abschnitt [Unterschiede bei der plattformbasierten Administration ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

Bei Verwendung der ADFS-Abmelde-URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) erhalten Sie eine Nachrichtenseite mit dem Fehler: „Beim Zugriff auf die Website ist ein Problem aufgetreten. Versuchen Sie erneut, auf die Website zuzugreifen.“

Wenn das Problem weiterhin besteht, wenden Sie sich an den Administrator dieser Website und geben Sie die folgende Referenznummer an, um das Problem zu identifizieren: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] License</td> 
   <td> 
   <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>  
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Wechseln Sie auf Ihrem ADFS-Manager-Server zu **[!UICONTROL Vertrauensstellungen]** > **[!UICONTROL Vertrauensstellungen von vertrauenden Parteien]** > `<your party trust>`.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Endpunkte“ auf **[!UICONTROL Hinzufügen]**.

1. **[!UICONTROL Endpunkttyp]** = SAML-Abmeldung, Bindung = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Sie können eine Antwort-URL festlegen, wenn Sie sie auf eine andere Seite umleiten möchten. Wir empfehlen jedoch die ADFS-Website, da sie Sie warnt, dass Sie abgemeldet sind, aber Sie sollten dennoch Ihren Browser schließen.
