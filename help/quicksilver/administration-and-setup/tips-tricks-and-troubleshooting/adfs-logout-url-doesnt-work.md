---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS-Abmelde-URL funktioniert nicht
description: Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in der Adobe Admin Console integriert sind.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# ADFS-Abmelde-URL funktioniert nicht

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die [!UICONTROL Adobe Admin Console].
>
>Wenn Ihr Unternehmen bei der [!UICONTROL Adobe Admin Console], siehe [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problem

Bei Verwendung der ADFS-Abmelde-URL (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0) erhalten Sie eine Meldungsseite mit dem Fehler: &quot;Beim Zugriff auf die Site ist ein Problem aufgetreten. Versuchen Sie, die Site erneut zu besuchen.&quot;

Wenn das Problem weiterhin besteht, wenden Sie sich an den Administrator dieser Website und geben Sie die folgende Referenznummer an, um das Problem zu identifizieren: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] Lizenz</td> 
   <td> 
   <p>Neu: Standard</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Wechseln Sie in Ihrem ADFS-Manager-Server zu **[!UICONTROL Vertrauensbeziehungen]** > **[!UICONTROL Vertrauen in Partei]** > `<your party trust>` Eigenschaften.

1. Unter dem **[!UICONTROL Endpunkte]** Registerkarte, klicken **[!UICONTROL Hinzufügen]**.

1. **[!UICONTROL Endpunkttyp]** = SAML-Abmeldung, Bindung = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Sie können eine Antwort-URL festlegen, wenn Sie möchten, dass sie zu einer anderen Seite umgeleitet wird. Wir empfehlen jedoch die ADFS-Website, da sie warnt, dass Sie abgemeldet sind, Sie sollten jedoch weiterhin Ihren Browser schließen.
