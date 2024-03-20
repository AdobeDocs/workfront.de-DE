---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Verwalten von Stundentypen
description: Sie können Stundentypen mit Ihren Stundeneinträgen verknüpfen. Hour-Typen sind Bezeichnungen, mit denen Sie Ihre Stundeneinträge definieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Verwalten von Stundentypen

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Sie können Stundentypen mit Ihren Stundeneinträgen verknüpfen. Hour-Typen sind Bezeichnungen, mit denen Sie Ihre Stundeneinträge definieren.

Es gibt zwei Stundentypen:

* **Projektspezifische Stundentypen**: Dies ist die Zeit, die bei Projekten, Aufgaben und Problemen protokolliert wird. Projektspezifische Stundentypen können überall in [!DNL Adobe Workfront] wo Sie die Zeit für Projekte, Aufgaben und Probleme protokollieren können.

  Beim Anmelden [!DNL Workfront], hängen die verfügbaren projektspezifischen Stundentypen von den auf System-, Projekt- und Benutzerebene festgelegten Konfigurationsoptionen ab.

  Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar:

   * Projektzeit
   * Aufgabenzeit
   * Problemzeit

  Die [!DNL Workfront] Der Administrator bestimmt, welche projektspezifischen Stundentypen verfügbar gemacht werden, wie unter [Festlegen von Stundentypen und Verfügbarkeit für Timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Wenn Sie projektspezifische Stundentypen in Ihrer [!DNL Workfront] -System muss mindestens ein projektspezifischer Stundentyp für jedes Projekt in Ihrem System aktiviert sein. Sie können einen projektspezifischen Stundentyp nicht auf Systemebene aktivieren und auf Projektebene sind keine projektspezifischen Stundentypen verfügbar.

* **Allgemeine Stündentypen**: Allgemeine Stunden können nicht mit einem Projekt, einer Aufgabe oder einem Problem verknüpft werden und werden direkt in einem Timesheet protokolliert. Weitere Informationen zur Protokollierungszeit finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]-Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Integrierte Stundentypen

Workfront verfügt über eine Reihe integrierter Stundentypen. Diese Stundentypen können nicht bearbeitet werden und können nicht ausgeblendet werden.

Die mitgelieferten Stundentypen [!DNL Workfront] sind:

* **[!UICONTROL Wartezeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Die &quot;Sick Time&quot;-Stunden können nicht als Umsatz gezählt werden.
* **[!UICONTROL Urlaubszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Die Urlaubszeit kann nicht als Umsatz gezählt werden.
* **[!UICONTROL Allgemeine Gemeinkosten]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Es kann jedoch als Umsatz in Ihrem Projektplanungsprozess zählen.
* **[!UICONTROL Projektzeit]**: Ein allgemeiner Stundentyp, der nur mit Stundeneinträgen in einem Projekt verknüpft werden kann.
* **[!UICONTROL Task Time]**: Ein allgemeiner Stundentyp, der nur mit Stundeneinträgen einer Aufgabe verknüpft werden kann.
* **[!UICONTROL Problemzeit]**:Ein allgemeiner Stundentyp, der nur mit Stundeneinträgen zu einem Problem verknüpft werden kann.

## Erstellen von Stundentypen

Als [!DNL Workfront] -Administrator können Sie für Ihre Organisation neue Stundentypen erstellen, sowohl auf System- als auch auf Projektebene. Nachdem Sie Stundentypen auf System- und Projektebene erstellt haben, können Benutzer festlegen, welche Stundentypen für bestimmte Projekte und Benutzer verfügbar sind. Weitere Informationen finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit für Timesheets](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

So erstellen Sie neue Stundentypen:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicks **[!UICONTROL Datenblatt und Stunden]** > **[!UICONTROL Stündungstypen]**.

1. Klicks **[!UICONTROL Neuer Stundentyp].**
1. Geben Sie die folgenden Informationen im **[!UICONTROL Neuer Stundentyp]** form:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geben Sie Ihrem neuen Stundentyp einen Namen, der im System leicht erkennbar ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Fügen Sie eine Beschreibung für Ihren Stundentyp hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Umfang]</td> 
      <td> <p>Definieren Sie, ob der Stundentyp ein allgemeiner oder projektspezifischer Stundentyp ist, indem Sie im Dropdown-Menü den richtigen Bereich auswählen.</p> <p>Allgemeine Stundentypen sind nur in Timesheets sichtbar und können nicht mit Projekten, Aufgaben oder Problemen verknüpft werden.</p> <p><b>WICHTIG</b>: Wenn Sie über einen benutzerdefinierten Stündentyp verfügen, der [!UICONTROL Project Specific] ist, ändern Sie ihn zu [!UICONTROL General], werden alle vorhandenen Aufgaben, Probleme und Projektstunden auf ihre Systemstandardtypen festgelegt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Als Umsatz zählen]</td> 
      <td><p>Wählen Sie diese Option aus, wenn sich der mit diesem Stundentyp verknüpfte Stundeneintrag auf Ihre Umsatzberechnungen auswirken soll.</p>
      <p>Die Wartezeit und die Urlaubszeit können nicht als Umsatz gezählt werden.</p>
      <p><b>NOTIZ</b></p>
      <p>Wenn allgemeine Stundentypen als Umsatz gezählt werden, wird die Kostensatz, die dem Profil des Benutzers zugeordnet ist, der die Zeit protokolliert, mit den Stundenkosten verknüpft.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Als Umsatz zählen]**: Wählen Sie diese Option aus, wenn der mit diesem Stundentyp verknüpfte Stundeneintrag Auswirkungen auf Ihre Umsatzberechnungen haben soll.

1. Klicks **[!UICONTROL Starttyp erstellen].**

## Deaktivieren der Stundentypen

Wenn die Stundentypen veraltet werden und Sie nicht mehr möchten, dass Benutzer ihnen ihre Stundeneinträge zuordnen, können Sie die Stundentypen deaktivieren.

Durch Deaktivieren der Stundentypen werden die Stundentypen von überall in ausgeblendet. [!DNL Workfront] wo Stundentypen sichtbar sind.

So deaktivieren Sie einen Stundentyp:

1. Klicks **[!UICONTROL Einrichtung]** in der Nähe der oberen rechten Ecke von [!DNL Adobe Workfront] in der Leiste &quot;Globale Navigation&quot;.

1. Erweitern **[!UICONTROL Voreinstellungen für Zeitblatt und Stunden]** Klicken Sie auf **[!UICONTROL Stündungstypen]**.

1. Wählen Sie den zu deaktivierenden Stundentyp aus.

1. Klicks **[!UICONTROL Deaktivieren]**.
