---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook-Verbindungen testen
description: Webhook-Verbindungen testen
author: Becky
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Webhook-Verbindungen testen

Führen Sie die manuellen Tests in diesem Abschnitt durch, um zu überprüfen, ob Ihre Dokument-Webhook-Implementierung ordnungsgemäß funktioniert. Diese Schritte durchlaufen die Adobe Workfront-Web-Oberfläche und treffen indirekt die Endpunkte für Ihre Webhook-Implementierung.

## Voraussetzungen

Zum Ausführen der Tests sind folgende Voraussetzungen erforderlich:

* Ein Workfront-Konto mit aktivierter erweiterter Dokumentenverwaltung (ADM)

* Ein Workfront-Benutzer für dieses Konto mit Systemadministratorrechten

* Eine Document Webhook-Instanz mit HTTP-Endpunkten, auf die Workfront zugreifen kann

Bei diesen Tests wird außerdem davon ausgegangen, dass Ihre Document Webhook-Instanz registriert ist. (Sie können Ihre Instanz in Workfront unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen registrieren.)

**Test 1: Bereitstellen des Document Webhook-Dienstes für einen Benutzer**

Testen Sie die Authentifizierungs-URL und die Token-Endpunkt-URL für OAuth-basierte Webhook-Provider.

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Klicken Sie auf das Dropdown-Menü Dokumente hinzufügen und wählen Sie Ihren Document Webhook-Dienst unter Dienst hinzufügen aus.
1. (Nur OAuth-Dienste) Nach Abschluss des vorherigen Schritts wird die OAuth2-Authentifizierungsseite Ihres Dienstes in einem Popup-Fenster geladen. (Hinweis: Sie werden möglicherweise aufgefordert, sich zuerst bei Ihrem Dienst anzumelden.) Gewähren Sie auf der Authentifizierungsseite Workfront Zugriff auf das Benutzerkonto, indem Sie auf die Schaltfläche Vertrauen oder Zulassen klicken.
1. Vergewissern Sie sich, dass Ihr Dienst der Dropdown-Liste Dokumente hinzufügen hinzugefügt wurde. Wenn Sie ihn anfangs nicht sehen, versuchen Sie, den Browser zu aktualisieren.

**Test 2: Verknüpfen Sie ein Dokument mit Workfront-Tests mit den folgenden Endpunkten: /files, /metadata**

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Dienst unter &quot;Dokumente hinzufügen&quot;aus.
1. Navigieren Sie vom Modal aus durch die Ordnerstruktur.
1. Stellen Sie sicher, dass Sie in der Ordnerstruktur navigieren können.
1. Auswählen und Verknüpfen eines Dokuments mit Workfront

**Test 3: Navigieren zu einem Dokument im Content Management System**

Testet die folgenden Endpunkte: /metadata (insbesondere viewLink)

1. Dokument in Workfront verknüpfen
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Überprüfen Sie, ob das Dokument in einer neuen Registerkarte geöffnet wird.

**Test 4: Navigieren zu einem Dokument im Content Management System (mit Anmeldung)**

Testet die folgenden Endpunkte: /metadata (insbesondere viewLink)

1. Stellen Sie sicher, dass Sie vom Content Management System abgemeldet wurden.
1. Verknüpfen Sie ein Dokument mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Stellen Sie sicher, dass der Anmeldebildschirm des Content Management-Systems in einer neuen Registerkarte geladen wird.
1. Melden Sie sich an und vergewissern Sie sich, dass Sie zum Dokument gelangt sind.

**Test 5: Laden Sie das Dokument aus dem Content Management System herunter**

Testet die folgenden Endpunkte (insbesondere den Download-Link): /metadata 

1. Verknüpfen Sie ein Dokument mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Herunterladen .
1. Vergewissern Sie sich, dass der Download beginnt.

**Test 6: Suche nach Inhalt**

Testet die folgenden Endpunkte: /search

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Dienst unter &quot;Dokumente hinzufügen&quot;aus.
1. Führen Sie im Modal eine Suche durch.
1. Überprüfen Sie, ob die Suchergebnisse korrekt sind.

**Test 7: Senden von Dokumenten von Workfront an das Content Management System**

Testet die folgenden Endpunkte: /files, /uploadInit, /upload

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Hochladen eines Dokuments von Ihrem Computer in Workfront
1. Navigieren Sie zur Seite mit den Dokumentdetails .
1. Wählen Sie im Dropdown-Menü Dokumentaktionen Ihren Document Webhook-Dienst unter Senden an... aus.
1. Wechseln Sie zum gewünschten Zielordner und klicken Sie auf die Schaltfläche Speichern .
1. Stellen Sie sicher, dass das Dokument an die richtige Stelle im Content Management System hochgeladen wurde.

**Test 8: Anzeigen von Miniaturansichten in Workfront**

Testet die folgenden Endpunkte: /thumbnail

1. Verknüpfen Sie ein Dokument mit Workfront.
1. Wählen Sie das Dokument in der Liste aus.
1. Stellen Sie sicher, dass die Miniaturansicht im rechten Bereich angezeigt wird.

**Test 9: Abrufen der Inhalts-Bytes**

Testet die folgenden Endpunkte: /download

1. Verknüpfen Sie ein Dokument mit Workfront.
1. Rufen Sie die Seite mit den Dokumentdetails auf.
1. Senden Sie das Dokument an Workfront, indem Sie &quot;Dokumentaktionen&quot;> &quot;Senden an...&quot;> &quot;Workfront&quot;auswählen. Dadurch wird eine neue Dokumentversion in Workfront erstellt.
1. Laden Sie das Dokument von Workfront herunter, indem Sie auf den Link Herunterladen klicken.

**Test 10: Zugriffstoken aktualisieren (nur OAuth2 Webhook-Anbieter)**

Testet die folgenden Endpunkte: Token-Endpunkt-URL

1. Bereitstellen eines Document Webhook-Dienstes für einen Benutzer
1. Invalidierung des Zugriffstokens des Benutzers durch 1) Warten auf eine Zeitüberschreitung oder 2) manuelles Invalidieren des Zugriffs-Tokens im externen System.
1. Aktualisieren Sie das Zugriffstoken in Workfront. Dazu können Sie beispielsweise ein Dokument mit Workfront verknüpfen. Sie wissen, dass das Zugriffstoken erfolgreich aktualisiert wurde, wenn Sie zu einem Dokument navigieren und es verknüpfen konnten.

>[!NOTE]
>
>Zurzeit ist das Senden an... nicht für verknüpfte Dokumente verfügbar. Dieser wird von Workfront hinzugefügt. Sie können den Endpunkt /download testen, indem Sie den Endpunkt manuell mithilfe eines REST-Clients wie Postman aufrufen. Alternativ kann der Endpunkt /download durch Generieren eines digitalen Testversands getestet werden. Wenden Sie sich zur Aktivierung des digitalen Testversands an Workfront.
