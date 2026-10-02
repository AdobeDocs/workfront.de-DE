---
user-type: administrator
product-area: system-administration;setup
title: Konfigurieren der benutzerdefinierten Lokalisierung
description: Benutzerdefinierte Lokalisierung ermöglicht es Ihnen, benutzerdefinierte Begriffe und Ausdrücke in verschiedenen Sprachen zu definieren. Workfront zeigt diese Begriffe dann in der Sprache an, die in den Browsereinstellungen festgelegt ist.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 5%
---
# Konfigurieren der benutzerdefinierten Lokalisierung

{{highlighted-preview}}

Mit der benutzerdefinierten Lokalisierung können Sie <span class="preview"> KI verwenden</span> um benutzerdefinierte Begriffe und Ausdrücke in verschiedenen Sprachen zu definieren. Workfront zeigt diese Begriffe dann in der Sprache an, die in den Adobe Identity Management (IMS)-Einstellungen des Benutzers festgelegt ist.

Beispielsweise kann die Bezeichnung „Zielgruppe“ in das deutsche Wort „Zielgruppe“ übersetzt werden. Jeder Benutzer, dessen Deutsch als Hauptsprache seines Browsers ausgewählt wurde, sieht das Wort „Zielgruppe“ als Bezeichnung für alle Felder, die auf Englisch mit „Zielgruppe“ gekennzeichnet sind.

Sie können Übersetzungen in mehrere Sprachen konfigurieren. Derzeit verfügbare Sprachen:

* Chinesisch (traditionell)
* Chinesisch (vereinfacht)
* Französisch
* Deutsch
* Italienisch
* Japanisch
* Koreanisch
* Portugiesisch (Brasilien)
* Spanisch

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Workflow-Prime oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein, um Übersetzungen konfigurieren zu können.</p>  </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Überlegungen beim Festlegen von Lokalisierungen

Beachten Sie beim Konfigurieren der Lokalisierung Folgendes:

* Sie können einen Begriff so konfigurieren, dass er in mehrere Sprachen übersetzt wird.
* Die Lokalisierung gilt für benutzerdefinierte Feldbeschriftungen (einschließlich bei Verwendung als Spaltenüberschrift) und QuickInfos.
* Die benutzerdefinierte Lokalisierung kann auf Nachrichten angewendet werden, die aus Geschäftsregeln generiert werden, muss aber in der Geschäftsregel aktiviert werden.

  Anweisungen finden Sie unter [Aktivieren der Lokalisierung in einer Geschäftsregel](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) im Artikel Erstellen und Bearbeiten von Geschäftsregeln.

## Übersetzungen konfigurieren

Übersetzungen werden im Bereich Setup konfiguriert.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im Bereich Setup **linken** auf „Lokalisierung“.
1. Um eine neue Übersetzung hinzuzufügen, klicken Sie auf **Neue Zeile**.
1. Geben Sie in **Spalte &quot;**&quot; den englischen Begriff ein, der übersetzt werden soll.
1. Geben Sie in der Spalte für die Sprache, in die der Begriff übersetzt werden soll, den Begriff in der Zielsprache ein.
1. (Optional) Um das Wort in zusätzliche Sprachen zu übersetzen, fügen Sie die Übersetzung in die entsprechende Sprachspalte hinzu.
1. (Optional) Um die Sprachspalten neu anzuordnen, klicken Sie auf die Kopfzeile einer Spalte, die Sie verschieben möchten, und ziehen Sie sie an die gewünschte Position.
1. (Optional) Um Übersetzungen für einen Begriff zu löschen, aktivieren Sie das Kontrollkästchen neben dem Begriff und klicken **unten auf der Seite in** blauen Leiste auf „Löschen“.

<div class="preview">

## Lokalisieren von nicht übersetztem benutzerdefiniertem Text mithilfe von KI-Übersetzungen

Sie können KI verwenden, um benutzerdefinierten Text zu lokalisieren. Sie wählen den Begriff und die Sprachen aus und können die Übersetzungen genehmigen, bevor sie angewendet werden.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im Bereich Setup **linken** auf „Lokalisierung“.
1. Wählen Sie im Bereich Lokalisierung die Registerkarte **Nicht übersetzter benutzerdefinierter Text** aus.

   Eine Liste mit nicht übersetztem benutzerdefiniertem Text wird angezeigt. Dazu gehören Text wie Feldbezeichnungen und benutzerdefinierte Regelmeldungen.

1. Wählen Sie einen oder mehrere Begriffe aus, die Sie lokalisieren möchten.
1. Wählen Sie in der blauen Leiste am unteren Bildschirmrand **Mit KI übersetzen** aus.

   Das Fenster Übersetzungen erstellen wird geöffnet.

1. Klicken Sie auf die Sprachen, in die Sie den Begriff oder die Begriffe übersetzen möchten. Um schnell alle Sprachen auszuwählen, klicken Sie auf **Alle auswählen**.
1. (Optional) Um eine spezifischere Anleitung für die Übersetzung bereitzustellen, geben Sie Anweisungen in das Feld „Anweisungen für KI“ ein.
1. Klicken Sie auf **Generieren**.

   KI beginnt mit der Erstellung von Übersetzungen.

   Das Fenster Übersetzungen überprüfen wird geöffnet.

1. (Optional) Um Übersetzungen anzupassen oder eine eigene Übersetzung hinzuzufügen, klicken Sie auf das entsprechende Quadrat der Tabelle und geben Sie die gewünschte Übersetzung ein.
1. Klicken Sie auf **Speichern**.

## Übersetzen Sie einen lokalisierten Begriff in zusätzliche Sprachen.

Sie können einen bereits lokalisierten Begriff mithilfe von KI in neue Sprachen übersetzen oder Ihre eigene Übersetzung bereitstellen.

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im Bereich Setup **linken** auf „Lokalisierung“.
1. Wählen Sie im Bereich Lokalisierung die Registerkarte **Übersetzungen** aus.

   Eine Liste der zuvor übersetzten Begriffe und der zugehörigen Übersetzungen wird angezeigt.

1. (Optional) Um eine Übersetzung zu bearbeiten oder direkt einzugeben, klicken Sie in der Tabelle auf das entsprechende Feld und geben Sie die gewünschte Übersetzung ein.
1. Wählen Sie die Begriffe aus, für die Sie zusätzliche Übersetzungen generieren möchten, indem Sie die Kontrollkästchen neben diesen Begriffen aktivieren.
1. Klicken Sie in der blauen Leiste unten auf der Seite auf **Mit KI ausfüllen**.


   Das Fenster Übersetzungen erstellen wird geöffnet.

1. Klicken Sie auf die Sprachen, in die Sie den Begriff oder die Begriffe übersetzen möchten. Um schnell alle Sprachen auszuwählen, klicken Sie auf **Alle auswählen**.
1. (Optional) Um eine spezifischere Anleitung für die Übersetzung bereitzustellen, geben Sie Anweisungen in das Feld „Anweisungen für KI“ ein.
1. Klicken Sie auf **Generieren**.

   KI beginnt mit der Erstellung von Übersetzungen.

   Das Fenster Übersetzungen überprüfen wird geöffnet.

1. (Optional) Um Übersetzungen anzupassen oder eine eigene Übersetzung hinzuzufügen, klicken Sie auf das entsprechende Quadrat der Tabelle und geben Sie die gewünschte Übersetzung ein.
1. Klicken Sie auf **Speichern**.
1. (Optional) Um alle Übersetzungen für einen Begriff zu löschen, aktivieren Sie das Kontrollkästchen neben dem Begriff und klicken **auf „Löschen** in der blauen Leiste unten auf der Seite.


</div>
