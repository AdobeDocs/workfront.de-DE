---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen Sie neue Vorlagen in [!DNL Adobe Workfront Fusion]
description: Sie können neue Szenariovorlagen in  [!DNL Adobe] Workfront Fusion erstellen.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]

Sie können in [!DNL Adobe] Workfront Fusion neue Szenariovorlagen erstellen.

>[!TIP]
>
>Bevor Sie eine neue Vorlage erstellen, können Sie die Registerkarte [!UICONTROL Öffentliche Vorlagen] überprüfen, um sicherzustellen, dass die Vorlage, die Sie erstellen möchten, nicht bereits verfügbar ist.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
  <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Erstellen einer neuen Vorlage

Sie können eine Vorlage in einem Prozess erstellen, der dem Erstellen eines Szenarios ähnelt. Fusion-Administratoren können auch Vorlagen aus vorhandenen Szenarien erstellen.

* [Erstellen einer Vorlage](#build-a-template)
* [Erstellen einer Vorlage aus einem Szenario](#create-a-template-from-a-scenario)

### Erstellen einer Vorlage

1. Klicken Sie **[!UICONTROL linken Navigationsbereich]** Vorlagen![](assets/fusion-template-icon.png).
1. Klicken **[!UICONTROL oben]** auf „Neue Vorlage erstellen“.
1. (Optional) Benennen Sie die Vorlage um, indem Sie in **[!UICONTROL linken oberen Ecke den Standardwert]** Neuer Vorlagenname“ ersetzen.
1. (Optional) Um die Sprache Ihrer Vorlage zu ändern, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und wählen Sie die Sprache aus der Dropdown-Liste Sprache aus.

   >[!IMPORTANT]
   >
   >Die Sprachauswahl entspricht den in den Systemeinstellungen verfügbaren Sprachen und betrifft nur den Namen der öffentlichen Vorlage und deren Beschreibung. Sie können eine Vorlagensprache nicht mehr ändern, nachdem die Vorlage gespeichert wurde.

1. (Optional) Um eine Beschreibung der Vorlage einzugeben, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und geben Sie die Beschreibung ein.
1. Fügen Sie Apps, Module und Tools auf die gleiche Weise hinzu wie beim Erstellen eines Standardszenarios.

   Informationen zum Hinzufügen von kontextueller Hilfe zu den Modulen finden Sie unter [Einrichten [!UICONTROL Assistent]-Funktionalität](#set-up-wizard-functionality) in diesem Artikel.

   Weitere Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Wenn Ihre Vorlage Module enthält, für die das Hinzufügen der Verbindung, der Anmeldeinformationen oder anderer vertraulicher Informationen zum Datenschutz erforderlich ist, werden diese Informationen nicht für die Vorlagenbenutzer freigegeben.

1. (Optional) Klicken Sie auf **[!UICONTROL Einmal ausführen]** um Ihre Vorlage zu testen.
1. Klicken Sie auf **[!UICONTROL Symbol]** Speichern![](assets/save-icon.png).

>[!NOTE]
>
>Durch Speichern der Vorlage machen Sie sie für alle Team-Mitglieder sichtbar. Wenn Sie möchten, dass Ihre Vorlage außerhalb Ihres Teams zugänglich ist, müssen Sie eine Anfrage einreichen, um sie genehmigen und veröffentlichen zu lassen. Die Anfrage kommt zur Genehmigung an Adobe Workfront und sobald sie genehmigt wurde, kann auf die Vorlage von anderen Personen außerhalb Ihres Teams zugegriffen werden.
>
>Informationen zum Veröffentlichen von Vorlagen finden Sie unter [Publish und Freigabe [!DNL Adobe Workfront Fusion] Vorlagen](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Erstellen einer Vorlage aus einem Szenario

>[!NOTE]
>
>Sie müssen ein Fusion-Administrator sein, um eine Vorlage aus einem Szenario erstellen zu können.

1. Öffnen Sie die Seite mit den Szenario-Details für das Szenario, aus dem Sie ein Szenario erstellen möchten.
1. Klicken Sie auf **Admin**-Dropdown in der oberen rechten Ecke der Seite.
1. Wählen Sie **Als Vorlage klonen** aus.

   Das Szenario wird in eine neue Vorlagenseite kopiert.
1. (Optional) Benennen Sie die Vorlage um, indem Sie in **[!UICONTROL linken oberen Ecke den Standardwert]** Neuer Vorlagenname“ ersetzen.
1. (Optional) Um die Sprache Ihrer Vorlage zu ändern, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und wählen Sie die Sprache aus der Dropdown-Liste Sprache aus.

   >[!IMPORTANT]
   >
   >Die Sprachauswahl entspricht den in den Systemeinstellungen verfügbaren Sprachen und betrifft nur den Namen der öffentlichen Vorlage und deren Beschreibung. Sie können eine Vorlagensprache nicht mehr ändern, nachdem die Vorlage gespeichert wurde.

1. (Optional) Um eine Beschreibung der Vorlage einzugeben, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und geben Sie die Beschreibung ein.
1. Bearbeiten Sie Apps, Module und Tools auf die gleiche Weise wie beim Bearbeiten eines Standardszenarios.

   Informationen zum Hinzufügen von kontextueller Hilfe zu den Modulen finden Sie unter [Einrichten [!UICONTROL Assistent]-Funktionalität](#set-up-wizard-functionality) in diesem Artikel.

   >[!NOTE]
   >
   >Wenn Ihre Vorlage Module enthält, für die das Hinzufügen der Verbindung, der Anmeldeinformationen oder anderer vertraulicher Informationen zum Datenschutz erforderlich ist, werden diese Informationen nicht für die Vorlagenbenutzer freigegeben.

1. (Optional) Klicken Sie auf **[!UICONTROL Einmal ausführen]** um Ihre Vorlage zu testen.
1. Klicken Sie auf **[!UICONTROL Symbol]** Speichern![](assets/save-icon.png).

## Einrichten der [!UICONTROL Wizard]-Funktion {#set-up-wizard-functionality}

Mit [!DNL Workfront Fusion template] [!UICONTROL Assistent] können Sie zukünftigen Benutzern Ihrer Vorlage Anweisungen oder Informationen zu den spezifischen Feldern bereitstellen, die in -Modulen verwendet werden.

1. Klicken Sie auf das Modul, das der Vorlage hinzugefügt wurde, um die Felder des Moduls anzuzeigen.
1. Suchen Sie das Feld, in dem Sie [!UICONTROL Assistent]-Informationen hinzufügen möchten, und aktivieren Sie **[!UICONTROL Verwenden im Assistenten]** für dieses Feld.
1. Geben Sie die Informationen, die für die Benutzer sichtbar sein sollen, in das Feld [!UICONTROL Hilfe] ein.
1. (Optional) Damit Benutzer diesen Text bei Verwendung der Vorlage sehen können, aktivieren Sie **[!UICONTROL Als Standardwert verwenden]**.
1. Wiederholen Sie die Schritte 2-4 für jedes Feld, für das Sie Informationen bereitstellen möchten.
1. Klicken Sie auf **[!UICONTROL OK]**, um die Änderungen zu speichern und das Modul zu schließen.
