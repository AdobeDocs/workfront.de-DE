---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Berechnung des Nettowertrisikos in einem Portfolio
description: Im Portfolio Optimizer misst der Indikator "[!UICONTROL Risiko zu Nettowert]"das potenzielle Risiko unter Berücksichtigung des Nettowerts, der von allen im Portfolio Optimizer angezeigten Projekten bereitgestellt wird.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Berechnung des [!UICONTROL Nettowertrisikos] in einem Portfolio

Im Indikator [!UICONTROL Portfolio-Optimizer] misst der Indikator [!UICONTROL Risiko-Nettowert] das potenzielle Risiko unter Berücksichtigung des [!UICONTROL Nettowerts], der von allen im [!UICONTROL Portfolio-Optimizer] angezeigten Projekten bereitgestellt wird. 

Um die höchste Effizienz im Portfolio zu erzielen, sollten Sie sehen, dass der Indikator [!UICONTROL Risiko] niedrig ist und der Indikator [!UICONTROL Nettowert] hoch ist. 

Die Indikatoren [!UICONTROL Risiko] und [!UICONTROL Nettowert] werden aus der Perspektive dargestellt, wie sie miteinander verbunden sind.

[!DNL Adobe Workfront] berechnet die Indikatoren [!UICONTROL Risiko] und [!UICONTROL Nettowert] anhand der folgenden Formeln:

* Der Indikator [!UICONTROL Risiko] wird anhand der folgenden Formel berechnet:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* Der Indikator [!DNL Net Value] wird anhand der folgenden Formeln berechnet:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  Oder

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>Der Indikator &quot;[!UICONTROL Risiko bis Nettowert]&quot;berechnet sich auf der Grundlage der Projekte, die Sie im [!UICONTROL Portfolio Optimizer] anzeigen, und nicht auf allen mit dem Portfolio verknüpften Projekten. 
