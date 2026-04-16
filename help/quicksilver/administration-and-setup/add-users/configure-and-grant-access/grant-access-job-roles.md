---
title: Zugriff auf Aufgabengebiete gewähren
description: Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Aufgabengebiete in Workfront über seine Zugriffsebene definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: a5ba79da-37f3-43f8-a7e2-4ccd75b56fef
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 11%

---

# Zugriff auf Aufgabengebiete gewähren

Als Adobe Workfront-Administrator können Sie den Zugriff eines Benutzers auf Aufgabengebiete über die Zugriffsebene des Benutzers definieren, wie in [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Informationen zu Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerzugriff konfigurieren, um Aufgabengebiete mithilfe einer benutzerdefinierten Zugriffsebene zu bearbeiten

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) der Schaltfläche **Anzeigen** oder **Bearbeiten** rechts neben „Aufgabengebiete“ und wählen Sie dann unter **Einstellungen optimieren** die Funktionen aus, die Sie gewähren möchten.

   >[!NOTE]
   >
   >**Ansicht** ist der Standardzugriff für Aufgabengebiete.

   ![Feinabstimmung des Zugriffs auf Aufgabengebiete](assets/job-role-access-view-fine-tune.png)

   Benutzer mit **View**-Zugriff können vorhandene Aufgabengebiete anzeigen und optional Folgendes tun:

   * Abrechnungssätze für Aufgabengebiete anzeigen
   * Kostensätze für Aufgabengebiete anzeigen
   * Felder für allgemeine Finanzen (die nicht mit Abrechnungs- oder Kostensätzen in Verbindung stehen) für Aufgabengebiete anzeigen

   Benutzer mit **Bearbeiten**-Zugriff können vorhandene Aufgabengebiete anzeigen und bearbeiten und optional Folgendes tun:

   * Erstellen neuer Aufgabengebiete
   * Löschen von Aufgabengebieten
   * Abrechnungssätze für Aufgabengebiete bearbeiten
   * Kostensätze für Aufgabengebiete bearbeiten
   * Felder für allgemeine Finanzen (die nicht mit Abrechnungs- oder Kostensätzen in Zusammenhang stehen) für Aufgabengebiete bearbeiten
   * Aufgabengebiet-Abrechnungssätze, Kostensätze und Felder für allgemeine Finanzen anzeigen

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der Artikel fort, die unter [Zugriff auf Adobe Workfront konfigurieren“ aufgeführt sind](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Aufgabengebiete nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Aufgabengebieten tun können, finden Sie im Abschnitt [Aufgabengebiete](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#job-roles) im Artikel [Für jeden Objekttyp verfügbare Funktionen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
