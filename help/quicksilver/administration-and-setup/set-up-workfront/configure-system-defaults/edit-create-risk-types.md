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
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 2%

---

# Risikotypen bearbeiten und erstellen

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Adobe Workfront verfügt über eine Reihe von Standardrisikotypen, die Sie Projekten in der Planungsphase zuordnen können, um potenzielle Hindernisse zu identifizieren, bevor Sie Arbeiten genehmigen.

Risiken sind mögliche Ereignisse, die den termingerechten oder budgetären Abschluss des Projekts verhindern könnten.

Zusätzlich zu den standardmäßigen Risikotypen können Sie einen neuen Risikotyp hinzufügen, um die Anforderungen in Ihrem Unternehmen widerzuspiegeln.

Sie können Risikotypen mit Projektrisiken verknüpfen, um festzustellen, auf welche Art von Risiko ein Projekt stoßen könnte.

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
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
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

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Risikotypen

Risikotypen sind Kennzeichnungen, die Sie Ihren Risiken zuordnen können, um sie zu Berichtszwecken zu kategorisieren.

Als [!DNL Workfront] können Sie [!UICONTROL Risikotypen] im Bereich [!UICONTROL **Setup**] erstellen.

Nach der Einrichtung der Risikotypen sind sie für Ihr System universell.

Alle Projekteigentümer können für ihre Projekte dieselben Risikotypen verwenden.

## Risikotypen bearbeiten und erstellen

Einige Risikotypen sind standardmäßig bereits in [!DNL Workfront].


Sie können Folgendes tun, um die Anzahl der Risikotypen in Ihrer Workfront-Instanz zu erhöhen:

* [Bestehende Risikotypen bearbeiten](#edit-existing-risk-types)
* [Risikotypen erstellen](#create-risk-types)

### Bestehende Risikotypen bearbeiten {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Risikotypen]**.
1. Wählen Sie den Risikotyp aus, den Sie bearbeiten möchten.
1. Klicken Sie auf das **[!UICONTROL Bearbeiten]**-Symbol ![Bearbeiten](assets/edit-icon.png).

   <span class="preview">Das Feld [!UICONTROL **Risikotyp bearbeiten**] wird geöffnet.</span>

   ![Feld „Risikotyp bearbeiten“](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >   Sie können Risikotypinformationen inline bearbeiten, wenn Sie auf den Namen oder die Beschreibung eines Risikotyps in einer Liste von Risikotypen doppelklicken.

1. (Optional) Ändern Sie den Namen und die Beschreibung des Risikotyps.

   Für die Felder **[!UICONTROL Name“ und]** Beschreibung **gibt es eine Zeichenbeschränkung von** 0 Zeichen.

1. Klicken Sie **[!UICONTROL Änderungen speichern].**

1. (Optional) Um einen Risikotyp zu löschen, wählen Sie ihn in der Liste aus und klicken dann auf das [!UICONTROL **Löschen**]-Symbol ![Löschen](assets/delete.png) und dann auf [!UICONTROL **Ja, Löschen**]. Der Risikotyp wurde gelöscht und kann nicht wiederhergestellt werden.

1. (Optional) Um eine Liste von Risikotypen zu exportieren, klicken Sie auf das Symbol [!UICONTROL **Exportieren**] (Symbol ![Exportieren](assets/export-icon.png). Sie können in die folgenden Dateitypen exportieren:

   * PDF
   * Excel
   * Excel (xlsx)
   * Durch Tabulatoren getrennt

   >[!TIP]
   >
   >   Sie können zunächst eine begrenzte Anzahl von Risikotypen auswählen und diese dann für eine kleinere Liste exportieren.


### Risikotypen erstellen {#create-risk-types}

Zusätzlich zu den standardmäßigen Risikotypen können Sie Risikotypen erstellen.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Risikotypen]**.

1. Klicken Sie **[!UICONTROL Neuer Risikotyp]**, um das Feld [!UICONTROL **Neuer Risikotyp**] zu öffnen

   Oder

   Klicken Sie [!UICONTROL **Weitere Risikotypen hinzufügen**] in der linken unteren Ecke der Liste der Risikotypen, um Risikotypen inline hinzuzufügen.

   <span class="preview">Das Feld **Neuer Risikotyp** wird geöffnet. <span>

   ![Feld „Neuer Risikotyp“](assets/new-risk-type-box.png)


1. Fügen Sie **[!UICONTROL Risikotyp einen]** Namen“ (erforderlich) und **[!UICONTROL Beschreibung]** (optional) hinzu.

   Für die Felder **[!UICONTROL Name“ und]** Beschreibung **gibt es eine Zeichenbeschränkung von** 0 Zeichen.

1. Klicken Sie **[!UICONTROL Risikotyp erstellen]**,

   Wenn Sie den Risikotyp mithilfe der Inline-Bearbeitung hinzugefügt haben, klicken Sie nach Abschluss **[!UICONTROL auf]** Eingabetaste“.

   >[!TIP]
   >
   >Informationen zum Bearbeiten eines benutzerdefinierten Risikotyps finden Sie im Abschnitt [[!UICONTROL Bearbeiten &#x200B;] Risikotypen](#edit-existing-risk-types) in diesem Artikel.

## Risiken mit Risikotypen an Projekte anhängen

Sie können Risikotypen verwenden, um zu Ihren Projekten hinzugefügte Risiken zu kennzeichnen.

Weitere Informationen zum Hinzufügen von Risiken zu Projekten finden Sie unter [Erstellen und Bearbeiten von Risiken in Projekten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
