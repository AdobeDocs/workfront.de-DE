---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Erstellen und Bearbeiten von Risiken für Projekte
description: Risiken sind mögliche Ereignisse oder Faktoren, die verhindern, dass ein Projekt rechtzeitig oder innerhalb des Budgets beendet wird. Risiken können im Rahmen der Erstellung des Geschäftsszenarios eines Projekts oder mithilfe des Tabs Risiken aufgezeichnet werden. Risiken werden nur für ein Projekt erstellt. Sie können keine Risiken mit Aufgaben oder Problemen verknüpfen.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Risiken für Projekte

Risiken sind mögliche Ereignisse oder Faktoren, die verhindern, dass ein Projekt rechtzeitig oder innerhalb des Budgets beendet wird. Risiken können im Rahmen der Erstellung des Geschäftsszenarios eines Projekts oder mithilfe des Tabs Risiken aufgezeichnet werden. Risiken werden nur für ein Projekt erstellt. Sie können keine Risiken mit Aufgaben oder Problemen verknüpfen.

Risiken können mit Kosten verbunden sein, die tatsächlichen Risikokosten wirken sich jedoch nicht auf die tatsächlichen Kosten des Projekts aus.

>[!NOTE]
>
>In diesem Artikel werden die mit dem Projekt verbundenen Risiken definiert, da Sie sie im Geschäftsfall des Projekts definieren oder auf der Registerkarte Risiken des Projekts hinzufügen. Informationen zum Risikofeld, das beim Bearbeiten eines Projekts verfügbar ist, finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten Sie Berechtigungen, die "Finanzen verwalten"für das Projekt enthalten, für das Sie Risiken erstellen oder bearbeiten möchten </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen und Bearbeiten von Risiken im Geschäftsfall

Sie können Risiken im Rahmen der Planung des Geschäftsszenarios eines Projekts schaffen. Sie können sie später im Geschäftsfall bearbeiten, wenn beispielsweise Änderungen an der Wahrscheinlichkeit, dem Abmilderungsplan oder den Kosten eintreten. Informationen zum Erstellen eines Geschäftsfalls finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Ihr Workfront-Administrator oder -Gruppenadministrator muss die Option **Risiken** im Bereich &quot;Projektvoreinstellungen&quot;in Ihrem Geschäftsszenario, bevor Sie ihn auf Projektebene im Abschnitt &quot;Geschäftsszenario&quot;anzeigen können. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Das Erstellen und Bearbeiten von Risiken im Geschäftsfall ist identisch.

So erstellen oder bearbeiten Sie ein Risiko im Geschäftsfall:

1. Gehen Sie zu dem Projekt, für das Sie Risiken erstellen möchten.
1. Klicken **Geschäftsfall** im linken Bereich.
1. Im **Risiken** Abschnitt, klicken Sie auf **Risiken bearbeiten**.
1. Geben Sie die folgenden Informationen ein oder bearbeiten Sie sie:

   * **Beschreibung:** das Risiko beschreiben.

   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.

   * **Wahrscheinlichkeit**: gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.

   * **Typ:** Geben Sie an, unter welche Kategorie das Risiko fällt.
   * **Abmilderungsplan**: die Beschreibung des Plans zur Risikominderung aktualisieren.

   * **Minderungskosten**: Geben Sie die Kosten des Minderungsplans an, den Sie einrichten müssen, um zu verhindern, dass das Risiko eintritt.

   ![](assets/crp1-350x117.png)

1. (Optional) Klicken Sie auf **Ein weiteres Risiko hinzufügen** zusätzliche Risiken.
1. Klicken Sie auf **Speichern**.

## Risiken im Bereich Risiken erstellen und bearbeiten

Zusätzlich zum Erstellen und Bearbeiten von Risiken im Geschäftsfall können Sie dies mit dem **Risiken** -Abschnitt eines Projekts.

* [Risiken im Risikobereich schaffen](#create-risks-in-the-risks-area)
* [Risiken im Risikobereich bearbeiten](#edit-risks-in-the-risks-area)

### Risiken im Risikobereich schaffen {#create-risks-in-the-risks-area}

1. Gehen Sie zu dem Projekt, für das Sie Risiken erstellen möchten.
1. Klicken **Risiken** im linken Bereich.

   ![Risikoabschnitt der Aufgabe](assets/risks-section-on-project-2022.png)

1. Klicken **Hinzufügen von Risiken** und Risiken durch die Inline-Bearbeitung ihrer Informationen schaffen.

   Oder

   Klicken **Neues Risiko**. Die **Neues Risiko** wird geöffnet.

1. Geben Sie die folgenden Informationen ein:

   * **Beschreibung**: das Risiko beschreiben.
   * **Risikotyp**: Geben Sie an, unter welche Kategorie das Risiko fällt.\
      Ihr Workfront-Administrator definiert die in Ihrer Umgebung verfügbaren Risikotypen. Informationen zur Definition von Risikotypen finden Sie im Artikel [Risikotypen bearbeiten und erstellen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Wahrscheinlichkeit**: gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.
   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.
   * **Minderungskosten**: Geben Sie die Kosten des Minderungsplans an, den Sie einrichten müssen, um zu verhindern, dass das Risiko eintritt.
   * **Tatsächliche Kosten**: Geben Sie die tatsächlichen Kosten des Risikos an, falls das Risiko eintritt.
   * **Abmilderungsplan**: die Beschreibung des Plans zur Risikominderung aktualisieren.

1. (Bedingt) Klicken Sie auf **Eingabe** , wenn Sie das Risiko inline erstellen.

   Oder

   Klicken **Speichern** Wenn Sie die Informationen in der **Neues Risiko** Dialogfeld.

1. (Optional) Wählen Sie eine andere **Status** für das Risiko in der **Status** Dropdown-Menü beim Anwenden der **Standard** die Liste der Risiken.

   Standardmäßig lautet der Status eines Risikos **Identifiziert**.

### Risiken im Risikobereich bearbeiten {#edit-risks-in-the-risks-area}

Sie können Risiken während der Laufzeit eines Projekts bearbeiten, wenn beispielsweise Änderungen an der Wahrscheinlichkeit, den potenziellen Kosten oder dem Status auftreten.

Sie können ein Risiko gleichzeitig bearbeiten oder mehrere Risiken in großen Mengen bearbeiten.

So bearbeiten Sie Risiken:

1. Navigieren Sie zu einem Projekt, für das Sie vorhandene Risiken bearbeiten möchten.
1. Klicken **Risiken** im linken Bereich.
1. Beginnen Sie mit der Inline-Bearbeitung der Felder für die Risiken, die Sie in der Liste sehen, um jeweils ein Risiko zu bearbeiten.

   Oder

   Wählen Sie ein oder mehrere Risiken aus und klicken Sie auf **Bearbeiten** um mehrere Risiken gleichzeitig zu bearbeiten.

   >[!NOTE]
   >
   >Sie wenden dieselben Informationen auf alle ausgewählten Risiken an, wenn Sie mehrere Risiken gleichzeitig bearbeiten. Die mit den einzelnen Risiken verknüpften Informationen vor den Änderungen werden in einer Massenbearbeitung überschrieben.

1. Wenn Sie auf **Bearbeiten**, die **Risiko bearbeiten** wird geöffnet.

   Bearbeiten Sie die folgenden Felder:

   * **Beschreibung**: die Beschreibung des Risikos zu ändern.
   * **Risikotyp**: Geben Sie an, unter welche Kategorie das Risiko fällt.
   * **Wahrscheinlichkeit**: gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.
   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.
   * **Minderungskosten**: Geben Sie die Kosten des Minderungsplans an, den Sie einrichten müssen, um zu verhindern, dass das Risiko eintritt.
   * **Tatsächliche Kosten**: Geben Sie die tatsächlichen Kosten des Risikos an, falls das Risiko eintritt.
   * **Abmilderungsplan**: die Beschreibung des Plans zur Risikominderung aktualisieren.

1. Klicken **Änderungen speichern**.
1. (Optional) Bearbeiten Sie die **Status** für ein Risiko im **Status** Dropdown-Menü beim Anwenden der **Standard** die Liste der Risiken.

   >[!NOTE]
   >
   >Sie können die **Status** der Risiken in **Risiko bearbeiten** Dialogfeld. Dies ist nur in einer Inline-Bearbeitung möglich.
