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
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# Deaktivieren Sie die Option für die automatische Aktualisierung für nicht bezahlte Benutzer im neuen Lizenzplan

Die Entscheidungen über die Prüfung und die Dokumentierung sind auf alle nicht bezahlten Workfront-Lizenzen für die neuen Pläne beschränkt. Wenn Benutzer die zugewiesene Anzahl von Entscheidungen erreichen, werden sie standardmäßig auf eine Light-Lizenz aktualisiert.

Sie können die Option für die automatische Aktualisierung im Setup-Bereich deaktivieren. Weitere Informationen zur Funktionsweise von automatischen Aktualisierungen finden Sie unter [Begrenzte Dokument- und Testentscheidung für nicht bezahlte Benutzer - Übersicht](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

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
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Neuer Plan: Standard
   <p>oder</p>
   <p>Aktueller Plan: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

## Deaktivieren Sie automatische Upgrades für nicht bezahlte Benutzer.

{{step-1-to-setup}}

1. Erweitern Sie [!UICONTROL **System**] im linken Navigationsbereich und klicken Sie dann auf [!UICONTROL **Voreinstellungen**].
1. Aktivieren Sie im Abschnitt [!UICONTROL **Allgemeine Voreinstellungen**] die Option [!UICONTROL **Automatische Aktualisierung in Zugriffsebenen deaktivieren**] .
1. Klicken Sie auf [!UICONTROL **Speichern**].
