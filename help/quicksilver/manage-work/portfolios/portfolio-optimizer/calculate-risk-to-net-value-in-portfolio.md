---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Berechnung des Risikos zum Nettowert in einem Portfolio
description: In Portfolio Optimizer misst der Indikator [!UICONTROL Risiko bis Nettowert] das potenzielle Risiko unter Berücksichtigung des Nettowerts aller in Portfolio Optimizer angezeigten Projekte.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Berechnung des [!UICONTROL Risiko/Nettowert] in einem Portfolio

In [!UICONTROL Portfolio Optimizer] misst der Indikator [!UICONTROL Risiko für Nettowert] das potenzielle Risiko unter Berücksichtigung des [!UICONTROL Nettowerts], der von allen in [!UICONTROL Portfolio Optimizer angezeigten Projekten bereitgestellt &#x200B;].

Um die größte Effizienz innerhalb des Portfolios zu erzielen, sollten Sie sehen, dass der [!UICONTROL Risiko]-Indikator niedrig und der [!UICONTROL Nettowert]-Indikator hoch ist.

Die [!UICONTROL Risiko] und [!UICONTROL Nettowert] sind aus der Perspektive ihrer Beziehung zueinander dargestellt.

[!DNL Adobe Workfront] berechnet die Indikatoren [!UICONTROL Risiko] und [!UICONTROL Nettowert] anhand der folgenden Formeln:

* Der [!UICONTROL Risiko]-Indikator wird anhand der folgenden Formel berechnet:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* Der [!DNL Net Value] wird anhand der folgenden Formeln berechnet:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  ODER

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>Der Indikator [!UICONTROL Risiko bis Nettowert] wird anhand der Projekte berechnet, die Sie im [!UICONTROL Portfolio Optimizer] anzeigen, und nicht basierend auf allen Projekten, die mit dem Portfolio verknüpft sind.
