---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Vermeiden von doppelten Benutzern
description: Bei der Erstellung eines neuen Benutzers in Adobe Workfront können Sie keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, selbst wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist (z. B. JohnDoe@example.com und johndoe@example.com). Um sich auf zukünftige Authentifizierungsverbesserungen vorzubereiten, stellen Sie außerdem sicher, dass alle Benutzer über eindeutige E-Mail-Adressen in einer Workfront-Instanz verfügen.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Vermeiden doppelter Benutzer

Bei der Erstellung eines neuen Benutzers in Adobe Workfront können Sie keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, selbst wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist (z. B. JohnDoe@example.com und johndoe@example.com). Um sich auf zukünftige Authentifizierungsverbesserungen vorzubereiten, stellen Sie außerdem sicher, dass alle Benutzer über eindeutige E-Mail-Adressen in einer Workfront-Instanz verfügen.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Erstellen von Benutzern mit eindeutigen E-Mail-Adressen

Ab Version 2019.4 können Sie bei der Erstellung eines neuen Benutzers in Workfront keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, selbst wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist. Sie können beispielsweise keinen Benutzer mit der E-Mail-Adresse JohnDoe@example.com erstellen, wenn ein anderer Benutzer die E-Mail-Adresse johndoe@example.com hat.

## E-Mail-Adressen vorhandener Benutzer in Ihrer Workfront-Instanz aktualisieren

Als Workfront-Administrator müssen Sie bestehende Benutzer aktualisieren, deren E-Mail-Adressen nur von Fall zu Fall verschieden sind.
So beheben Sie doppelte E-Mail-Adressen in einer Workfront-Instanz:

1. Untersuchen Sie doppelte Benutzer und entscheiden Sie, welcher Benutzer nicht mehr benötigt wird.

   {{step-1-to-users}}

   1. Wählen Sie im Menü **Filter** die Option **Alle** aus.

   1. Wählen Sie im Menü **Ansicht** die Option **Benutzeranmeldung**.

   1. Wählen Sie im Menü **Gruppierung** die Option **Nichts** aus.

   1. Passen Sie die Ansicht &quot;User Login&quot;an.

      1. Klicken Sie auf **Ansicht** > **Ansicht anpassen**.

      1. Ersetzen Sie die Spalte **ID** durch die Spalte **E-Mail-Adresse** .

      1. Benennen Sie die Ansicht um und speichern Sie sie.

   1. Erstellen Sie eine neue Gruppierung.

      1. Klicken Sie auf **Gruppierung** > **Neue Gruppierung**.

      1. Klicken Sie oben rechts auf der Seite auf **In den Textmodus wechseln** .
      1. Fügen Sie den folgenden Textmoduscode ein:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Benennen Sie die Gruppierung um und speichern Sie sie.

1. Führen Sie einen der folgenden Schritte aus:

   * (Bevorzugte Methode) Fügen Sie für jedes zusätzliche Konto eine + -Adresse zur E-Mail-Adresse des Benutzers hinzu.

     Wählen Sie diese Option, wenn ein einzelner Benutzer in Ihrem Unternehmen Zugriff auf mehr als ein Benutzerkonto benötigt. Wenn die plus-Adresse von Ihrem E-Mail-Anbieter nicht unterstützt wird, müssen Sie für jedes Workfront-Konto ein separates E-Mail-Konto angeben.

     John Doe kann beispielsweise über ein Benutzerkonto für sein tägliches Nutzungskonto und eines für Testzwecke verfügen:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Ändern Sie die Domain, um eine gefälschte Domain zu verwenden, indem Sie den folgenden Text an die E-Mail-Adresse anhängen:

     `.inactive`

     John Doe könnte beispielsweise die folgenden Domänen haben: (Diese müssen eindeutig sein.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Sie können sich nicht mehr bei diesen Konten anmelden, da für die Zurücksetzung von Passwörtern eine gültige E-Mail-Adresse erforderlich ist. Auf diese Konten kann nur mit der Funktion Anmelden als zugegriffen werden.

   * Nicht benötigte Benutzer löschen

     >[!IMPORTANT]
     >
     >Wählen Sie diese Option nur für versehentlich erstellte Konten oder für Testkonten. Diese Option wird normalerweise nur für Konten mit null oder 1 versehentlicher Anmeldung ausgeführt. Regelmäßig verwendete Konten sollten niemals gelöscht werden.

Wenn Sie Benutzer in einer Workfront-Instanz haben, deren E-Mail-Adressen nur von Fall zu Fall verschieden sind, kontaktiert Workfront Sie mit zusätzlichen Informationen und einer Zeitleiste, wenn diese aktualisiert werden müssen.
