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
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Ratenkarten verwalten

{{highlighted-preview-article-level}}

Mit Ratenkarten können Sie mehrere Abrechnungsraten pro Rolle festlegen, basierend auf dem Standort. Sie könnten eine berufliche Rolle mit Designer mit Sitz in Paris und eine zweite Designer mit Sitz in New York mit jeweils unterschiedlichen Abrechnungsraten haben. Für Auftragsrollen auf einer Ratenkarte ist jedoch kein Ort erforderlich. Eine Abrechnungsrate für eine Stellenrolle (und möglicherweise einen Ort) auf einer Ratenkarte kann auch effektive Daten enthalten.

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
   <td>Zugriff auf [!UICONTROL Finanzdaten bearbeiten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Um eine für Sie freigegebene Ratenkarte zu bearbeiten, benötigen Sie die Berechtigung zum Verwalten der Ratenkarte.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Preiskarte hinzufügen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Karten mit Ratenanzahl**].
1. Klicken Sie auf [!UICONTROL **Neue Ratenkarte**] und geben Sie dann im Feld [!UICONTROL Neue Ratenkarte] einen Namen für die Ratenkarte ein, um &quot;Unbenannte Ratenkarte&quot;zu ersetzen.
1. (Optional) Fügen Sie auf dem Bildschirm &quot;Details der Ratenkarte&quot;eine [!UICONTROL **Beschreibung**] hinzu.
1. (Optional) Um ein benutzerdefiniertes Formular an die Ratenkarte anzuhängen, klicken Sie oben rechts auf das Feld [!UICONTROL **Benutzerdefiniertes Formular hinzufügen**] und wählen Sie ein benutzerdefiniertes Formular aus der angezeigten Liste aus.

   Weitere Informationen zum Anhängen eines benutzerdefinierten Formulars finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Klicken Sie im linken Navigationsbereich auf [!UICONTROL **Vorgangsrollen und -raten**] .
1. Klicken Sie auf dem Bildschirm &quot;Auftragsrollen und -raten für die Ratenkarte&quot;auf [!UICONTROL **Auftragsrolle hinzufügen**].
1. Wählen Sie im Dialogfeld eine [!UICONTROL **Auftragsrolle**] aus, für die Sie die Abrechnungsraten festlegen möchten.

   Die standardmäßige Abrechnungsrate zeigt die Rate auf Systemebene für diese Auftragsrolle an, sofern eine definiert ist.

   ![Dialogfeld &quot;Neue Abrechnungsrate&quot;](assets/location-rate-for-rate-card.png)

1. Wählen Sie eine [!UICONTROL **Währung**] für die Auftragsrolle aus.
1. (Optional) Wählen Sie eine [!UICONTROL **Position**] für die Auftragsrolle aus.
1. Geben Sie im Feld [!UICONTROL **Abrechnungsrate 1**] den Abrechnungskurs für diesen Ort ein. Klicken Sie dann auf [!UICONTROL **Speichern**] , um die Abrechnungsrate einmal zu überschreiben.

   Oder

   Klicken Sie auf [!UICONTROL **Rate hinzufügen**] , um standortspezifische Abrechnungssätze mit effektiven Datumswerten hinzuzufügen.

1. (Bedingt) Wenn Sie mehr als eine Abrechnungsrate für diesen Ort hinzufügen, geben Sie die folgenden Informationen ein:

   * **[!UICONTROL Abrechnungsrate 1], 2 usw.:** Der Wert des Abrechnungskurses für den Zeitraum.
   * **[!UICONTROL Startdatum]:** Das Datum, an dem die Überschreibung der Rate beginnt.
   * **[!UICONTROL Enddatum]:** Das Datum, an dem die Rate überschrieben wird.

     Der Abrechnungskurs 1 hat kein Startdatum und der letzte Abrechnungskurs hat kein Enddatum. Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungsrate 1 kein Enddatum hat und Sie Abrechnungsrate 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird zum Abrechnungskurs 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

1. Klicken Sie auf [!UICONTROL **Speichern**].
1. (Optional) Um eine weitere Abrechnungsrate hinzuzufügen, entweder für dieselbe Auftragsrolle an einem anderen Ort oder für eine andere Auftragsrolle, klicken Sie auf [!UICONTROL **Auftragsrolle hinzufügen**].
1. (Optional) Um eine Ratenkarte zu bearbeiten, klicken Sie auf den Namen der Ratenkarte in der Liste &quot;Ratenkarten&quot;in der Einrichtung. Um eine Abrechnungsrate zu bearbeiten, klicken Sie im linken Navigationsbereich der Ratenkarte auf [!UICONTROL **Auftragsrollen und -raten**] . Wählen Sie dann die Rate aus und klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten-Symbol](assets/edit-icon.png).

## Preiskarte kopieren

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Karten mit Ratenanzahl**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf das Symbol **Kopieren** ![Kopieren-Symbol](assets/copy-icon.png).
1. Geben Sie einen Namen für die Ratenkarte in das Feld [!UICONTROL Ratenkarte kopieren] ein, um &quot;Unbenannte Ratenkarte&quot;zu ersetzen. Klicken Sie dann auf **Speichern**.

   Die neue Ratenkarte wird gespeichert. Bearbeiten Sie die Details zur Ratenkarte, die Rollen und Tarife nach Bedarf.

## Gesamte Ratenkarte löschen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf [!UICONTROL **Karten mit Ratenanzahl**].
1. Aktivieren Sie das Kontrollkästchen neben der Ratenkarte in der Liste und klicken Sie auf das Symbol **Löschen** ![Löschen](assets/delete.png) .

   >[!NOTE]
   >
   >Eine an ein Projekt angehängte Ratenkarte wird aus dem Projekt gelöscht.
