---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion-Organisationen und -Teams
description: Die Organisations- und Teams-Funktionen von Adobe Workfront Fusion ermöglichen es Unternehmen, den Zugriff auf Szenarien und andere Funktionen innerhalb von Fusion zu steuern.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Organisationen und Teams

[!DNL Adobe Workfront Fusion]Die Organisations- und Teams-Funktionen ermöglichen es Unternehmen, den Zugriff auf Szenarien und andere Funktionen in Fusion zu steuern.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>Workfront Fusion für Arbeitsautomatisierung und -integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihre Organisation.</p>
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihr Team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

<p>**Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen, siehe <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] Lizenzen</a></p>


## Organisationen

[!DNL Workfront Fusion] -Benutzer gehören einer Organisation an. Ihre [!DNL Fusion] -Lizenz bestimmt, wie viele aktive Szenarien und Connectoren in Ihrem Unternehmen verfügbar sind.

[!DNL Fusion] Die Lizenzierung bestimmt die Anzahl der aktiven Szenarien und aktiven Apps, die für ein Unternehmen verfügbar sind. [!DNL Fusion] zeigt die aktuellen &quot;Aktive Szenarien&quot;und &quot;Aktive Apps&quot;im Dashboard der Organisation an.

* [Organisationsrollen](#organization-roles)
* [Einladen von Benutzern zu einer Organisation](#inviting-users-to-an-organization)

### Organisationsrollen

Ein Benutzer hat in einer Organisation eine der folgenden Rollen:

* **[!UICONTROL Inhaber]**: Der Eigentümer verfügt über alle Berechtigungen, die in der Organisation verfügbar sind.
* **[!UICONTROL Admin]**: Die Administratorrolle ermöglicht es einem Benutzer, Teams und Benutzer für die Organisation zu erstellen und zu verwalten.
* **[!UICONTROL Mitglied]**: Mitglieder können [!DNL Workfront Fusion] können jedoch keine organisatorischen Änderungen vornehmen.
* **[!UICONTROL Buchhalter]**: Eine Rolle &quot;Buchhalter&quot;ermöglicht es Benutzern nur, Lizenzinformationen im Dashboard der Organisation anzuzeigen.
* **[!UICONTROL App-Entwickler]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird demnächst bereitgestellt. Es wird empfohlen, dieser Rolle derzeit keine Benutzer zuzuweisen.

### Einladen von Benutzern zu einer Organisation

Standardmäßig kann ein Organisationsinhaber (oder autorisierter Benutzer) eine andere Person einladen, ihrer Organisation beizutreten.

So laden Sie einen Benutzer zum Beitritt zu einer Organisation ein:

1. Klicken **[!UICONTROL Details ändern]** in der oberen rechten Ecke des Bildschirms.
1. Auswählen **[!UICONTROL Neuen Benutzer einladen]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Geben Sie die E-Mail-Adresse und den Namen des Benutzers ein.
1. Wählen Sie eine Rolle für den Benutzer aus. Weitere Informationen zu Rollen finden Sie unter [Organisationsrollen](#organization-roles) in diesem Dokument.
1. (Optional) Fügen Sie eine Anmerkung hinzu. Dieser Hinweis wird in der Einladungs-E-Mail angezeigt, die der Benutzer erhält.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

[!DNL Fusion] sendet eine E-Mail mit einer Einladung an die jeweilige Organisation und einer [!UICONTROL Rolle akzeptieren] Schaltfläche.

![](assets/accept-the-role.png)

Wenn der Empfänger auf die Schaltfläche klickt, wird er zur Einladungsseite weitergeleitet, wo er die Einladung annehmen kann.

Die Einladung läuft in einem Tag ab.

>[!NOTE]
>
>Wenn der Benutzer neu bei [!DNL Fusion], [!DNL Fusion] erstellt automatisch ein Konto für sie und sendet eine E-Mail mit einem temporären Kennwort, um den neuen Benutzer anzuweisen, sich anzumelden und sein Kennwort zu ändern.

## Teams

Teams sind Benutzergruppen, die Zugriff auf bestimmte Ressourcen haben. Diese Ressourcen können Folgendes umfassen:

* Szenarios
* Verbindungen
* Webhooks
* Schlüssel
* Datenspeicher
* Datenstrukturen
* Einstellungen für E-Mail-Benachrichtigungen

>[!NOTE]
>
>Da Teams den Zugriff auf Ressourcen steuern, ist es manchmal nützlich, wenn ein Team nur über ein Mitglied verfügt. Beispielsweise können Benutzer in Schulungen Verbindungen zu ihren einzelnen [!DNL Google] Konten. Alle Teammitglieder können sich auch mit der Person verbinden [!DNL Google] -Konto, daher ist es in diesem Fall am besten, dass der Benutzer das einzige Mitglied eines Trainings-Teams ist.

Organisationen können über beliebig viele Teams verfügen und Benutzer können einem oder mehreren Teams angehören.

Benutzer können ihr Team aus der Dropdown-Liste im linken Navigationsbereich auswählen. Benutzer sehen nur Teams, denen sie angehören. Durch die Auswahl eines Teams kann ein Benutzer auf die Ressourcen dieses Teams zugreifen.

* [Teamrollen](#team-roles)
* [Team-Management](#team-management)

### Teamrollen

Ein Benutzer hat in jedem seiner Teams eine der folgenden Rollen:

* **[!UICONTROL Team Admin]**: Zusätzlich zu den Funktionen der anderen Teamrollen ermöglicht es die Admin-Rolle dem Benutzer, die Rolle eines Teammitglieds hinzuzufügen, zu entfernen oder zu ändern.
* **[!UICONTROL Team Member]**: Mit der Teammitgliederrolle können Benutzer Szenarien erstellen und ausführen.
* **[!UICONTROL Team-Überwachung]**: Die [!UICONTROL Monitoring] -Rolle ermöglicht Benutzern den Zugriff auf Ausführungsinformationen für Szenarien, sie können jedoch keine Szenarien entwerfen oder ihren Status &quot;Aktiv&quot;ändern.
* **[!UICONTROL Team-Operator]**: Die [!UICONTROL operator] -Rolle ermöglicht es Benutzern, Ausführungsdaten anzuzeigen und den Status &quot;Aktiv&quot;von Szenarien zu ändern.
* **[!UICONTROL Team Eingeschränktes Mitglied]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird demnächst bereitgestellt. Es wird empfohlen, dieser Rolle derzeit keine Benutzer zuzuweisen.

### Team-Management

* [Team erstellen](#create-a-team)
* [Festlegen von Team-Benachrichtigungsoptionen](#set-team-notification-options)

#### Team erstellen

Organisationseigentümer und -administratoren können Teams erstellen.

So erstellen Sie ein Team:

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Einrichtung]**
1. Wählen Sie die **[!UICONTROL Team]** Registerkarte.
1. Klicken **[!UICONTROL Neues Team hinzufügen]** unter der Liste der Teams.
1. Geben Sie einen Namen für das neue Team ein und klicken Sie auf **Hinzufügen**.

#### Festlegen von Team-Benachrichtigungsoptionen

Die Optionen für E-Mail-Benachrichtigungen werden auf Teamebene festgelegt.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Team]**
1. Wählen Sie die **[!UICONTROL Benachrichtigungsoptionen]** Registerkarte.
1. Aktivieren Sie die Benachrichtigungen, die das Team erhalten soll.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL Warnung im Szenario-Run]'</td> 
      <td> <p>Eine E-Mail erhalten, wenn in einem Szenario eine Warnung angezeigt wird</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Fehler in Szenario run]</td> 
      <td>Erhalten Sie eine E-Mail, wenn bei einem Szenario ein Fehler auftritt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Szenario-Deaktivierung]</p> </td> 
      <td><p>Erhalten Sie eine E-Mail, wenn ein Szenario deaktiviert wird.</p><p><b>Hinweis:</b> Sie werden nur über die Deaktivierung eines Szenarios benachrichtigt, wenn das Szenario aufgrund von Fehlern automatisch deaktiviert wurde. Sie erhalten keine Benachrichtigungen zu Szenarien, die manuell deaktiviert werden.</p><p>In einigen Fällen kann ein Szenario vom [!DNL Workfront Fusion] Technikerteam, da das Szenario Leistungsprobleme oder andere Probleme verursacht. In diesen Fällen erhalten Sie keine Benachrichtigungen in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Änderungen an Benachrichtigungsoptionen werden automatisch gespeichert

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->