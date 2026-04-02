---
user-type: administrator
product-area: system-administration;setup
title: Konfigurieren der benutzerdefinierten Lokalisierung
description: Benutzerdefinierte Lokalisierung ermöglicht es Ihnen, benutzerdefinierte Begriffe und Ausdrücke in verschiedenen Sprachen zu definieren. Workfront zeigt diese Begriffe dann in der Sprache an, die in den Browsereinstellungen festgelegt ist.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 18211a3529b612a6fcdcedf7820aecfe38cb3b6f
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 10%

---

# Konfigurieren der benutzerdefinierten Lokalisierung

Benutzerdefinierte Lokalisierung ermöglicht es Ihnen, benutzerdefinierte Begriffe und Ausdrücke in verschiedenen Sprachen zu definieren. Workfront zeigt diese Begriffe dann in der Sprache an, die in den Einstellungen für Adobe Identity Management (IMS) des Benutzers festgelegt ist. Wenn der Benutzer nicht über Adobe IMS verfügt, werden die Begriffe in der Sprache angezeigt, die in den Browser-Einstellungen des Benutzers festgelegt ist.

Beispielsweise können Sie die Bezeichnung „Zielgruppe“ so einstellen, dass das deutsche Wort „Zielgruppe“ übersetzt wird. Jeder Benutzer, dessen Deutsch als Hauptsprache seines Browsers ausgewählt wurde, sieht das Wort „Zielgruppe“ als Bezeichnung für alle Felder, die auf Englisch mit „Zielgruppe“ gekennzeichnet sind.

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

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **** Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im Bereich Setup **linken** auf „Lokalisierung“.
1. Um eine neue Übersetzung hinzuzufügen, klicken Sie auf **Neue Zeile**.
1. Geben Sie in **Spalte &quot;**&quot; den englischen Begriff ein, der übersetzt werden soll.
1. Geben Sie in der Spalte für die Sprache, in die der Begriff übersetzt werden soll, den Begriff in der Zielsprache ein.
1. Um das Wort in zusätzliche Sprachen zu übersetzen, fügen Sie die Übersetzung in die entsprechende Sprachspalte hinzu.
1. Um die Sprachspalten neu anzuordnen, klicken Sie auf die Kopfzeile einer Spalte, die Sie verschieben möchten, und ziehen Sie sie an die gewünschte Position.
