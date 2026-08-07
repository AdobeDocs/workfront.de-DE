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
source-git-commit: 22e8acb748ddc4768dc1724aaa2f515b863ab0cf
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 8%

---

# Änderungen der Push-Rate an Projekten

Wenn einem Projekt eine Tarifkarte beigefügt ist<!--or a staffing plan--> können die Tarife auf der Tarifkarte dennoch angepasst werden. Anschließend können Sie diese Tarife optional an die Projekte weiterleiten, an die die Tarifkarte angehängt ist. Wenn Sie die neuen Sätze nicht nach oben verschieben, bleiben die ursprünglichen Sätze im Projekt erhalten.
<!-- and staffing plans -->
<!-- or staffing plan -->

>[!NOTE]
>
>Wenn ein Aufgabengebiet oder ein Benutzer-Abrechnungssatz auf Projektebene manuell überschrieben wird, bleibt dieser Satz im Projekt, wenn die Tarifkartenänderungen an das Projekt übertragen werden. Nur die mit der Tarifkarte verknüpften Tarife werden aktualisiert.

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
