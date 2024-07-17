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
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf die Rollen "Aufträge"</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Löschen von Auftragsrollen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

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
