---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivieren des Adobe-Cloud-Speichers für Ihr Unternehmen
description: Sie können Adobe Cloud Storage für Ihr Unternehmen aktivieren, um eine Unified Storage-Lösung für alle Adobe-Produkte zu verwenden.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 5d487a068f747eb538775846cca80ab5a3a612bf
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 5%

---
# Aktivieren des Adobe-Cloud-Speichers für Ihr Unternehmen

Adobe Cloud-Speicher ist eine einheitliche, Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient. In diesem Artikel wird beschrieben, wie Sie die Adobe-Cloud-Datenspeicherung als standardmäßige Speicheroption für Ihr gesamtes Unternehmen oder für bestimmte Gruppen aktivieren.

>[!IMPORTANT]
>
>Ihre Umgebung ändert sich erst, wenn Sie die Adobe-Cloud-Datenspeicherung im Bereich „Setup“ von Workfront aktivieren.<br>
>Sobald Sie die Adobe-Cloud-Datenspeicherung aktiviert haben, verwenden nur noch neue Projekte den Adobe-Cloud-Speicher, der die Viewer-Genehmigungen Frame.io und Unified Approvals enthält. Ihre vorhandenen Projekte nutzen weiterhin ihren aktuellen Speicher und bleiben unberührt.

Da Sie den zeitlichen Ablauf steuern, können Sie das Erlebnis testen, Ihre Workfront Fusion-Szenarien aktualisieren und Berichtsänderungen planen, bevor jemand damit arbeitet. Weitere Informationen zu den Unterschieden und zur Planung des Rollouts finden Sie unter [Wechseln zu Workfront auf Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Funktionsweise von Genehmigungen mit Adobe Cloud Storage

Der Adobe-Cloud-Speicher bestimmt, welchen Validierungs-Service ein Projekt verwendet. Der Wechsel zu einer Version von Workfront, die Adobe Cloud Storage unterstützt, schaltet nicht automatisch Ihr gesamtes Unternehmen auf einheitliche Genehmigungen um. Stattdessen hängt der Validierungs-Service vom Speichermodell jedes Projekts ab:

* **Adobe-Cloud-**: Verwenden Sie standardmäßig einheitliche Genehmigungen, mit Prüfung und Genehmigung im Frame.io-Viewer.
* **Ältere Workfront-Speicherprojekte** Behalten Sie den von ihnen bereits verwendeten Validierungs-Service bei. Abhängig von Ihrem Unternehmen kann dies einheitliche Genehmigungen oder Legacy-Dokumentgenehmigungen sein.

Weitere Informationen zur Überprüfung und Genehmigung von Adobe Cloud Storage finden Sie unter [Wechseln zu Workfront auf Adobe Cloud Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

   * **Gesamte Organisation**: Mit dieser Option wird der standardmäßige Speicheranbieter auf die gesamte Workfront-Umgebung angewendet. Jedes Mal, wenn ein Benutzer ein neues Projekt erstellt, wird der standardmäßige Speicheranbieter verwendet.
   * **Spezifische Gruppen**: Mit dieser Option wird der standardmäßige Speicheranbieter nur auf bestimmte Gruppen in Ihrer Organisation angewendet. Jedes Mal, wenn ein Benutzer in den angegebenen Gruppen ein neues Projekt erstellt, wird der standardmäßige Speicheranbieter verwendet.

     ![Speichergruppen - Voreinstellungen](assets/configure-storage-preference.png)

1. Klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Vorhandene Projekte behalten das Speichermodell bei, mit dem sie erstellt wurden. Beispielsweise verwenden Projekte, die den Adobe-Cloud-Speicher verwenden, weiterhin den Adobe-Cloud-Speicher, nachdem Sie die standardmäßige Speichervoreinstellung geändert haben.



## Adobe Cloud-Speicher in Sandbox-Umgebungen

Der Adobe-Cloud-Speicher ist in [!DNL Workfront] Sandbox-Umgebungen verfügbar, sodass Sie die in diesem Artikel beschriebenen Funktionen testen können, bevor Sie sie in der Produktion einführen. Der Frame.io-Viewer ist jedoch nicht in Sandbox verfügbar, sodass das vollständige, einheitliche Überprüfungs- und Validierungserlebnis in der Produktion validiert werden muss.

Wenn Sie über eine benutzerdefinierte Aktualisierungs-Sandbox verfügen, müssen Sie sie nach dem Upgrade auf eine Version von Workfront aktualisieren, die den Adobe-Cloud-Speicher unterstützt. Durch die Aktualisierung erhält die Sandbox Zugriff auf die Adobe-Cloud-Speicherfunktion, damit Sie mit dem Testen beginnen können. Weitere Informationen finden Sie unter [Die benutzerdefinierte  [!DNL Adobe Workfront] -Sandbox-Umgebung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).
