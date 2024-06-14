---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Benutzer für Single Sign-on aktualisieren
description: Sie können Benutzer für Single Sign-on in Workfront aktualisieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 1%

---

# Benutzer für Single Sign-on aktualisieren

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Wenn Single Sign-on (SSO) in Ihrer Adobe Workfront-Instanz aktiviert ist, können sich Ihre Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden.

Wenn Sie über ein vorhandenes System verfügen, das bereits mit Benutzern gefüllt ist, die SSO-Anmeldeinformationen zugeordnet sind, können Sie die IDs der Benutzer in Workfront importieren, indem Sie eine Datei mit kommagetrennten Werten (CSV) in Workfront importieren.

Weitere Informationen zur Integration von Workfront in ein SSO-System finden Sie unter [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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
   <td> <p>Sie müssen Workfront-Administrator sein.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SSO-Benutzernamen

Je nachdem, welche SSO-Lösung Sie verwenden, kann der Benutzername in Ihrer SSO-Umgebung wie folgt aufgerufen werden:

* SSO-Benutzername
* Federation-ID
* Federation Username

Unabhängig davon, wie der Benutzername in Ihrer SSO-Umgebung aufgerufen wird, wird der Wert des Felds im Feld SSO-Benutzername im Objekt Benutzer gespeichert.

Damit sich Ihre Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden können, müssen Sie ihr Profil so aktualisieren, dass neben ihrem Workfront-Benutzernamen auch ihr SSO-Benutzername angegeben wird.

Als Workfront-Administrator können Sie das Feld SSO-Benutzername für Ihre Workfront-Benutzer stapelweise aktualisieren, indem Sie eine Liste von Benutzernamen in Workfront importieren. Diese Liste muss

* Enthält die Workfront User ID (GUID) sowie den entsprechenden SSO-Benutzernamen für jeden Benutzer
* Als CSV- oder TSV-Datei speichern.

Dieser Prozess aktualisiert entweder vorhandene SSO-Benutzernamen in Workfront oder fügt einen neuen SSO-Benutzernamen hinzu, wenn dieser für Benutzer fehlt.

## Importdatei vorbereiten {#prepare-the-import-file}

Sie können mit der Vorbereitung Ihrer Importdatei beginnen, indem Sie einen Bericht aller Benutzer in Workfront erstellen, deren Felder für SSO-Benutzernamen aktualisiert werden müssen.

1. Erstellen Sie einen Benutzerbericht in Workfront.

   Anweisungen zum Erstellen von Benutzerberichten in Workfront finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie die folgenden Felder in Ihrem Bericht aus:

   | Feld | Erklärung |
   |---|---|
   | Name | Der vollständige Name des Workfront-Benutzers. |
   | ID | Die ID ist die alphanumerische Workfront-GUID. |
   | SSO-Benutzername | Das Feld SSO-Benutzername wird hinzugefügt, um sicherzustellen, dass Sie bei Ihrem Import keine Benutzernamen überschreiben. Dieses Feld sollte für alle Benutzer leer sein, wenn Ihre Benutzer noch nicht für SSO aktualisiert wurden. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Speichern Sie den Bericht.
1. Klicks **Export** oben im Bericht und exportieren Sie den Bericht nach Excel.
1. Öffnen Sie die exportierte Excel-Datei und fügen Sie in der Spalte SSO-Benutzername Ihre SSO-Benutzernamen für jeden Benutzer in den Bericht ein.

   >[!IMPORTANT]
   >
   >Bei SSO-Benutzernamen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Löschen Sie alle Spalten in der Excel-Datei mit Ausnahme der **ID** und **SSO-Benutzername** Spalten.

1. Löschen Sie die Spaltenüberschriften und stellen Sie sicher, dass oben im Bericht keine leeren Zeilen vorhanden sind.

   Die Datei, die Sie zum Aktualisieren Ihrer Workfront-Benutzer mit den SSO-Benutzernamen verwenden **must** enthalten nur 2 Spalten in der folgenden Reihenfolge:

   * In der ersten Spalte muss die Workfront-Benutzer-ID (die Benutzer-GUID, wie in Workfront zu finden) angezeigt werden.
   * Die zweite Spalte muss den SSO-Benutzernamen enthalten, wie er in Ihrem SSO-System angezeigt wird.
   * Die Spalten dürfen keine Kopfzeilen enthalten und dürfen oben in der Namensliste keine leeren Zeilen stehen.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Speichern Sie den Bericht als CSV- oder TSV-Datei auf Ihrem Computer.

## Benutzer für SSO aktualisieren {#update-your-users-for-sso}

Durch die Aktualisierung von Benutzern für SSO wird das Feld SSO-Benutzername entweder zu Ihren Workfront-Benutzern hinzugefügt, wenn kein Benutzer vorhanden ist, oder der Wert in diesem Feld aktualisiert, wenn bereits ein mit den Benutzern verknüpfter Wert vorhanden ist.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie auf **System** und wählen Sie **Benutzer für SSO aktualisieren**.

1. Klicks **Datei auswählen** um nach der von Ihnen vorbereiteten Datei zu suchen.

   Weitere Informationen zum Vorbereiten dieser Datei finden Sie unter [Importdatei vorbereiten](#prepare-the-import-file).

1. Wählen Sie die Datei aus, in der sie auf Ihrem Computer gespeichert ist, und klicken Sie dann auf **Öffnen**.

   Dadurch werden die SSO-Anmeldeinformationen in Workfront eingefügt, sodass sich alle Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden können.

   Die **Nur erlauben `<SSO Configuration>` Authentifizierung** ist für alle Benutzer aktiviert, die in der CSV-Datei enthalten sind. Dadurch wird sichergestellt, dass sich Benutzer über SSO anmelden müssen.

## SSO anhand der Workfront-Benutzernamen Ihrer Benutzer überprüfen

Anweisungen zum Erstellen eines Benutzerberichts mit Informationen zu SSO-Benutzernamen finden Sie unter [Importdatei vorbereiten](#prepare-the-import-file).

1. Führen Sie einen Benutzerbericht aus, der Informationen zu SSO-Benutzernamen enthält.

   Beachten Sie, dass die Spalte &quot;SSO-Benutzername&quot;für jeden Benutzer gefüllt ist.

1. Stellen Sie sicher, dass die Werte für die Spalte &quot;SSO-Benutzername&quot;mit dem SSO-Benutzernamen auf Ihrem SSO-Server übereinstimmen.
1. Wenn die Spalte &quot;SSO-Benutzername&quot;leer ist, aktualisieren Sie die SSO-Benutzernamen Ihrer Benutzer.

   ![](assets/users-with-sso-field-updated.png)

   Anweisungen zum Aktualisieren Ihrer Benutzer für SSO finden Sie unter [Benutzer für SSO aktualisieren](#update-your-users-for-sso).
