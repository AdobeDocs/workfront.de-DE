---
title: Adobe Workfront mit einer Layout-Vorlage markieren
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layout-Vorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Aufgabengebiete und Benutzende anzupassen. Dies ist besonders für Gruppen in einem großen Unternehmen nützlich, die über ein eigenes Branding verfügen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Adobe Workfront mit einer Layout-Vorlage markieren

<!--Audited: 09/2024-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in [!DNL Adobe Experience Cloud] integriert wurden.
>
> Wenn Ihre Organisation in [!DNL Adobe Experience Cloud] integriert wurde, ist kein Branding verfügbar.

Sie können eine Layout-Vorlage verwenden, um die Logos im oberen Navigationsbereich und im Hauptmenü für bestimmte Gruppen, Teams, Aufgabengebiete und Benutzer anzupassen. Dies ist besonders für Gruppen in einem großen Unternehmen nützlich, die über ein eigenes Branding verfügen.

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann die gleichen Branding-Anpassungen für das gesamte Unternehmen auf Systemebene vornehmen, wie in [Branding Ihrer Adobe Workfront-Instanz](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md) beschrieben. Das Branding in einer Layout-Vorlage überschreibt jedoch das Branding auf Systemebene.
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adobe Workfront mit einer Layout-Vorlage markieren

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie auf den Abwärtspfeil ![Abwärtspfeil](assets/dropdown-arrow.png) unter **Anpassen, was Benutzer sehen** und klicken Sie dann auf **Branding**.
1. Nehmen Sie eine der folgenden Änderungen vor, um Workfront mit Branding-Bildern für diejenigen anzupassen, denen diese Layout-Vorlage zugewiesen ist.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Markieren Sie das Symbol Startseite <span style="font-weight: normal;">(wird ganz links im oberen Navigationsbereich angezeigt)</span></p> </td> 
      <td> <p>Klicken Sie im <strong>oberen Navigationsbereich</strong> unter <strong>Startseitensymbol</strong> auf eine beliebige Stelle im Feld, suchen Sie dann nach Ihrem Logo und wählen Sie es aus. Oder ziehen Sie ein Bild in das Feld.</p> <p>Um das Bild zu beschneiden, verwenden Sie die Steuerelemente zum Scrollen und ziehen Sie das Bild an die gewünschte Position innerhalb des vorgeschriebenen Bereichs.</p> <p>Wir empfehlen ein 120 x 120 Bild. Es kann in einem der folgenden Formate vorliegen: GIF, JPG, PNG, SVG.</p> <p>Dieses Symbol wird auch in Berichten, Listen, Dashboards und bereitgestellten Berichten angezeigt, die Benutzende als PDF-Dateien exportieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Branding des Hauptmenüs <img src="assets/main-menu-icon.png"> Logo-<span style="font-weight: normal;"> (wird in der oberen rechten Ecke des Hauptmenüs angezeigt)</span></p> </td> 
      <td> <p> <p> <p>Klicken Sie im <strong>oberen Navigationsbereich</strong> unter <strong>Hauptmenü-Logo</strong> auf eine beliebige Stelle im Feld, suchen Sie nach Ihrem Logo und wählen Sie es aus. Oder ziehen Sie ein Bild in das Feld.</p> <p>Um das Bild zu beschneiden, verwenden Sie die Steuerelemente zum Scrollen und ziehen Sie das Bild an die gewünschte Position innerhalb des vorgeschriebenen Bereichs.</p> <p>Wir empfehlen ein Bild in der Größe 300 x 120 Pixel. Es kann in einem der folgenden Formate vorliegen: GIF, JPG, PNG, SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um Ihren Fortschritt zu speichern, und dann später mit dem Ändern der Vorlage fortfahren.

1. Klicken Sie auf **Speichern**.

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
