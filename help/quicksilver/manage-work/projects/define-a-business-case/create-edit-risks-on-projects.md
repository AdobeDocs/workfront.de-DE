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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten Sie Berechtigungen, die "Finanzen verwalten"für das Projekt enthalten, für das Sie Risiken erstellen oder bearbeiten möchten </p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Projekt in Adobe Workfront freigeben</a> .</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen und Bearbeiten von Risiken im Geschäftsfall

Sie können Risiken im Rahmen der Planung des Geschäftsszenarios eines Projekts schaffen. Sie können sie später im Geschäftsfall bearbeiten, wenn beispielsweise Änderungen an der Wahrscheinlichkeit, dem Abmilderungsplan oder den Kosten eintreten. Informationen zum Erstellen eines Geschäftsfeldes finden Sie unter [Erstellen eines Geschäftsfeldes für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Ihr Workfront-Administrator oder Gruppenadministrator muss den Abschnitt **Risiken** in Ihrem Geschäftsszenario im Bereich &quot;Projekteinstellungen&quot;aktivieren, bevor Sie ihn auf Projektebene im Abschnitt &quot;Geschäftsfall&quot;anzeigen können. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Konfigurieren von systemweiten Projekteigenschaften](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Das Erstellen und Bearbeiten von Risiken im Geschäftsfall ist identisch.

So erstellen oder bearbeiten Sie ein Risiko im Geschäftsfall:

1. Gehen Sie zu dem Projekt, für das Sie Risiken erstellen möchten.
1. Klicken Sie im linken Bereich auf **Geschäftsszenario** .
1. Klicken Sie im Abschnitt **Risiken** auf **Risiken bearbeiten**.
1. Geben Sie die folgenden Informationen ein oder bearbeiten Sie sie:

   * **Beschreibung:** Beschreiben Sie das Risiko.

   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.

   * **Wahrscheinlichkeit**: Gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.

   * **Typ:** Geben Sie an, zu welcher Kategorie das Risiko gehört.
   * **Reduzierungsplan**: Aktualisieren Sie die Beschreibung des Plans, um das Risiko zu verringern.

   * **Schadensminderungskosten**: Geben Sie die Kosten des Schadensminderungsplans an, den Sie einrichten müssen, um das Auftreten des Risikos zu verhindern.

   ![](assets/crp1-350x117.png)

1. (Optional) Klicken Sie auf **Neues Risiko hinzufügen** , um zusätzliche Risiken hinzuzufügen.
1. Klicken Sie auf **Speichern**.

## Risiken im Bereich Risiken erstellen und bearbeiten

Zusätzlich zum Erstellen und Bearbeiten von Risiken im Geschäftsfall können Sie dies mit dem Abschnitt **Risiken** eines Projekts tun.

* [Erstellen Sie Risiken im Risikobereich](#create-risks-in-the-risks-area)
* [Risiken im Risikobereich bearbeiten](#edit-risks-in-the-risks-area)

### Risiken im Risikobereich schaffen {#create-risks-in-the-risks-area}

1. Gehen Sie zu dem Projekt, für das Sie Risiken erstellen möchten.
1. Klicken Sie im linken Bereich auf **Risiken** .

   ![Risikoabschnitt der Aufgabe](assets/risks-section-on-project-2022.png)

1. Klicken Sie auf **Hinzufügen von Risiken beginnen** und erstellen Sie Risiken durch Inline-Bearbeitung ihrer Informationen.

   Oder

   Klicken Sie auf **Neues Risiko**. Das Dialogfeld **Neues Risiko** wird geöffnet.

1. Geben Sie die folgenden Informationen ein:

   * **Beschreibung**: Beschreiben Sie das Risiko.
   * **Risikotyp**: Geben Sie an, zu welcher Kategorie das Risiko gehört.\
     Ihr Workfront-Administrator definiert die in Ihrer Umgebung verfügbaren Risikotypen. Informationen zum Definieren von Risikotypen finden Sie im Artikel [Bearbeiten und Erstellen von Risikotypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Wahrscheinlichkeit**: Gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.
   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.
   * **Schadensminderungskosten**: Geben Sie die Kosten des Schadensminderungsplans an, den Sie einrichten müssen, um das Auftreten des Risikos zu verhindern.
   * **Tatsächliche Kosten**: Geben Sie die tatsächlichen Kosten des Risikos an, wenn das Risiko eintritt.
   * **Reduzierungsplan**: Aktualisieren Sie die Beschreibung des Plans, um das Risiko zu verringern.

1. (Bedingt) Klicken Sie auf **Enter** , wenn Sie das Risiko inline erstellen.

   Oder

   Klicken Sie auf **Speichern** , wenn Sie die Informationen im Dialogfeld **Neues Risiko** bearbeiten.

1. (Optional) Wählen Sie im Dropdownmenü **Status** einen anderen **Status** für das Risiko aus, wenn Sie die Ansicht **Standard** auf die Liste der Risiken anwenden.

   Standardmäßig lautet der Status eines Risikos **Identifiziert**.

### Risiken im Risikobereich bearbeiten {#edit-risks-in-the-risks-area}

Sie können Risiken während der Laufzeit eines Projekts bearbeiten, wenn beispielsweise Änderungen an der Wahrscheinlichkeit, den potenziellen Kosten oder dem Status auftreten.

Sie können ein Risiko gleichzeitig bearbeiten oder mehrere Risiken in großen Mengen bearbeiten.

So bearbeiten Sie Risiken:

1. Navigieren Sie zu einem Projekt, für das Sie vorhandene Risiken bearbeiten möchten.
1. Klicken Sie im linken Bereich auf **Risiken** .
1. Beginnen Sie mit der Inline-Bearbeitung der Felder für die Risiken, die Sie in der Liste sehen, um jeweils ein Risiko zu bearbeiten.

   Oder

   Wählen Sie ein oder mehrere Risiken aus und klicken Sie dann auf **Bearbeiten** , um mehrere Risiken gleichzeitig zu bearbeiten.

   >[!NOTE]
   >
   >Sie wenden dieselben Informationen auf alle ausgewählten Risiken an, wenn Sie mehrere Risiken gleichzeitig bearbeiten. Die mit den einzelnen Risiken verknüpften Informationen vor den Änderungen werden in einer Massenbearbeitung überschrieben.

1. Wenn Sie auf **Bearbeiten** geklickt haben, wird das Dialogfeld **Risiko bearbeiten** geöffnet.

   Bearbeiten Sie die folgenden Felder:

   * **Beschreibung**: Bearbeiten Sie die Beschreibung des Risikos.
   * **Risikotyp**: Geben Sie an, zu welcher Kategorie das Risiko gehört.
   * **Wahrscheinlichkeit**: Gibt die Wahrscheinlichkeit des Auftretens des Risikos als Prozentwert an.
   * **Potenzielle Kosten**: Geben Sie die geschätzten Kosten an, falls das Risiko eintritt.
   * **Schadensminderungskosten**: Geben Sie die Kosten des Schadensminderungsplans an, den Sie einrichten müssen, um das Auftreten des Risikos zu verhindern.
   * **Tatsächliche Kosten**: Geben Sie die tatsächlichen Kosten des Risikos an, wenn das Risiko eintritt.
   * **Reduzierungsplan**: Aktualisieren Sie die Beschreibung des Plans, um das Risiko zu verringern.

1. Klicken Sie auf **Änderungen speichern**.
1. (Optional) Bearbeiten Sie den **Status** für ein Risiko im Dropdown-Menü **Status** , wenn Sie die Ansicht **Standard** auf die Liste der Risiken anwenden.

   >[!NOTE]
   >
   >Sie können den **Status** der Risiken im Dialogfeld **Risiko bearbeiten** nicht bearbeiten. Dies ist nur in einer Inline-Bearbeitung möglich.
