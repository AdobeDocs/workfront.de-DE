---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: KI-Mitwirkende konfigurieren
description: Als Adobe Workfront-Administrator können Sie KI-Mitwirkende konfigurieren und sie Projekten und Aufgaben zuweisen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 7d359a2536860d13658d3ec0c95264a55db7ab29
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 6%

---

# KI-Mitwirkende konfigurieren

>[!IMPORTANT]
>
>Derzeit ist Content Reviewer der einzige verfügbare KI-Mitwirkende-Typ. In Zukunft werden weitere KI-Collaborator-Funktionen verfügbar sein.

{{highlighted-preview-article-level}}

KI-Mitwirkende sind eine Möglichkeit, KI-Agenten in Ihre Projekte und Aufgaben einzubinden. Sie können einen KI-Mitwirkenden konfigurieren und ihn dann wie einen Benutzer zuweisen.

Sie können beispielsweise einen KI-Mitarbeiter vom Typ „Prüfer“ mit Markenrichtlinien konfigurieren und diesen Mitarbeiter dann zuweisen, um ein Dokument zu überprüfen.

Zu den verfügbaren KI-Typen für Mitwirkende gehören:

* Reviewer: Erstellen Sie einen Mitarbeiter mit Marken <!-- or Adobe Brand Intelligence--> weisen Sie ihn dann als Reviewer für Assets zu.

  Weitere Informationen finden Sie unter [Erste Schritte mit dem Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Standard, Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen



* Ihr Unternehmen muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.

  Weitere Informationen finden Sie unter [Unterschreiben des Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)Abkommens im Artikel KI-Assistent in Workfront.
* Sie müssen eine Marke in Workfront konfiguriert haben, bevor Sie sie für einen KI-Mitwirkenden vom Typ Prüfer verwenden können.

  Anweisungen finden Sie unter [Erstellen und Verwalten von Marken für den Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Erstellen eines neuen KI-Mitarbeiters vom Typ „Prüfer“

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. Klicken **oben rechts** Bildschirm auf „Neuer Mitarbeiter“.
1. Klicken Sie **Reviewer** und dann auf **Weiter**.

   >[!NOTE]
   >
   >Derzeit ist nur der Reviewer-Typ verfügbar. In Zukunft werden weitere KI-Typen für Mitwirkende verfügbar sein.

1. Geben Sie im Feld Name des Mitarbeiters einen Namen für den Mitarbeiter ein. Dies ist der Name, der in der Liste der verfügbaren Bevollmächtigten für eine Aufgabe angezeigt wird.
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. &#x200B;<!--(Conditional) If the AI Collaborator will use a Brand,-->Wählen Sie die zu verwendende Marken- und Markenrichtlinie aus.
1. Klicken Sie auf **Speichern**.

## KI-Mitwirkende verwalten

Sie können vorhandene KI-Mitwirkende bearbeiten, kopieren und löschen.

{{step-1-to-setup}}

1. Klicken Sie in der linken Navigation auf **KI-Mitwirkende**.
1. (Bedingt) Um einen Mitarbeiter zu bearbeiten, klicken Sie auf den Namen des Mitarbeiters, den Sie bearbeiten möchten, nehmen Sie im Fenster „Mitarbeiter bearbeiten“ Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Mitwirkenden zu kopieren, klicken Sie auf das Kopiersymbol ![Kopiersymbol](assets/copy-ai-collaborator.png) in der Zeile des KI-Mitwirkenden, die Sie kopieren möchten, klicken Sie auf den Namen der Kopie, nehmen Sie im Fenster Mitwirkende bearbeiten Änderungen vor und klicken Sie auf **Speichern**.
1. (Bedingt) Um einen Kollaborateur zu löschen, klicken Sie auf das Löschsymbol ![Löschsymbol](assets/delete-collaborator-icon.png) in der Zeile des KI-Mitarbeiters, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
