---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Konfigurieren der persönlichen Ausfallzeit
description: Es ist wichtig, in Adobe Workfront anzugeben, wann genehmigte Ausfallzeiten eintreten, da sich dies auf Ihren Zeitplan und die geplanten Abschlussdaten der Aufgaben auswirkt, denen Sie zugewiesen sind.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e0f6078cfab1b325302dbda8a656d2a65ee0b95c
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 1%

---

# Konfigurieren der persönlichen Ausfallzeit

{{highlighted-preview}}

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] ist nicht dafür konzipiert, bestehende Systeme zur Verwaltung, Ansammlung und Verfolgung persönlicher Ausfallzeiten zu replizieren oder zu ersetzen.

Es ist jedoch wichtig anzugeben, wann genehmigte Ausfallzeiten eintreten, da dies sowohl Ihren Zeitplan als auch [!UICONTROL geplanten Abschlussdaten] der Aufgaben beeinflusst, denen Sie zugewiesen sind.

Wenn Sie beispielsweise einer Aufgabe zugewiesen sind, die zwei Wochen dauern soll, und Sie planen, während dieser Zeit drei Tage frei zu nehmen, fügt [!DNL Workfront] der Aufgabenzeitleiste drei Tage hinzu, um die Ausfallzeit zu berücksichtigen.

Ressourcen-Management-Tools verwenden auch Ihre persönliche Auszeit, um anzugeben, wann Sie für die Arbeit zur Verfügung stehen.

>[!NOTE]
>
>Um sicherzustellen, dass es nicht zu Inkonsistenzen mit den Daten kommt, für die Sie Ihre Ausfallzeit planen, empfehlen wir, dass die Zeitzone Ihres Benutzerprofils mit der Ihres Zeitplans übereinstimmt. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Standard (zur Konfiguration der Urlaubszeiten)</p>
        <p>oder</p>
        <p>Aktuell: Arbeit oder höher (zur Konfiguration der persönlichen Ausfallzeit)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Manager] mit [!UICONTROL Benutzer bearbeiten]-Zugriff (um Änderungen am Urlaubskalender anderer Benutzer vorzunehmen)<br>
   <strong>HINWEIS</strong> Wenn ein Manager den persönlichen Urlaubskalender eines anderen Benutzers bearbeitet, werden alle Einträge in der Zeitzone des Benutzers und nicht in der Zeitzone des Managers angezeigt.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Konfigurieren der persönlichen Ausfallzeit in [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Wenn Sie Adobe Unified Experience verwenden, können Sie auf Ihr Workfront-Profil zugreifen, indem Sie im oberen Navigationsbereich auf das Adobe-Kontomenü (Ihr Profilbild) klicken und dann auf Workfront-Profil klicken.
>
>![Workfront-Profil](assets/aue-profile.png)

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL Auszeit]**.
1. Wählen Sie das gewünschte Datum für Ihre persönliche Auszeit aus.

   <span class="preview">Beispielbild in der Vorschau-Umgebung:</span>
   ![Persönlicher Urlaubskalender](assets/personal-time-off-calendar-0925.png)

   Beispielbild in der Produktionsumgebung:
   ![Persönlicher Urlaubskalender](assets/personal-time-off-calendar.png)

1. Wählen Sie **[!UICONTROL Den ganzen]** aus, wenn Sie sich einen ganzen Tag freinehmen möchten.

   Lassen Sie das Kontrollkästchen deaktiviert, wenn Sie weniger als einen ganzen Tag Urlaub nehmen, und geben Sie die Anfangs- und Endzeiten Ihrer Urlaubszeit an.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Ihre Ausfallzeit ist jetzt im gesamten [!DNL Workfront]-System in den Tools für das Ressourcenmanagement sichtbar, z. B. im Ressourcenplaner und im Workload-Balancer. Wenn Ihnen in dieser Zeit Arbeit zugewiesen wird, wird dem Benutzer ein Tooltip angezeigt, dass Sie Ausfallzeiten geplant haben.
