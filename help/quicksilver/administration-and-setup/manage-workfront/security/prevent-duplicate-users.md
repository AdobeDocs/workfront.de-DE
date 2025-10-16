---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Verhindern von Benutzerduplikaten
description: Beim Erstellen eines neuen Benutzers in Adobe Workfront können Sie keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, auch wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist (z. B. JohnDoe@example.com und johndoe@example.com). Um sich auf künftige Authentifizierungsverbesserungen vorzubereiten, stellen Sie außerdem sicher, dass alle Benutzer über eindeutige E-Mail-Adressen in einer Workfront-Instanz verfügen.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Verhindern von Benutzerduplikaten

Beim Erstellen eines neuen Benutzers in Adobe Workfront können Sie keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, auch wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist (z. B. JohnDoe@example.com und johndoe@example.com). Um sich auf künftige Authentifizierungsverbesserungen vorzubereiten, stellen Sie außerdem sicher, dass alle Benutzer über eindeutige E-Mail-Adressen in einer Workfront-Instanz verfügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzer mit eindeutigen E-Mail-Adressen erstellen

Ab Version 2019.4 können Sie bei der Erstellung eines neuen Benutzers in Workfront keine E-Mail-Adresse mehr verwenden, die bereits von einem anderen Benutzer verwendet wird, auch wenn die E-Mail-Adresse von Fall zu Fall unterschiedlich ist. Sie können beispielsweise keinen Benutzer mit der E-Mail-Adresse JohnDoe@example.com erstellen, wenn ein anderer Benutzer die E-Mail-Adresse johndoe@example.com hat.

## Aktualisieren der E-Mail-Adressen bestehender Benutzender in Ihrer Workfront-Instanz

Als Workfront-Administrator müssen Sie bestehende Benutzende mit übereinstimmenden E-Mail-Adressen aktualisieren, die sich nur durch die Groß-/Kleinschreibung unterscheiden.
So beheben Sie doppelte E-Mail-Adressen in einer Workfront-Instanz:

1. Untersuchen Sie alle doppelten Benutzer und entscheiden Sie, welcher Benutzer nicht mehr benötigt wird.

   {{step-1-to-users}}

   1. Wählen Sie im **Filter**-Menü **Alle** aus.

   1. Wählen Sie im **Ansicht**-Menü **Benutzeranmeldung** aus.

   1. Wählen Sie im **Gruppierung** die Option **Nichts** aus.

   1. Anpassen der Ansicht „Benutzeranmeldung“.

      1. Klicken Sie **Ansicht** > **Ansicht anpassen**.

      1. Ersetzen Sie die Spalte **ID** durch die Spalte **E-Mail-Adresse** .

      1. Benennen Sie die Ansicht um und speichern Sie sie.

   1. Erstellen Sie eine neue Gruppierung.

      1. Klicken Sie **Gruppierung** > **Neue Gruppierung**.

      1. Klicken **oben rechts auf** Seite auf „Zum Textmodus wechseln“.
      1. Fügen Sie den folgenden Textmodus-Code ein:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Benennen Sie die Gruppierung um und speichern Sie sie.

1. Führen Sie einen der folgenden Schritte aus:

   * (Bevorzugte Methode) Fügen Sie der E-Mail-Adresse des Benutzers für jedes zusätzliche Konto eine + -Adresse hinzu.

     Wählen Sie diese Option aus, wenn ein einzelner Benutzer in Ihrer Organisation Zugriff auf mehr als ein Benutzerkonto benötigt. Wenn die Plus-Adressierung von Ihrem E-Mail-Anbieter nicht unterstützt wird, müssen Sie für jedes Workfront-Konto ein separates E-Mail-Konto angeben.

     John Doe kann beispielsweise ein Benutzerkonto für sein Täglichkeitskonto und eines für Testzwecke haben:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Ändern Sie die Domain, um eine gefälschte Domain zu verwenden, indem Sie den folgenden Text an die E-Mail-Adresse anhängen:

     `.inactive`

     Beispielsweise könnte Martin Müller die folgenden Domains haben: (Diese müssen eindeutig sein.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Sie können sich nicht mehr bei diesen Konten anmelden, da für das Zurücksetzen des Kennworts eine gültige E-Mail-Adresse erforderlich ist. Auf diese Konten kann nur über die Funktion „Anmelden als“ zugegriffen werden.

   * Nicht benötigte Benutzer löschen

     >[!IMPORTANT]
     >
     >Wählen Sie diese Option nur für Konten aus, die versehentlich erstellt wurden, oder für Testkonten. Diese Option wird in der Regel nur für Konten mit null oder 1 falschen Anmeldung durchgeführt. Konten, die regelmäßig verwendet wurden, sollten niemals gelöscht werden.

Wenn sich Benutzende in einer Workfront-Instanz mit übereinstimmenden E-Mail-Adressen befinden, die sich nur von Fall zu Fall unterscheiden, wird Workfront Sie mit zusätzlichen Informationen und einem Zeitplan kontaktieren, wenn diese aktualisiert werden müssen.
