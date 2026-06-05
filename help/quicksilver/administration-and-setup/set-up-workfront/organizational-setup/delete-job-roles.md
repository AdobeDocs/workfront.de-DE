---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Aufgabengebiete löschen
description: Sie können Aufgabengebiete löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, Aufgabengebiete nicht zu löschen, wenn sie in der Vergangenheit mit Arbeitselementen verknüpft waren. Um alle historischen Informationen über Arbeitsaufträge zu speichern, empfehlen wir, Rollen zu deaktivieren und nicht zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter Deaktivieren von Aufgabengebieten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
TQID: https://experienceleague.adobe.com/jJA7M34HwNyM-906Poo9-uTVmB4kQnXMv8iBWminjjg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 9%

---

# Löschen von Aufgabengebieten

Sie können Aufgabengebiete löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, Aufgabengebiete nicht zu löschen, wenn sie in der Vergangenheit mit Arbeitselementen verknüpft waren.

Um alle historischen Informationen über Arbeitsaufträge zu speichern, empfehlen wir, Rollen zu deaktivieren und nicht zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter [Deaktivieren von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Zugriffsanforderungen

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf Aufgabengebiete</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Aufgabengebiet löschen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Aufgabengebiete].**
1. Wählen Sie das Aufgabengebiet aus, das Sie löschen möchten, und klicken Sie dann auf **[!UICONTROL Löschen].**
1. Wenn Objekte (Benutzer, Aufgaben, Probleme) vorhanden sind, die dem Aufgabengebiet zugewiesen sind, führen Sie einen der folgenden Schritte aus:

   * **Ersetzen Sie das Aufgabengebiet durch ein anderes Aufgabengebiet:** Wählen Sie das neue Aufgabengebiet aus der Dropdown-Liste aus.

     Alle aktuellen und vergangenen Ressourcenzuteilungen, die mit dem gelöschten Aufgabengebiet verknüpft sind, werden in das von Ihnen ausgewählte Aufgabengebiet übertragen.

     Benutzende, denen nur ein Aufgabengebiet zugewiesen wurde, werden dem von Ihnen ausgewählten Aufgabengebiet neu zugewiesen. Benutzende, denen ein sekundäres Aufgabengebiet zugewiesen wurde, werden nicht dem von Ihnen ausgewählten Aufgabengebiet neu zugewiesen.

   * **Aufgabengebiet und Ressourcenzuordnung löschen:** Wählen Sie **[!UICONTROL Keine]** aus der Dropdown-Liste aus.

     >[!IMPORTANT]
     >
     >Durch das Löschen eines Aufgabengebiets wird die gesamte aktuelle und frühere Ressourcenzuordnung im Zusammenhang mit diesem Aufgabengebiet für alle Projekte gelöscht.

     &#x200B;Wenn beispielsweise eine Aufgabe oder ein Problem nur diesem Aufgabengebiet zugewiesen ist, wird die Zuweisung der Aufgabe oder des Problems aufgehoben, nachdem das Aufgabengebiet gelöscht wurde.

1. Klicken Sie **[!UICONTROL Ja, löschen]**.
