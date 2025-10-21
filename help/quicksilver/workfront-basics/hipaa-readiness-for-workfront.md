---
content-type: reference
navigation-topic: get-started-with-workfront
title: HIPAA-Bereitschaft für Workfront
description: Ein Workfront-Kunde, der gemäß der Definition in HIPAA ein Business Associate und/oder die abgedeckte Entität ist, für die der Business Associate Adobe Workfront bereitstellt, sollte die folgenden Richtlinien verwenden, um Workfront für die HIPAA-fähige Verwendung zu konfigurieren.
feature: Get Started with Workfront
author: Courtney
exl-id: e3cdaa03-d523-46a4-954b-8456d5f190e4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# HIPAA-Bereitschaft für Workfront

Ein Workfront-Kunde, der gemäß der Definition in HIPAA ein Business Associate und/oder die abgedeckte Entität ist, für die der Business Associate Adobe Workfront bereitstellt, sollte die folgenden Richtlinien verwenden, um Workfront für die HIPAA-fähige Verwendung zu konfigurieren:


## Passwortanforderungen

| **Sicherheitseinstellung** | **Was ist das?** | **Anforderung** |
|----------------------|------------------|------------------|
| Mindestkennwortstärke für Vereinbarungen | Wie hoch ist die Mindeststärke für Vereinbarungspasswörter? | Mindestens 8 Zeichen |
| Minimale Kennwortstärke für Benutzerkennwörter | Wie hoch ist die Mindeststärke für Benutzerkennwörter? | Zeichen aus drei der folgenden Kategorien:<br> Großbuchstaben (lateinisches Alphabet)<br> Kleinbuchstaben (lateinisches Alphabet)<br> Basis 10 Ziffern<br> Nicht alphanumerische Zeichen |
| Kennwortdauer | Wie lange sollten Kennwörter unverändert bleiben dürfen? | Kennwörter sollten mindestens alle 90 Tage geändert werden |
| Kennwortverlauf | Wie viele alte Passwörter sollten gespeichert und nicht zugelassen werden? | Mindestens 5 |


## Anmeldeanforderungen

| **Sicherheitseinstellung** | **Was ist das?** | **Anforderung** |
|----------------------|------------------|------------------|
| Maximale Anzahl an Anmeldefehlern | Wie viele fehlgeschlagene Anmeldeversuche führen dazu, dass der Benutzer gesperrt wird? | Nicht mehr als 5 Versuche innerhalb eines 5-minütigen Zeitraums; ein erneuter Versuch ist nach 30 Minuten zulässig |
| Maximale SSO-Überprüfungsfehler | Wie viele fehlgeschlagene SSO-Verifizierungsversuche führen zu einer Sperrung? | Höchstens 5 (gilt nur für Kunden, die SSO verwenden) |


## Sitzungsanforderungen

| **Sicherheitseinstellung** | **Was ist das?** | **Anforderung** |
|----------------------|------------------|------------------|
| Sitzungs-Timeout | Wie viele Minuten ohne Aktivität führen zu einer Abmeldung? | Nicht mehr als 15 Minuten |

## Zuständigkeiten des Kunden

Stellen Sie sicher, dass alle Mitarbeiter, Repräsentanten und/oder Vertreter die Bedingungen in den Lizenzierungs- und/oder Serviceverträgen, die zwischen den Parteien unterzeichnet wurden und für die Verwendung von Daten mit Workfront relevant sind, kennen und verstehen.

Insbesondere sollten die folgenden Zuständigkeiten und Pflichten überprüft und mitgeteilt werden: 

* Der Kunde ist für die Nutzung des Workfront-Dienstes durch alle seine Nutzer verantwortlich. 

* Der Kunde ist verpflichtet, alle Bedingungen seiner Vereinbarung mit Adobe einzuhalten, die das Hochladen verbotener Datenelemente in Workfront beinhalten. 

* Jegliche vertraulichen Daten, einschließlich, aber nicht beschränkt auf ePHI, werden auf eigene Gefahr des Kunden hochgeladen.  Der Kunde ist jederzeit für alle Kundendaten verantwortlich. 


## Datenschutz und Compliance

>[!IMPORTANT]
>
>Workfront ist nicht als Repository für elektronische Patientenakten (EHR) konzipiert. ePHI darf nur verarbeitet werden, wenn Adobe dies ausdrücklich schriftlich genehmigt hat. 

* Stellen Sie für jede Workfront-Datenbank, auf die ePHI zugreifen kann **sicher, dass „Encryption at Rest (EAR)** aktiviert ist.
   * Wenden Sie sich an Ihren Kundenbetreuer, um zu bestätigen, dass EAR in Ihrem Workfront-Kauf enthalten ist.
   * Konfigurieren Sie Systeme/Datenbanken, auf die über Workfront zugegriffen werden kann, um Compliance-Verpflichtungen zu erfüllen.
* Stellen Sie sicher, dass ePHI nicht mit anderen nicht HIPAA-fähigen Adobe-Lösungen übertragen, verknüpft oder freigegeben wird.
* Stellen Sie sicher, dass über Workfront verarbeitete Patientenfotos sicher und nicht öffentlich zugänglich aufbewahrt werden.
