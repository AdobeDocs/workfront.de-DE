---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Löschen von Vorgangsrollen
description: Sie können Auftragsrollen löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, keine Auftrags-Rollen zu löschen, wenn sie bereits in der Vergangenheit mit Arbeitselementen verknüpft wurden. Um all Ihre historischen Informationen zu Arbeitsaufträgen zu erhalten, empfehlen wir, Rollen zu deaktivieren, anstatt sie zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter Deaktivieren von Vorgangsrollen .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Löschen von Vorgangsrollen

Sie können Auftragsrollen löschen, die Ihr Unternehmen nicht mehr verwendet. Es wird empfohlen, keine Auftrags-Rollen zu löschen, wenn sie bereits in der Vergangenheit mit Arbeitselementen verknüpft wurden.

Um all Ihre historischen Informationen zu Arbeitsaufträgen zu erhalten, empfehlen wir, Rollen zu deaktivieren, anstatt sie zu löschen, wenn sie veraltet sind. Informationen zum Deaktivieren von Rollen finden Sie unter [Deaktivieren von Vorgangsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf die Rollen "Aufträge"</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Löschen von Auftragsrollen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Vorgangsrollen].**
1. Wählen Sie die Auftragsrolle aus, die Sie löschen möchten, und klicken Sie dann auf **[!UICONTROL Löschen].**
1. Führen Sie einen der folgenden Schritte aus, wenn der Auftragsrolle Objekte (Benutzer, Aufgaben, Probleme) zugewiesen sind:

   * **Ersetzen Sie die Auftragsrolle durch eine andere Auftragsrolle:** Wählen Sie aus der Dropdown-Liste die neue Auftragsrolle aus.

      Sämtliche aktuellen und vergangene Ressourcenzuweisungen, die mit der Rolle &quot;gelöschter Auftrag&quot;verknüpft sind, werden an die von Ihnen ausgewählte Auftragsrolle übertragen.

      Benutzer, denen nur eine Rolle zugewiesen wurde, werden der von Ihnen ausgewählten Rolle &quot;Job&quot;zugewiesen. Benutzern, denen eine sekundäre Rolle zugewiesen wurde, wird nicht die von Ihnen ausgewählte Rolle zugewiesen.

   * **Löschen Sie die Auftrags- und Ressourcenzuordnung:** Auswählen **[!UICONTROL Keines]** aus der Dropdown-Liste aus.

      >[!IMPORTANT]
      >
      >Durch Löschen einer Auftragsrolle werden alle aktuellen und vergangene Ressourcenzuweisungen, die sich auf diese Stellenrolle beziehen, für alle Projekte gelöscht.

      &#x200B; z. B. wenn eine Aufgabe oder ein Problem nur dieser Aufgabenrolle zugewiesen ist, wird die Zuweisung der Aufgabe oder des Problems aufgehoben, nachdem die Auftragsrolle gelöscht wurde.

1. Klicken  **[!UICONTROL Ja, löschen]**.
