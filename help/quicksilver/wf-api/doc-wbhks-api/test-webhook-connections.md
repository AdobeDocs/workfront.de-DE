---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook-Verbindungen testen
description: Webhook-Verbindungen testen
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Webhook-Verbindungen testen

Um sicherzustellen, dass Ihre Webhook-Implementierung ordnungsgemäß funktioniert, führen Sie die manuellen Tests in diesem Abschnitt aus. Diese Schritte durchlaufen die Adobe Workfront-Web-Oberfläche und treffen indirekt die Endpunkte für Ihre Webhook-Implementierung.

## Voraussetzungen

Die folgenden Voraussetzungen sind für die Durchführung der Tests erforderlich:

* Ein Workfront-Konto mit aktiviertem Advanced Document Management (ADM)

* Ein Workfront-Benutzer für dieses Konto mit Systemadministratorrechten

* Eine Document Webhook-Instanz mit HTTP-Endpunkten, auf die Workfront zugreifen kann

Bei diesen Tests wird außerdem davon ausgegangen, dass Ihre Document Webhook-Instanz registriert ist. (Sie können Ihre Instanz in Workfront unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen registrieren.)

**Test 1: Bereitstellen des Document Webhook-Service für einen Benutzer**

Testet die Authentifizierungs-URL und Token-Endpunkt-URL für OAuth-basierte Webhook-Anbieter.

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Klicken Sie auf die Dropdown-Liste Dokumente hinzufügen und wählen Sie unter Service hinzufügen Ihren Document Webhook-Service aus.
1. (Nur OAuth-Services) Nach Abschluss des vorherigen Schritts wird die OAuth2-Authentifizierungsseite Ihres Services in einem Popup-Fenster geladen. (Hinweis: Sie werden möglicherweise aufgefordert, sich zuerst bei Ihrem Dienst anzumelden.) Gewähren Sie auf der Authentifizierungsseite Workfront Zugriff auf das Konto des Benutzers, indem Sie auf die Schaltfläche Trust oder Allow klicken.
1. Stellen Sie sicher, dass Ihr Dienst zur Dropdown-Liste Dokumente hinzufügen hinzugefügt wurde. Wenn Sie sie anfangs nicht sehen, versuchen Sie, Ihren Browser zu aktualisieren.

**Test 2: Verknüpfen eines Dokuments mit Workfront Testet die folgenden Endpunkte: /files, /metadata**

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Service unter Dokumente hinzufügen aus.
1. Navigieren Sie im Modal durch die Ordnerstruktur.
1. Stellen Sie sicher, dass Sie in der Lage sind, in der Ordnerstruktur zu navigieren.
1. Dokument auswählen und mit Workfront verknüpfen

**Test 3: Navigieren Sie zu einem Dokument im Content-Management-System**

Testet die folgenden Endpunkte: /metadata (insbesondere den viewLink)

1. Verknüpfen eines Dokuments mit Workfront
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Stellen Sie sicher, dass das Dokument auf einer neuen Registerkarte geöffnet wird.

**Test 4: Navigieren Sie zu einem Dokument im Content-Management-System (mit Anmeldung)**

Testet die folgenden Endpunkte: /metadata (insbesondere den viewLink)

1. Stellen Sie sicher, dass Sie vom Content-Management-System abgemeldet sind.
1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Stellen Sie sicher, dass der Anmeldebildschirm des Content Management Systems auf einer neuen Registerkarte geladen wird.
1. Melden Sie sich an und stellen Sie sicher, dass Sie zum Dokument weitergeleitet werden

**Test 5: Laden Sie das Dokument aus dem Content-Management-System herunter**

Testet die folgenden Endpunkte (insbesondere den Download-Link): /metadata 

1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Herunterladen .
1. Stellen Sie sicher, dass der Download beginnt.

**Test 6: Suchen nach Inhalten**

Testet die folgenden Endpunkte: /search

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Service unter Dokumente hinzufügen aus.
1. Führen Sie über das Modal eine Suche durch.
1. Überprüfen Sie, ob die Suchergebnisse korrekt sind.

**Test 7: Senden Sie ein Dokument von Workfront an das Content-Management-System**

Testet die folgenden Endpunkte: /files, /uploadInit, /upload

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Dokument von Ihrem Computer in Workfront hochladen
1. Zur Seite mit den Dokumentdetails
1. Wählen Sie im Dropdown-Menü Dokumentaktionen unter Senden an… Ihren Dokument-Webhook-Service aus.
1. Wechseln Sie zum gewünschten Zielordner und klicken Sie auf die Schaltfläche Speichern .
1. Überprüfen Sie, ob das Dokument an den richtigen Speicherort im Content Management System hochgeladen wurde.

**Test 8: Anzeigen von Miniaturansichten in Workfront**

Testet die folgenden Endpunkte: /thumbnail

1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument in der Liste aus.
1. Stellen Sie sicher, dass die Miniaturansicht im rechten Bedienfeld angezeigt wird.

**Test 9: Abrufen der Inhalts-Bytes**

Testet die folgenden Endpunkte: /download

1. Verknüpfen eines Dokuments mit Workfront.
1. Navigieren Sie zur Seite mit den Dokumentdetails.
1. Senden Sie das Dokument an Workfront, indem Sie Dokumentaktionen > Senden an… > Workfront auswählen. Dadurch wird eine neue Dokumentversion in Workfront erstellt.
1. Laden Sie das Dokument von Workfront herunter, indem Sie auf den Download-Link klicken.

**Test 10: Zugriffstoken aktualisieren (nur OAuth2-Webhook-Anbieter)**

Testet die folgenden Endpunkte: Token Endpoint URL

1. Bereitstellen des Document Webhook-Services für einen Benutzer
1. Invalidieren Sie das Zugriffs-Token des Benutzers, indem Sie entweder 1 ) auf die Zeitüberschreitung warten oder 2) es im externen System manuell invalidieren.
1. Aktualisieren Sie das Zugriffstoken in Workfront. Dies können Sie beispielsweise tun, indem Sie ein Dokument mit Workfront verknüpfen. Das Zugriffstoken wurde erfolgreich aktualisiert, wenn Sie zu einem Dokument navigieren und es verknüpfen konnten.

>[!NOTE]
>
>Derzeit ist „Senden an…“ nicht für verknüpfte Dokumente verfügbar. Dies wird von Workfront hinzugefügt. Sie können den /download-Endpunkt testen, indem Sie mit einem REST-Client wie Postman manuell auf den Endpunkt klicken. Alternativ kann der Endpunkt /download getestet werden, indem ein digitaler Korrekturabzug generiert wird. Wenden Sie sich zur Aktivierung des digitalen Proofings an Workfront.
