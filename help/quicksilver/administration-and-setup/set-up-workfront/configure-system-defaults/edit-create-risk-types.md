---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Bearbeiten und Erstellen von Risikotypen
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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Risikotypen

Risikotypen sind Beschriftungen, die Sie für Ihre Risiken verwenden können, um sie zu Berichtszwecken zu kategorisieren. Sie werden im Bereich **[!UICONTROL Einrichtung]** vom [!DNL Adobe Workfront] -Administrator erstellt. Nachdem die Risikotypen in Ihrem **[!UICONTROL Setup]** -Bereich festgelegt wurden, sind sie universell für Ihr System. Alle Projekteigentümer können für ihre Projekte die gleichen Risikotypen verwenden.

## Risikotypen bearbeiten und erstellen

Einige Risikotypen befinden sich standardmäßig bereits in [!DNL Workfront]. Um die Anforderungen Ihrer Organisation widerzuspiegeln, können Sie entweder die vorhandenen Risikotypen bearbeiten oder neue Risikotypen erstellen.

* [Vorhandene Risikotypen bearbeiten](#edit-existing-risk-types)
* [Neue Risikotypen erstellen](#create-new-risk-types)

### Vorhandene Risikotypen bearbeiten {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Risikotypen]**.
1. Wählen Sie den Risikotyp aus, den Sie bearbeiten möchten.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. (Optional) Ändern Sie den Namen und die Beschreibung des Risikotyps.

   Für die Felder **[!UICONTROL Name]** und **[!UICONTROL Beschreibung]** gilt eine Zeichenbeschränkung von 50 Zeichen.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern].**

### Neue Risikotypen erstellen {#create-new-risk-types}

Sie können neben den Standardrisikokarten auch neue Risikotypen erstellen, die den Anforderungen Ihres Unternehmens gerecht werden.

So erstellen Sie einen neuen Risikotyp:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Risikotypen]**.
1. Klicken Sie auf **[!UICONTROL Neuer Risikotyp]**.
1. Geben Sie einen **[!UICONTROL Namen]** (erforderlich) und eine **[!UICONTROL Beschreibung]** (optional) für den Risikotyp ein.

   Für die Felder **[!UICONTROL Name]** und **[!UICONTROL Beschreibung]** gilt eine Zeichenbeschränkung von 50 Zeichen.

1. Klicken Sie auf &quot;**[!UICONTROL Risikotyp erstellen]**&quot;. Wenn Sie die Inline-Bearbeitung zum Hinzufügen Ihres Risikotyps verwendet haben, klicken Sie auf **[!UICONTROL Enter]** , wenn Sie fertig sind.

   >[!NOTE]
   >
   >Wenn Sie einen benutzerdefinierten Risikotyp bearbeiten müssen, lesen Sie den Abschnitt [[!UICONTROL Vorhandene ] Risikotypen bearbeiten](#edit-existing-risk-types) in diesem Artikel.

## Anhängen von Risiken mit Risikotypen an Projekte

Risikotypen können zur Kennzeichnung von Risiken verwendet werden, die zu Ihren Projekten hinzugefügt werden. Weitere Informationen zum Hinzufügen von Risiken zu Projekten finden Sie unter [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
