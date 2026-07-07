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
source-git-commit: d645aeb9d2d49432b49b6f2e2c4748f50075c42b
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 9%

---

# Änderungen der Push-Rate an Projekten

Wenn eine Tarifkarte an eine <!--or a staffing plan--> angehängt wird, können die Tarife auf der Tarifkarte weiterhin angepasst werden. Anschließend können Sie diese Tarife optional an die Projekte weiterleiten, an die die Tarifkarte angehängt ist. Wenn Sie die neuen Sätze nicht nach oben verschieben, bleiben die ursprünglichen Sätze im Projekt erhalten.
<!-- and staffing plans -->
<!-- or staffing plan -->

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
1. Im Dialogfeld [!UICONTROL **Auf alle Projekte anwenden**] werden alle Projekte, die diese Tarifkarte verwenden, standardmäßig ausgewählt. Wenn Sie nicht möchten, dass ein Projekt die Tarifänderungen anwendet, müssen Sie die Auswahl aufheben.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

   >[!NOTE]
   >
   >Im Dialogfeld werden nur Projekte mit veralteten Tarifen angezeigt. Wenn ein Projekt diese Tarifkarte verwendet und die Preise für das Projekt aktuell sind, wird sie nicht angezeigt.

1. Klicken Sie auf [!UICONTROL **Speichern**].

   Die neuen Tarife spiegeln sich nun in den Projekten wider<!--and staffing plans --> die die Tarifkarte verwenden.
