---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Ratenkarten verwalten
description: Mit Ratenkarten können Sie mehrere Abrechnungsraten pro Rolle festlegen, basierend auf dem Standort.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '532'
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
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Veralteter Plan: [!UICONTROL Plan]</p>
       <p>Aktueller Plan: [!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf [!UICONTROL Finanzdaten bearbeiten</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
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
1. Klicken [!UICONTROL **Neue Ratenkarte**] und geben Sie dann den Namen und die Beschreibung der Ratenkarte in die Liste ein.
1. Um Abrechnungsraten hinzuzufügen, klicken Sie auf den Namen der Ratenkarte in der Liste.
1. Klicken Sie auf dem Kartenbildschirm auf [!UICONTROL **Neuer Abrechnungskurs**].
1. Wählen Sie im Dialogfeld &quot;Neue Abrechnungsrate&quot;eine [!UICONTROL **Auftragsrolle**] , um die Abrechnungsraten für festzulegen.

   Die standardmäßige Abrechnungsrate zeigt die Systemebene der Auftragsrolle an.

   ![Dialogfeld &quot;Neue Abrechnungsrate&quot;](assets/location-rate-for-rate-card.png)

1. Wählen Sie eine [!UICONTROL **Währung**] für die Rolle &quot;Arbeit&quot;.
1. (Optional) Wählen Sie eine [!UICONTROL **Standort**] für die Rolle &quot;Arbeit&quot;.
1. Im [!UICONTROL **Abrechnungskurs 1**] Geben Sie den Abrechnungskurs für diesen Ort ein. Klicken Sie anschließend auf [!UICONTROL **Speichern**] um die Abrechnungsrate einmal zu überschreiben.

   Oder

   Klicken [!UICONTROL **Rate hinzufügen**] um standortspezifischere Abrechnungssätze mit effektiven Daten hinzuzufügen.

1. (Bedingt) Wenn Sie mehr als eine Abrechnungsrate für diesen Ort hinzufügen, geben Sie die folgenden Informationen ein:

   * **[!UICONTROL Abrechnungskurs 1], 2 usw.:** Der Wert des Abrechnungskurses für den Zeitraum.
   * **[!UICONTROL Startdatum]:** Das Datum, an dem die Außerkraftsetzung der Rate beginnt.
   * **[!UICONTROL Enddatum]:** Das Datum, an dem die Außerkraftsetzung der Rate endet.

     Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum. Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie Abrechnungsrate 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird zum Abrechnungskurs 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

1. Klicken Sie auf [!UICONTROL **Speichern**].
1. (Optional) Um eine weitere Abrechnungsrate hinzuzufügen, klicken Sie entweder für dieselbe Auftragsrolle an einem anderen Ort oder für eine andere Auftragsrolle auf [!UICONTROL **Neuer Abrechnungskurs**].

## Preiskarte kopieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Ratenkarten**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf die **Kopieren** icon ![Kopiersymbol](assets/copy-icon.png).

   Eine Karte mit doppelter Rate wird hinzugefügt. Klicken Sie auf den Namen der Ratenkarte in der Liste, um ihren Namen zu ändern.

## Eine Ratenkarte löschen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Ratenkarten**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf die **Löschen** icon ![Löschsymbol](assets/delete.png).

   >[!NOTE]
   >
   >Eine an ein Projekt angehängte Ratenkarte wird aus dem Projekt gelöscht.
