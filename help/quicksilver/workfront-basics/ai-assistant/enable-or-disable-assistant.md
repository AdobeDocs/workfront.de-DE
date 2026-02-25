---
title: Aktivieren oder Deaktivieren des KI-Assistenten
content-type: reference
description: Sie können steuern, welche Zugriffsebenen in Ihrer Organisation Zugriff auf den KI-Assistenten haben.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 14%

---

# Aktivieren oder Deaktivieren des KI-Assistenten

Als Workfront-Administrator können Sie steuern, für welche Benutzenden in Ihrem Unternehmen der KI-Assistent aktiviert ist. Dies wird über Zugriffsebenen verwaltet.

Sie müssen den KI-Assistenten für Ihre Organisation aktivieren, bevor Sie ihn für eine Zugriffsebene aktivieren können.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Aktivieren oder Deaktivieren des KI-Assistenten für Ihre Organisation

So aktivieren Sie den KI-Assistenten für Ihr Unternehmen:

{{step-1-to-setup}}

1. Wählen Sie **linken Navigationsbereich** System“ und dann **Voreinstellungen** aus.
1. Scrollen Sie nach unten zum Abschnitt **KI-Voreinstellungen** .
1. Schalten Sie den Umschalter **KI aktivieren** ein.

>[!IMPORTANT]
>
>Sie müssen über eine unterzeichnete Gen-KI-Vereinbarung mit Adobe verfügen, bevor Sie den KI-Assistenten verwenden können.
>Weitere Informationen zum Gen-AI-Abkommen finden Sie unter [Unterzeichnung des Adobe-Gen-AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)Abkommens im Artikel KI-Assistent in Workfront.

## Aktivieren oder Deaktivieren des KI-Assistenten für eine Zugriffsebene

So aktivieren Sie den KI-Assistenten für eine bestimmte Zugriffsebene:

{{step-1-to-setup}}

1. Wählen **Zugriffsebenen** in der linken Navigationsleiste aus.
1. Wählen Sie die gewünschte Zugriffsebene aus und klicken Sie dann auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png) oberhalb der Liste.
1. Deaktivieren Sie im Bereich **Zusätzliche Einschränkungen festlegen…** des Kontrollkästchens **Zugriffsebene bearbeiten** das Kontrollkästchen **Workfront-KI-Assistenten deaktivieren**.
1. Klicken Sie auf **Speichern**.
1. Wiederholen Sie die Schritte 3-5 für jede Zugriffsebene, für die Sie den KI-Assistenten aktivieren möchten.



>[!NOTE]
>
>* Der KI-Assistent ist für Benutzende ohne Administratorrechte standardmäßig deaktiviert.
>* Wenn Benutzende ohne Administratorrechte mit dem Symbol KI-Assistent in Workfront interagieren, werden sie in der KI-Assistentenvereinbarung aufgefordert, die Nutzungsbedingungen zu akzeptieren. Wenn er/sie die Vereinbarung akzeptiert, kann er/sie den KI-Assistenten verwenden, obwohl er/sie in seiner Layout-Vorlage deaktiviert ist.

