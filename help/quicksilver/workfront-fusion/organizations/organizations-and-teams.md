---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organisationen und Teams von Adobe Workfront Fusion
description: Die Organisations- und Team-Funktionen von Adobe Workfront Fusion ermöglichen es Unternehmen, den Zugriff auf Szenarien und andere Funktionen innerhalb von Fusion zu steuern.
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 063c4a885d43b41ba6ff72ac22a1552486531fa6
workflow-type: tm+mt
source-wordcount: '1239'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] Organisationen und Teams

Die Funktionen von [!DNL Adobe Workfront Fusion] für Organisation und Teams ermöglichen es Unternehmen, den Zugriff auf Szenarien und andere Funktionen in Fusion zu steuern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen ein [!DNL Workfront Fusion]-Administrator für Ihre Organisation sein.</p>
     <p>Sie müssen [!DNL Workfront Fusion] für Ihr Team sein.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

<p>**Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] von Lizenzen</a></p>


## Organisationen

[!DNL Workfront Fusion] Benutzer gehören einer Organisation an.

* [Organisationsrollen](#organization-roles)
* [Einladen von Benutzern in eine Organisation](#inviting-users-to-an-organization)
* [Wechseln zwischen Organisationen](#switch-between-organizations)

### Organisationsrollen

Ein Benutzer hat in einer Organisation eine der folgenden Rollen:

* **[!UICONTROL Inhaber]**: Der/die Verantwortliche verfügt über alle in der Organisation verfügbaren Berechtigungen.
* **[!UICONTROL Admin]**: Mit der Administratorrolle kann ein Benutzer Teams und Benutzer für die Organisation erstellen und verwalten.
* **[!UICONTROL Mitglied]**: Mitglieder können [!DNL Workfront Fusion] verwenden, aber keine organisatorischen Änderungen vornehmen.
* **[!UICONTROL Buchhalter]**: In einer Buchhalterrolle können Benutzende nur Lizenzinformationen im Organisations-Dashboard anzeigen.
* **[!UICONTROL App-]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird in naher Zukunft verfügbar gemacht. Es wird derzeit nicht empfohlen, dieser Rolle Benutzer zuzuweisen.

Informationen zu bestimmten Aktionen, die Benutzern in den einzelnen Organisationsrollen zur Verfügung stehen, finden Sie unter [Organisation und Teamrollen](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Einladen von Benutzern in eine Organisation

Standardmäßig kann ein Organisationsverantwortlicher (oder ein autorisierter Benutzer) eine andere Person einladen, ihrer Organisation beizutreten.

So laden Sie einen Benutzer ein, einer Organisation beizutreten:

1. Klicken **[!UICONTROL oben rechts]** Bildschirm auf „Details ändern“.
1. Wählen Sie **[!UICONTROL Neuen Benutzer einladen]** aus.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. Geben Sie die E-Mail-Adresse und den Namen des Benutzers ein.
1. Wählen Sie eine Rolle für den Benutzer aus. Weitere Informationen zu Rollen finden Sie unter [Organisationsrollen](#organization-roles) in diesem Dokument.
1. (Optional) Fügen Sie eine Anmerkung hinzu. Diese Anmerkung wird in der Einladungs-E-Mail angezeigt, die der Benutzer erhält.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

[!DNL Fusion] sendet eine E-Mail mit einer Einladung an die bestimmte Organisation und einer Schaltfläche [!UICONTROL Rolle annehmen].

Wenn der Empfänger auf die Schaltfläche klickt, wird er zur Einladungsseite weitergeleitet, auf der er die Einladung annehmen kann.

Die Einladung läuft in einem Tag aus.

>[!NOTE]
>
>Wenn [!DNL Fusion] für den Benutzer neu ist, erstellt [!DNL Fusion] automatisch ein Konto für ihn und sendet eine E-Mail mit einem temporären Kennwort, in der der neue Benutzer aufgefordert wird, sich anzumelden und sein Kennwort zu ändern.

### Wechseln zwischen Organisationen

Sie können Teil von mehr als einer Organisation in Fusion sein. Ressourcen werden nicht zwischen Organisationen geteilt.

Sie können innerhalb des einheitlichen Adobe-Erlebnisses zwischen Organisationen wechseln, indem Sie oben rechts auf den Organisationsnamen klicken und die neue Organisation aus der Dropdown-Liste auswählen. In der Dropdown-Liste werden nur Organisationen angezeigt, die über ein Fusion-Konto verfügen, auch wenn Sie Mitglied anderer Organisationen in Adobe sind.

## Teams

Teams sind Benutzergruppen, die den Zugriff auf bestimmte Ressourcen gemeinsam nutzen. Diese Ressourcen können Folgendes umfassen:

* Szenarios
* Verbindungen
* Webhooks
* Schlüssel
* Datenspeicher
* Datenstrukturen
* E-Mail-Benachrichtigungseinstellungen

>[!NOTE]
>
>Da Teams den Zugriff auf Ressourcen steuern, ist es manchmal nützlich, wenn ein Team nur über ein Mitglied verfügt. Beispielsweise können Benutzende in der Schulung Verbindungen zu ihren individuellen [!DNL Google]-Konten erstellen. Jedes Teammitglied kann sich auch mit dem individuellen [!DNL Google]-Konto verbinden. In diesem Fall ist es also am besten, wenn der Benutzer das einzige Mitglied eines Schulungsteams ist.

Organisationen können so viele Teams haben, wie sie benötigen, und Benutzer können zu einem oder mehreren Teams gehören.

Benutzer können ihr Team aus der Dropdown-Liste im linken Navigationsbereich auswählen. Benutzende sehen nur Teams, denen sie angehören. Die Auswahl eines Teams ermöglicht einem Benutzer den Zugriff auf die Ressourcen dieses Teams.

* [Teamfunktionen](#team-roles)
* [Team-Management](#team-management)

### Teamfunktionen

Benutzende haben in jedem ihrer Teams eine der folgenden Rollen:

* **[!UICONTROL Team-]**: Zusätzlich zu den Funktionen der anderen Teamrollen ermöglicht die Administratorrolle dem Benutzer das Hinzufügen, Entfernen oder Ändern der Rolle eines Teammitglieds.
* **[!UICONTROL Teammitglied]**: Die Rolle „Teammitglied“ ermöglicht Benutzern das Erstellen und Ausführen von Szenarien.
* **[!UICONTROL Team-Überwachung]**: Die Rolle [!UICONTROL Überwachung] ermöglicht Benutzern den Zugriff auf Ausführungsinformationen für Szenarien, sie können jedoch keine Szenarien entwerfen oder ihren „aktiven“ Status ändern.
* **[!UICONTROL Teamoperator]**: Die Rolle [!UICONTROL Operator] ermöglicht es Benutzern, Ausführungsdaten anzuzeigen und den Status „Aktiv“ von Szenarien zu ändern.
* **[!UICONTROL Team Eingeschränktes Mitglied]**: Die Funktionalität für diese Rolle ist derzeit nicht verfügbar und wird in naher Zukunft verfügbar gemacht. Es wird derzeit nicht empfohlen, dieser Rolle Benutzer zuzuweisen.

Informationen zu bestimmten Aktionen, die Benutzern in den einzelnen Team-Rollen zur Verfügung stehen, finden Sie unter [Organisation und Team-Rollen](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### Team-Management

* [Erstellen eines Teams](#create-a-team)
* [Festlegen der Team-Benachrichtigungsoptionen](#set-team-notification-options)

#### Erstellen eines Teams

Organisationsverantwortliche und Administratoren können Teams erstellen.

So erstellen Sie ein Team:

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Organisation]**
1. Wählen Sie die Registerkarte **[!UICONTROL Team]** aus.
1. Klicken Sie **[!UICONTROL Neues Team hinzufügen]** unter der Liste der Teams auf.
1. Geben Sie einen Namen für das neue Team ein und klicken Sie auf **Hinzufügen**.

#### Festlegen der Team-Benachrichtigungsoptionen

>[!NOTE]
>
>Wenn Ihr Unternehmen in die Unified Shell verschoben wurde, erhalten Sie Benachrichtigungen über den Bereich Adobe-Benachrichtigungen . Sie müssen Unified Shell verwenden, um Benachrichtigungen im Bereich Adobe-Benachrichtigungen anzeigen zu können.
>
>Um Unified Shell einschließlich des Bereichs Adobe-Benachrichtigungen zu verwenden, klicken Sie oben auf der Seite auf die Schaltfläche Neue Fusion-Benutzeroberfläche in Unified Experience ausprobieren . Diese Schaltfläche ist nur verfügbar, wenn Ihre Organisation in die Unified Shell verschoben wurde.
>
>Weitere Informationen finden Sie unter [Zugriff auf Ihre Benachrichtigungen](/help/quicksilver/workfront-fusion/fusion-in-admin-console/fusion-unified-experience.md#access-your-notifications) in [!DNL Adobe Unified Experience] für [!DNL Workfront Fusion].

Die Optionen für E-Mail-Benachrichtigungen werden auf Team-Ebene festgelegt.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Team]**
1. Wählen Sie die **[!UICONTROL Benachrichtigungsoptionen]** aus.
1. Aktivieren Sie die Benachrichtigungen, die Sie an das Team senden möchten.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[!UICONTROL-Warnung in Szenarioausführung]'</td> 
      <td> <p>Erhalten einer E-Mail bei einer Warnung in einem ausgeführten Szenario</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Fehler bei Szenarioausführung]</td> 
      <td>Erhalten Sie eine E-Mail, wenn bei der Ausführung eines Szenarios ein Fehler auftritt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Szenario-Deaktivierung]</p> </td> 
      <td><p>Erhalten Sie eine E-Mail, wenn ein Szenario deaktiviert wird.</p><p><b>Hinweis:</b> Sie werden nur dann über die Deaktivierung des Szenarios benachrichtigt, wenn das Szenario aufgrund von Fehlern automatisch deaktiviert wurde. Sie erhalten keine Benachrichtigungen über Szenarien, die manuell deaktiviert werden.</p><p>In einigen Fällen kann ein Szenario vom [!DNL Workfront Fusion]-Engineering-Team deaktiviert werden, da das Szenario Leistungs- oder andere Probleme verursacht. In diesen Fällen erhalten Sie keine Benachrichtigungen in [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

Änderungen an Benachrichtigungsoptionen werden automatisch gespeichert

#### Zwischen Teams wechseln

Sie können Teil von mehr als einem Team in Fusion sein. Da Teams keine gemeinsamen Ressourcen nutzen, müssen Sie möglicherweise Teams wechseln, um auf bestimmte Szenarien oder andere Ressourcen zuzugreifen.

Wenn Ihr Unternehmen nicht auf dem Adobe Unified Experience Platform ist, können Sie Teams wechseln, indem Sie im linken Navigationsbereich auf den Team-Namen klicken und dann aus der Dropdown-Liste ein Team auswählen.

Wenn sich Ihr Team auf der Adobe Unified Experience befindet, können Sie ein neues Team auswählen, indem Sie auf den Team-Namen in der Kopfzeile klicken und dann ein Team aus der Dropdown-Liste auswählen. Diese Option ist auf allen Seiten verfügbar, die für ein bestimmtes Team spezifisch sind, z. B. auf einer Szenarioseite oder auf der Seite Verbindungen .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->