---
title: Löschen klassischer Layoutvorlagen
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Layout-Vorlagen aus dem klassischen Workfront-Erlebnis sind nicht mehr in der Workfront-Benutzeroberfläche verfügbar, können sich aber dennoch auf Workfront-Daten auswirken. Dies kann zu Inkonsistenzen in Feldern führen, die von Layout-Vorlagen (z. B. „Freigegeben für“) in Berichten oder Dashboards betroffen sind.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 51%

---

# Administratorzugriff für eine Layoutvorlage gewähren

Layout-Vorlagen aus dem klassischen Workfront-Erlebnis sind nicht mehr in der Workfront-Benutzeroberfläche verfügbar, können sich aber dennoch auf Workfront-Daten auswirken. Dies kann zu Inkonsistenzen in Feldern führen, die von Layout-Vorlagen (z. B. „Freigegeben für“) in Berichten oder Dashboards betroffen sind.

Sie können diese Inkonsistenzen beheben, indem Sie die klassischen Layoutvorlagen löschen. Da sie nicht in der Workfront-Benutzeroberfläche verfügbar sind, müssen Sie die Workfront-API verwenden, um sie zu löschen.

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen Sie die klassischen Layoutvorlagen mithilfe eines API-Aufrufs

Sie können API-Aufrufe in die URL-Leiste Ihres Browsers eingeben und die Eingabetaste drücken. Die API-Antwort wird in Ihrem Browser angezeigt.

>[!NOTE]
>
>Vorlagen für globale und System-Layouts können nicht gelöscht werden.

1. Melden Sie sich bei Workfront an.
1. Suchen Sie die Layout-Vorlage, die Sie löschen möchten, mithilfe des folgenden API-Aufrufs:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Notieren Sie sich die ID der Layout-Vorlage, die Sie löschen möchten.
1. Suchen Sie Ihre Sitzungs-ID mithilfe des folgenden API-Aufrufs:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Geben Sie Ihre Sitzungs-ID niemals an andere weiter.

1. Fügen Sie die Layout-Vorlagen-ID und die Sitzungs-ID in den folgenden API-Aufruf ein:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Fügen Sie den API-Aufruf aus Schritt 4 in die URL-Leiste Ihres Browsers ein und drücken Sie die Eingabetaste.

   Dadurch wird die Layout-Vorlage gelöscht.
