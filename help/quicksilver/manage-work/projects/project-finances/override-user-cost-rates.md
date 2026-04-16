---
content-type: overview
product-area: projects
navigation-topic: financials
title: Benutzerkostensätze auf Projektebene überschreiben
description: In diesem Artikel wird beschrieben, wie Sie die Kostensätze der Systembenutzenden für ein Projekt überschreiben können.
author: Lisa
feature: Work Management
exl-id: ff1110fd-2d24-48a7-8000-712e551ca61a
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 5%

---

# Benutzerkostensätze auf Projektebene überschreiben

Sie können angeben, wie hoch der Kostensatz für eine Benutzerin oder einen Benutzer bei einem bestimmten Projekt ist. Dieser Kostensatz auf Projektebene setzt den Kostensatz auf Systemebene für diesen Benutzer außer Kraft. Workfront verwendet zur Berechnung der Kosten den Kostensatz auf Projektebene des Aufgabengebiets, anstatt den Kostensatz auf Systemebene zu verwenden.

In diesem Artikel wird beschrieben, wie Sie die Kostensätze der Systembenutzenden für ein Projekt überschreiben können.

Weitere Informationen zur Kostenberechnung für das Projekt finden Sie unter [Übersicht über Umsatz und Kostenhierarchie](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) und [Kosten nachverfolgen](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte und Finanzdaten bearbeiten</p>
       <p><p>Sie müssen außerdem über eine der folgenden verfügen:</p> 
        <ul> 
          <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
          <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten Sie Berechtigungen für das Projekt, einschließlich Bearbeitungskostensätze </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Für den Benutzer muss das Feld **Überschreiben des Kostensatzes zulässig** in seinem Benutzerprofil aktiviert sein. Wenn ein(e) Benutzende(r) das Feld „Kostenüberschreibungen“ nicht aktiviert hat, sind für diesen/n Benutzenden keine Kostenüberschreibungen für ein Projekt zulässig, und das System verwendet den Satz im Benutzerprofil, um die Kosten zu berechnen.

Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Benutzerkostensätze auf Projektebene überschreiben

1. Wechseln Sie zu dem Projekt, für das Sie Kostensätze überschreiben möchten.
1. Klicken Sie **linken** auf „Tarife“. Möglicherweise müssen Sie zunächst auf &quot;**anzeigen“**.
1. Klicken Sie auf **Registerkarte** Kosten“, falls diese Option noch nicht ausgewählt ist.
1. Klicken Sie **Kostensatz hinzufügen** > **Neuer Benutzerkostensatz**.

   Das Feld Neuer Benutzerkostensatz wird geöffnet.

1. Wählen **im Feld** den Benutzer aus, für den Sie den Kostensatz ändern möchten.
1. Wählen Sie **Währung** für die Außerkraftsetzung des Kostensatzes.
1. Geben Sie **Feld „Kostensatz** die erste Überschreibung des Kostensatzes ein.
1. (Optional) Klicken Sie auf **Gültigen Datumssatz hinzufügen**, um weitere Überschreibungen des Kostensatzes hinzuzufügen.

   >[!NOTE]
   >
   >Wenn Sie eine einmalige Tarifüberschreibungen eingeben, gilt dies für die gesamte Lebensdauer des Projekts.
   >Wenn Sie im Laufe der Zeit unterschiedliche Raten haben möchten, können Sie mehrere datumswirksame Überschreibungen hinzufügen.

1. (Bedingt) Wenn Sie mehrere Überschreibungen von Kostensätzen hinzufügen, geben Sie die folgenden Informationen für jede Zeile an:

   * **Kostensatz**: Der Wert des Kostensatzes während des angegebenen Zeitraums.
   * **Startdatum**: Das Datum, an dem die Überschreibung des Kostensatzes beginnt.
   * **Enddatum**: Das Datum, an dem die Außerkraftsetzung des Kostensatzes endet.

   ![Feld „Neuer Benutzerkostensatz“ mit Gültigkeitsdaten](assets/new-user-cost-rate-box.png)

   Workfront wendet den Satz für Aufgabengebiete überschreiben auf die Stunden an, die während dieser Zeitrahmen bei der Berechnung der Kosten für das Projekt auftreten.

   Workfront ermöglicht es Ihnen, Lücken zwischen Überschreibungszeitrahmen zu hinterlassen, Sie erhalten jedoch eine Warnung, die bestätigt, dass dies beabsichtigt ist.

   Es ist nicht erforderlich, ein Startdatum für den ersten Überschreibungssatz oder ein Enddatum für den letzten Überschreibungssatz anzugeben.

   Es wird empfohlen, den Standardsatz für die erste Überschreibungsrate zu verwenden.

   Workfront geht davon aus, dass die erste Überschreibungsrate auf alle Stunden angewendet wird, deren Datum älter als das Enddatum der ersten Überschreibungsrate ist, und dass die letzte Überschreibungsrate auf alle Stunden angewendet wird, deren Datum neuer als das Startdatum der letzten Überschreibung ist.

   Wenn eine Stunde vor dem geplanten Startdatum des Projekts protokolliert wird, wird der allererste Kostensatz verwendet.

   Wenn eine Stunde nach dem geplanten Abschlussdatum des Projekts protokolliert wird, wird der letzte Kostensatz verwendet.

1. Klicken Sie auf **Speichern**.
