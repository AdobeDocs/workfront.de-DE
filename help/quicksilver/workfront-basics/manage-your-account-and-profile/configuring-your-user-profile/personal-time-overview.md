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

[!DNL Adobe Workfront] ist nicht dazu konzipiert, Ihre vorhandenen Systeme für die Verwaltung, Ansammlung und Verfolgung von Zeitlimits zu replizieren oder zu ersetzen.

Es ist jedoch wichtig anzugeben, wann die genehmigte Zeit verstreichen muss, da dies sowohl Ihren Zeitplan als auch die [!UICONTROL geplanten Abschlussdaten] der Aufgaben betrifft, denen Sie zugewiesen sind.

Wenn Sie beispielsweise einer Aufgabe zugewiesen sind, die zwei Wochen dauern soll, und Sie planen, drei Tage in dieser Zeit freizugeben, fügt [!DNL Workfront] der Zeitleiste der Aufgabe drei Tage hinzu, um die Zeitdauer zu berücksichtigen.

Tools für die Ressourcenverwaltung verwenden auch Ihre persönliche Zeitspanne, um anzugeben, wann Sie für die Arbeitszeitplanung zur Verfügung stehen.

>[!NOTE]
>
>Um sicherzustellen, dass keine Inkonsistenzen mit den Daten auftreten, für die Sie die Zeitdauer planen, empfehlen wir, dass die Zeitzone Ihres Benutzerprofils mit der Zeitzone Ihres Zeitplans übereinstimmt. Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
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
   <strong>HINWEIS:</strong> Wenn ein Manager die persönliche Zeit eines anderen Benutzers außerhalb des Kalenders bearbeitet, werden alle Einträge in der Zeitzone des Benutzers und nicht in der Zeitzone des Managers angezeigt.</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Persönliche Zeit in [!DNL Workfront] konfigurieren

{{step1-click-profile-pic}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Ausschaltzeit]**.
1. Wählen Sie das gewünschte Datum für Ihre persönliche Zeit aus.

   ![Persönliche Zeit des Kalenders](assets/personal-time-off-calendar.png)

1. Wählen Sie **[!UICONTROL Den ganzen Tag]** aus, wenn Sie einen vollen Tag freinehmen.

   Lassen Sie das Kontrollkästchen deaktiviert, wenn Sie weniger als einen vollen Tag frei nehmen, und geben Sie die Start- und Endzeit Ihrer Freizeit an.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Ihre Auszeit ist jetzt im gesamten System [!DNL Workfront] in den Tools für die Ressourcenverwaltung sichtbar, wie im Ressourcen-Planer und im Lastenausgleich. Wenn Ihnen während dieser Zeit Arbeit zugewiesen wird, informiert ein QuickInfo den Benutzer darüber, dass Sie eine geplante Zeitüberschreitung vorgenommen haben.
