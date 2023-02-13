---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Benutzerattribute zuordnen und neue Benutzer automatisch bereitstellen
description: Mit Single Sign-On (SSO) können Sie Attribute aus dem Active Directory Ihres Identitäts-Providers an Ihre Adobe Workfront-Benutzer übergeben. Sie können Workfront auch neue Benutzer über die Option "Automatische Bereitstellung"hinzufügen (auch "Just-in-Time-Bereitstellung"oder "JIT"genannt).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# Benutzerattribute zuordnen und neue Benutzer automatisch bereitstellen

Mit Single Sign-On (SSO) können Sie Attribute aus dem Active Directory Ihres Identitäts-Providers an Ihre Adobe Workfront-Benutzer übergeben. Sie können Workfront auch neue Benutzer über die Option &quot;Automatische Bereitstellung&quot;hinzufügen (auch &quot;Just-in-Time-Bereitstellung&quot;oder &quot;JIT&quot;genannt).

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde. Weitere Informationen erhalten Sie von Ihrem Netzwerk- oder IT-Administrator.


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipps für Zuordnungsattribute

Beachten Sie beim Zuordnen von Attributen Folgendes:

* Testen Sie immer in einer Vorschau-Sandbox oder einer Sandbox mit Kundenaktualisierung (CR).
* Testen Sie mit Administrator- und Nicht-Administrator-Konten, um sicherzustellen, dass Sie Attribute korrekt zuordnen.
* Attribute werden jedes Mal zugeordnet, wenn sich ein Benutzer über SSO bei Workfront anmeldet, nicht nur während der automatischen Bereitstellung.

## Benutzerattribute zuordnen und neue Benutzer automatisch bereitstellen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **System** > **Single Sign-On (SSO)**.

1. Im **Typ** Dropdown, klicken Sie auf **SAML 2.0**.

1. Klicken **Benutzerattribute zuordnen**.

   ![](assets/map-user-attributes.png)

1. (Optional) Wenn Sie möchten, dass Workfront automatisch neue Benutzer aus Ihrem Active Directory erstellt, klicken Sie auf **Benutzer für die automatische Bereitstellung**.

   Diese Funktion erfordert die Zuordnung von Attributen.

1. Ordnen Sie in der angezeigten Optionszeile die Attribute zu, die Sie für Ihre Workfront-Benutzer benötigen.

   Sie können Attribute wie &quot;Adresse&quot;, &quot;Manager&quot;, &quot;Auftragsrolle&quot;, &quot;Homepage&quot;usw. zuordnen.

   Attributzuordnungen funktionieren mit einem Verhältnis von 1:1. Sie können beispielsweise nicht jede Gruppe festlegen, zu der ein Benutzer gehört. Sie können pro Benutzer nur einen festlegen.

   >[!IMPORTANT]
   >
   >Die folgenden Attribute sind für jeden Benutzer erforderlich:
   >      
   >* Vorname
   >* Nachname
   >* E-Mail-Adresse

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
      <td>Geben Sie die SSO-Attributbeschriftung ein, die Sie verwenden möchten./td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">Standardwert</td> 
      <td> <p>Wenn Sie ein Workfront-Benutzerattribut ausgewählt haben und der Wert während der Verbindung NULL ist, wird dieses Feld mit dem entsprechenden Standardwert im System ausgefüllt. Geben Sie hier nur einen Wert ein, wenn Sie Attributzuordnungsregeln anwenden möchten (siehe Schritt 7). Der Standardwert dient als Ausnahme zu diesen Regeln.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Klicken Sie auf **Regeln** , um dem Attribut eine Regel hinzuzufügen.

   1. Wählen Sie in der Dropdown-Liste den gewünschten Attributmodifikator aus.
   1. Geben Sie in die 2 Felder rechts den Wert des Ordnerattributs und den Wert ein, durch den Sie ihn ersetzen möchten.

      ![](assets/rule-fields.png)
   Sie können auf **Regel hinzufügen** , um dem Attribut weitere Regeln hinzuzufügen.

1. (Optional) Um weitere Benutzerattribute zuzuordnen, klicken Sie auf **Zuordnung hinzufügen** und wiederholen Sie die Schritte 6 bis 7.
1. Klicken Sie auf **Speichern**.
