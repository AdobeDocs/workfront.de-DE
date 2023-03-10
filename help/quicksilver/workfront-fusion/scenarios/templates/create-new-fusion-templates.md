---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]
description: Sie können neue Szenario-Vorlagen in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Erstellen neuer Vorlagen in [!DNL Adobe Workfront Fusion]

Sie können neue Szenario-Vorlagen in [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Vor der Erstellung einer neuen Vorlage können Sie die [!UICONTROL Öffentliche Vorlagen] um sicherzustellen, dass die Vorlage, die Sie erstellen möchten, nicht bereits verfügbar ist.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Neue Vorlage erstellen

1. Klicken **[!UICONTROL Vorlagen]** ![](assets/fusion-template-icon.png) im linken Navigationsbereich.
1. Klicken **[!UICONTROL Neue Vorlage erstellen]** in der oberen rechten Ecke.
1. (Optional) Benennen Sie die Vorlage um, indem Sie die Standardeinstellung ersetzen. **[!UICONTROL Neuer Vorlagenname]** in der oberen linken Ecke.
1. (Optional) Um die Sprache Ihrer Vorlage zu ändern, klicken Sie auf **[!UICONTROL Einrichten einer Vorlage]** ![](assets/fusion-scenario-settings-icon.png) und wählen Sie die Sprache aus der Dropdown-Liste Sprache aus.

   >[!IMPORTANT]
   >
   >Die Auswahl Sprachen entspricht den in den Systemeinstellungen verfügbaren Sprachen und betrifft nur den Namen der öffentlichen Vorlage und deren Beschreibung. Eine Vorlagensprache kann nach dem Speichern der Vorlage nicht mehr geändert werden.

1. (Optional) Um eine Beschreibung der Vorlage einzugeben, klicken Sie auf **[!UICONTROL Einrichten einer Vorlage]** ![](assets/fusion-scenario-settings-icon.png) und geben Sie die Beschreibung ein.
1. Fügen Sie Apps, Module und Tools auf die gleiche Weise hinzu wie beim Erstellen eines Standardszenarios.

   Informationen zum Hinzufügen der kontextuellen Hilfe zu den Modulen finden Sie unter [Einrichten [!UICONTROL Assistent] Funktion](#set-up-wizard-functionality) in diesem Artikel.

   Weitere Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Wenn Ihre Vorlage Module enthält, die das Hinzufügen der Verbindung, der Anmeldeinformationen oder anderer vertraulicher Informationen erfordern, werden diese Informationen nicht für die Vorlagenbenutzer freigegeben.

1. (Optional) Klicken Sie auf **[!UICONTROL Einmal ausführen]** , um Ihre Vorlage zu testen.
1. Klicken Sie auf **[!UICONTROL Speichern]** icon ![](assets/save-icon.png).

>[!NOTE]
>
>Durch das Speichern Ihrer Vorlage wird sie für alle Teammitglieder sichtbar. Wenn Sie möchten, dass Ihre Vorlage außerhalb Ihres Teams zugänglich ist, müssen Sie sie veröffentlichen und dann einen freigegebenen Link verwenden oder Ihren Administrator bitten, die Vorlage zu genehmigen und zu veröffentlichen.

## Einrichten [!UICONTROL Assistent] Funktion {#set-up-wizard-functionality}

Die [!DNL Workfront Fusion template] [!UICONTROL Assistent] ermöglicht es Ihnen, künftigen Benutzern Ihrer Vorlage Anweisungen oder Informationen zu den in Modulen verwendeten Feldern bereitzustellen.

1. Klicken Sie auf das Modul, das der Vorlage hinzugefügt wurde, um die Felder des Moduls anzuzeigen.
1. Suchen Sie das Feld, dem Sie hinzufügen möchten [!UICONTROL Assistent] und aktivieren Sie **[!UICONTROL Verwenden des Assistenten]** für dieses Feld.
1. Geben Sie die Informationen ein, die Sie für Benutzer sichtbar machen möchten, in die [!UICONTROL Hilfe] -Feld.
1. (Optional) Wenn Benutzer diesen Text bei Verwendung der Vorlage sehen können, aktivieren Sie **[!UICONTROL Use as default value]**.
1. Wiederholen Sie die Schritte 2 bis 4 für jedes Feld, für das Sie Informationen bereitstellen möchten.
1. Klicken **[!UICONTROL OK]** , um Änderungen zu speichern und das Modul zu schließen.
