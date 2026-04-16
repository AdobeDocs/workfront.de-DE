---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Änderungen der Push-Rate an Projekten
description: Eine Tarifkarte stellt die vertragliche Vereinbarung mit Ihrem Kunden dar, in der Stundensätze für die Aufgabengebiete definiert sind, die die Arbeit abschließen. In einer Tarifkarte können Sie mehrere Abrechnungssätze pro Aufgabengebiet basierend auf Attributen definieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 10%

---

# Änderungen der Push-Rate an Projekten

Wenn eine Tarifkarte an eine <!--or a staffing plan--> angehängt wird, können die Tarife auf der Tarifkarte weiterhin angepasst werden. Anschließend können Sie diese Tarife optional an die Projekte pushen, <!--and staffing plans --> denen die Tarifkarte angehängt ist. Wenn Sie die neuen Sätze nicht überweisen, bleiben die ursprünglichen Sätze im Projekt<!-- or staffing plan-->.

Informationen zum Anhängen einer Tarifkarte an ein Projekt finden Sie unter [Anhängen einer Tarifkarte an ein Projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf [!UICONTROL Rate Cards] bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Um eine Tarifkarte zu bearbeiten, die für Sie freigegeben wurde, müssen Sie über Verwaltungsberechtigungen für die Tarifkarte verfügen.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Änderungen der Push-Rate an Projekten

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf [!UICONTROL **Tarifkarten**].
1. Klicken Sie auf den Namen der Tarifkarte in der Liste Tarifkarten .
1. Überprüfen Sie auf dem Bildschirm Tarifkarte > Aufgabengebiete und Tarife, ob die Tarife korrekt sind, und bearbeiten Sie die Tarife nach Bedarf.
1. Klicken Sie [!UICONTROL **Änderungen per Push übertragen**].
1. Im Dialogfeld [!UICONTROL **Auf alle Projekte anwenden**]<!--/staffing plans--> werden alle Projekte <!--and staffing plans -->die diese Tarifkarte verwenden) standardmäßig ausgewählt. Wenn Sie nicht möchten, dass ein Projekt <!--or staffing plan -->die Tarifänderungen anwendet, müssen Sie die Auswahl aufheben.
1. Klicken Sie auf [!UICONTROL **Speichern**].

   Die neuen Tarife spiegeln sich nun in den Projekten wider<!--and staffing plans --> die die Tarifkarte verwenden.
