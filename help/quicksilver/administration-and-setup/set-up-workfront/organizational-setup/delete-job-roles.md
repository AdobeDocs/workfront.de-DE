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
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Aufgabengebiete löschen

Sie können Aufgabengebiete löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, Aufgabengebiete nicht zu löschen, wenn sie in der Vergangenheit mit Arbeitselementen verknüpft waren.

Um alle historischen Informationen über Arbeitsaufträge zu speichern, empfehlen wir, Rollen zu deaktivieren und nicht zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter [Deaktivieren von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: [!UICONTROL Standard]</p>
   <p>Oder</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Administrativer Zugriff auf Aufgabengebiete</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
