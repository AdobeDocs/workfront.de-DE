---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Persönliche Zeit konfigurieren
description: Es ist wichtig, in Adobe Workfront anzugeben, wann eine genehmigte Zeitüberschreitung eintritt, da dies sich auf Ihren Zeitplan auswirkt und sich auf die geplanten Abschlussdaten der Aufgaben auswirkt, denen Sie zugewiesen sind.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Persönliche Zeit konfigurieren

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] ist nicht dazu konzipiert, Ihre vorhandenen Systeme für die Verwaltung, Ansammlung und Nachverfolgung persönlicher Zeit zu replizieren oder zu ersetzen.

Es ist jedoch wichtig anzugeben, wann die genehmigte Zeitüberschreitung eintritt, da dies sowohl Ihren Zeitplan als auch die [!UICONTROL Geplante Abschlussdaten] der Aufgaben, denen Sie zugewiesen sind.

Wenn Sie beispielsweise einer Aufgabe zugewiesen sind, die zwei Wochen in Anspruch nehmen soll, und Sie planen, während dieser Zeit drei Tage freizugeben, [!DNL Workfront] fügt der Zeitleiste der Aufgabe drei Tage hinzu, um die Zeitdauer zu berücksichtigen.

Tools für die Ressourcenverwaltung verwenden auch Ihre persönliche Zeitspanne, um anzugeben, wann Sie für die Arbeitszeitplanung zur Verfügung stehen.

>[!NOTE]
>
>Um sicherzustellen, dass keine Inkonsistenzen mit den Daten auftreten, für die Sie die Zeitdauer planen, empfehlen wir, dass die Zeitzone Ihres Benutzerprofils mit der Zeitzone Ihres Zeitplans übereinstimmt. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Zeitplan erstellen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
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
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Standard (zur Konfiguration Ihrer persönlichen Zeit)</p>
        <p>oder</p>
        <p>Aktuell: Arbeit oder höher (zur Konfiguration Ihrer persönlichen Zeit)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Manager] mit Zugriff auf [!UICONTROL Benutzer bearbeiten] (um Änderungen an der Zeitdauer anderer Benutzer vorzunehmen)<br>
   <strong>NOTE:</strong> Wenn ein Manager die persönliche Zeit eines anderen Benutzers außerhalb des Kalenders bearbeitet, werden alle Einträge in der Zeitzone des Benutzers und nicht in der Zeitzone des Managers angezeigt.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Persönliche Zeit konfigurieren in [!DNL Workfront]

{{step1-click-profile-pic}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Zeitlimit]**.
1. Wählen Sie das gewünschte Datum für Ihre persönliche Zeit aus.

   ![Persönliche Uhrzeit des Kalenders](assets/personal-time-off-calendar.png)

1. Auswählen **[!UICONTROL Ganztägig]**, wenn Sie sich einen ganzen Tag freinehmen.

   Lassen Sie das Kontrollkästchen deaktiviert, wenn Sie weniger als einen vollen Tag frei nehmen, und geben Sie die Start- und Endzeit Ihrer Freizeit an.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Ihre Zeitdauer ist jetzt für alle [!DNL Workfront] in den Tools zur Ressourcenverwaltung wie dem Resource Planer und dem Workload Balancer. Wenn Ihnen während dieser Zeit Arbeit zugewiesen wird, informiert ein QuickInfo den Benutzer darüber, dass Sie eine geplante Zeitüberschreitung vorgenommen haben.
