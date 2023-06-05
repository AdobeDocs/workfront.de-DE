---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verwalten gesperrter Szenarien in [!DNL Adobe Workfront Fusion]
description: Verwalten gesperrter Szenarien in [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 014434dc-7548-42d1-bacd-89ddf627b647
source-git-commit: 9050684504f2335f5631f63978a9f65c25fd8d5f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Verwalten gesperrter Szenarien in [!DNL Adobe Workfront Fusion]

In einigen Fällen ist ein Szenario möglicherweise vorübergehend gesperrt in [!DNL Workfront Fusion]. Gesperrte Ausführungen werden automatisch innerhalb von 2-4 Stunden entsperrt. Sie können Szenarien auch manuell entsperren.

>[!IMPORTANT]
>
>Das manuelle Entsperren eines Szenarios kann bei den Ausführungen eines Szenarios zu Fehlern führen.

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

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Grundlegendes zu gesperrten Szenarien

Szenarien können aus verschiedenen Gründen gesperrt werden.

Workfront Fusion unterstützt keine parallele Verarbeitung geplanter Szenarien. Diese Szenarien werden zu Beginn der Szenario-Ausführung gesperrt und nach Abschluss entsperrt. Wenn die Ausführung unterbrochen wird, wird das Szenario möglicherweise nicht entsperrt. Dies kann vorkommen, wenn ein Benutzer das Szenario manuell erzwingt oder ein Systemproblem vorliegt.

Darüber hinaus kann das Workfront Fusion Engineering-Team ein Szenario sperren, da es Leistungs- oder andere Probleme verursacht.

Unabhängig von der Ursache eines gesperrten Szenarios wird das Szenario 2-4 Stunden nach seiner Sperrung automatisch entsperrt.

## Sperrszenario entsperren

Gesperrte Szenarien werden 2-4 Stunden nach der Sperrung entsperrt. Sie können ein Szenario manuell entsperren, bevor es automatisch entsperrt werden soll.

Das manuelle Entsperren eines Szenarios kann bei den Ausführungen eines Szenarios zu Fehlern führen. Es wird empfohlen, Szenarien nur dann manuell zu entsperren, wenn ein Szenario aufgrund der Ausführung und Beendigung von Ausführungen im Rahmen des Designs des Szenarios gesperrt ist. Unter anderen Umständen empfehlen wir, auf die automatische Entsperrung des Szenarios zu warten.

>[!IMPORTANT]
>
>Das manuelle Entsperren eines Szenarios kann bei den Ausführungen eines Szenarios zu Fehlern führen.

1. Rufen Sie die Seite mit den Szenario-Details des gesperrten Szenarios auf.
1. Klicken **[!UICONTROL Optionen]** in der oberen rechten Ecke des Bildschirms.
1. Auswählen **[!UICONTROL Ausführung entsperren]**.
1. Klicken **[!UICONTROL Entsperren]**.
