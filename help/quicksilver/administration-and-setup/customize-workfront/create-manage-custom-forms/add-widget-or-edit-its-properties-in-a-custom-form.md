---
title: Hinzufügen oder Bearbeiten von Bildern oder anderen Asset-Widgets in einem benutzerdefinierten Formular
description: Sie können die Eigenschaften der folgenden Asset-Widgets wie Bilder, Videos, PDF-Dateien und Adobe XD-Dateien in einem benutzerdefinierten Formular hinzufügen oder bearbeiten. Dies ist nützlich, wenn Sie visuelle Inhalte wie Branding-Bilder, ein Video mit Anweisungen oder einen interaktiven Prototyp für eine App einbeziehen müssen, die Sie entwerfen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: 8e903592456512f1ebf5f1e8d6e496e577a7b352
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 1%

---

# Hinzufügen oder Bearbeiten von Bildern oder anderen Asset-Widgets in einem benutzerdefinierten Formular

Sie können die Eigenschaften der folgenden Asset-Widgets in einem benutzerdefinierten Formular hinzufügen oder bearbeiten:

* Bild
* Video
* PDF-Datei
* Adobe XD-Datei

Dies ist nützlich, wenn Sie visuelle Inhalte wie Branding-Bilder, ein Video mit Anweisungen oder einen interaktiven Prototyp für eine App einbeziehen müssen, die Sie entwerfen.

Wenn ein benutzerdefiniertes Formular, das ein Widget enthält, an ein Objekt angehängt wird, können Benutzer, die mit dem Objekt arbeiten, es in den folgenden Bereichen sehen:

* Der Detailbereich des Objekts (z. B. für ein Projekt, den Bereich Projektdetails )
* Das Feld &quot;Bearbeiten&quot;für das Objekt, wenn das neue Adobe Workfront-Erlebnis wie &quot;Projekt bearbeiten&quot;und &quot;Aufgabe bearbeiten&quot;angezeigt wird

Derzeit können Benutzer das Widget nicht in den folgenden Bereichen sehen: &#x200B;

* Listen und Berichte
* Startseite und Zusammenfassung
* Das Feld &quot;Bearbeiten&quot;für das Objekt, wenn es nicht das neue Adobe Workfront-Erlebnis anzeigt (z. B. das Feld &quot;Kosten bearbeiten&quot;)
* Die mobile Workfront-App


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Hinzufügen oder Bearbeiten eines Asset-Widgets in einem benutzerdefinierten Formular

1. Beginnen Sie mit der Arbeit an einem benutzerdefinierten Formular, wie beschrieben in [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Mit dem **Feld hinzufügen** öffnen, führen Sie einen der folgenden Schritte aus:

   * Wenn Sie ein neues Widget hinzufügen, wählen Sie **Bild**, **PDF** oder **Video** , um es am unteren Rand des Formulars hinzuzufügen, oder ziehen Sie es an die gewünschte Position im Formular.

      ![](assets/add-widget.png)


   * Wenn Sie ein Widget hinzufügen möchten, das bereits zu einem anderen benutzerdefinierten Formular hinzugefügt wurde, klicken Sie auf **Feldbibliothek** und klicken Sie dann in der angezeigten Liste auf den Namen des Widgets. Weitere Informationen finden Sie unter [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Wenn Sie ein Widget bearbeiten, das dem benutzerdefinierten Formular bereits hinzugefügt wurde, wählen Sie es aus.

1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget.</p> <p>Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> <p><b>WICHTIG</b>: Obwohl dies möglich ist, empfehlen wir, diesen Namen nicht zu ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Widget beginnen. Ist dies der Fall, erkennt das System das Widget nicht mehr, wo es jetzt in anderen Bereichen von Workfront referenziert wird. </p> <p>Jeder Widget-Name muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben oder fügen Sie die URL des Widgets ein, in dem es im Internet gespeichert ist.</p> 
       <p><strong>Wichtig</strong>: Die URL für muss eine öffentliche URL sein. </p>
      <p>Wenn Sie ein Video-Widget hinzufügen, können Sie dies derzeit tun, indem Sie Folgendes in das URL-Feld hinzufügen:</p> 
      <ul> 
      <li> <p>YouTube- oder Vimeo-Link</p> </li> 
      <li> <p>Videolink "Google Drive"</p> </li> 
      <li> <p>Link zum Video mit MP4- und MOV-Erweiterung</p> </li> 
      <li> <p>Link zu Video, das bereits in den Bereich "Dokumente"in Ihrer Workfront-Instanz hochgeladen wurde. Anweisungen finden Sie unter <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich "Dokumente"</a> in diesem Artikel.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitungen</td> 
      <td> <p>Geben Sie weitere Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größe</td> 
      <td>Ändern Sie die Anzeigegröße des Widgets nach Bedarf.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Anwenden**.
1. Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Benutzerdefiniertes Formular in der Vorschau anzeigen und ausfüllen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Hinzufügen einer XD-Datei zu einem benutzerdefinierten Formular

1. Beginnen Sie mit der Arbeit an einem benutzerdefinierten Formular, wie beschrieben in [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Mit dem **Feld hinzufügen** öffnen, wählen Sie **Adobe XD**.
1. Geben Sie eine der folgenden Eigenschaften für das Widget ein oder bearbeiten Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Bezeichnung</td> 
      <td> <p>(Erforderlich) Geben Sie eine beschreibende Bezeichnung ein, die über dem Widget angezeigt werden soll. Sie können den Titel jederzeit ändern.</p> <p><b>WICHTIG</b>: Vermeiden Sie die Verwendung von Sonderzeichen in dieser Bezeichnung. Sie werden in Berichten nicht korrekt angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>(Erforderlich) Mit diesem Namen identifiziert das System das Widget.</p> <p>Wenn Sie das Widget zum ersten Mal konfigurieren und den Titel eingeben, wird das Feld Name automatisch entsprechend ausgefüllt. Die Felder Titel und Name werden jedoch nicht synchronisiert. Dies gibt Ihnen die Möglichkeit, die Beschriftung zu ändern, die Ihre Benutzer sehen, ohne den Namen ändern zu müssen, den das System sieht.</p> <p><b>WICHTIG</b>: Obwohl dies möglich ist, empfehlen wir, diesen Namen nicht zu ändern, nachdem Sie oder andere Benutzer mit der Verwendung des benutzerdefinierten Formulars in Widget beginnen. Ist dies der Fall, erkennt das System das Widget nicht mehr, wo es jetzt in anderen Bereichen von Workfront referenziert wird. </p> <p>Jeder Widget-Name muss in der Workfront-Instanz Ihres Unternehmens eindeutig sein. Auf diese Weise können Sie ein bereits für ein anderes benutzerdefiniertes Formular erstelltes Formular wiederverwenden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Erforderlich) Geben Sie einen gültigen XD Prototyplink ein oder fügen Sie ihn ein.</p> 
      <p>Hinweis: Die Einstellung Link-Zugriff auf die Registerkarte Freigabe in Adobe XD muss auf Jeder mit dem Link festgelegt sein. Andernfalls können Benutzer den Prototyp nicht anzeigen. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anleitungen</td> 
      <td> <p>(Optional) Geben Sie zusätzliche Informationen zum Widget ein. Wenn Benutzer das benutzerdefinierte Formular ausfüllen, können sie den Mauszeiger über das Fragezeichen-Symbol bewegen, um eine QuickInfo mit den hier eingegebenen Informationen anzuzeigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Größe</td> 
      <td>(Optional) Ändern Sie bei Bedarf die Anzeigegröße des Widgets.</td> 
     </tr> 
    </tbody> 
   </table>

1. Wenn Sie Ihr benutzerdefiniertes Formular auf andere Weise weiter erstellen möchten, führen Sie einen der folgenden Artikel aus:

   * [Positionieren von benutzerdefinierten Feldern und Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Wiederverwenden eines benutzerdefinierten Felds oder Widgets in einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Vorhandenes berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular wiederverwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Anzeigenlogik hinzufügen und Logik zu einem benutzerdefinierten Formular überspringen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Benutzerdefiniertes Formular in der Vorschau anzeigen und ausfüllen](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Hinzufügen eines Video-Widgets zu einem benutzerdefinierten Formular aus dem Bereich &quot;Dokumente&quot; {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Wenn Sie einem benutzerdefinierten Formular auf diese Weise ein Video hinzufügen, gelten nur die für das benutzerdefinierte Formular festgelegten Berechtigungen für das Video, wenn Benutzer auf das Formular eines Objekts zugreifen, nicht die Berechtigungen, die für das Video im Bereich &quot;Dokumente&quot;festgelegt wurden.

1. Gehen Sie zum Video im Bereich Dokumente und generieren Sie einen Testversand dafür, wie beschrieben in [Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öffnen Sie den Testversand.
1. Klicken Sie mit der rechten Maustaste auf eine beliebige Stelle im Video und wählen Sie **Videoadresse kopieren**.
1. Fügen Sie die kopierte Adresse in das benutzerdefinierte Formular ein, in das Sie das Video-Widget einfügen. **URL** ankreuzen.
