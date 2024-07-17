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
source-git-commit: 063c4a885d43b41ba6ff72ac22a1552486531fa6
workflow-type: tm+mt
source-wordcount: '1239'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Organisationen und Teams

Die Organisations- und Teams-Funktionen von [!DNL Adobe Workfront Fusion] ermöglichen es Unternehmen, den Zugriff auf Szenarien und andere Funktionen in Fusion zu steuern.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen ein [!DNL Workfront Fusion] -Administrator für Ihre Organisation sein.</p>
     <p>Sie müssen ein [!DNL Workfront Fusion] -Administrator für Ihr Team sein.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<p>**Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] Lizenzen</a></p>


## Organisationen

[!DNL Workfront Fusion] -Benutzer gehören einer Organisation an.

* [Organisationsrollen](#organization-roles)
* [Einladen von Benutzern zu einer Organisation](#inviting-users-to-an-organization)
* [Zwischen Organisationen wechseln](#switch-between-organizations)

### Organisationsrollen

Ein Benutzer hat in einer Organisation eine der folgenden Rollen:

* **[!UICONTROL Inhaber]**: Der Eigentümer verfügt über alle Berechtigungen, die in der Organisation verfügbar sind.
* **[!UICONTROL Admin]**: Die Administratorrolle ermöglicht es einem Benutzer, Teams und Benutzer für die Organisation zu erstellen und zu verwalten.
* **[!UICONTROL Member]**: Mitglieder können [!DNL Workfront Fusion] verwenden, können jedoch keine organisatorischen Änderungen vornehmen.
* **[!UICONTROL Kontoinhaber]**: Eine Kontorolle ermöglicht es Benutzern nur, Lizenzinformationen im Organisations-Dashboard anzuzeigen.
* **[!UICONTROL App-Entwickler]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird demnächst bereitgestellt. Es wird empfohlen, dieser Rolle derzeit keine Benutzer zuzuweisen.

Informationen zu bestimmten Aktionen, die Benutzern in den verschiedenen Rollen der Organisation zur Verfügung stehen, finden Sie unter [Organisations- und Teamrollen](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Einladen von Benutzern zu einer Organisation

Standardmäßig kann ein Organisationsinhaber (oder autorisierter Benutzer) eine andere Person einladen, ihrer Organisation beizutreten.

So laden Sie einen Benutzer zum Beitritt zu einer Organisation ein:

1. Klicken Sie oben rechts im Bildschirm auf **[!UICONTROL Details ändern]** .
1. Wählen Sie **[!UICONTROL Neuen Benutzer einladen]** aus.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Geben Sie die E-Mail-Adresse und den Namen des Benutzers ein.
1. Wählen Sie eine Rolle für den Benutzer aus. Weitere Informationen zu Rollen finden Sie unter [Organisationsrollen](#organization-roles) in diesem Dokument.
1. (Optional) Fügen Sie eine Anmerkung hinzu. Dieser Hinweis wird in der Einladungs-E-Mail angezeigt, die der Benutzer erhält.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

[!DNL Fusion] sendet eine E-Mail mit einer Einladung an die jeweilige Organisation und der Schaltfläche [!UICONTROL Rolle akzeptieren] .

Wenn der Empfänger auf die Schaltfläche klickt, wird er zur Einladungsseite weitergeleitet, wo er die Einladung annehmen kann.

Die Einladung läuft in einem Tag ab.

>[!NOTE]
>
>Wenn der Benutzer neu bei [!DNL Fusion] ist, erstellt [!DNL Fusion] automatisch ein Konto für ihn und sendet eine E-Mail mit einem temporären Kennwort, wodurch der neue Benutzer angewiesen wird, sich anzumelden und sein Kennwort zu ändern.

### Zwischen Organisationen wechseln

Sie können Teil mehrerer Organisationen in Fusion sein. Ressourcen werden nicht zwischen Organisationen freigegeben.

Sie können Organisationen innerhalb des Adobe Unified Experience wechseln, indem Sie auf den Organisationsnamen oben rechts klicken und die neue Organisation aus der Dropdown-Liste auswählen. Nur Organisationen mit einem Fusion-Konto werden in der Dropdown-Liste angezeigt, auch wenn Sie Mitglied anderer Organisationen im Adobe sind.

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
>Da Teams den Zugriff auf Ressourcen steuern, ist es manchmal nützlich, wenn ein Team nur über ein Mitglied verfügt. Beispielsweise können Benutzer in der Schulung Verbindungen zu ihren einzelnen [!DNL Google]-Konten erstellen. Alle Teammitglieder können sich auch mit dem jeweiligen [!DNL Google]-Konto verbinden. In diesem Fall ist es also am besten, dass der Benutzer das einzige Mitglied eines Trainings-Teams ist.

Organisationen können über beliebig viele Teams verfügen und Benutzer können einem oder mehreren Teams angehören.

Benutzer können ihr Team aus der Dropdown-Liste im linken Navigationsbereich auswählen. Benutzer sehen nur Teams, denen sie angehören. Durch die Auswahl eines Teams kann ein Benutzer auf die Ressourcen dieses Teams zugreifen.

* [Teamrollen](#team-roles)
* [Team-Management](#team-management)

### Teamrollen

Ein Benutzer hat in jedem seiner Teams eine der folgenden Rollen:

* **[!UICONTROL Team-Administrator]**: Neben den Funktionen der anderen Teamrollen ermöglicht die Administratorrolle dem Benutzer das Hinzufügen, Entfernen und Ändern der Rolle eines Teammitglieds.
* **[!UICONTROL Team-Mitglied]**: Mit der Team-Mitgliederrolle können Benutzer Szenarien erstellen und ausführen.
* **[!UICONTROL Team Monitoring]**: Die Rolle [!UICONTROL Monitoring] ermöglicht Benutzern den Zugriff auf Ausführungsinformationen für Szenarien, kann jedoch keine Szenarien entwerfen oder ihren Status &quot;Aktiv&quot;ändern.
* **[!UICONTROL Team-Operator]**: Mit der Rolle [!UICONTROL Operator] können Benutzer Ausführungsdaten anzeigen und den Status &quot;Aktiv&quot;von Szenarien ändern.
* **[!UICONTROL Team Restricted Member]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird in naher Zukunft bereitgestellt. Es wird empfohlen, dieser Rolle derzeit keine Benutzer zuzuweisen.

Informationen zu bestimmten Aktionen, die Benutzern in den einzelnen Teamrollen zur Verfügung stehen, finden Sie unter [Organisations- und Teamrollen](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Team-Management

* [Team erstellen](#create-a-team)
* [Festlegen von Team-Benachrichtigungsoptionen](#set-team-notification-options)

#### Team erstellen

Organisationseigentümer und -administratoren können Teams erstellen.

So erstellen Sie ein Team:

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Organisation]** .
1. Wählen Sie die Registerkarte **[!UICONTROL Team]** aus.
1. Klicken Sie unter der Liste der Teams auf **[!UICONTROL Neues Team hinzufügen]** .
1. Geben Sie einen Namen für das neue Team ein und klicken Sie auf **Hinzufügen**.

#### Festlegen von Team-Benachrichtigungsoptionen

>[!NOTE]
>
>Wenn Ihr Unternehmen in Unified Shell verschoben wurde, erhalten Sie Benachrichtigungen über den Bereich Adobe-Benachrichtigungen. Sie müssen das Unified Shell-Erlebnis verwenden, um Benachrichtigungen im Bereich Adobe-Benachrichtigungen anzeigen zu können.
>
>Um das Unified Shell-Erlebnis, einschließlich des Bereichs Adobe-Benachrichtigungen, zu verwenden, klicken Sie oben auf der Seite auf die Schaltfläche Neue Fusion ausprobieren in Unified Experience . Diese Schaltfläche ist nur verfügbar, wenn Ihr Unternehmen in die Unified Shell verschoben wurde.
>
>Weitere Informationen finden Sie unter [Zugriff auf Ihre Benachrichtigungen](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) in [!DNL Adobe Unified Experience] für [!DNL Workfront Fusion].

Die Optionen für E-Mail-Benachrichtigungen werden auf Teamebene festgelegt.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Team]** .
1. Wählen Sie die Registerkarte **[!UICONTROL Benachrichtigungsoptionen]** aus.
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
      <td><p>Erhalten Sie eine E-Mail, wenn ein Szenario deaktiviert wird.</p><p><b>Hinweis:</b> Sie werden nur über die Deaktivierung eines Szenarios benachrichtigt, wenn das Szenario aufgrund von Fehlern automatisch deaktiviert wurde. Sie erhalten keine Benachrichtigungen zu Szenarien, die manuell deaktiviert werden.</p><p>In einigen Fällen kann ein Szenario vom [!DNL Workfront Fusion] -Technikerteam deaktiviert werden, da das Szenario Leistungsprobleme oder andere Probleme verursacht. In diesen Fällen erhalten Sie keine Benachrichtigungen in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Änderungen an Benachrichtigungsoptionen werden automatisch gespeichert

#### Zwischen Teams wechseln

Sie können Teil mehrerer Teams in Fusion sein. Da Teams keine Ressourcen gemeinsam nutzen, müssen Sie möglicherweise die Teams wechseln, um auf bestimmte Szenarien oder andere Ressourcen zuzugreifen.

Wenn Ihr Unternehmen nicht Teil des Adobe Unified Experience ist, können Sie zwischen Teams wechseln, indem Sie im linken Navigationsbereich auf den Teamnamen klicken und dann aus der Dropdown-Liste ein Team auswählen.

Wenn Ihr Team das einheitliche Adobe-Erlebnis nutzt, können Sie ein neues Team auswählen, indem Sie in der Kopfzeile auf den Teamnamen klicken und dann aus der Dropdown-Liste ein Team auswählen. Diese Option ist auf allen Seiten verfügbar, die für ein bestimmtes Team spezifisch sind, z. B. auf einer Szenario-Seite oder auf der Seite Verbindungen .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->