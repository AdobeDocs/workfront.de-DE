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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# Benutzerattribute zuordnen

<!--Audited 2/2024-->

Mit Single Sign-on (SSO) können Sie Attribute aus dem Active Directory Ihres Identitätsanbieters an Ihre Adobe Workfront-Benutzenden übergeben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipps zum Zuordnen von Attributen

Beachten Sie beim Zuordnen von Attributen Folgendes:

* Immer in einer Vorschau-Sandbox oder einer Kunden-Aktualisierungs-Sandbox (CR) testen.
* Testen Sie sowohl mit Administrator- als auch mit Nicht-Administrator-Konten, um zu bestätigen, dass Sie Attribute korrekt zuordnen.
* Zugeordnete Attribute werden jedes Mal angewendet, wenn sich ein Benutzer per Single Sign-on anmeldet.

  Beispiel: Wenn Sie „Nachname“ zuordnen und ihren Namen in Workfront aktualisieren, ohne den Wert in ihrem Identity Provider zu aktualisieren, wird der Nachname überschrieben, sodass er mit dem Wert des entsprechenden Elements im Identity Provider übereinstimmt, wenn sich der Benutzer das nächste Mal anmeldet.

## Zuordnen von Benutzerattributen für Ihre Organisation

Das Verfahren zum Zuordnen von Attributen unterscheidet sich, je nachdem, ob Ihr Unternehmen das einheitliche Adobe-Erlebnis nutzt.

Um festzustellen, ob sich Ihr Unternehmen auf dem einheitlichen Adobe-Erlebnis befindet, überprüfen Sie die URL, die Sie für den Zugriff auf Workfront verwenden.

| URL | Adobe Experience |
|---|---|
| (CompanyName).my.workfront.com | Klassische Erfahrung |
| experience.adobe.com | Adobe Unified Experience |

* [Zuordnen von Benutzerattributen im klassischen Erlebnis](#map-user-attributes-in-the-classic-experience)
* [Zuordnen von Benutzerattributen im einheitlichen Adobe-Erlebnis](#map-user-attributes-in-the-adobe-unified-experience)

### Zuordnen von Benutzerattributen im klassischen Erlebnis

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **System** > **Single Sign-On (SSO)**.

1. Klicken Sie in **Dropdown** Typ“ auf **SAML 2.0**.

1. Klicken Sie **Benutzerattribute zuordnen**.

   ![Benutzerattribute zuordnen](assets/map-user-attributes.png)

1. Ordnen Sie in der angezeigten Optionszeile die Attribute zu, die Sie für Ihre Workfront-Benutzenden benötigen.

   Sie können Attribute wie Adresse, Manager, Aufgabengebiet, Hauptgruppe usw. zuordnen.

   Attributzuordnungen funktionieren im Verhältnis 1:1. Sie können beispielsweise nicht jede Gruppe festlegen, zu der ein Benutzer gehört; Sie können nur eine pro Benutzer festlegen.

   >[!IMPORTANT]
   >
   >Es wird nicht empfohlen, Zugriffsebenen in den Attributzuordnungen zuzuordnen. Gehen Sie in diesem Fall beim Festlegen des Standardwerts vorsichtig vor, um sicherzustellen, dass Sie den Administratorzugriff nicht versehentlich entfernen.

   In der folgenden Tabelle werden die Felder erläutert, die Sie zum Zuordnen von Attributen verwenden können:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront-Benutzerattribut</td> 
      <td>Namen des Attributs auswählen, das Sie zuordnen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verzeichnisattribut</td> 
      <td>Geben Sie die SSO-Attributbeschriftung ein, die Sie verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardwert</td> 
      <td> <p>Wenn Sie ein Workfront-Benutzerattribut ausgewählt haben und der Wert während der Verbindung NULL ist, wird dieses Feld mit dem entsprechenden Standardwert im System ausgefüllt. Geben Sie hier nur dann einen Wert ein, wenn Sie Attributzuordnungsregeln anwenden möchten (siehe Schritt 7). Der Standardwert bildet eine Ausnahme zu diesen Regeln.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf **Regeln**, um dem Attribut eine Regel hinzuzufügen.

   1. Wählen Sie in der Dropdown-Liste den Attributmodifikator aus, den Sie verwenden möchten.
   1. Geben Sie in die zwei Felder rechts den Verzeichnisattributwert und den Wert ein, durch den Sie ihn ersetzen möchten.

      ![Regelfelder](assets/rule-fields.png)

   Sie können auf **Regel hinzufügen** klicken, um dem Attribut weitere Regeln hinzuzufügen.

1. (Optional) Um weitere Benutzerattribute zuzuordnen, klicken Sie auf **Zuordnung hinzufügen** und wiederholen Sie die Schritte 6 bis 7.
1. Klicken Sie auf **Speichern**.

### Zuordnen von Benutzerattributen im einheitlichen Adobe-Erlebnis

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-left.png) in der linken oberen Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **System** > **Single Sign-On (SSO)**.

1. Wählen Sie die Registerkarte **Adobe** aus.

1. (Optional und bedingt) Wenn in Ihrem Unternehmen die Attributzuordnung in der klassischen Version konfiguriert war und Sie diese Attributzuordnung in die einheitliche Adobe-Version kopieren möchten, klicken Sie auf **Zuordnungen migrieren**. Sie können diese Zuordnungen dann verwerfen, löschen oder bearbeiten.

   >[!NOTE]
   >
   >Es wird empfohlen, Zuordnungen beim ersten Konfigurieren von Zuordnungen im einheitlichen Adobe-Erlebnis zu migrieren. Es schadet nicht, sie später erneut zu migrieren, aber sie mehrmals zu migrieren ist unnötig.

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


