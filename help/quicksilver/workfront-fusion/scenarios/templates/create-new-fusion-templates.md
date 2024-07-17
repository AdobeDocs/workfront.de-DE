---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]
description: Sie können in der Workfront-Fusion neue Szenario-Vorlagen erstellen. [!DNL Adobe]
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]

Sie können neue Szenario-Vorlagen in [!DNL Adobe] Workfront Fusion erstellen.

>[!TIP]
>
>Bevor Sie eine neue Vorlage erstellen, können Sie die Registerkarte [!UICONTROL Öffentliche Vorlagen] aktivieren, um sicherzustellen, dass die Vorlage, die Sie erstellen möchten, noch nicht verfügbar ist.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
  <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Neue Vorlage erstellen

Sie können eine Vorlage in einem Prozess erstellen, der dem Erstellen eines Szenarios ähnelt. Fusion-Administratoren können auch Vorlagen aus vorhandenen Szenarien erstellen.

* [Erstellen einer Vorlage](#build-a-template)
* [Erstellen einer Vorlage aus einem Szenario](#create-a-template-from-a-scenario)

### Erstellen einer Vorlage

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Vorlagen]** ![](assets/fusion-template-icon.png) .
1. Klicken Sie oben rechts auf **[!UICONTROL Neue Vorlage erstellen]** .
1. (Optional) Benennen Sie die Vorlage um, indem Sie den standardmäßigen **[!UICONTROL neuen Vorlagennamen]** oben links ersetzen.
1. (Optional) Klicken Sie zum Ändern der Sprache Ihrer Vorlage auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und wählen Sie die Sprache aus der Dropdown-Liste Sprache aus.

   >[!IMPORTANT]
   >
   >Die Auswahl Sprachen entspricht den in den Systemeinstellungen verfügbaren Sprachen und betrifft nur den Namen der öffentlichen Vorlage und deren Beschreibung. Eine Vorlagensprache kann nach dem Speichern der Vorlage nicht mehr geändert werden.

1. (Optional) Um eine Beschreibung der Vorlage einzugeben, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und geben Sie die Beschreibung ein.
1. Fügen Sie Apps, Module und Tools auf die gleiche Weise hinzu wie beim Erstellen eines Standardszenarios.

   Informationen zum Hinzufügen von kontextueller Hilfe zu den Modulen finden Sie unter [Einrichten der Funktion [!UICONTROL Assistent]](#set-up-wizard-functionality) in diesem Artikel.

   Weitere Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in  [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Wenn Ihre Vorlage Module enthält, die das Hinzufügen der Verbindung, der Anmeldeinformationen oder anderer vertraulicher Informationen erfordern, werden diese Informationen nicht für die Vorlagenbenutzer freigegeben.

1. (Optional) Klicken Sie auf **[!UICONTROL Einmal ausführen]** , um Ihre Vorlage zu testen.
1. Klicken Sie auf das Symbol **[!UICONTROL Speichern]** ![](assets/save-icon.png).

>[!NOTE]
>
>Durch das Speichern Ihrer Vorlage wird sie für alle Teammitglieder sichtbar. Wenn Sie möchten, dass Ihre Vorlage außerhalb Ihres Teams zugänglich ist, müssen Sie eine Anfrage zur Genehmigung und Veröffentlichung senden. Die Anfrage wird zur Genehmigung an Adobe Workfront gesendet. Sobald sie genehmigt wurde, kann die Vorlage von anderen Benutzern außerhalb Ihres Teams verwendet werden.
>
>Informationen zu Veröffentlichungsvorlagen finden Sie unter [Publish und share [!DNL Adobe Workfront Fusion] templates](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Erstellen einer Vorlage aus einem Szenario

>[!NOTE]
>
>Sie müssen Fusion-Administrator sein, um eine Vorlage aus einem Szenario zu erstellen.

1. Öffnen Sie die Seite mit den Szenario-Details für das Szenario, aus dem Sie ein Szenario erstellen möchten.
1. Klicken Sie oben rechts auf der Seite auf das Dropdown-Menü **Admin** .
1. Wählen Sie **Als Vorlage klonen** aus.

   Das Szenario wird in eine Seite &quot;Neue Vorlage&quot;kopiert.
1. (Optional) Benennen Sie die Vorlage um, indem Sie den standardmäßigen **[!UICONTROL neuen Vorlagennamen]** oben links ersetzen.
1. (Optional) Klicken Sie zum Ändern der Sprache Ihrer Vorlage auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und wählen Sie die Sprache aus der Dropdown-Liste Sprache aus.

   >[!IMPORTANT]
   >
   >Die Auswahl Sprachen entspricht den in den Systemeinstellungen verfügbaren Sprachen und betrifft nur den Namen der öffentlichen Vorlage und deren Beschreibung. Eine Vorlagensprache kann nach dem Speichern der Vorlage nicht mehr geändert werden.

1. (Optional) Um eine Beschreibung der Vorlage einzugeben, klicken Sie auf **[!UICONTROL Vorlage einrichten]** ![](assets/fusion-scenario-settings-icon.png) und geben Sie die Beschreibung ein.
1. Bearbeiten Sie Apps, Module und Tools auf dieselbe Weise wie beim Bearbeiten eines Standardszenarios.

   Informationen zum Hinzufügen von kontextueller Hilfe zu den Modulen finden Sie unter [Einrichten der Funktion [!UICONTROL Assistent]](#set-up-wizard-functionality) in diesem Artikel.

   >[!NOTE]
   >
   >Wenn Ihre Vorlage Module enthält, die das Hinzufügen der Verbindung, der Anmeldeinformationen oder anderer vertraulicher Informationen erfordern, werden diese Informationen nicht für die Vorlagenbenutzer freigegeben.

1. (Optional) Klicken Sie auf **[!UICONTROL Einmal ausführen]** , um Ihre Vorlage zu testen.
1. Klicken Sie auf das Symbol **[!UICONTROL Speichern]** ![](assets/save-icon.png).

## Einrichten der Funktion [!UICONTROL Assistent] {#set-up-wizard-functionality}

Mit dem [!DNL Workfront Fusion template] [!UICONTROL Assistenten] können Sie künftigen Benutzern Ihrer Vorlage Anweisungen oder Informationen zu den spezifischen Feldern bereitstellen, die in Modulen verwendet werden.

1. Klicken Sie auf das Modul, das der Vorlage hinzugefügt wurde, um die Felder des Moduls anzuzeigen.
1. Suchen Sie das Feld, in das Sie Informationen zum [!UICONTROL Assistenten] hinzufügen möchten, und aktivieren Sie für dieses Feld die Option **[!UICONTROL Im Assistenten verwenden]** .
1. Geben Sie die Informationen, die Sie für Benutzer sichtbar machen möchten, in das Feld [!UICONTROL Hilfe] ein.
1. (Optional) Damit Benutzer diesen Text bei Verwendung der Vorlage sehen können, aktivieren Sie **[!UICONTROL Als Standardwert verwenden]**.
1. Wiederholen Sie die Schritte 2 bis 4 für jedes Feld, für das Sie Informationen bereitstellen möchten.
1. Klicken Sie auf **[!UICONTROL OK]** , um die Änderungen zu speichern und das Modul zu schließen.
