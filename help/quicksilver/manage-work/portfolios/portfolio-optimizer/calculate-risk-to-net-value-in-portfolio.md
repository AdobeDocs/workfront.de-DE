---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Berechnung des Nettowertrisikos in einem Portfolio
description: Im Portfolio Optimizer wird die [!UICONTROL Risiko des Nettowerts] misst das potenzielle Risiko unter Berücksichtigung des Nettowerts, der von allen im Portfolio Optimizer angezeigten Projekten bereitgestellt wird.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Berechnen Sie die [!UICONTROL Risiko des Nettowerts] in einem Portfolio

Im [!UICONTROL Portfolio Optimizer], die [!UICONTROL Risiko des Nettowerts] Indikator misst das potenzielle Risiko unter Berücksichtigung der [!UICONTROL Nettowert] bereitgestellt von allen Projekten, die in [!UICONTROL Portfolio Optimizer]. 

Um die höchste Effizienz innerhalb des Portfolios zu erreichen, möchten Sie sehen, dass die [!UICONTROL Risiko] der Indikator niedrig ist und [!UICONTROL Nettowert] ist hoch. 

Die [!UICONTROL Risiko] und [!UICONTROL Nettowert] Indikatoren werden aus der Perspektive ihrer Beziehung zueinander dargestellt.

[!DNL Adobe Workfront] berechnet die [!UICONTROL Risiko] und [!UICONTROL Nettowert] Indikatoren, die folgende Formeln verwenden:

* Die [!UICONTROL Risiko] Der Indikator wird anhand der folgenden Formel berechnet:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* Die [!DNL Net Value] Der Indikator wird anhand der folgenden Formeln berechnet:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   Oder

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>Die [!UICONTROL Risiko des Nettowerts] Indikator berechnet sich basierend auf den Projekten, die Sie in der [!UICONTROL Portfolio Optimizer]und nicht für alle Projekte, die mit dem Portfolio verbunden sind. 
