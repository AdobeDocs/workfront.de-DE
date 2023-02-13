---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Benutzer für Single Sign-on aktualisieren
description: Sie können Benutzer für Single Sign-on in Workfront aktualisieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Benutzer für Single Sign-on aktualisieren

{{important-admin-console-onboard}}

Wenn Single Sign-on (SSO) in Ihrer Adobe Workfront-Instanz aktiviert ist, können Sie sich mit Ihren SSO-Anmeldeinformationen bei Workfront anmelden.

Wenn Sie über ein vorhandenes System verfügen, das bereits mit Benutzern gefüllt ist, die SSO-Anmeldeinformationen zugeordnet sind, können Sie die IDs der Benutzer in Workfront importieren, indem Sie eine Datei mit kommagetrennten Werten (CSV) in Workfront importieren.

Weitere Informationen zur Integration von Workfront in ein SSO-System finden Sie unter [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO-Benutzernamen

Je nachdem, welche SSO-Lösung Sie verwenden, kann der Benutzername in Ihrer SSO-Umgebung wie folgt aufgerufen werden:

* SSO-Benutzername
* Federation-ID
* Federation Username

In Workfront werden alle diese Namen im Feld SSO-Benutzername im Benutzerobjekt gespeichert.

Damit sich Ihre Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden können, müssen Sie ihr Profil so aktualisieren, dass neben ihrem Workfront-Benutzernamen auch ihr SSO-Benutzername angegeben wird.

Als Workfront-Administrator können Sie das Feld &quot;SSO-Benutzername&quot;für Ihre Workfront-Benutzer stapelweise aktualisieren, indem Sie eine Liste mit Benutzernamen verwenden und es in Workfront importieren. Diese Liste muss die Workfront User ID (GUID) sowie den entsprechenden SSO-Benutzernamen für jeden Benutzer enthalten und als CSV- oder TSV-Datei gespeichert werden. Dieser Prozess aktualisiert entweder vorhandene SSO-Benutzernamen in Workfront oder fügt einen neuen SSO-Benutzernamen hinzu, wenn dieser für Benutzer fehlt.

## Importdatei vorbereiten {#prepare-the-import-file}

Sie können mit der Vorbereitung Ihrer Importdatei beginnen, indem Sie einen Bericht aller Benutzer in Workfront erstellen, deren Felder für SSO-Benutzernamen aktualisiert werden müssen.

1. Erstellen Sie einen Benutzerbericht in Workfront.

   Anweisungen zum Erstellen von Benutzerberichten in Workfront finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie die folgenden Felder in Ihrem Bericht aus:

   | Name | Der vollständige Name des Workfront-Benutzers. |
   |---|---|
   | ID | Die ID ist die alphanumerische Workfront-GUID. |
   | SSO-Benutzername | Wählen Sie das Feld SSO-Benutzername aus, um sicherzustellen, dass Sie bei Ihrem Import keine Benutzernamen überschreiben. Dieses Feld sollte für alle Benutzer leer sein, wenn Ihre Benutzer noch nicht für SSO aktualisiert wurden. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Speichern Sie den Bericht.
1. Klicken **Export** am oberen Rand des Berichts klicken und den Bericht nach Excel exportieren.
1. Öffnen Sie die exportierte Excel-Datei und fügen Sie in der Spalte &quot;SSO-Benutzername&quot;für jeden Benutzer im Bericht Ihre SSO-Benutzernamen hinzu.

   >[!IMPORTANT]
   >
   >Bei SSO-Benutzernamen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Alle Spalten in der Excel-Datei mit Ausnahme der **ID** und **SSO-Benutzername** Spalten.

1. Löschen Sie die Spaltenüberschriften und stellen Sie sicher, dass oben im Bericht keine leeren Zeilen vorhanden sind.

   Die Datei, die Sie zum Aktualisieren Ihrer Workfront-Benutzer mit den SSO-Benutzernamen verwenden, muss nur 2 Spalten in dieser Reihenfolge enthalten:

   * In der ersten Spalte sollte die Workfront-Benutzer-ID (die Benutzer-GUID, wie in Workfront zu finden) angezeigt werden.
   * Die zweite Spalte sollte den SSO-Benutzernamen enthalten, wie er in Ihrem SSO-System angezeigt wird.
   * Die Spalten sollten keine Kopfzeilen enthalten, und oben in der Namensliste dürfen keine leeren Zeilen stehen.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Speichern Sie den Bericht als CSV- oder TSV-Datei auf Ihrem Computer.

## Benutzer für SSO aktualisieren {#update-your-users-for-sso}

Durch die Aktualisierung von Benutzern für SSO wird das Feld SSO-Benutzername entweder zu Ihren Workfront-Benutzern hinzugefügt, wenn kein Benutzer vorhanden ist, oder der Wert in diesem Feld aktualisiert, wenn bereits ein mit den Benutzern verknüpfter Wert vorhanden ist.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **System** then **Benutzer für SSO aktualisieren**.

1. Klicken **Datei auswählen** um nach der von Ihnen vorbereiteten Datei zu suchen.

   Weitere Informationen zum Vorbereiten dieser Datei finden Sie unter [Importdatei vorbereiten](#prepare-the-import-file).

1. Wählen Sie die Datei aus, in der sie auf Ihrem Computer gespeichert ist, und klicken Sie dann auf **Öffnen**.

   Dadurch können sich alle Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden.

   Die **Nur erlauben `<SSO Configuration>` Authentifizierung** ist für alle Benutzer aktiviert, die in der CSV-Datei enthalten sind.

## Überprüfen Sie die SSO der Workfront-Benutzernamen Ihrer Benutzer.

Anweisungen zum Erstellen eines Benutzerberichts mit Informationen zu SSO-Benutzernamen finden Sie unter [Importdatei vorbereiten](#prepare-the-import-file).

1. Führen Sie einen Benutzerbericht aus, der Informationen zu SSO-Benutzernamen enthält.

   Beachten Sie, dass die Spalte &quot;SSO-Benutzername&quot;für jeden Benutzer gefüllt ist.

1. Stellen Sie sicher, dass die Werte für die Spalte &quot;SSO-Benutzername&quot;mit dem SSO-Benutzernamen auf Ihrem SSO-Server übereinstimmen.
1. Wenn die Spalte &quot;SSO-Benutzername&quot;leer ist, aktualisieren Sie die SSO-Benutzernamen Ihrer Benutzer.

   ![](assets/users-with-sso-field-updated.png)

   Anweisungen zum Aktualisieren Ihrer Benutzer für SSO finden Sie unter [Benutzer für SSO aktualisieren](#update-your-users-for-sso).
