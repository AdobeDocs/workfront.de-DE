---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Stundentypen verwalten
description: Stundentypen können mit Stundeneinträgen verknüpft werden. Stundentypen sind Beschriftungen, mit denen Sie Ihre Stundeneinträge definieren.
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

Stundentypen können mit Stundeneinträgen verknüpft werden. Stundentypen sind Beschriftungen, mit denen Sie Ihre Stundeneinträge definieren.

Es gibt zwei Gruppen von Stundentypen:

* **Projektspezifische Stundentypen**: Dies ist die Zeit, die für Projekte, Aufgaben und Probleme protokolliert wird. Projektspezifische Stundentypen können Stundeneinträgen überall in [!DNL Adobe Workfront] zugeordnet werden, wo Sie Zeit für Projekte, Aufgaben und Probleme protokollieren können.

  Beim Protokollieren der Zeit in [!DNL Workfront] hängen die verfügbaren projektspezifischen Stundentypen von den Konfigurationsoptionen ab, die auf System-, Projekt- und Benutzerebene festgelegt werden.

  Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar:

   * Projektzeit
   * Aufgabenzeit
   * Problemzeit

  Der [!DNL Workfront] legt fest, welche projektspezifischen Stundentypen zur Verfügung gestellt werden, wie unter [Definieren von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) beschrieben.

  >[!NOTE]
  >
  >Wenn Sie projektspezifische Stundentypen in Ihrem [!DNL Workfront] aktivieren, muss mindestens ein projektspezifischer Stundentyp für jedes Projekt in Ihrem System aktiviert sein. Sie können einen projektspezifischen Stundentyp nicht auf Systemebene aktivieren und haben keine projektspezifischen Stundentypen auf Projektebene.

* **Allgemeine Stundentypen**: Allgemeine Stunden können keinem Projekt, keiner Aufgabe und keinem Problem zugeordnet werden und werden direkt in einer Arbeitszeittabelle protokolliert.

Informationen zur Protokollierung von Stunden und deren Verknüpfung mit Stundentypen finden Sie unter [Zeit protokollieren](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrierte Stundentypen

Workfront verfügt über eine Reihe integrierter Stundentypen. Diese Stundentypen können nicht bearbeitet und nicht ausgeblendet werden.

Die im Lieferumfang von [!DNL Workfront] enthaltenen Stundentypen sind:

* **[!UICONTROL Krankheitszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Krankenstunden können nicht als Umsatz gezählt werden.
* **[!UICONTROL Urlaubszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Urlaubszeiten können nicht als Umsatz gezählt werden.
* **[!UICONTROL Allgemeiner]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Sie können jedoch in Ihrem Projektplanungsprozess als Umsatz zählen.
* **[!UICONTROL Projektzeit]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen in einem Projekt zugeordnet werden kann.
* **[!UICONTROL Aufgabenzeit]** Ein allgemeiner Stundentyp, der nur Stundeneinträgen für eine Aufgabe zugeordnet werden kann.
* **[!UICONTROL Anfragezeit]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen für ein Problem zugeordnet werden kann.

## Stundentypen erstellen

Als [!DNL Workfront] können Sie neue Stundentypen für Ihr Unternehmen sowohl auf System- als auch auf Projektebene erstellen. Nachdem Sie Stundentypen auf der System- und Projektebene erstellt haben, können Benutzer festlegen, welche Stundentypen für bestimmte Projekte und Benutzer verfügbar sind. Weitere Informationen finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

So erstellen Sie neue Stundentypen:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Arbeitszeittabelle und Stunden]** > **[!UICONTROL Stundentypen]**.

1. Klicken Sie **[!UICONTROL Neuer Stundentyp].**
1. Geben Sie folgende Informationen in das Formular **[!UICONTROL Neuer Stundentyp]** ein:

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
      <td role="rowheader">[!UICONTROL-Umfang]</td> 
      <td> <p>Legen Sie fest, ob es sich bei dem Stundentyp um einen allgemeinen oder einen projektspezifischen Stundentyp handelt, indem Sie im Dropdown-Menü den richtigen Bereich auswählen.</p> <p>Allgemeine Stundentypen sind nur in Arbeitszeittabellen sichtbar und können nicht mit Projekten, Aufgaben oder Problemen verknüpft werden.</p> <p><b>WICHTIG</b>: Wenn Sie einen benutzerdefinierten Stundentyp haben, der [!UICONTROL Project Specific] ist, ändern Sie ihn in [!UICONTROL General], alle vorhandenen Aufgaben, Probleme und Projektstunden werden auf ihre Systemstandardtypen festgelegt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anzahl als Umsatz]</td> 
      <td><p>Wählen Sie diese Option aus, wenn sich der mit diesem Stundentyp verknüpfte Stundeneintrag auf Ihre Umsatzberechnungen auswirken soll.</p>
      <p>Krankenstand und Urlaub können nicht als Umsatz gezählt werden.</p>
      <p><b>NOTIZ</b></p>
      <p>Wenn allgemeine Stundentypen als Umsatz gezählt werden, wird der Kostensatz, der dem Profil des Benutzers zugeordnet ist, der die Zeit erfasst, mit den Stundenkosten verknüpft.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Als Umsatz zählen]**: Wählen Sie diese Option aus, wenn sich der mit diesem Stundentyp verknüpfte Stundeneintrag auf Ihre Umsatzberechnungen auswirken soll.

1. Klicken Sie **[!UICONTROL Stundentyp erstellen].**

## Stundentypen deaktivieren

Wenn Stundentypen nicht mehr aktuell sind und Benutzende ihre Stundeneinträge nicht mehr mit ihnen verknüpfen sollen, können Sie die Stundentypen deaktivieren.

Wenn Sie „Stundentypen“ deaktivieren, werden die Stundentypen an allen Stellen in [!DNL Workfront] ausgeblendet, an denen Stundentypen sichtbar sind.

So deaktivieren Sie einen Stundentyp:

{{step-1-to-setup}}

1. Erweitern Sie **[!UICONTROL Arbeitszeittabelle und]**) und klicken Sie dann auf **[!UICONTROL Stundentypen]**.

1. Wählen Sie den Stundentyp aus, den Sie deaktivieren möchten.

1. Klicken Sie **[!UICONTROL Deaktivieren]**.
