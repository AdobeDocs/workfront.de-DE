---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Hour-Typen verwalten
description: Sie können Stundentypen mit Ihren Stundeneinträgen verknüpfen. Hour-Typen sind Bezeichnungen, mit denen Sie Ihre Stundeneinträge definieren.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Stundentypen verwalten

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Sie können Stundentypen mit Ihren Stundeneinträgen verknüpfen. Hour-Typen sind Bezeichnungen, mit denen Sie Ihre Stundeneinträge definieren.

Es gibt zwei Stundentypen:

* **Projektspezifische Stundentypen**: Dies ist die Zeit, die für Projekte, Aufgaben und Probleme protokolliert wird. Projektspezifische Stundentypen können an einer beliebigen Stelle in [!DNL Adobe Workfront] mit Stundeneinträgen verknüpft werden, wo Sie die Zeit für Projekte, Aufgaben und Probleme protokollieren können.

  Bei der Protokollierung der Zeit in [!DNL Workfront] hängen die verfügbaren projektspezifischen Stundentypen von den auf System-, Projekt- und Benutzerebene festgelegten Konfigurationsoptionen ab.

  Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar:

   * Projektzeit
   * Aufgabenzeit
   * Problemzeit

  Der Administrator &quot;[!DNL Workfront]&quot; bestimmt, welche projektspezifischen Stundentypen verfügbar gemacht werden, wie unter [Festlegen von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) beschrieben.

  >[!NOTE]
  >
  >Wenn Sie projektspezifische Stundentypen in Ihrem [!DNL Workfront] -System aktivieren, muss mindestens ein projektspezifischer Stundentyp für jedes Projekt in Ihrem System aktiviert sein. Sie können einen projektspezifischen Stundentyp nicht auf Systemebene aktivieren und auf Projektebene sind keine projektspezifischen Stundentypen verfügbar.

* **Allgemeine Stundentypen**: Allgemeine Stunden können nicht mit einem Projekt, einer Aufgabe oder einem Problem verknüpft werden und werden direkt in einem Timesheet protokolliert.

Informationen zur Protokollierung von Stunden und deren Zuordnung zu Stundentypen finden Sie unter [Protokollzeit](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Neu: [!UICONTROL Standard]</p>
   <p>Aktuell: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrierte Stundentypen

Workfront verfügt über eine Reihe integrierter Stundentypen. Diese Stundentypen können nicht bearbeitet werden und können nicht ausgeblendet werden.

Die mit [!DNL Workfront] gelieferten Stundentypen sind:

* **[!UICONTROL Sick Time]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Die &quot;Sick Time&quot;-Stunden können nicht als Umsatz gezählt werden.
* **[!UICONTROL Urlaubszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Die Urlaubszeit kann nicht als Umsatz gezählt werden.
* **[!UICONTROL Allgemeiner Overhead]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen eines Projekts, einer Aufgabe oder eines Problems verknüpft werden kann. Es kann jedoch als Umsatz in Ihrem Projektplanungsprozess zählen.
* **[!UICONTROL Projektzeit]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen in einem Projekt zugeordnet werden kann.
* **[!UICONTROL Task Time]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen für eine Aufgabe zugeordnet werden kann.
* **[!UICONTROL Problemzeit]**: Ein allgemeiner Stundentyp, der nur mit Stundeneinträgen zu einem Problem verknüpft werden kann.

## Erstellen von Stundentypen

Als [!DNL Workfront] -Administrator können Sie für Ihre Organisation neue Stundentypen erstellen, sowohl auf System- als auch auf Projektebene. Nachdem Sie Stundentypen auf System- und Projektebene erstellt haben, können Benutzer festlegen, welche Stundentypen für bestimmte Projekte und Benutzer verfügbar sind. Weitere Informationen finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) .

So erstellen Sie neue Stundentypen:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Zeitblatt &amp; Stunden]** > **[!UICONTROL Stunden-Typen]**.

1. Klicken Sie auf **[!UICONTROL New Hour Type].**
1. Geben Sie die folgenden Informationen im Formular **[!UICONTROL Neuer Stunden-Typ]** an:

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
      <td> <p>Definieren Sie, ob der Stundentyp ein allgemeiner oder projektspezifischer Stundentyp ist, indem Sie im Dropdown-Menü den richtigen Bereich auswählen.</p> <p>Allgemeine Stundentypen sind nur in Timesheets sichtbar und können nicht mit Projekten, Aufgaben oder Problemen verknüpft werden.</p> <p><b>WICHTIG</b>: Wenn Sie über einen benutzerdefinierten Stündentyp verfügen, der [!UICONTROL Project Specific] ist, ändern Sie ihn in [!UICONTROL General], werden alle vorhandenen Aufgaben, Probleme und Projektstunden auf ihre Systemstandardtypen festgelegt.</p> </td> 
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

   **[!UICONTROL Als Umsatz zählen]**: Wählen Sie diese Option aus, wenn sich der mit diesem Stundentyp verknüpfte Stundeneintrag auf Ihre Umsatzberechnungen auswirken soll.

1. Klicken Sie auf **[!UICONTROL Starttyp erstellen].**

## Deaktivieren der Stundentypen

Wenn die Stundentypen veraltet werden und Sie nicht mehr möchten, dass Benutzer ihnen ihre Stundeneinträge zuordnen, können Sie die Stundentypen deaktivieren.

Durch Deaktivieren der Stundentypen werden die Stundentypen an einer beliebigen Stelle in [!DNL Workfront] ausgeblendet, an der die Stundentypen sichtbar sind.

So deaktivieren Sie einen Stundentyp:

{{step-1-to-setup}}

1. Erweitern Sie **[!UICONTROL Voreinstellungen für das Zeitblatt und die Stunden]** und klicken Sie dann auf **[!UICONTROL Stündungstypen]**.

1. Wählen Sie den zu deaktivierenden Stundentyp aus.

1. Klicken Sie auf **[!UICONTROL Deaktivieren]**.
