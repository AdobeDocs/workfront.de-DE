---
title: Deaktivieren Sie die Option für die automatische Aktualisierung für nicht bezahlte Benutzer im neuen Lizenzplan
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,standard,light,contributor
navigation-topic: access-levels
description: Jeder Benutzer muss über eine Zugriffsstufe verfügen, um sich in Workfront anmelden und arbeiten zu können. Mit der Zugriffsebene können Sie steuern, was ein Benutzer mit bestimmten Workfront-Objekten und -Bereichen sehen und tun kann.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 1ff727f1-bc26-4ffe-a510-615bebfe5b96
source-git-commit: 8807636d2309435cb5f4e08d6a7d27246342200d
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 1%

---

# Deaktivieren Sie die Option für die automatische Aktualisierung für nicht bezahlte Benutzer im neuen Lizenzplan

Die Entscheidungen über die Prüfung und die Dokumentierung sind auf alle nicht bezahlten Workfront-Lizenzen für die neuen Pläne beschränkt. Wenn Benutzer die zugewiesene Anzahl von Entscheidungen erreichen, werden sie standardmäßig auf eine Light-Lizenz aktualisiert.

Sie können die Option für die automatische Aktualisierung im Setup-Bereich deaktivieren. Weitere Informationen zur Funktionsweise von automatischen Aktualisierungen finden Sie unter [Begrenzte Dokument- und Testentscheidung für nicht bezahlte Benutzer - Überblick](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Nach der Deaktivierung wird jeder nicht bezahlte Benutzer, der die zugewiesene Anzahl von Entscheidungen überschreitet, nicht automatisch aktualisiert.


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Aktueller Plan: Standard
   <p>oder</p>
   <p>Veralteter Plan: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

## Deaktivieren Sie automatische Upgrades für nicht bezahlte Benutzer.

{{step-1-to-setup}}

1. Erweitern [!UICONTROL **System**] Klicken Sie im linken Navigationsbereich auf [!UICONTROL **Voreinstellungen**].
1. Im [!UICONTROL **Allgemeine Voreinstellungen**] -Abschnitt, überprüfen Sie die [!UICONTROL **Deaktivieren Sie die automatische Aktualisierung innerhalb der Zugriffsebenen.**] ankreuzen.
1. Klicken Sie auf [!UICONTROL **Speichern**].
