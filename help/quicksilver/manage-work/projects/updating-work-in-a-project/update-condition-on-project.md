---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierungsbedingung für ein Projekt
description: Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird, um anzugeben, ob die damit verbundenen Arbeiten reibungslos verlaufen oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der anzeigt, ob Sie aktiv daran arbeiten oder nicht.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Aktualisierungsbedingung für ein Projekt

Die Bedingung eines Projekts ist eine Markierung, die darauf platziert wird, um anzugeben, ob die damit verbundenen Arbeiten reibungslos verlaufen oder ob Sie auf Hindernisse gestoßen sind. Dies unterscheidet sich vom Status des Projekts, der anzeigt, ob Sie aktiv daran arbeiten oder nicht.

Sie können die Bedingung eines Projekts entweder automatisch oder manuell festlegen. Um die Bedingung eines Projekts manuell zu ändern, müssen Sie Projekteigentümer sein oder über Administratorrechte verfügen.

Der Adobe Workfront-Administrator kann benutzerdefinierte Bedingungen für Ihre Umgebung erstellen, wie in [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>

Für die neuen Lizenzen:
<p>Standard</p>

Für aktuelle Lizenzen:
<ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Anzeigen oder Verbessern des Zugriffs auf Projekte</p> <p>Zugriff auf Aufgaben und Probleme bearbeiten </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder höherer Berechtigungen für Aufgaben und Probleme zur Anzeige ihrer Bedingung</p>
   <p>Verwalten von Berechtigungen für Aufgaben und Probleme zum Aktualisieren der Bedingung</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Bedingung automatisch festlegen

Das automatische Festlegen der Bedingung eines Projekts wird durch den Bedingungstyp des Projekts bestimmt. Der Bedingungstyp muss auf Fortschrittsstatus gesetzt werden, damit Workfront die Projektbedingung automatisch festlegt.

Ihr Workfront- oder Gruppenadministrator legt die Standardeinstellung des Felds Bedingungstyp für neue Projekte in Ihrem System fest, wenn Sie Projektvoreinstellungen im Bereich Einrichtung festlegen. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Wenn Sie ein Projekt erstellen, wird die Bedingung des Projekts automatisch so festgelegt, dass sie dem Fortschrittsstatus des Projekts zu diesem Zeitpunkt entspricht. Der Fortschrittsstatus des Projekts basiert auf dem Fortschritt der Aufgaben im Projekt.

Informationen zu den Projektbedingungen und dazu, wie sie basierend auf dem Fortschrittsstatus berechnet werden, finden Sie unter [Übersicht über den Projektfortschritt](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Manuelles Aktualisieren der Bedingung für ein Projekt

Wenn Sie den Bedingungstyp Ihres Projekts auf &quot;Manuell&quot;anstelle von &quot;Fortschrittsstatus&quot;festlegen, können Sie die Bedingung eines Projekts manuell aktualisieren.

1. Wechseln Sie zu dem Projekt, für das Sie die Bedingung aktualisieren möchten.
1. Klicken Sie im linken Bereich auf den Abschnitt **Projektdetails** .

1. Stellen Sie sicher, dass das Feld **Bedingungstyp** auf **Manuell** eingestellt ist.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Wählen Sie im Feld **Bedingung** aus den folgenden Optionen die Option aus, die Ihrem Verständnis entspricht, ob das damit verbundene Werk reibungslos läuft oder ob es Verzögerungen gibt:

   * **Auf Ziel**
   * **Risiko**
   * **In Trouble**

   Weitere Informationen zu Projektbedingungen finden Sie unter [Überblick über Projektbedingungen und Bedingungstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in Workfront finden Sie unter [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klicken Sie auf **Änderungen speichern**.
