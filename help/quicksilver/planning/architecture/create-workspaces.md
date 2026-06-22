---
title: Erstellen von Arbeitsbereichen
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen. Datensatztypen sind in einem Arbeitsbereich nach Abschnitten organisiert.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/LtHxTws4o0FI964-qOtFE-sbKaLGRQroBQvMD5fOUvY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 1311
ht-degree: 2%

---

# Erstellen von Arbeitsbereichen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning sind Arbeitsbereiche zentrale Orte, an denen Teams ihre Arbeit planen.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen.

Allgemeine Informationen zu Arbeitsbereichen finden Sie unter [Arbeitsbereiche - Übersicht](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront- oder Workflow-Paket</p> 
<p>Beliebiges Workfront-Planungspaket</p>
<p>Ein Workfront Planning Prime- oder höher-Paket zum Erstellen mehrerer Arbeitsbereiche gleichzeitig</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   <p>Systemadmin. zur gleichzeitigen Erstellung mehrerer Arbeitsbereiche mithilfe des Best-Practice-Vorlagenpakets</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Arbeitsbereich erstellen

Sie können einen Arbeitsbereich erstellen und Datensatztypen hinzufügen, um Ihre Objekte in Workfront Planning zu organisieren.

Weitere Informationen zum Bearbeiten eines Arbeitsbereichs finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).

Sie können Arbeitsbereiche wie folgt erstellen:

* Einen Arbeitsbereich von Grund auf neu oder aus einer Vorlage erstellen

  Weitere Informationen finden Sie im Abschnitt [Erstellen eines neuen Arbeitsbereichs oder einer Vorlage](#create-a-workspace-from-scratch-or-from-a-template) in diesem Artikel.
* Erstellen Sie mit der KI-gestützten Planungs-Designer einen Arbeitsbereich. Diese Funktion steht derzeit nur einer begrenzten Anzahl von Kunden in einem Beta-Programm zur Verfügung.

  Weitere Informationen finden Sie [Erste Schritte mit der Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

* Erstellen mehrerer Arbeitsbereiche mithilfe eines Best-Practice-Vorlagenpakets für mehrere Arbeitsbereiche

  Weitere Informationen finden Sie im Abschnitt [Erstellen mehrerer Arbeitsbereiche mithilfe eines Best-Practice-Vorlagenpakets für mehrere Arbeitsbereiche](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) in diesem Artikel

  >[!TIP]
  >
  >Sie können mehrere Arbeitsbereiche gleichzeitig erstellen, wenn Sie das Best-Practice-Vorlagenpaket verwenden.

### Arbeitsbereich von Grund auf neu oder aus einer Vorlage erstellen

{{step1-to-planning}}

1. Klicken Sie auf **Arbeitsbereich erstellen**

   Das Feld Arbeitsbereich erstellen wird angezeigt. Sie können einen Arbeitsbereich von Grund auf neu erstellen oder ihn mit einer der verfügbaren Vorlagen erstellen.

1. (Optional und bedingt) Klicken Sie **Vorschau** innerhalb einer der folgenden vordefinierten Arbeitsbereichsvorlagen:

   * Operations Initiative Studio
   * Kommunikationsstudio
   * Basis: Marketing-Management
   * Erweitert: Marketing-Management
   * Enterprise: Marketing-Management
   * Vertriebsleitung
   * Produkt-Management

   Das Vorschaufeld für Vorlagen wird geöffnet.

   Es gibt einen Hinweis darauf, welche Datensatztypen, Abschnitte und wie viele Felder mit jeder Vorlage verknüpft sind.

   ![Vorschau einer Workspace-Vorlage](assets/previewing-a-workspace-template.png)

   Weitere Informationen zu Workfront Planning Workspace-Vorlagen finden Sie unter [Liste der Workspace-Vorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicken Sie im Vorlagenvorschaufeld auf **Vorlage verwenden**, um den Arbeitsbereich aus der ausgewählten Vorlage zu erstellen

   ODER

   Klicken Sie auf **Zurück** und dann auf **Neuer Arbeitsbereich**, um einen neuen Arbeitsbereich zu erstellen.

   Es wird einer für die folgenden Typen von Arbeitsbereichen erstellt:

   * Ein leerer Arbeitsbereich mit dem **Nicht benannter Workspace** in dem Sie manuell mit dem Hinzufügen von Datensatztypen beginnen können, wenn Sie einen Arbeitsbereich von Grund auf neu erstellen.
   * Ein Arbeitsbereich, der nach der ausgewählten Vorlage benannt und mit Beispieldatensatztypen gefüllt ist. Sie können die Datensatztypen und den Arbeitsbereich weiter anpassen.

   Für Workfront-Administratoren wird der neue Arbeitsbereich auf der Registerkarte **Arbeitsbereiche, an denen ich mitwirke** angezeigt.

   Für alle anderen Benutzer, die Arbeitsbereiche erstellen können, wird der neue Arbeitsbereich im Bereich **Arbeitsbereiche** angezeigt.

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste.

1. (Optional und bedingt) Wenn Sie den Arbeitsbereich über eine Vorlage erstellt haben, klicken Sie in den Namen der Abschnitte **Operative Datensatztypen** oder **Taxonomien** .

   ODER

   Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und anschließend auf **Umbenennen**, um den Abschnitt umzubenennen.

   >[!TIP]
   >
   >Sie können jeden Abschnitt in jedem Arbeitsbereich umbenennen, auch wenn Sie den Abschnitt nicht erstellt haben.

   Weitere Informationen zum Bearbeiten von Arbeitsbereichen, einschließlich der Abschnitte zum Bearbeiten von Arbeitsbereichen, finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen**, um Datensatztypen zu dem Arbeitsbereich in einem beliebigen Abschnitt hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Eintragstypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Weitere Informationen zum Bearbeiten und Löschen von Datensatztypen in einem Arbeitsbereich finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Optional) Klicken Sie auf den Rückwärtspfeil links neben dem neuen Arbeitsbereich, um die Hauptseite von Planning zu öffnen. Auf der Registerkarte &quot;**&quot; wird eine neue Workspace-Karte für den neuen Workspace**.

   Der Name des Benutzers, der den Arbeitsbereich erstellt hat, wird auf der Arbeitsbereichskarte als Besitzer gespeichert.

   >[!TIP]
   >
   >Arbeitsbereiche, die von Benutzenden erstellt wurden, die nur Workfront besitzen und nicht zum Adobe Admin Console hinzugefügt wurden, werden so angezeigt, wie sie vom **System** erstellt wurden.
   >

### Erstellen mehrerer Arbeitsbereiche mithilfe eines Best-Practice-Vorlagenpakets für mehrere Arbeitsbereiche

>[!IMPORTANT]
>
>Das gleichzeitige Erstellen mehrerer Arbeitsbereiche mithilfe des Best-Practice-Vorlagenpakets ist nur verfügbar, wenn die folgenden Voraussetzungen erfüllt sind:
>
>* Ihr Unternehmen hat ein Workfront- oder Workflow Planning Prime- oder Ultimate-Paket erworben
>* Sie sind Systemadministrator

Sie können das Vorlagenpaket für mehrere Arbeitsbereiche verwenden, um mit einem Klick 6 Arbeitsbereiche zu erstellen.

Die im Bundle enthaltenen Vorlagen enthalten Arbeitsbereiche, Datensatztypen, Datensätze, Ansichten und Felder, um Ihnen den Einstieg in Ihre Planungsimplementierung zu erleichtern. Weitere Informationen finden Sie unter [Liste der Arbeitsbereichsvorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

>[!IMPORTANT]
>
>Die Namen der Arbeitsbereiche und Datensätze, die im Bundle enthalten sind, sind Beispiele und keine Spiegelung Ihrer eigenen Umgebung.
>
>Die Namen der Datensatztypen und -felder können in jeder Organisation als Standard für die Implementierung in jeder Branche gemäß unserer Empfehlung verwendet werden.
>

{{step1-to-planning}}

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie **Arbeitsbereich erstellen** und führen Sie dann die folgenden Schritte aus:

      1. Das Feld Arbeitsbereich erstellen wird angezeigt. Sie können einen Arbeitsbereich von Grund auf neu erstellen oder ihn mit einer der verfügbaren Vorlagen erstellen.

      1. Klicken Sie **Bereich** Hier beginnen (empfohlen **auf „Arbeitsbereich-Setup überprüfen**.
      1. (Optional) Klicken Sie **Vorschau** in einer der folgenden vordefinierten Arbeitsbereichsvorlagen, um das Vorschaufeld für jede Vorlage zu öffnen:

         * &#x200B;1. Globale Klassifizierungen und Taxonomien

           Die Vorlage Globale Klassifizierungen und Taxonomien enthält alle Datensatztypen und -felder, die Sie in Ihrer Umgebung für eine erfolgreiche Implementierung von Workfront Planning erstellen sollten.

           Sie können die Datensatztypen in dieser Vorlage später in andere von Ihnen erstellte Arbeitsbereiche verknüpfen oder importieren.
         * 2.Fréscopa Global Marketing
         * 3.Fréscopa Social Marketing
         * 4.Fréscopa Medien und PR
         * 5.Fréscopa Global Events
         * 6.Fréscopa Führende Unternehmensführung

      1. Nachdem Sie das Feld **Vorschau** für jede Arbeitsbereichsvorlage geöffnet haben, klicken Sie auf **Zurück**, um zum Feld **Arbeitsbereich erstellen** zurückzukehren, oder klicken Sie auf **Vorlagen verwenden**, um die Vorlagen zu verwenden, einschließlich im Bundle, und Arbeitsbereiche zu erstellen.

   <div class="preview">

   * Klicken Sie auf **Registerkarte** Beispielarbeitsbereiche“ und führen Sie dann die folgenden Schritte aus:

      1. Klicken Sie auf der Registerkarte auf eine der Arbeitsbereichsvorlagen, um die Datensatztypen und -felder in den einzelnen Vorlagen zu überprüfen. Vorlagen auf der Registerkarte **Beispiel-**&quot; sind schreibgeschützt.
      1. Klicken **oben rechts** einer Vorlage auf „Erstellen aus Vorlagen“.
      1. (Optional) Klicken Sie **einer** auf „Vorschau“, um die Datensatztypen und ihre Felder anzuzeigen.

         >[!TIP]
         >
         >Wenn Sie in einer Vorlage auf eine Karte für den Datensatztyp klicken, werden die Felder des Datensatztyps im rechten Bedienfeld angezeigt.
      1. Klicken Sie **Vorlagen verwenden**.

   </div>

   Die 6 Arbeitsbereiche werden erstellt und auf den Registerkarten **Arbeitsbereiche bin ich** und **Alle Arbeitsbereiche** für Systemadministratoren angezeigt. Alle Benutzer von Standardlizenzen sehen die Arbeitsbereiche in ihrem Arbeitsbereich, nachdem ein Systemadministrator sie erstellt und die neuen Arbeitsbereiche für sie freigegeben hat.

1. Beginnen Sie mit der Bearbeitung der von Ihnen erstellten Arbeitsbereiche und fügen Sie Datensatztypen, Datensätze, Ansichten und Felder hinzu, die für Ihre Organisation relevant sind.

   Weitere Informationen zu Best Practices für die Implementierung von Workfront finden Sie in den Artikeln im Abschnitt [Best Practices für die Adobe Workfront-Planung: ](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md).

   Informationen zum Bearbeiten von Arbeitsbereichen finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).



