---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzerattribute zuordnen
description: Mit Single Sign-On (SSO) können Sie Attribute aus dem Active Directory Ihres Identitäts-Providers an Ihre Adobe Workfront-Benutzer übergeben.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 1%

---

# Benutzerattribute zuordnen

<!--Audited 2/2024-->

Mit Single Sign-On (SSO) können Sie Attribute aus dem Active Directory Ihres Identitäts-Providers an Ihre Adobe Workfront-Benutzer übergeben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipps für Zuordnungsattribute

Beachten Sie beim Zuordnen von Attributen Folgendes:

* Testen Sie immer in einer Vorschau-Sandbox oder einer Sandbox mit Kundenaktualisierung (CR).
* Testen Sie mit Administrator- und Nicht-Administrator-Konten, um sicherzustellen, dass Sie Attribute korrekt zuordnen.
* Zugeordnete Attribute werden jedes Mal angewendet, wenn sich ein Benutzer über Single Sign-on anmeldet.

  Beispiel: Wenn Sie &quot;Nachname&quot;zuordnen und ihren Namen in Workfront aktualisieren, ohne den Wert in ihrem Identitätsanbieter zu aktualisieren, wird der Nachname überschrieben, sodass er mit dem Wert übereinstimmt, der im Identitätsanbieter vorhanden ist, wenn sich der Benutzer das nächste Mal anmeldet.

## Zuordnen von Benutzerattributen zu Ihrer Organisation

Das Verfahren für die Zuordnung von Attributen hängt davon ab, ob Ihr Unternehmen über das einheitliche Erlebnis auf Adobe verfügt.

Um festzustellen, ob Ihr Unternehmen das einheitliche Adobe-Erlebnis nutzt, überprüfen Sie die URL, die Sie für den Zugriff auf Workfront verwenden.

| URL | Adobe-Erlebnis |
|---|---|
| (CompanyName).my.workfront.com | Klassisches Erlebnis |
| experience.adobe.com | Einheitliches Adobe-Erlebnis |

* [Benutzerattribute im klassischen Erlebnis zuordnen](#map-user-attributes-in-the-classic-experience)
* [Zuordnen von Benutzerattributen zum einheitlichen Adobe-Erlebnis](#map-user-attributes-in-the-adobe-unified-experience)

### Benutzerattribute im klassischen Erlebnis zuordnen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **System** > **Single Sign-On (SSO)**.

1. Klicken Sie in der Dropdown-Liste **Typ** auf **SAML 2.0**.

1. Klicken Sie auf **Benutzerattribute zuordnen**.

   ![](assets/map-user-attributes.png)

1. Ordnen Sie in der angezeigten Optionszeile die Attribute zu, die Sie für Ihre Workfront-Benutzer benötigen.

   Sie können Attribute wie &quot;Adresse&quot;, &quot;Manager&quot;, &quot;Auftragsrolle&quot;, &quot;Homepage-Gruppe&quot;usw. zuordnen.

   Attributzuordnungen funktionieren mit einem Verhältnis von 1:1. Sie können beispielsweise nicht jede Gruppe festlegen, zu der ein Benutzer gehört. Sie können pro Benutzer nur eine festlegen.

   >[!IMPORTANT]
   >
   >Es wird nicht empfohlen, Zugriffsebenen in den Attributzuordnungen zuzuordnen. Gehen Sie in diesem Fall beim Festlegen des Standardwerts vorsichtig vor, um sicherzustellen, dass Sie den Admin-Zugriff nicht versehentlich entfernen.

   In der folgenden Tabelle werden die Felder erläutert, die Sie für die Zuordnung von Attributen verwenden können:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront-Benutzerattribut</td> 
      <td>Wählen Sie den Namen des Attributs aus, das Sie zuordnen möchten</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verzeichnisattribut</td> 
      <td>Geben Sie die SSO-Attributbeschriftung ein, die Sie verwenden möchten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardwert</td> 
      <td> <p>Wenn Sie ein Workfront-Benutzerattribut ausgewählt haben und der Wert während der Verbindung NULL ist, wird dieses Feld mit dem entsprechenden Standardwert im System ausgefüllt. Geben Sie hier nur einen Wert ein, wenn Sie Attributzuordnungsregeln anwenden möchten (siehe Schritt 7). Der Standardwert dient als Ausnahme zu diesen Regeln.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf **Regeln** , um dem Attribut eine Regel hinzuzufügen.

   1. Wählen Sie in der Dropdown-Liste den Attributmodifikator aus, den Sie verwenden möchten.
   1. Geben Sie in die 2 Felder rechts den Wert des Ordnerattributs und den Wert ein, durch den Sie ihn ersetzen möchten.

      ![](assets/rule-fields.png)

   Sie können auf **Regel hinzufügen** klicken, um dem Attribut weitere Regeln hinzuzufügen.

1. (Optional) Um weitere Benutzerattribute zuzuordnen, klicken Sie auf **Zuordnung hinzufügen** und wiederholen Sie die Schritte 6 bis 7.
1. Klicken Sie auf **Speichern**.

### Zuordnen von Benutzerattributen zum einheitlichen Adobe-Erlebnis

1. Klicken Sie auf das Symbol **Hauptmenü** oben links in Adobe Workfront und dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-left.png)

1. Klicken Sie auf **System** > **Single Sign-On (SSO)**.

1. Wählen Sie die Registerkarte **Adobe** aus.

1. (Optional und bedingt) Wenn für Ihr Unternehmen die Zuordnung von Attributen im klassischen Erlebnis konfiguriert wurde und Sie diese Zuordnung in das einheitliche Erlebnis auf Adobe kopieren möchten, klicken Sie auf **Zuordnungen migrieren**. Sie können diese Zuordnungen dann verwerfen, löschen oder bearbeiten.

   >[!NOTE]
   >
   >Es wird empfohlen, Zuordnungen beim ersten Konfigurieren von Zuordnungen im einheitlichen Erlebnis Adobe zu migrieren. Es schadet nicht, sie später erneut zu migrieren, aber es ist nicht nötig, sie mehr als einmal zu migrieren.

1. Um eine neue Attributzuordnung zu erstellen, klicken Sie auf **Zuordnung hinzufügen**.

1. Klicken Sie auf den Pfeil neben dem Workfront-Feldnamen und wählen Sie das Feld [!DNL Workfront] aus, das Sie zuordnen möchten.

1. (Optional) Wenn Sie mehr als eine Regel für ein bestimmtes Feld erstellen möchten, klicken Sie auf den Pfeil neben **Immer** und wählen Sie den Operator aus, den die Regel verwenden soll.

1. (Bedingt) Wenn Sie neben &quot;Immer&quot;einen Operator ausgewählt haben, wählen Sie das Feld Workfront und den Wert aus, für den der Operator gilt.

   >[!NOTE]
   >
   >Die Operatoren `Is Truthy` und `Is Falsy` benötigen keine Werte.

1. Wählen Sie aus, ob Sie den Wert eines Attributs in Ihrem Identitätsmanager auf das Workfront-Feld anwenden möchten oder ob Sie einen bestimmten Konstantenwert anwenden möchten.

1. Geben Sie den Namen des Identitäts-Manager-Felds ein, das Sie anwenden möchten, oder geben Sie den Text der Konstante ein, die Sie anwenden möchten.

1. (Optional) Um weitere Regeln für dasselbe Workfront-Feld hinzuzufügen, klicken Sie auf **Neue Regel hinzufügen** und führen Sie die Schritte 4 bis 9 aus.

   >[!IMPORTANT]
   >
   > * Jede Regel unterhalb einer Immer -Regel wird ignoriert. Wenn Sie über eine Regel vom Typ Immer verfügen, müssen Sie sie an den unteren Rand der Regelliste verschieben. Sie können Regeln in der Liste verschieben, indem Sie auf das Menü mit den drei Punkten rechts von der Regel klicken und die Regel nach oben oder unten verschieben.
   > * Um eine Regel in der Mitte der Liste zu erstellen, klicken Sie auf das Menü mit den drei Punkten neben der Regel, die über oder unter der neuen Regel liegen soll, und wählen Sie **Regel über** oder **Regel darunter hinzufügen** aus.

1. Um eine Regel zu löschen, klicken Sie auf das Menü mit drei Punkten neben der Regel, die Sie löschen möchten, und wählen Sie **Löschen** aus.
1. Um eine Zuordnung zu löschen, klicken Sie auf das Symbol **Löschen** auf der Karte für diese Zuordnung.

1. Scrollen Sie zum Speichern zum oberen Rand der Seite und klicken Sie auf **Speichern**.


