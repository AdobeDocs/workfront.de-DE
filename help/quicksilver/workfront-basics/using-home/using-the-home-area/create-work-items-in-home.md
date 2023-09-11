---
product-area: projects
navigation-topic: use-the-home-area
title: Erstellen von Arbeitselementen aus dem Startbereich
description: Erstellen von Arbeitselementen aus dem Startbereich
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: ecbba9b1da674328df866ec30e48fe44dd02cb86
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# Erstellen von Arbeitselementen aus dem Startbereich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

Sie können Arbeitselemente aus dem [!UICONTROL Startseite] Bereich. Sie können persönliche Aufgaben für sich selbst erstellen, Arbeiten von anderen Benutzern anfordern oder Aufgaben zu bestimmten Projekten hinzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker]</p> <p><b>NOTIZ</b></p> 
   <p>Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher für Aufgaben</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Persönliche Aufgabe erstellen

Sie können eine persönliche Aufgabe erstellen, die nur Ihnen im [!UICONTROL Startseite] Bereich:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Klicks **[!UICONTROL Neue Aufgabe]** > **[!UICONTROL Persönlich]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. Im **[!UICONTROL Name]** -Feld einen Namen für die Aufgabe angeben.
1. (Optional) Klicken Sie auf **[!UICONTROL Datum auswählen]** und wählen Sie dann das Datum aus, an dem die Aufgabe fällig wird. Dadurch wird die [!UICONTROL Geplantes Abschlussdatum] für die Aufgabe.\
   Sie können die **[!UICONTROL Geplantes Abschlussdatum]** durch Klicken auf das Datum im rechten Bereich oder durch Bearbeiten der **[!UICONTROL Dies geschieht durch]** Datum direkt in der Aufgabe.

1. Klicks **[!UICONTROL Erstellen]** , um die Aufgabe zu speichern.\
   Die Aufgabe wird Ihnen zugewiesen und ist im [!UICONTROL Startseite] Bereich.

>[!NOTE]
>
>* Wenn Sie eine persönliche Aufgabe erstellen, wird sie in einem &quot;ausgeblendeten&quot;Projekt gespeichert, das in [!UICONTROL Workfront]. Das Projekt trägt den Namen &quot;&lt; Benutzername >&#39;s Tasks&quot;. Der &quot;Benutzername&quot;ist der vollständige Name des Benutzers, der die Aufgabe erstellt hat. Sie können nur auf dieses Projekt zugreifen, wenn Sie auf die persönliche Aufgabe in der [!UICONTROL Startseite] -Bereich, beispielsweise aus dem Breadcrumb der Aufgabe.
>
>* Im Gegensatz zu regulären Projektaufgaben haben persönliche Aufgaben eine begrenzte Anzahl von Feldern, die in der Workfront-Benutzeroberfläche sichtbar sind und keinen Einfluss auf die Planung oder den Fortschritt von Projekten haben. Wenn Sie eine persönliche Aufgabe einem anderen Benutzer zuweisen, werden alle Aufgabenfelder zu einer persönlichen Aufgabe hinzugefügt. Die Aufgabe verbleibt jedoch im persönlichen Projekt des Benutzers, der die Aufgabe erstellt hat.
>
>
>* Persönliche Aufgaben werden nur dann auf Timesheets angezeigt, wenn sie Stunden protokolliert haben oder auf das Timesheet fixiert sind. Sie können eine persönliche Aufgabe nur dann in ein Timesheet einfügen, wenn Stunden für die Aufgabe protokolliert sind. Weitere Informationen finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).
> 
>* Es wird empfohlen, ein Projekt zu erstellen und persönliche Aufgaben dorthin zu verschieben, wenn Sie persönliche Aufgaben in den regulären Arbeitsablauf einbinden möchten.
>
> ![[!UICONTROL Projekt für persönliche Aufgaben]](assets/createworkitems-personal--project-350x105.png)

## Arbeit von einem anderen Benutzer anfordern

Sie können Arbeiten von einem anderen Benutzer direkt über den Startbereich anfordern. Wenn Sie eine Arbeit von einem anderen Benutzer anfordern, wie in diesem Abschnitt beschrieben, wird die Aufgabe als Anforderung im Startbereich des Benutzers angezeigt, bis der Benutzer auf **[!UICONTROL Arbeiten daran]**.

So fordern Sie Arbeiten von einem anderen Benutzer von der [!UICONTROL Startseite] Bereich:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **[!UICONTROL Startseite]**.
1. Klicks **[!UICONTROL Neue Aufgabe]**, wählen Sie **[!UICONTROL Anfrage]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. Im **[!UICONTROL Name]** -Feld einen Namen für die Aufgabe angeben.
1. Im **[!UICONTROL Zuweisen zu]** ein, geben Sie den Namen des Benutzers, Teams oder der Rolle ein, den/die Sie zuweisen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.
1. Im [!UICONTROL Hinzufügen von als] Dropdown-Menü auswählen, ob eine Aufgabe oder ein Problem hinzugefügt werden soll.
1. Klicks **[!UICONTROL Datum auswählen]** und wählen Sie dann das Datum und die Uhrzeit für die Fälligkeit der Aufgabe aus.
1. Klicks **[!UICONTROL Erstellen]** , um die Aufgabe zu speichern.\
   Die Aufgabe wird als Arbeitsanforderung in der [!UICONTROL Startseite] Bereich des von Ihnen ausgewählten Benutzers.

## Aufgabe oder Problem zu einem Projekt hinzufügen

Sie können eine Aufgabe oder ein Problem direkt über den Bereich Startseite zu einem vorhandenen Projekt hinzufügen:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **Startseite**.
1. Klicks **[!UICONTROL Neue Aufgabe]**, wählen Sie **[!UICONTROL Projektaufgabe]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. Im **[!UICONTROL Name]** -Feld einen Namen für die Aufgabe oder das Problem angeben.
1. Im **[!UICONTROL Zuweisen zu]** ein, geben Sie den Namen des Benutzers, Teams oder der Rolle ein, den/die Sie zuweisen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.
1. Geben Sie den Namen des Projekts ein, in dem Sie die Aufgabe oder das Problem erstellen möchten, und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.

   >[!IMPORTANT]
   >
   >Die Aufgabe oder das Problem wird auf der Seite [!UICONTROL Arbeitsliste] nur beim Projekt [!UICONTROL Status] auf [!UICONTROL Aktuell].

1. (Bedingt) Um ein Problem zu erstellen, wählen Sie **[!UICONTROL Problem]** aus dem **[!UICONTROL Hinzufügen von als]** Dropdown-Menü. Standardmäßig ist **[!UICONTROL Aufgabe]** ausgewählt ist.

1. Klicks **[!UICONTROL Datum auswählen]** und wählen Sie dann das Datum und die Uhrzeit für die Fälligkeit der Aufgabe aus.
1. Klicks **[!UICONTROL Erstellen]** , um die Aufgabe zu speichern.
