---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzerattribute zuordnen
description: Mit Single Sign-on (SSO) können Sie Attribute aus dem Active Directory Ihres Identitätsanbieters an Ihre Adobe Workfront-Benutzenden übergeben.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: d8ccdeac9a658ca7a2862781e98c2c3c6fa0e8a0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 6%

---

# Zuordnen von Benutzerattributen

<!--Audited 2/2024-->

Mit Single Sign-on (SSO) können Sie Attribute aus dem Active Directory Ihres Identitätsanbieters an Ihre Adobe Workfront-Benutzenden übergeben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Sie müssen ein Workfront-Administrator sein</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Tipps zum Zuordnen von Attributen

Beachten Sie beim Zuordnen von Attributen Folgendes:

* Immer in einer Vorschau-Sandbox oder einer Kunden-Aktualisierungs-Sandbox (CR) testen.
* Testen Sie sowohl mit Administrator- als auch mit Nicht-Administrator-Konten, um zu bestätigen, dass Sie Attribute korrekt zuordnen.
* Zugeordnete Attribute werden jedes Mal angewendet, wenn sich ein Benutzer per Single Sign-on anmeldet.

  Beispiel: Wenn Sie „Nachname“ zuordnen und ihren Namen in Workfront aktualisieren, ohne den Wert in ihrem Identity Provider zu aktualisieren, wird der Nachname überschrieben, sodass er mit dem Wert des entsprechenden Elements im Identity Provider übereinstimmt, wenn sich der Benutzer das nächste Mal anmeldet.

## Zuordnen von Benutzerattributen für Ihre Organisation

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-left.png) in der linken oberen Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **System** > **Single Sign-On (SSO)**.

1. Wählen Sie die Registerkarte **Adobe** aus.

1. (Optional und bedingt) Wenn in Ihrem Unternehmen die Attributzuordnung in der klassischen Version konfiguriert war und Sie diese Attributzuordnung in die Adobe Unified Experience kopieren möchten, klicken Sie auf **Zuordnungen migrieren**. Sie können diese Zuordnungen dann verwerfen, löschen oder bearbeiten.

   >[!NOTE]
   >
   >Es wird empfohlen, Zuordnungen zu migrieren, wenn Sie im einheitlichen Adobe-Erlebnis zum ersten Mal Zuordnungen konfigurieren. Es schadet nicht, sie später erneut zu migrieren, aber sie mehrmals zu migrieren ist unnötig.

1. Um eine neue Attributzuordnung zu erstellen, klicken Sie auf **Zuordnung hinzufügen**.

1. Klicken Sie auf den Pfeil neben dem Workfront-Feldnamen und wählen Sie das [!DNL Workfront] aus, dem Sie das Feld zuordnen möchten.

1. (Optional) Wenn Sie mehr als eine Regel für ein bestimmtes Feld erstellen möchten, klicken Sie auf den Pfeil neben **Immer** und wählen Sie den Operator aus, den die Regel verwenden soll.

1. (Bedingt) Wenn Sie neben Immer einen Operator ausgewählt haben, wählen Sie das Workfront-Feld und den Wert aus, für die der Operator gilt.

   >[!NOTE]
   >
   >Die Operatoren `Is Truthy` und `Is Falsy` erfordern keine Werte.

1. Wählen Sie aus, ob Sie den Wert eines Attributs in Ihrem Identity Manager auf das Workfront-Feld anwenden möchten, oder ob Sie einen bestimmten konstanten Wert anwenden möchten.

1. Geben Sie den Namen des Identity Manager-Felds ein, das Sie anwenden möchten, oder geben Sie den Text des konstanten Werts ein, den Sie anwenden möchten.

1. (Optional) Um weitere Regeln für dasselbe Workfront-Feld hinzuzufügen, klicken Sie auf **Neue Regel hinzufügen** und führen Sie die Schritte 4 bis 9 aus.

   >[!IMPORTANT]
   >
   > * Jede Regel unterhalb einer Always-Regel wird ignoriert. Wenn Sie eine Regel vom Typ Immer haben, müssen Sie sie an das Ende der Liste der Regeln verschieben. Sie können Regeln in der Liste verschieben, indem Sie auf das Dreipunkt-Menü rechts neben der Regel klicken und die Regel nach oben oder unten verschieben.
   > * Um eine Regel in der Mitte der Liste zu erstellen, klicken Sie auf das Dreipunkt-Menü neben der Regel, die Sie über oder unter der neuen Regel platzieren möchten, und wählen Sie **Regel über hinzufügen** oder **Regel unten hinzufügen**.

1. Um eine Regel zu löschen, klicken Sie auf das Dreipunkt-Menü neben der zu löschenden Regel und wählen Sie **Löschen**.
1. Um eine Zuordnung zu löschen, klicken Sie auf das Symbol **Löschen**, das sich auf der Karte für diese Zuordnung befindet.

1. Scrollen Sie zum Speichern nach oben auf der Seite und klicken Sie auf **Speichern**.


