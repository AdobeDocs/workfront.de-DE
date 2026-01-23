---
product-area: documents
navigation-topic: approvals
title: Einrichten von Marken für den KI-Reviewer
description: Einrichten von Marken für den KI-Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cd2a5560fdf446e8e971afcb640af38b4d301d40
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 5%

---

# Einrichten von Marken für den KI-Reviewer

>[!IMPORTANT]
>
>Diese Funktion befindet sich derzeit in der Betaphase.

Der KI-Reviewer verwendet Markenrichtlinien, um Inhalte während des Überprüfungsprozesses zu bewerten. Sie können in Workfront Marken erstellen, indem Sie PDF-Dateien mit Ihren Markenrichtlinien hochladen oder manuell Markenelemente eingeben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Systemadministrator sein.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console-Berechtigungen</td> 
   <td> <p>Sie müssen GenStudio Brand Manager verwenden.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Voraussetzungen

* Ihr Unternehmen muss zu Adobe IMS (Identity Management System) migriert sein.
* Für Ihre Workfront-Instanz müssen einheitliche Genehmigungen aktiviert sein.
* Ihr Unternehmen muss über GenStudio Foundation verfügen.
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.
Weitere Informationen zur Unterzeichnung des Abkommens finden Sie unter [Unterzeichnung des Adobe Gen AI-Abkommens](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## Erstellen einer Marke mit einer PDF

{{step-1-to-setup}}

1. Navigieren Sie im linken Bereich zu **Überprüfen und**) > **Marken**.
1. Klicken **oben rechts** Bildschirm auf „Marke hinzufügen“.
1. Benennen Sie die Marke.
1. Klicken Sie auf PDF hochladen , um Markendateien hochzuladen.
   ![Marken-PDFs hochladen](assets/upload-PDF.png)
1. Klicken Sie auf **Fortfahren**.
1. Laden Sie eine oder mehrere PDF-Dateien hoch, die Ihre Markenrichtlinien enthalten, und klicken Sie dann auf **Marke hinzufügen**.
1. Überprüfen Sie nach dem Hochladen der Dateien die extrahierten Markenelemente, um sicherzustellen, dass sie mit Ihren Markenrichtlinien übereinstimmen.

   >[!IMPORTANT]
   >
   >Richtlinien werden mithilfe Ihrer -Dateien und der Technologie der generativen KI generiert und können ungenau sein. Lesen Sie die extrahierten Richtlinien auf fehlende oder falsche Details und bearbeiten Sie sie, bevor Sie diese Marke veröffentlichen.

1. Klicken Sie abschließend auf **Veröffentlichen**, um die Marke für den KI-Reviewer verfügbar zu machen.

## Manuelles Erstellen einer Marke

{{step-1-to-setup}}

1. Navigieren Sie im linken Bereich zu **Überprüfen und**) > **Marken**.
1. Klicken **oben rechts** Bildschirm auf „Marke hinzufügen“.
1. Benennen Sie die Marke.
1. Klicken Sie **Manuell hinzufügen**, um eine Marke mit einzelnen Elementen zu erstellen.
1. Füllen Sie die Markendetails nach Bedarf aus. Sie können die folgenden Elemente hinzufügen:

   <table>
    <tr>
        <td>Verwendungszeitpunkt</td>
        <td>Informieren Sie die Marketing-Fachleute darüber, wann diese Marke verwendet werden sollte.</td>
    </tr>
    <tr>
        <td>Sprachrichtlinien</td>
        <td>Geben Sie Anleitungen zu Ton und Stil der Markenstimme.</td>
    </tr>
    <tr>
        <td>Bildrichtlinien</td>
        <td>Geben Sie die Arten von Bildern an, die mit der Identität der Marke übereinstimmen.</td>
    </tr>
    <tr>
        <td>Kanalrichtlinien</td>
        <td>Beschreiben Sie die geeigneten Kanäle für die Markenkommunikation.</td>
    </tr>
    <tr>
        <td>Logos</td>
        <td>Fügen Sie die offiziellen Logos der Marke hinzu.</td>
    </tr>
    <tr>
        <td>Farben</td>
        <td>Geben Sie die Farbpalette der Marke an.</td>
    </tr>
    </table>

   ![Manuelles Hinzufügen von Markenelementen](assets/brand-elements.png)


1. Klicken Sie abschließend auf **Veröffentlichen**, um die Marke für den KI-Reviewer verfügbar zu machen.
