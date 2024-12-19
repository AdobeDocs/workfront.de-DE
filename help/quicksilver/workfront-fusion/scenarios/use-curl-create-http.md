---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwenden von cURL zum Hinzufügen eines HTTP-Moduls
description: Sie können eine cURL-Anfrage in Ihr Szenario einfügen, und Fusion erstellt ein HTTP-Modul, das aus der cURL-Anfrage konfiguriert ist.
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 785f39fabcb19233fd1bc79c14222225a3ea72a2
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 1%

---

# Verwenden von cURL zum Hinzufügen eines HTTP-Moduls

Sie können eine cURL-Anfrage in Ihr Szenario einfügen, und Fusion erstellt ein HTTP-Modul, das aus der cURL-Anfrage konfiguriert ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-Plan</td>  
      <td>Beliebig</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-Lizenz</td>  
      <td>
        Neu: Standard<br>
        Oder<br>
        Aktuell: Arbeit oder höher
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-Lizenz</td>  
      <td> 
        Aktuell: Keine Workfront Fusion-Lizenzanforderung.<br>
        Oder<br>
        Legacy: Beliebig
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Neu: Wählen Sie oder Prime Workfront Plan: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.<br>
        Ultimate Workfront Plan: Workfront Fusion ist enthalten.<br>
        Oder<br>
        Aktuell: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.
      </td>  
    </tr> 
  </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Erstellen eines HTTP-Moduls aus einer cURL-Anfrage


So erstellen Sie ein HTTP-Modul mit cURL:

1. Erstellen Sie den Text der cURL-Anfrage außerhalb von Fusion, z. B. in einem Texteditor.
1. Kopieren Sie die cURL-Anfrage in die Zwischenablage.
1. Klicken Sie auf **[!UICONTROL Registerkarte]** Szenario“ im linken Bedienfeld.
1. Wählen Sie das Szenario aus, in dem Sie das Modul erstellen möchten.
1. Klicken Sie auf eine beliebige Stelle im Szenario, um den Szenario-Editor aufzurufen.
1. Klicken Sie mit der rechten Maustaste auf eine beliebige Leerstelle im Szenario-Editor und wählen Sie **Einfügen**.

   Oder

   Drücken Sie Strg+V (Windows) oder Befehl+V (Mac).


   Ein HTML-Modul wird erstellt.
1. Ziehen Sie das Modul, um es mit Ihrem Szenario zu verbinden.

## Fehlerbehebung

Wenn Ihre cURL nicht in Ihr Szenario eingefügt wird, überprüfen Sie Ihre Browser-Einstellungen, um sicherzustellen, dass das Einfügen aus der Zwischenablage aktiviert ist.


