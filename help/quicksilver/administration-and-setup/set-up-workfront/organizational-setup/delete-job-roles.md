---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Aufgabengebiete löschen
description: Sie können Auftragsrollen löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, keine Auftrags-Rollen zu löschen, wenn sie bereits in der Vergangenheit mit Arbeitselementen verknüpft wurden. Um all Ihre historischen Informationen zu Arbeitsaufträgen zu erhalten, empfehlen wir, Rollen zu deaktivieren, anstatt sie zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter Deaktivieren von Vorgangsrollen .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Löschen von Vorgangsrollen

Sie können Auftragsrollen löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, keine Auftrags-Rollen zu löschen, wenn sie bereits in der Vergangenheit mit Arbeitselementen verknüpft wurden.

Um all Ihre historischen Informationen zu Arbeitsaufträgen zu erhalten, empfehlen wir, Rollen zu deaktivieren, anstatt sie zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter [Deaktivieren von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: [!UICONTROL Standard]</p>
   <p>Oder</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Administratorzugriff auf Auftragsrollen</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen von Auftragsrollen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Vorgangsrollen].**
1. Wählen Sie die Auftragsrolle aus, die Sie löschen möchten, und klicken Sie dann auf **[!UICONTROL Löschen].**
1. Führen Sie einen der folgenden Schritte aus, wenn der Auftragsrolle Objekte (Benutzer, Aufgaben, Probleme) zugewiesen sind:

   * **Ersetzen Sie die Auftragsrolle durch eine andere Auftragsrolle:** Wählen Sie die neue Auftragsrolle aus der Dropdownliste aus.

     Sämtliche aktuellen und vergangene Ressourcenzuweisungen, die mit der Rolle &quot;gelöschter Auftrag&quot;verknüpft sind, werden an die von Ihnen ausgewählte Auftragsrolle übertragen.

     Benutzer, denen nur eine Rolle zugewiesen wurde, werden der von Ihnen ausgewählten Rolle als Job zugewiesen. Benutzer, denen eine Rolle als sekundärer Job zugewiesen wurde, werden nicht der von Ihnen ausgewählten Rolle als Job zugewiesen.

   * **Löschen Sie die Auftrags- und Ressourcenzuordnung:** Wählen Sie **[!UICONTROL Keine]** aus der Dropdownliste aus.

     >[!IMPORTANT]
     >
     >Durch Löschen einer Auftragsrolle werden alle aktuellen und vergangene Ressourcenzuweisungen, die sich auf diese Stellenrolle beziehen, für alle Projekte gelöscht.

     &#x200B; z. B. wenn eine Aufgabe oder ein Problem nur dieser Aufgabenrolle zugewiesen ist, wird die Zuweisung der Aufgabe oder des Problems aufgehoben, nachdem die Auftragsrolle gelöscht wurde.

1. Klicken Sie auf **[!UICONTROL Ja, löschen Sie es]**.
