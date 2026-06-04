---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Berechnen des Risikos für den Nettowert in einem Portfolio
description: In Portfolio Optimizer misst der Indikator [!UICONTROL Risiko bis Nettowert] das potenzielle Risiko unter Berücksichtigung des Nettowerts aller in Portfolio Optimizer angezeigten Projekte.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 5%

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
