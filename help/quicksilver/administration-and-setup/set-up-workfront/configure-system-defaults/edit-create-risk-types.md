---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Risikotypen bearbeiten und erstellen
description: Sie können einem Projekt in der Planungsphase Risiken hinzufügen, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu identifizieren. Risiken sind mögliche Ereignisse, die den termingerechten oder budgetären Abschluss des Projekts verhindern könnten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 2%

---

# Risikotypen bearbeiten und erstellen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Sie können einem Projekt in der Planungsphase Risiken hinzufügen, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu identifizieren. Risiken sind mögliche Ereignisse, die den termingerechten oder budgetären Abschluss des Projekts verhindern könnten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Risikotypen

Risikotypen sind Kennzeichnungen, die Sie Ihren Risiken zuordnen können, um sie zu Berichtszwecken zu kategorisieren. Sie werden im Bereich **[!UICONTROL Setup]** vom [!DNL Adobe Workfront] erstellt. Nachdem Risikotypen in Ihrem **[!UICONTROL Setup) festgelegt wurden]** sind sie für Ihr System universell. Alle Projekteigentümer können für ihre Projekte dieselben Risikotypen verwenden.

## Risikotypen bearbeiten und erstellen

Einige Risikotypen sind standardmäßig bereits in [!DNL Workfront]. Um die Anforderungen Ihres Unternehmens widerzuspiegeln, können Sie entweder die vorhandenen Risikotypen bearbeiten oder neue Risikotypen erstellen.

* [Bestehende Risikotypen bearbeiten](#edit-existing-risk-types)
* [Neue Risikotypen erstellen](#create-new-risk-types)

### Bestehende Risikotypen bearbeiten {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Risikotypen]**.
1. Wählen Sie den Risikotyp aus, den Sie bearbeiten möchten.
1. Klicken Sie **[!UICONTROL Bearbeiten]**.
1. (Optional) Ändern Sie den Namen und die Beschreibung des Risikotyps.

   Für die Felder **[!UICONTROL Name“ und]** Beschreibung ]**gibt es eine Zeichenbeschränkung von**[!UICONTROL  0 Zeichen.

1. Klicken Sie **[!UICONTROL Änderungen speichern].**

### Neue Risikotypen erstellen {#create-new-risk-types}

Zusätzlich zu den standardmäßigen Risikotypen können Sie neue Risikotypen erstellen, um die Anforderungen Ihres Unternehmens widerzuspiegeln.

Einen neuen Risikotyp erstellen:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Risikotypen]**.
1. Klicken Sie **[!UICONTROL Neuer Risikotyp]**.
1. Geben Sie **[!UICONTROL Risikotyp einen]** Namen“ (erforderlich) und einen **[!UICONTROL Beschreibung]** (optional) ein.

   Für die Felder **[!UICONTROL Name“ und]** Beschreibung ]**gibt es eine Zeichenbeschränkung von**[!UICONTROL  0 Zeichen.

1. Klicken Sie **[!UICONTROL Risikotyp erstellen]**. Wenn Sie die Inline-Bearbeitung zum Hinzufügen Ihres Risikotyps verwendet haben, klicken Sie auf **[!UICONTROL Eingabetaste]** wenn Sie fertig sind.

   >[!NOTE]
   >
   >Wenn Sie einen benutzerdefinierten Risikotyp bearbeiten müssen, lesen Sie den Abschnitt [[!UICONTROL Bearbeiten vorhandener] Risikotypen](#edit-existing-risk-types) in diesem Artikel.

## Risiken mit Risikotypen an Projekte anhängen

Risikotypen können zum Beschriften von Risiken verwendet werden, die zu Ihren Projekten hinzugefügt werden. Weitere Informationen zum Hinzufügen von Risiken zu Projekten finden Sie unter [Erstellen und Bearbeiten von Risiken in Projekten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
