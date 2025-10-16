---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Benutzer für einmaliges Anmelden aktualisieren
description: Sie können Benutzende für einmaliges Anmelden in Workfront aktualisieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 2%

---

# Benutzende für Single Sign-on aktualisieren

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Wenn Single Sign-on (SSO) in Ihrer Adobe Workfront-Instanz aktiviert ist, können sich Ihre Benutzerinnen und Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden.

Wenn Sie über ein bestehendes System verfügen, das bereits mit Benutzern gefüllt ist, die mit SSO-Anmeldeinformationen verknüpft sind, können Sie die Benutzer-IDs in Workfront importieren, indem Sie eine CSV-Datei (kommagetrennte Werte) in Workfront importieren.

Weitere Informationen zur Integration von Workfront in ein SSO-System finden Sie [Übersicht über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO-Benutzernamen

Je nachdem, welche SSO-Lösung Sie verwenden, kann der Benutzername in Ihrer SSO-Umgebung wie folgt bezeichnet werden:

* SSO-Benutzername
* Federation-ID
* Federation-Benutzername

Unabhängig davon, wie der Benutzername in Ihrer SSO-Umgebung aufgerufen wird, wird der Wert des Felds im Feld SSO-Benutzername im Benutzerobjekt gespeichert.

Damit sich Ihre Benutzerinnen und Benutzer mit ihren SSO-Anmeldeinformationen bei Workfront anmelden können, müssen Sie ihr Profil aktualisieren, um neben ihrem Workfront-Benutzernamen auch ihren SSO-Benutzernamen einzuschließen.

Als Workfront-Administrator können Sie für Ihre Workfront-Benutzer das Feld SSO-Benutzername stapelweise aktualisieren, indem Sie eine Liste von Benutzernamen in Workfront importieren. Diese Liste muss:

* Enthalten für jeden Benutzer die Workfront-Benutzer-ID (GUID) sowie den entsprechenden SSO-Benutzernamen
* als CSV- oder TSV-Datei gespeichert werden.

Dieser Prozess aktualisiert entweder bestehende SSO-Benutzernamen in Workfront oder fügt einen neuen SSO-Benutzernamen hinzu, wenn einer für Benutzende fehlt.

## Importdatei vorbereiten {#prepare-the-import-file}

Sie können mit der Vorbereitung Ihrer Importdatei beginnen, indem Sie einen Bericht aller Workfront-Benutzer erstellen, deren SSO-Benutzernamenfelder aktualisiert werden müssen.

1. Erstellen Sie einen Benutzerbericht in Workfront.

   Anweisungen zum Erstellen von Benutzerberichten in Workfront finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Folgende Felder in Ihrem Bericht auswählen:

   | Feld | Erklärung |
   |---|---|
   | Name | Der vollständige Name des Workfront-Benutzers. |
   | ID | Die ID ist die alphanumerische GUID von Workfront. |
   | SSO-Benutzername | Durch Hinzufügen des Felds SSO-Benutzername wird sichergestellt, dass keine Benutzernamen vorhanden sind, die durch den Import überschrieben werden. Dieses Feld sollte für alle Benutzer leer sein, wenn Ihre Benutzer noch nicht für SSO aktualisiert wurden. |

   ![Benutzer mit SSO-Benutzername, aber ohne Zugriff](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Speichern Sie den Bericht.
1. Klicken **oben** Bericht auf „Exportieren“ und exportieren Sie den Bericht nach Excel.
1. Öffnen Sie die exportierte Excel-Datei und fügen Sie Ihre SSO-Benutzernamen für jeden Benutzer im Bericht in der Spalte SSO-Benutzername hinzu.

   >[!IMPORTANT]
   >
   >Bei SSO-Benutzernamen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Löschen Sie alle Spalten in der Excel-Datei, mit Ausnahme der **ID** und der **SSO Username**-Spalten.

1. Löschen Sie die Spaltenüberschriften und stellen Sie sicher, dass oben im Bericht keine leeren Zeilen vorhanden sind.

   Die Datei, die Sie zum Aktualisieren Ihrer Workfront-Benutzer mit den SSO-Benutzernamen verwenden **muss** 2 Spalten in der folgenden Reihenfolge enthalten:

   * In der ersten Spalte muss die Workfront-Benutzer-ID angezeigt werden (die Benutzer-GUID wie in Workfront).
   * Die zweite Spalte muss den SSO-Benutzernamen enthalten, wie er in Ihrem SSO-System angezeigt wird.
   * Die Spalten dürfen keine Kopfzeilen und keine leeren Zeilen oben in der Namensliste enthalten.

     ![Benutzer-CSV aktualisieren](assets/update-users-for-sso-csv-file-for-import.png)

1. Speichern Sie den Bericht als CSV- oder TSV-Datei auf Ihrem Computer.

## Benutzer für SSO aktualisieren {#update-your-users-for-sso}

Beim Aktualisieren von Benutzern für SSO wird entweder das Feld SSO-Benutzername zu Ihren Workfront-Benutzern hinzugefügt, wenn noch kein SSO-Benutzername vorhanden ist, oder der Wert in diesem Feld wird aktualisiert, wenn den Benutzern bereits ein Wert zugeordnet ist.

{{step-1-to-setup}}

1. Klicken Sie auf **System** und wählen Sie dann **Benutzer für SSO aktualisieren** aus.

1. Klicken Sie **Datei auswählen**, um nach der von Ihnen vorbereiteten Datei zu suchen.

   Weitere Informationen zum Vorbereiten dieser Datei finden Sie unter [Vorbereiten der Importdatei](#prepare-the-import-file).

1. Wählen Sie die Datei aus, in der sie auf Ihrem Computer gespeichert ist, und klicken Sie dann auf **Öffnen**.

   Dadurch werden die SSO-Anmeldeinformationen in Workfront eingefügt, sodass sich alle Benutzenden mit ihren SSO-Anmeldeinformationen bei Workfront anmelden können.

   Die **Nur `<SSO Configuration>` Authentifizierung zulassen** Einstellung ist für alle in der CSV-Datei enthaltenen Benutzer aktiviert. Dadurch wird sichergestellt, dass sich Benutzer über SSO anmelden müssen.

## Überprüfen von SSO anhand der Workfront-Benutzernamen Ihrer Benutzer

Anweisungen zum Erstellen eines Benutzerberichts mit SSO-Benutzernamen-Informationen finden Sie unter [Importdatei vorbereiten](#prepare-the-import-file).

1. Führen Sie einen Benutzerbericht aus, der SSO-Benutzernameninformationen enthält.

   Beachten Sie, dass die Spalte SSO-Benutzername für jeden Benutzer ausgefüllt ist.

1. Stellen Sie sicher, dass die Werte für die Spalte SSO-Benutzername mit dem SSO-Benutzernamen auf Ihrem SSO-Server übereinstimmen.
1. Wenn die Spalte SSO-Benutzername leer ist, aktualisieren Sie die SSO-Benutzernamen Ihrer Benutzer.

   ![Benutzer mit SSO-Feld](assets/users-with-sso-field-updated.png)

   Anweisungen zum Aktualisieren Ihrer Benutzer für SSO finden Sie unter [Aktualisieren Ihrer Benutzer für SSO](#update-your-users-for-sso).
