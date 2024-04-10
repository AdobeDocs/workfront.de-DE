---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Ratenkarten verwalten
description: Mit Ratenkarten können Sie mehrere Abrechnungsraten pro Rolle festlegen, basierend auf dem Standort.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Ratenkarten verwalten

{{highlighted-preview-article-level}}

Mit Ratenkarten können Sie mehrere Abrechnungsraten pro Rolle festlegen, basierend auf dem Standort. Sie könnten eine berufliche Rolle in Designer mit Sitz in Paris und einen zweiten Designer mit Sitz in New York mit jeweils unterschiedlichen Abrechnungsraten haben. Für Auftragsrollen auf einer Ratenkarte ist jedoch kein Ort erforderlich. Eine Abrechnungsrate für eine Stellenrolle (und möglicherweise einen Ort) auf einer Ratenkarte kann auch effektive Daten enthalten.

## Zugriffsanforderungen

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
   <td><p>Neuer Plan: [!UICONTROL Standard] </p>
       <p>oder</p> 
       <p>Aktueller Plan: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf [!UICONTROL Finanzdaten bearbeiten</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Um eine für Sie freigegebene Ratenkarte zu bearbeiten, benötigen Sie die Berechtigung zum Verwalten der Ratenkarte.</td> 
  </tr> 
 </tbody> 
</table>

## Preiskarte hinzufügen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Ratenkarten**].
1. Klicks [!UICONTROL **Neue Preiskarte**] und geben Sie dann einen Namen für die Ratenkarte im [!UICONTROL Neue Preiskarte] , um &quot;Untitled Rate Card&quot;zu ersetzen.
1. (Optional) Fügen Sie im Bildschirm &quot;Details der Ratenkarte&quot;eine [!UICONTROL **Beschreibung**].
1. (Optional) Um ein benutzerdefiniertes Formular an die Ratenkarte anzuhängen, klicken Sie auf die [!UICONTROL **Benutzerdefiniertes Formular hinzufügen**] in der oberen rechten Ecke ein benutzerdefiniertes Formular aus der angezeigten Liste auswählen.

   Weitere Informationen zum Anhängen eines benutzerdefinierten Formulars finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicks [!UICONTROL **Auftragsrollen und -raten**] im linken Navigationsbereich.
1. Klicken Sie auf dem Bildschirm &quot;Auftragseingänge und -raten von Karten bewerten&quot;auf [!UICONTROL **Hinzufügen von Aufgabenrollen**].
1. Wählen Sie im Dialogfeld eine [!UICONTROL **Auftragsrolle**] , um die Abrechnungsraten für festzulegen.

   Die standardmäßige Abrechnungsrate zeigt die Rate auf Systemebene für diese Auftragsrolle an, sofern eine definiert ist.

   ![Dialogfeld &quot;Neue Abrechnungsrate&quot;](assets/location-rate-for-rate-card.png)

1. Wählen Sie eine [!UICONTROL **Währung**] für die Rolle &quot;Arbeit&quot;.
1. (Optional) Wählen Sie eine [!UICONTROL **Standort**] für die Rolle &quot;Arbeit&quot;.
1. Im [!UICONTROL **Abrechnungskurs 1**] Geben Sie den Abrechnungskurs für diesen Ort ein. Klicken Sie anschließend auf [!UICONTROL **Speichern**] um die Abrechnungsrate einmal zu überschreiben.

   Oder

   Klicks [!UICONTROL **Rate hinzufügen**] um standortspezifischere Abrechnungssätze mit effektiven Daten hinzuzufügen.

1. (Bedingt) Wenn Sie mehr als eine Abrechnungsrate für diesen Ort hinzufügen, geben Sie die folgenden Informationen ein:

   * **[!UICONTROL Abrechnungskurs 1], 2 usw.:** Der Wert des Abrechnungskurses für den Zeitraum.
   * **[!UICONTROL Startdatum]:** Das Datum, an dem die Überschreibung der Rate beginnt.
   * **[!UICONTROL Enddatum]:** Das Datum, an dem die Außerkraftsetzung der Rate endet.

     Der Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum. Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie Abrechnungsrate 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird zum Abrechnungskurs 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

1. Klicken Sie auf [!UICONTROL **Speichern**].
1. (Optional) Um eine weitere Abrechnungsrate hinzuzufügen, klicken Sie entweder für dieselbe Auftragsrolle an einem anderen Ort oder für eine andere Auftragsrolle auf [!UICONTROL **Hinzufügen von Aufgabenrollen**].
1. (Optional) Um eine Ratenkarte zu bearbeiten, klicken Sie auf den Namen der Ratenkarte in der Liste &quot;Ratenkarten&quot;in der Einrichtung. Klicken Sie auf die Schaltfläche [!UICONTROL **Auftragsrollen und -raten**] im linken Navigationsbereich der Ratenkarte. Wählen Sie dann die Rate aus und klicken Sie auf die **Bearbeiten** icon ![Symbol Bearbeiten](assets/edit-icon.png).

## Preiskarte kopieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Ratenkarten**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf die **Kopieren** icon ![Kopiersymbol](assets/copy-icon.png).
1. Geben Sie einen Namen für die Ratenkarte im [!UICONTROL Ratenkarte kopieren] , um &quot;Untitled Rate Card&quot;zu ersetzen. Klicken Sie anschließend auf **Speichern**.

   Die neue Ratenkarte wird gespeichert. Bearbeiten Sie die Details zur Ratenkarte, die Rollen und Tarife nach Bedarf.

## Gesamte Ratenkarte löschen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Ratenkarten**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf die **Löschen** icon ![Löschsymbol](assets/delete.png).

   >[!NOTE]
   >
   >Eine an ein Projekt angehängte Ratenkarte wird aus dem Projekt gelöscht.
