---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Konfigurieren der persönlichen Ausfallzeit
description: Es ist wichtig, in Adobe Workfront anzugeben, wann genehmigte Ausfallzeiten eintreten, da sich dies auf Ihren Zeitplan und die geplanten Abschlussdaten der Aufgaben auswirkt, denen Sie zugewiesen sind.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: e25ea757129e9645f7b5f0729cd498d5947f49f2
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Konfigurieren der persönlichen Ausfallzeit

<!-- Audited: 12/2023 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau -Umgebung verfügbar und wird in einem schrittweisen Rollout in die Produktion veröffentlicht.</span>

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Zur Konfiguration Ihrer persönlichen Ausfallzeit benötigen Sie Folgendes:</p>
        <p>Standard (zur Konfiguration der Urlaubszeiten)</p>
        <p>Arbeit oder höher (zur Konfiguration der Urlaubszeiten)</p> </td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Wenn Sie Änderungen am Urlaubskalender eines anderen Benutzers vornehmen möchten, müssen Sie dessen Manager sein und über Zugriff auf „Benutzer bearbeiten“ verfügen.</p>
   <p><strong>HINWEIS</strong> Wenn ein Manager den persönlichen Urlaubskalender eines anderen Benutzers bearbeitet, werden alle Einträge in der Zeitzone des Benutzers und nicht in der Zeitzone des Managers angezeigt.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
