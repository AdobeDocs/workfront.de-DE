---
title: Brand Adobe Workfront mit einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Rollen und Benutzer anzupassen. Dies ist besonders für Gruppen in einer großen Organisation nützlich, die über ein eigenes Branding verfügen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Brand Adobe Workfront mit einer Layoutvorlage

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht integriert sind in [!DNL Adobe Experience Cloud].
>
> Wenn Ihr Unternehmen bei [!DNL Adobe Experience Cloud], ist das Branding nicht verfügbar.

Sie können eine Layoutvorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Rollen und Benutzer anzupassen. Dies ist besonders für Gruppen in einer großen Organisation nützlich, die über ein eigenes Branding verfügen.

Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann dieselben Branding-Anpassungen für das gesamte Unternehmen auf Systemebene vornehmen, wie hier beschrieben: [Markieren Sie Ihre Adobe Workfront-Instanz.](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md). Das Branding in einer Layoutvorlage setzt jedoch das Branding auf Systemebene außer Kraft.
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Brand Adobe Workfront mit einer Layoutvorlage

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicken Sie auf den Abwärtspfeil. ![](assets/dropdown-arrow.png) under **Anpassen der Ansicht von Benutzern** Klicken Sie auf **Branding**.
1. Nehmen Sie eine der folgenden Änderungen vor, um Workfront mit Branding-Bildern für diejenigen anzupassen, denen diese Layoutvorlage zugewiesen ist.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Markieren des Startseiten-Symbols <span style="font-weight: normal;">(wird ganz links im oberen Navigationsbereich angezeigt)</span></p> </td> 
      <td> <p>Im <strong>Navigationsbereich oben</strong> Abschnitt <strong>Startseite</strong>, klicken Sie auf eine beliebige Stelle im Feld, suchen und wählen Sie dann Ihr Logo-Bild aus. Oder ziehen Sie ein Bild in das Feld.</p> <p>Um das Bild zu beschneiden, verwenden Sie die Scroll-Steuerelemente und ziehen Sie das Bild an die gewünschte Position innerhalb des vorgeschriebenen Bereichs.</p> <p>Wir empfehlen ein Bild im Format 120 x 120. Sie kann in einem der folgenden Formate vorliegen: GIF, JPG, PNG, SVG.</p> <p>Dieses Symbol wird auch in Berichten, Listen, Dashboards und bereitgestellten Berichten angezeigt, die Benutzer als PDF-Dateien exportieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Marke des Hauptmenüs <img src="assets/main-menu-icon.png"> logo <span style="font-weight: normal;">(wird in der oberen rechten Ecke des Hauptmenüs angezeigt)</span></p> </td> 
      <td> <p> <p> <p>Im <strong>Navigationsbereich oben</strong> Abschnitt <strong>Hauptmenü-Logo</strong>, klicken Sie auf eine beliebige Stelle im Feld, suchen und wählen Sie dann Ihr Logo-Bild aus. Oder ziehen Sie ein Bild in das Feld.</p> <p>Um das Bild zu beschneiden, verwenden Sie die Scroll-Steuerelemente und ziehen Sie das Bild an die gewünschte Position innerhalb des vorgeschriebenen Bereichs.</p> <p>Wir empfehlen ein 300 x 120 Pixelbild. Sie kann in einem der folgenden Formate vorliegen: GIF, JPG, PNG, SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.

1. Klicken Sie auf **Speichern**.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
