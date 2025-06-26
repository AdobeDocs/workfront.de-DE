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
source-git-commit: f35da9077b0422ba939ed9f6285835897f28874c
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# Stundentypen verwalten

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<div class="preview">

Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Dieselben Funktionen werden nach einer Woche ab der Vorschau-Version auch in der Produktionsumgebung für alle Kunden verfügbar sein.

Weitere Informationen finden Sie unter [Schnittstellenmodernisierung](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Stundentypen sind Beschriftungen, mit denen Sie Ihre Stundeneinträge definieren. Stundentypen können mit Stundeneinträgen verknüpft werden.

Es gibt zwei Kategorien von Stundentypen:

* **Projektspezifische Stundentypen**: Dies ist die Zeit, die für Projekte, Aufgaben und Probleme protokolliert wird. Projektspezifische Stundentypen können Stundeneinträgen überall in [!DNL Adobe Workfront] zugeordnet werden, wo Sie Zeit für Projekte, Aufgaben und Probleme protokollieren können.

  Beim Protokollieren der Zeit in [!DNL Workfront] hängen die verfügbaren projektspezifischen Stundentypen von den Konfigurationsoptionen ab, die auf System-, Projekt- und Benutzerebene festgelegt werden.

  Die folgenden standardmäßigen projektspezifischen Stundentypen sind immer verfügbar:

   * Projektzeit
   * Aufgabenzeit
   * Problemzeit

  Der [!DNL Workfront] legt fest, welche projektspezifischen Stundentypen zur Verfügung gestellt werden, wie unter [Definieren von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md) beschrieben.

  >[!NOTE]
  >
  >Wenn Sie projektspezifische Stundentypen in Ihrem [!DNL Workfront] aktivieren, muss mindestens ein projektspezifischer Stundentyp für jedes Projekt in Ihrem System aktiviert sein. Sie können einen projektspezifischen Stundentyp nicht auf Systemebene aktivieren und haben keine projektspezifischen Stundentypen auf Projektebene verfügbar.

* **Allgemeine Stundentypen**: Allgemeine Stunden können keinem Projekt, keiner Aufgabe und keinem Problem zugeordnet werden und werden direkt in einer Arbeitszeittabelle protokolliert.

Informationen zur Protokollierung von Stunden und deren Verknüpfung mit Stundentypen finden Sie unter [Zeit protokollieren](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td>Systemadministrator</td>
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrierte Stundentypen

Workfront verfügt über eine Reihe integrierter Stundentypen. Diese Stundentypen können nicht bearbeitet oder ausgeblendet werden.

Die im Lieferumfang von [!DNL Workfront] enthaltenen Stundentypen sind:

* **[!UICONTROL Krankheitszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Krankenstunden können nicht als Umsatz gezählt werden.
* **[!UICONTROL Urlaubszeit]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Urlaubszeiten können nicht als Umsatz gezählt werden.
* **[!UICONTROL Allgemeiner]**: Ein allgemeiner Stundentyp, der nicht mit Stundeneinträgen für ein Projekt, eine Aufgabe oder ein Problem verknüpft werden kann. Sie können in Ihrem Projektplanungsprozess als Umsatz zählen.
* **[!UICONTROL Projektzeit]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen in einem Projekt zugeordnet werden kann.
* **[!UICONTROL Aufgabenzeit]** Ein allgemeiner Stundentyp, der nur Stundeneinträgen für eine Aufgabe zugeordnet werden kann.
* **[!UICONTROL Anfragezeit]**: Ein allgemeiner Stundentyp, der nur Stundeneinträgen für ein Problem zugeordnet werden kann.

## Stundentypen erstellen

Als [!DNL Workfront] können Sie Stundentypen für Ihr Unternehmen auf System- und Projektebene erstellen.

Nachdem Sie Stundentypen auf Systemebene definiert haben, können Benutzerinnen und Benutzer definieren, welche Stundentypen für bestimmte Projekte oder für bestimmte Benutzerinnen und Benutzer verfügbar sind.

Weitere Informationen finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Stundentypen erstellen:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Arbeitszeittabelle und Stunden** und dann auf **Stundentypen**.

1. Klicken Sie **Abschnitt** Stundentypen“ auf **Neuer Stundentyp**.
1. Geben **im Dialogfeld &quot;** Stundentypen“ die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geben Sie einen Namen für den Stundentyp ein, der im System leicht zu erkennen ist.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Fügen Sie eine Beschreibung für Ihren Stundentyp hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Umfang]</td> 
      <td> <p>Wählen Sie im Dropdown-Menü <strong>Umfang“ aus, ob es sich bei dem Stundentyp um einen allgemeinen oder </strong> projektspezifischen Stundentyp handelt.</p> <p>Allgemeine Stundentypen sind nur in Arbeitszeittabellen sichtbar und können nicht mit Projekten, Aufgaben oder Problemen verknüpft werden.</p> <p><b>WICHTIG</b>: Wenn Sie einen benutzerdefinierten Stundentyp haben, der [!UICONTROL Project Specific] ist, und Sie ihn in [!UICONTROL General] ändern, werden alle vorhandenen Aufgaben, Probleme und Projektstunden auf ihre Systemstandardtypen gesetzt.</p> </td> 
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

1. Klicken Sie **[!UICONTROL Stundentyp erstellen].**

   Der Stundentyp wird Ihrem Workfront-System hinzugefügt und ist standardmäßig aktiviert.

## Stundentypen deaktivieren

Sie können Stundentypen deaktivieren, wenn Sie nicht mehr möchten, dass ihnen Benutzer ihre Stunden zuordnen. Wenn Sie Stundentypen deaktivieren, werden sie an allen Stellen in [!DNL Workfront] ausgeblendet, an denen Stundentypen sichtbar sind.

>[!NOTE]
>
>* Integrierte Stundentypen können nicht deaktiviert werden.
>* Wenn Sie einen projektspezifischen Stundentyp deaktivieren, wird die gesamte für diesen Typ protokollierte Zeit automatisch auf einen integrierten projektspezifischen Stundentyp eingestellt. Beispiel: Für ein Projekt protokollierte Zeit ist standardmäßig der Stundentyp Projektzeit; für eine Aufgabe protokollierte Zeit ist standardmäßig der Stundentyp Aufgabenzeit.
>


So deaktivieren Sie einen Stundentyp:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Arbeitszeittabelle und Stunden]** und dann auf **[!UICONTROL Stundentypen]**.

1. Wählen Sie den Stundentyp aus, den Sie deaktivieren möchten.


1. <span class="preview">Klicken Sie auf **Mehr** und dann auf **Deaktivieren**.</span>

   <span class="preview">![Aktivieren und Deaktivieren von Links zum Stundentyp](assets/activate-and-deactivate-hour-type-links.png)</span>

   <span class="preview">Der Stundentyp ist deaktiviert und kann von Benutzenden beim Protokollieren von Stunden nicht mehr gefunden werden.</span>

1. <span class="preview">(Optional) Um einen Stundentyp erneut zu aktivieren, wählen Sie ihn in der Liste **Stundentypen** aus und klicken Sie dann auf **Mehr** > **Aktivieren**. </span>

