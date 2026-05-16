---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivieren des Adobe-Cloud-Speichers für Ihr Unternehmen
description: Sie können Adobe Cloud Storage für Ihr Unternehmen aktivieren, um eine Unified Storage-Lösung für alle Adobe-Produkte zu verwenden.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 7%

---

# Aktivieren des Adobe-Cloud-Speichers für Ihr Unternehmen

Adobe Cloud Storage ist eine einheitliche Speicherlösung für alle Adobe-Produkte. Es handelt sich dabei um eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient.

Die Adobe-Cloud-Datenspeicherung ist standardmäßig für neue Kunden aktiviert und kann für Bestandskunden bei Vertragsverlängerung aktiviert werden.

Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebiges Workflow-Paket</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Aktivieren des Adobe-Cloud-Speichers für Ihr Unternehmen

So aktivieren Sie die Adobe-Cloud-Datenspeicherung für Ihr Unternehmen:

{{step-1-to-setup}}

1. Wählen Sie **linken Navigationsbereich** System“ und dann **Voreinstellungen** aus.
1. Scrollen Sie nach unten zum Abschnitt **Speichereinstellungen**.
1. Wählen Sie im Dropdown-Menü Standard die Option **Adobe Cloud-Speicher**.
1. (Optional) Wenn Sie eine Kombination aus Adobe-Cloud-Speicher und Legacy-Workfront-Speicher verwenden möchten, aktivieren Sie das Kontrollkästchen **Auswahl des Speicheranbieters durch den Benutzer**.

   >[!NOTE]
   >
   >Wenn diese Option aktiviert ist, können Benutzer den Speicheranbieter auswählen, wenn sie ein neues Projekt erstellen. Der Adobe-Cloud-Speicher wird als „Neues Projekt“ gekennzeichnet, da er der standardmäßige Speicheranbieter ist. Legacy-Workfront-Speicher wird als „Legacy-Projekt“ bezeichnet.
   >
   >![Optionen für neue Projekte und veraltete Projekte](assets/new-esm-project.png)

1. Wählen Sie im Dropdown-Menü Gilt für eine der folgenden Optionen:

   - **Gesamte Organisation**: Mit dieser Option wird der standardmäßige Speicheranbieter auf die gesamte Workfront-Umgebung angewendet. Jedes Mal, wenn ein Benutzer ein neues Projekt erstellt, wird der standardmäßige Speicheranbieter verwendet.
   - **Spezifische Gruppen**: Mit dieser Option wird der standardmäßige Speicheranbieter nur auf bestimmte Gruppen in Ihrer Organisation angewendet. Jedes Mal, wenn ein Benutzer in den angegebenen Gruppen ein neues Projekt erstellt, wird der standardmäßige Speicheranbieter verwendet

1. Klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Vorhandene Projekte behalten das Speichermodell bei, mit dem sie erstellt wurden. Beispielsweise verwenden Projekte, die den Adobe-Cloud-Speicher verwenden, weiterhin den Adobe-Cloud-Speicher, nachdem Sie die standardmäßige Speichervoreinstellung geändert haben.

## Adobe Cloud-Speicher in Sandbox-Umgebungen

Der Adobe-Cloud-Speicher ist in [!DNL Workfront] Sandbox-Umgebungen verfügbar, sodass Sie die in diesem Artikel beschriebenen Funktionen testen können, bevor Sie sie in der Produktion einführen. Der Frame.io-Viewer ist jedoch nicht in Sandbox verfügbar, sodass das vollständige, einheitliche Überprüfungs- und Validierungserlebnis in der Produktion validiert werden muss.

Wenn Sie über eine benutzerdefinierte Aktualisierungs-Sandbox verfügen, müssen Sie sie nach dem Upgrade auf eine Version von Workfront aktualisieren, die den Adobe-Cloud-Speicher unterstützt. Durch die Aktualisierung erhält die Sandbox Zugriff auf die Adobe-Cloud-Speicherfunktion, damit Sie mit dem Testen beginnen können. Weitere Informationen finden Sie unter [Die benutzerdefinierte  [!DNL Adobe Workfront] -Sandbox-Umgebung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
